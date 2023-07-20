# Comparing `tmp/bose-2.0.8.tar.gz` & `tmp/bose-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-2.0.8.tar", last modified: Mon Jul 17 03:57:16 2023, max compression
+gzip compressed data, was "bose-2.0.9.tar", last modified: Thu Jul 20 10:38:21 2023, max compression
```

## Comparing `bose-2.0.8.tar` & `bose-2.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 03:57:16.158173 bose-2.0.8/
--rw-rw-rw-   0        0        0    14120 2023-07-17 03:57:16.158173 bose-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    10357 2023-07-06 11:59:35.580609 bose-2.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-17 03:57:16.158173 bose-2.0.8/bose/
--rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.8/bose/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.8/bose/account_generator.py
--rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.8/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.8/bose/base_data.py
--rw-rw-rw-   0        0        0     8356 2023-07-17 03:55:40.349391 bose-2.0.8/bose/base_task.py
--rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.8/bose/beep_utils.py
--rw-rw-rw-   0        0        0    10586 2023-07-13 15:33:35.445633 bose-2.0.8/bose/bose_driver.py
--rw-rw-rw-   0        0        0    10384 2023-07-06 11:56:35.717259 bose-2.0.8/bose/bose_undetected_driver.py
--rw-rw-rw-   0        0        0     7884 2023-07-01 17:18:08.107702 bose-2.0.8/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.8/bose/download_driver.py
--rw-rw-rw-   0        0        0      993 2023-07-06 10:42:02.261172 bose-2.0.8/bose/ip_utils.py
--rw-rw-rw-   0        0        0     3040 2023-07-09 14:30:45.891095 bose-2.0.8/bose/launch_tasks.py
--rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.8/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.8/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.8/bose/opponent.py
--rw-rw-rw-   0        0        0     3130 2023-07-11 16:45:26.788592 bose-2.0.8/bose/output.py
--rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.8/bose/profile.py
--rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.8/bose/schedule_utils.py
--rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.8/bose/task_config.py
--rw-rw-rw-   0        0        0     1859 2023-07-17 03:55:54.165141 bose-2.0.8/bose/task_info.py
--rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.8/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.8/bose/user_agent.py
--rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.8/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.8/bose/wait.py
--rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.8/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-07-17 03:56:45.238680 bose-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 10:38:21.850759 bose-2.0.9/
+-rw-rw-rw-   0        0        0    14120 2023-07-20 10:38:21.851760 bose-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10357 2023-07-06 11:59:35.580609 bose-2.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-20 10:38:21.849757 bose-2.0.9/bose/
+-rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.9/bose/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.9/bose/account_generator.py
+-rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.9/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.9/bose/base_data.py
+-rw-rw-rw-   0        0        0     7170 2023-07-20 10:35:42.731134 bose-2.0.9/bose/base_task.py
+-rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.9/bose/beep_utils.py
+-rw-rw-rw-   0        0        0    11650 2023-07-19 12:44:32.472591 bose-2.0.9/bose/bose_driver.py
+-rw-rw-rw-   0        0        0    10384 2023-07-06 11:56:35.717259 bose-2.0.9/bose/bose_undetected_driver.py
+-rw-rw-rw-   0        0        0     9925 2023-07-19 09:27:56.338778 bose-2.0.9/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.9/bose/download_driver.py
+-rw-rw-rw-   0        0        0     1389 2023-07-20 08:22:20.488811 bose-2.0.9/bose/ip_utils.py
+-rw-rw-rw-   0        0        0     3040 2023-07-09 14:30:45.891095 bose-2.0.9/bose/launch_tasks.py
+-rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.9/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.9/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.9/bose/opponent.py
+-rw-rw-rw-   0        0        0     3647 2023-07-19 12:47:43.522593 bose-2.0.9/bose/output.py
+-rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.9/bose/profile.py
+-rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.9/bose/schedule_utils.py
+-rw-rw-rw-   0        0        0      511 2023-07-20 10:37:03.387959 bose-2.0.9/bose/task_config.py
+-rw-rw-rw-   0        0        0     1859 2023-07-17 03:55:54.165141 bose-2.0.9/bose/task_info.py
+-rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.9/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.9/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6488 2023-07-19 12:43:31.059425 bose-2.0.9/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.9/bose/wait.py
+-rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.9/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2334 2023-07-20 10:38:11.302390 bose-2.0.9/setup.py
```

### Comparing `bose-2.0.8/PKG-INFO` & `bose-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 2.0.8
+Version: 2.0.9
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
```

### Comparing `bose-2.0.8/README.rst` & `bose-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/account_generator.py` & `bose-2.0.9/bose/account_generator.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/analytics.py` & `bose-2.0.9/bose/analytics.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/base_data.py` & `bose-2.0.9/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/base_task.py` & `bose-2.0.9/bose/base_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import traceback
-from .beep_utils import beep_input
+from joblib import Parallel, delayed
 
 from .profile import Profile
 
 from .schedule_utils import ScheduleUtils
 from .create_driver import BrowserConfig, create_driver
 from .bose_driver import BoseDriver
-from .utils import relative_path,read_json,  merge_dicts_in_one_dict, write_file, write_html, write_json,get_driver_path
+from .utils import relative_path,merge_dicts_in_one_dict, write_file, write_html, write_json,get_driver_path
 from .local_storage import LocalStorage
 from .analytics import Analytics
 from .task_info import TaskInfo
 from .task_config import TaskConfig
 
 class RetryException(Exception):
     pass
@@ -28,63 +28,14 @@
     except:
         return "Failed to get page_source"
 
 
 def _download_driver():
     from .download_driver import download_driver
     download_driver()
-    
-
-def get_current_profile_path(config: BrowserConfig): 
-    profiles_path = f'profiles/{config.profile}/'
-    # profiles_path =  relative_path(path, 0)
-    return profiles_path
-    
-def save_cookies(driver, config):
-    current_profile_data = get_current_profile_path(config) + 'profile.json'
-    current_profile_data_path =  relative_path(current_profile_data, 0)
-
-    driver.execute_cdp_cmd('Network.enable', {})
-    cookies = (driver.execute_cdp_cmd('Network.getAllCookies', {}))
-    driver.execute_cdp_cmd('Network.disable', {})
-
-    if type(cookies) is not list:
-         cookies = cookies.get('cookies')
-    write_json(cookies, current_profile_data_path)
-
-def load_cookies(driver: BoseDriver, config):
-    current_profile = get_current_profile_path(config)
-    current_profile_path =  relative_path(current_profile, 0)
-
-    if not os.path.exists(current_profile_path):
-        os.makedirs(current_profile_path)
-    
-
-    current_profile_data = get_current_profile_path(config) + 'profile.json'
-    current_profile_data_path =  relative_path(current_profile_data, 0)
-
-    if not os.path.isfile(current_profile_data_path):
-        return
-
-    cookies = read_json(current_profile_data_path)
-    # Enables network tracking so we may use Network.setCookie method
-    driver.execute_cdp_cmd('Network.enable', {})
-    # Iterate through pickle dict and add all the cookies
-    for cookie in cookies:
-        # Fix issue Chrome exports 'expiry' key but expects 'expire' on import
-        if 'expiry' in cookie:
-            cookie['expires'] = cookie['expiry']
-            del cookie['expiry']
-        # Replace domain 'apple.com' with 'microsoft.com' cookies
-        cookie['domain'] = cookie['domain'].replace('apple.com', 'microsoft.com')
-        # Set the actual cookie
-        driver.execute_cdp_cmd('Network.setCookie', cookie)
-        
-    driver.execute_cdp_cmd('Network.disable', {})
-
 
 class BaseTask():
     def __init__(self):
         self.task_path = None
         self.task_id = None        
 
 
@@ -107,17 +58,43 @@
     def schedule(self, data):
         """
             Seconds delay between each run
         """
         return ScheduleUtils.no_delay(data)
 
 
+
+        
+    def set_config_on_driver(self, driver):
+            driver.task_id = self.task_id
+            driver.task_path = self.task_path
+            driver.beep = self._task_config.beep
+
     def create_driver(self, config: BrowserConfig):
-        return create_driver(config)
+        driver =  create_driver(config)
+        self.set_config_on_driver(driver)
+        return driver
     
+    # simple headless drivers no profile options
+    def parallel(self, callable, data_list= [None], n = 2):
+        def run(data):
+            config = self.get_browser_config(data)
+            driver = self.create_driver(config)
+            
+            result = callable(driver, data)
+            
+            driver.close()
+            return result
+        
+        n = min(len(data_list), n)
+
+        result = (Parallel(n_jobs=n, backend="threading")(delayed(run)(l) for l in data_list))
+        return result 
+        
+
     def begin_task(self, data, task_config:TaskConfig):
         def create_directories(task_path):
 
             driver_path =  relative_path(get_driver_path(), 0)
             if not os.path.isfile(driver_path):
                 print('[INFO] Downloading Chrome Driver in build/ directory. This is a one-time process. Download in progress...')
                 _download_driver()
@@ -134,14 +111,15 @@
             if not os.path.exists(profiles_path):
                 os.makedirs(profiles_path)
 
             path =  relative_path(task_path, 0)
             if not os.path.exists(path):
                 os.makedirs(path)
 
+        
         def run_task(is_retry, retry_attempt):
             # print('Launching Task')
             task = TaskInfo()
             task_name = self.__class__.__name__
             task.set_task_name(task_name)
 
             final_image = "final.png"
@@ -174,38 +152,38 @@
 
             self.task_path = f'tasks/{count}' 
             self.task_id = count
 
             create_directories(self.task_path)
             
             task.start()
+
+            self._task_config = task_config 
             config = self.get_browser_config(data)
             driver = self.create_driver(config)
 
             if config.profile is not None:
                 Profile.profile = config.profile
 
-            driver.task_id = self.task_id
-            driver.task_path = self.task_path
-            driver.beep = task_config.beep
+
+            self.set_config_on_driver(driver)
+
             self.beep = task_config.beep
 
             final_image_path = f'{self.task_path}/{final_image}'
             
-            
-            if config.is_tiny_profile:
-                load_cookies(driver, config)
-
-            def close_driver(driver):
+            def close_driver(driver:BoseDriver):
                 print("Closing Browser")                
-                if config.is_tiny_profile:
-                    save_cookies(driver, config)
                 # set tiny profile data
                 driver.close()
-                print("Closed Browser")                
+                print("Closed Browser")  
+
+                if self.task_config.log_time:
+                    duration = task.get_data()['duration']
+                    print(f'Task done in {duration}.')              
 
             result = None
             try:
                 result = self.run(driver, data)
                 end_task(driver)
                 close_driver(driver)
                 print(f'View Final Screenshot at {final_image_path}')
```

### Comparing `bose-2.0.8/bose/bose_driver.py` & `bose-2.0.9/bose/bose_undetected_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import traceback
-from datetime import datetime
-from selenium import webdriver
+from undetected_chromedriver import Chrome
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 import random
 from time import sleep
 from .beep_utils import beep_input
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
 from .utils import relative_path, sleep_for_n_seconds, sleep_forever
+from datetime import datetime
 
 
-class BoseDriver(webdriver.Chrome):
+class BoseUndetectedDriver(Chrome):
 
     def get_by_current_page_referrer(self, link, wait=None):
 
         # selenium.common.exceptions.WebDriverException
         self.execute_script(f"""
                 window.location.href = "{link}";
             """)
@@ -124,27 +124,25 @@
         except:
             return None
 
     def scroll_site(self):
         self.execute_script(""" 
 window.scrollBy(0, 10000);
 """)
-        
-    def can_element_be_scrolled(self, element):
-        # <=3 is a fix to handle floating point numbers
-        result = not (self.execute_script(
-            "return Math.abs(arguments[0].scrollTop - (arguments[0].scrollHeight - arguments[0].offsetHeight)) <= 3", element))
-        return result
 
     def scroll_element(self, element):
-        if self.can_element_be_scrolled(element):
+
+        did_element_scroll = self.execute_script(
+            "return Math.round(arguments[0].scrollTop) === Math.round(Math.round(arguments[0].scrollHeight) - Math.round(arguments[0].offsetHeight))", element)
+
+        if did_element_scroll:
+            return False
+        else:
             self.execute_script("arguments[0].scrollBy(0, 10000)", element)
             return True
-        else:
-            return False
 
     def get_cookies_dict(self):
         all_cookies = self.get_cookies()
         cookies_dict = {}
         for cookie in all_cookies:
             cookies_dict[cookie['name']] = cookie['value']
         return cookies_dict
@@ -267,19 +265,14 @@
         if raise_exception:
             raise Exception(f"Page {target} not found")
         return False
 
 
     def save_screenshot(self, filename=datetime.now().strftime('%Y-%m-%d_%H-%M-%S') + ".png"):
         try:
-
-
-            if not filename.endswith(".png"):
-                filename = filename + ".png"
-
             saving_screenshot_at = relative_path(
                 f'{self.task_path}/{filename}', 0)
             self.get_screenshot_as_file(
                 saving_screenshot_at)
         except:
             traceback.print_exc()
             print('Failed to save screenshot')
```

### Comparing `bose-2.0.8/bose/bose_undetected_driver.py` & `bose-2.0.9/bose/bose_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 import traceback
-from undetected_chromedriver import Chrome
+from datetime import datetime
+from selenium import webdriver
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 import random
 from time import sleep
 from .beep_utils import beep_input
 from .local_storage_driver import LocalStorage
 from .opponent import Opponent
-from .utils import relative_path, sleep_for_n_seconds, sleep_forever
-from datetime import datetime
+from .utils import get_current_profile_path, read_file, relative_path, sleep_for_n_seconds, sleep_forever, write_json
+
+    
+def save_cookies(driver, config):
+            current_profile_data = get_current_profile_path(config) + 'profile.json'
+            current_profile_data_path =  relative_path(current_profile_data, 0)
+
+            driver.execute_cdp_cmd('Network.enable', {})
+            cookies = (driver.execute_cdp_cmd('Network.getAllCookies', {}))
+            driver.execute_cdp_cmd('Network.disable', {})
+
+            if type(cookies) is not list:
+                cookies = cookies.get('cookies')
+            write_json(cookies, current_profile_data_path)
 
 
-class BoseUndetectedDriver(Chrome):
+class BoseDriver(webdriver.Chrome):
+    beep = True
 
     def get_by_current_page_referrer(self, link, wait=None):
 
         # selenium.common.exceptions.WebDriverException
         self.execute_script(f"""
                 window.location.href = "{link}";
             """)
@@ -125,24 +139,26 @@
             return None
 
     def scroll_site(self):
         self.execute_script(""" 
 window.scrollBy(0, 10000);
 """)
 
-    def scroll_element(self, element):
-
-        did_element_scroll = self.execute_script(
-            "return Math.round(arguments[0].scrollTop) === Math.round(Math.round(arguments[0].scrollHeight) - Math.round(arguments[0].offsetHeight))", element)
+    def can_element_be_scrolled(self, element):
+        # <=3 is a fix to handle floating point numbers
+        result = not (self.execute_script(
+            "return Math.abs(arguments[0].scrollTop - (arguments[0].scrollHeight - arguments[0].offsetHeight)) <= 3", element))
+        return result
 
-        if did_element_scroll:
-            return False
-        else:
+    def scroll_element(self, element):
+        if self.can_element_be_scrolled(element):
             self.execute_script("arguments[0].scrollBy(0, 10000)", element)
             return True
+        else:
+            return False
 
     def get_cookies_dict(self):
         all_cookies = self.get_cookies()
         cookies_dict = {}
         for cookie in all_cookies:
             cookies_dict[cookie['name']] = cookie['value']
         return cookies_dict
@@ -213,14 +229,22 @@
         def is_starts_with(link):
             if search == None:
                 return True
             return search in link
 
         return list(filter(is_starts_with, filter(is_not_none, links)))
 
+
+
+    def execute_file(self, filename):
+        if not filename.endswith(".js"):
+            filename = filename + ".js"
+        content = read_file(filename)
+        return self.execute_script(content)
+
     def get_images(self, search=None, wait=None):
 
         def extract_links(elements):
             def extract_link(el):
                 return el.get_attribute("src")
 
             return list(map(extract_link, elements))
@@ -262,32 +286,37 @@
                 time += sleep_time
                 sleep(sleep_time)
 
         if raise_exception:
             raise Exception(f"Page {target} not found")
         return False
 
-
     def save_screenshot(self, filename=datetime.now().strftime('%Y-%m-%d_%H-%M-%S') + ".png"):
         try:
+
+            if not filename.endswith(".png"):
+                filename = filename + ".png"
+
+            final_path = f'{self.task_path}/{filename}'
             saving_screenshot_at = relative_path(
-                f'{self.task_path}/{filename}', 0)
+                final_path, 0)
             self.get_screenshot_as_file(
                 saving_screenshot_at)
+            # print('Saved screenshot at {0}'.format(final_path))
         except:
             traceback.print_exc()
             print('Failed to save screenshot')
 
-    def prompt_to_solve_captcha(self, more_rules = []):
+    def prompt_to_solve_captcha(self, more_rules=[]):
         print('')
         print('   __ _ _ _    _                          _       _           ')
         print('  / _(_) | |  (_)                        | |     | |          ')
         print(' | |_ _| | |   _ _ __      ___ __ _ _ __ | |_ ___| |__   __ _ ')
-        print(' |  _| | | |  | | `_ \    / __/ _` | `_ \| __/ __| `_ \ / _` |') 
-        print(' | | | | | |  | | | | |  | (_| (_| | |_) | || (__| | | | (_| |')   # Tells user to solve captcha
+        print(' |  _| | | |  | | `_ \    / __/ _` | `_ \| __/ __| `_ \ / _` |')
+        print(' | | | | | |  | | | | |  | (_| (_| | |_) | || (__| | | | (_| |')
         print(' |_| |_|_|_|  |_|_| |_|   \___\__,_| .__/ \__\___|_| |_|\__,_|')
         print('                                   | |                        ')
         print('                                   |_|                        ')
         print('')
 
         print('General Rules of Captcha Solving')
         print(' - Solve it Fast')
@@ -296,7 +325,12 @@
             print(t)
         # print('- Solve it Fast')
         # print('1. If')
 
         return beep_input('Press fill in the captcha, the faster the less detectable, then press enter to continue ...', self.beep)
 
         # return beep_input('Press fill in the captcha and press enter to continue ...', self.beep)
+    def close(self) -> None:
+        if (self.browser_config.is_tiny_profile):
+            save_cookies(self, self.browser_config)
+
+        return super().close()
```

### Comparing `bose-2.0.8/bose/create_driver.py` & `bose-2.0.9/bose/create_driver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 from selenium.common.exceptions import WebDriverException
 from .user_agent import UserAgentInstance, UserAgent
 from .window_size import WindowSize, WindowSizeInstance
-from .utils import NETWORK_ERRORS, is_windows, relative_path, retry_if_is_error, silentremove
+from .utils import NETWORK_ERRORS, get_current_profile_path, is_windows, read_json, relative_path, retry_if_is_error, silentremove
 from selenium.webdriver.chrome.options import Options as GoogleChromeOptions
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from undetected_chromedriver import ChromeOptions
 from .bose_driver import BoseDriver
 
 from .bose_undetected_driver import BoseUndetectedDriver
 import shutil
 import os
 
+
 class RetryException(Exception):
     pass
 
 class BrowserConfig:
-    def __init__(self, user_agent=None, headless= False,  window_size=WindowSize.window_size_1920_1080, profile=None, is_eager=False, use_undetected_driver=False, is_tiny_profile=False):
+    def __init__( self, 
+                  headless=False,  
+                  use_undetected_driver=False, 
+                  block_images_fonts_css = False, 
+                  profile=None, 
+                  is_tiny_profile=False,
+                  user_agent=None,
+                  window_size=WindowSize.window_size_1920_1080, 
+                  is_eager=False, 
+                  ):
         self.user_agent = user_agent
-        self.headless = headless    
+        self.headless = headless
         self.window_size = window_size
-        
+        self.block_images_fonts_css = block_images_fonts_css
+
+
         if profile is not None:
             self.profile = str(profile)
-        else: 
+        else:
             self.profile = None
         self.is_eager = is_eager
         self.use_undetected_driver = use_undetected_driver
-        
+
         self.is_tiny_profile = is_tiny_profile
 
         if self.is_tiny_profile and self.profile is None:
             raise Exception('Profile must be given when using tiny profile')
 
 
 def delete_cache(driver):
@@ -152,27 +164,67 @@
 
 def get_driver_path():
     executable_name = "chromedriver.exe" if is_windows() else "chromedriver"
     dest_path = f"build/{executable_name}"
     return dest_path
 
 
+def load_cookies(driver: BoseDriver, config):
+    current_profile = get_current_profile_path(config)
+    current_profile_path = relative_path(current_profile, 0)
+
+    if not os.path.exists(current_profile_path):
+        os.makedirs(current_profile_path)
+
+    current_profile_data = get_current_profile_path(config) + 'profile.json'
+    current_profile_data_path = relative_path(current_profile_data, 0)
+
+    if not os.path.isfile(current_profile_data_path):
+        return
+
+    cookies = read_json(current_profile_data_path)
+    # Enables network tracking so we may use Network.setCookie method
+    driver.execute_cdp_cmd('Network.enable', {})
+    # Iterate through pickle dict and add all the cookies
+    for cookie in cookies:
+        # Fix issue Chrome exports 'expiry' key but expects 'expire' on import
+        if 'expiry' in cookie:
+            cookie['expires'] = cookie['expiry']
+            del cookie['expiry']
+        # Replace domain 'apple.com' with 'microsoft.com' cookies
+        cookie['domain'] = cookie['domain'].replace(
+            'apple.com', 'microsoft.com')
+        # Set the actual cookie
+        driver.execute_cdp_cmd('Network.setCookie', cookie)
+
+    driver.execute_cdp_cmd('Network.disable', {})
+
+
 def create_driver(config: BrowserConfig):
     def run():
         is_undetected = config.use_undetected_driver
         options = ChromeOptions() if is_undetected else GoogleChromeOptions()
 
         if config.headless:
             options.add_argument('--headless=new')
 
         if is_docker():
             print("Running in Docker, So adding sandbox arguments")
             options.arguments.extend(
                 ["--no-sandbox", "--disable-setuid-sandbox"])
 
+        if config.block_images_fonts_css:
+            options.add_experimental_option(
+                "prefs", {
+                    "profile.managed_default_content_settings.images": 2,
+                    "profile.managed_default_content_settings.stylesheet": 2,
+                    "profile.managed_default_content_settings.fonts": 2,
+                }
+            )
+
         driver_attributes = add_essential_options(
             options, None if config.is_tiny_profile else config.profile, config.window_size, config.user_agent)
 
         if driver_attributes["profile"] is not None:
             driver_string = "Creating Driver with profile {}, window_size={}, and user_agent={}".format(
                 driver_attributes["profile"], driver_attributes["window_size"], driver_attributes["user_agent"])
         else:
@@ -212,8 +264,12 @@
 
         driver._init_data = driver_attributes
         return driver
     driver = retry_if_is_error(
         run, NETWORK_ERRORS + [(WebDriverException, lambda: delete_corrupted_files(config.profile) if config.profile else None)], 5)
     print("Launched Browser")
 
+    if config.is_tiny_profile:
+        load_cookies(driver, config)
+
+    driver.browser_config = config
     return driver
```

### Comparing `bose-2.0.8/bose/download_driver.py` & `bose-2.0.9/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/ip_utils.py` & `bose-2.0.9/bose/ip_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import requests
 from requests.exceptions import ReadTimeout
 import traceback
-
-def find_ip_details():
+def find_ip_details(max_retries=5):
     url = 'https://www.omkar.cloud/backend/ipinfo/'
     try:
         response = requests.get(url, timeout=10)
-        data =  (response.json())
+        data = response.json()
 
         if "readme" in data:
            del data["readme"]
         return data
-    except ReadTimeout:
-        print('Refetching IP')
-        return find_ip_details()
-    except Exception:
+    except requests.exceptions.ReadTimeout:
+        if max_retries > 0:
+            print('ReadTimeout occurred. Retrying...')
+            return find_ip_details(max_retries - 1)
+        else:
+            print('Max retries exceeded. Unable to fetch IP details.')
+            return None
+    except Exception as e:
         traceback.print_exc()
         return None
-    
 
-def find_ip():
+def find_ip(attempts=5):
     url = 'https://checkip.amazonaws.com/'
     try:
         response = requests.get(url, timeout=10)
-        return (response.text).strip()
+        return response.text.strip()
 
-        # requests.exceptions.ReadTimeout
     except ReadTimeout:
-        return None
-    except Exception:
+        if attempts > 1:
+            print("ReadTimeout occurred. Retrying...")
+            return find_ip(attempts - 1)
+        else:
+            print("Max attempts reached. Failed to get IP address.")
+            return None
+
+    except Exception as e:
         traceback.print_exc()
         return None
 
 
 def get_valid_ip():
     ip = find_ip()
     while ip is None:
```

### Comparing `bose-2.0.8/bose/launch_tasks.py` & `bose-2.0.9/bose/launch_tasks.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/local_storage.py` & `bose-2.0.9/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/local_storage_driver.py` & `bose-2.0.9/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/output.py` & `bose-2.0.9/bose/output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import csv
-from .utils import relative_path, write_json, read_json, write_html
+from .utils import read_file, relative_path, write_json, read_json, write_html
 
 class Output:
 
     def read_json(filename):
         if not filename.startswith("output/"):
             filename = "output/" +  filename
 
@@ -24,26 +24,30 @@
         if not filename.endswith(".json"):
             filename = filename + ".json"
 
         write_json(data, filename)
         print(f"View written JSON file at {filename}")        
 
     def write_csv(data, filename):
+        
         """
         Save a list of dictionaries as a CSV file.
 
         Args:
             data: a list of dictionaries
             filename: the name of the CSV file to save
         """
+        
+        if type(data) is dict:
+            data = [data]
+
         if len(data) == 0:
             print("Data is empty.")
             return
 
-
         if not filename.startswith("output/"):
             filename = "output/" +  filename
 
         if not filename.endswith(".csv"):
             filename = filename + ".csv"
 
         with open(filename, 'w', newline='', encoding='utf-8') as csvfile:
@@ -89,18 +93,32 @@
         if not filename.endswith(".html"):
             filename = filename + ".html"
 
         write_html(data, filename)
         print(f"View written HTML file at {filename}")
 
 
+    def read_html(data, filename):
+        if not filename.startswith("output/"):
+            filename = "output/" +  filename
+
+        if not filename.endswith(".html"):
+            filename = filename + ".html"
+
+        return read_file(filename)
+
 
     def write_file(data, filename):
         if not filename.startswith("output/"):
             filename = "output/" +  filename
 
 
         write_html(data, filename)
         print(f"View written file at {filename}")
 
 
+    def read_file(data, filename):
+        if not filename.startswith("output/"):
+            filename = "output/" +  filename
+
+        return read_file(filename)
```

### Comparing `bose-2.0.8/bose/profile.py` & `bose-2.0.9/bose/profile.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/schedule_utils.py` & `bose-2.0.9/bose/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/task_info.py` & `bose-2.0.9/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/temp_mail.py` & `bose-2.0.9/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/user_agent.py` & `bose-2.0.9/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/bose/utils.py` & `bose-2.0.9/bose/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,15 +248,20 @@
         fp.write(data)
 
 
 def read_json(path):
     with open(path, 'r') as fp:
         users = json.load(fp)
         return users
-    
+
+def read_file(path):
+    with open(path, 'r') as fp:
+        content = fp.read()
+        return content
+        
 def write_json(data, path,  indent=4):
     with open(path, 'w') as fp:
         json.dump(data, fp, indent=indent)
 
 
 def get_driver_path():
     executable_name = "chromedriver.exe" if is_windows() else "chromedriver"
@@ -271,7 +276,11 @@
         when, datetime_format)
 
 
 def datetime_to_str(when):
     return when.strftime(datetime_format)
 
 
+def get_current_profile_path(config): 
+    profiles_path = f'profiles/{config.profile}/'
+    # profiles_path =  relative_path(path, 0)
+    return profiles_path
```

### Comparing `bose-2.0.8/bose/window_size.py` & `bose-2.0.9/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.8/setup.py` & `bose-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 install_requires = [
     "requests",
     "chromedriver-autoinstaller==0.4.0",
     "selenium==4.5.0",
     "undetected_chromedriver>=3.4.6",
     "beautifulsoup4>=4.11.2",
+    "joblib==1.2.0",
 
 ]
 extras_require = {}
 cpython_dependencies = [
     "PyDispatcher>=2.0.5",
 ]
 
@@ -20,15 +21,15 @@
     except:
       return None
     
             
 setup(
     name='bose',
     packages=['bose'],
-    version='2.0.8',
+    version='2.0.9',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/",
         "Source": "https://github.com/omkarcloud/bose",
         "Tracker": "https://github.com/omkarcloud/bose/issues",
     },
```

