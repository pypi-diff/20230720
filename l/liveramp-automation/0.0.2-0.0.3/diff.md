# Comparing `tmp/liveramp_automation-0.0.2-py3-none-any.whl.zip` & `tmp/liveramp_automation-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 9396 bytes, number of entries: 15
+Zip file size: 9893 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     1711 b- defN 23-Jul-19 08:04 liveramp_automation/helper_bucket.py
--rw-r--r--  2.0 unx     2238 b- defN 23-Jul-17 09:37 liveramp_automation/helper_file.py
--rw-r--r--  2.0 unx     3116 b- defN 23-Jul-17 09:39 liveramp_automation/helper_login.py
+-rw-r--r--  2.0 unx     2320 b- defN 23-Jul-19 09:47 liveramp_automation/helper_file.py
+-rw-r--r--  2.0 unx     3564 b- defN 23-Jul-20 06:17 liveramp_automation/helper_login.py
 -rw-r--r--  2.0 unx       70 b- defN 23-Jul-19 08:17 liveramp_automation/helper_notification.py
--rw-r--r--  2.0 unx      692 b- defN 23-Jul-19 08:17 liveramp_automation/util_allure.py
--rw-r--r--  2.0 unx     2541 b- defN 23-Jul-19 08:39 liveramp_automation/util_log.py
--rw-r--r--  2.0 unx      723 b- defN 23-Jul-19 02:39 liveramp_automation/util_parsers.py
+-rw-r--r--  2.0 unx     1057 b- defN 23-Jul-20 06:17 liveramp_automation/util_allure.py
+-rw-r--r--  2.0 unx     2516 b- defN 23-Jul-20 06:21 liveramp_automation/util_log.py
+-rw-r--r--  2.0 unx      902 b- defN 23-Jul-20 09:35 liveramp_automation/util_parsers.py
 -rw-r--r--  2.0 unx      742 b- defN 23-Jul-17 06:23 liveramp_automation/util_playwright.py
--rw-r--r--  2.0 unx     7058 b- defN 23-Jul-19 08:17 liveramp_automation/util_request.py
+-rw-r--r--  2.0 unx     7304 b- defN 23-Jul-20 06:30 liveramp_automation/util_request.py
 -rw-r--r--  2.0 unx      743 b- defN 23-Jul-17 06:23 liveramp_automation/util_selenium.py
--rw-r--r--  2.0 unx      779 b- defN 23-Jul-17 02:34 liveramp_automation/util_time.py
--rw-r--r--  2.0 unx     2431 b- defN 23-Jul-19 08:48 liveramp_automation-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 08:48 liveramp_automation-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-19 08:48 liveramp_automation-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1354 b- defN 23-Jul-19 08:48 liveramp_automation-0.0.2.dist-info/RECORD
-15 files, 24310 bytes uncompressed, 7106 bytes compressed:  70.8%
+-rw-r--r--  2.0 unx      988 b- defN 23-Jul-20 06:35 liveramp_automation/util_time.py
+-rw-r--r--  2.0 unx     2431 b- defN 23-Jul-20 09:36 liveramp_automation-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 09:36 liveramp_automation-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-20 09:36 liveramp_automation-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1355 b- defN 23-Jul-20 09:36 liveramp_automation-0.0.3.dist-info/RECORD
+15 files, 25815 bytes uncompressed, 7603 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: liveramp_automation/util_selenium.py
 Comment: 
 
 Filename: liveramp_automation/util_time.py
 Comment: 
 
-Filename: liveramp_automation-0.0.2.dist-info/METADATA
+Filename: liveramp_automation-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: liveramp_automation-0.0.2.dist-info/WHEEL
+Filename: liveramp_automation-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: liveramp_automation-0.0.2.dist-info/top_level.txt
+Filename: liveramp_automation-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: liveramp_automation-0.0.2.dist-info/RECORD
+Filename: liveramp_automation-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## liveramp_automation/helper_file.py

```diff
@@ -10,16 +10,17 @@
         with open(path, 'r') as file:
             # Read all the content of the file
             json_string = file.read()
             data = json.loads(json_string)
         return data
 
     @staticmethod
-    def load_config(env):
-        with open(f"config/config.{env}.yaml") as f:
+    def load_env_yaml(env):
+        # This method is to read the resources accroding to different envrionments
+        with open(f"config/res.{env}.yaml") as f:
             return yaml.safe_load(f)
 
     @staticmethod
     def deal_api_json(item):
         nodeid = item["nodeid"]
         outcome = item["outcome"]
         groupName = nodeid.split("/")[1]
```

## liveramp_automation/helper_login.py

```diff
@@ -3,70 +3,76 @@
 from selenium.webdriver.common.by import By
 from liveramp_automation.util_log import Logger
 from liveramp_automation.util_time import fixed_wait
 
 
 class LoginHepler:
 
+    # This method liveramp_okta_login_page is to login okta with Playwright.
+    # The username and passowrd are requried.
+    # Please try to call this API with the username and password provided in os.environ[]
     @staticmethod
-    def liveramp_okta_login_page(page, config, USERNAME, PASSWORD):
+    def liveramp_okta_login_page(page, config, username, password):
         # navigate to the Okta login page
         Logger.info("We are going to login to OKTA")
         url = config['login_url']
         Logger.info("The login url is {}".format(url))
         page.goto(url)
         fixed_wait()
         url_new = page.url
         Logger.info("The current url is {}".format(url_new))
         if url_new.__contains__(url):
             Logger.info("We've already logan to OKTA succefully")
         else:
-            page.fill('#idp-discovery-username', USERNAME)
+            page.fill('#idp-discovery-username', username)
             page.get_by_role("button", name="Next").click()
-            page.get_by_role("textbox", name="Password").fill(PASSWORD)
+            page.get_by_role("textbox", name="Password").fill(password)
             page.get_by_role("button", name="Sign In").click()
             Logger.info("We could login to OKTA successfully")
             # wait for the login process to complete
             fixed_wait(20)
 
+    # This method liveramp_okta_login_driver is to login okta with Selenium.
+    # The username and passowrd are requried.
+    # Please try to call this API with the username and password provided in os.environ[]
     @staticmethod
-    def liveramp_okta_login_driver(driver, config, USERNAME, PASSWORD):
+    def liveramp_okta_login_driver(driver, config, username, password):
         # navigate to the Okta login page
         Logger.info("We are going to login to OKTA")
         url = config['login_url']
         Logger.info("The login url is {}".format(url))
         driver.get(url)
         fixed_wait()
         if driver.current_url.__contains__(url):
             Logger.info("We've already logan to OKTA succefully")
         else:
-            # username = driver.find_element_by_id('idp-discovery-username')
             username = driver.find_element(by=By.ID, value='idp-discovery-username')
-            username.send_keys(USERNAME)
+            username.send_keys(username)
             username.send_keys(Keys.ENTER)
             fixed_wait()
-            # password = driver.find_element_by_id('okta-signin-password')
             password = driver.find_element(by=By.ID, value='okta-signin-password')
-            password.send_keys(PASSWORD)
-            # driver.find_element_by_id('okta-signin-submit').click()
+            password.send_keys(password)
             submit_button = driver.find_element(by=By.ID, value='okta-signin-submit')
             submit_button.click()
             Logger.info("We could login to OKTA successfully")
             # wait for the login process to complete
             fixed_wait(20)
 
+    # This method call_oauth2_get_token is to all oauth2 to login, the API username and password(sereect) are required.
+    # The username and passowrd are requried.
+    # Please try to call this API with the username and password provided in os.environ[]
     @staticmethod
-    def call_oauth2_get_token(APIUSERNAME, APIPASSWORD):
+    def call_oauth2_get_token(username, password):
         params = {
             "grant_type": "password",
             "scope": "openid",
             "client_id": "liveramp-api"
         }
         Logger.info("The default params are the {}".format(params))
         headers = {"content-type": "application/x-www-form-urlencoded"}
-        params.update(username=APIUSERNAME)
-        params.update(password=APIPASSWORD)
+        params.update(username=username)
+        params.update(password=password)
         response = requests.post(
             "https://serviceaccounts.liveramp.com/authn/v1/oauth2/token", params=params, headers=headers)
         assert 200 == response.status_code
         access_token = response.json()['access_token']
         return "Bearer {}".format(access_token)
```

## liveramp_automation/util_allure.py

```diff
@@ -1,21 +1,26 @@
 import allure
 
 
+# Call allure_page_screenshot to show the screenshot while using Playright
 def allure_page_screenshot(page, name):
     allure.attach(page.screenshot(), name=name, attachment_type=allure.attachment_type.PNG)
 
 
-def allure_page_screenshot(driver, name):
+# Call allure_drive_screenshot to show the screenshot while using Selenium
+def allure_drive_screenshot(driver, name):
     allure.attach(driver.save_screenshot(), name=name, attachment_type=allure.attachment_type.PNG)
 
 
+# Call allure_attach_video to show the recording video,the video path should be provided.
 def allure_attach_video(path, video_name):
     allure.attach.file(path, name=video_name, attachment_type=allure.attachment_type.MP4)
 
 
-def allure_attach_text(description, content):
-    allure.attach(description, content, attachment_type=allure.attachment_type.TEXT)
+# Call allure_attach_text to show the content in text format.
+def allure_attach_text(content, description):
+    allure.attach(content, description, attachment_type=allure.attachment_type.TEXT)
 
 
-def allure_attach_json(description, content):
-    allure.attach(description, content, attachment_type=allure.attachment_type.JSON)
+# Call allure_attach_json to show the content in json format.
+def allure_attach_json(content, description):
+    allure.attach(content, description, attachment_type=allure.attachment_type.JSON)
```

## liveramp_automation/util_log.py

```diff
@@ -4,14 +4,17 @@
 import logging
 from datetime import datetime
 from logging import handlers
 from threading import Lock
 
 
 class LoggerUtils:
+    # This object is a single pattern instance to log.
+    # If we haven't set the default log_path in the pytest.ini file, it would use the path = "reports/"
+    # If we haven't set the default log_name in the pytest.ini file, it would use the log_name = "%Y%m%d%H%M%S.log"
     _instance = None
     _lock = Lock()
 
     @classmethod
     def get_logger(cls):
         if not cls._instance:
             with cls._lock:
@@ -22,23 +25,22 @@
     @staticmethod
     def _configure_logging():
         config = configparser.ConfigParser()
         try:
             with open("pytest.ini", 'r') as file:
                 config.read_file(file)
                 try:
-                    log_path = config.get('default', 'log_path')
+                    log_path = config.get('log', 'log_path')
                 except (configparser.NoSectionError, configparser.NoOptionError):
                     log_path = "reports/"
                 try:
-                    log_name = config.get('default', 'log_name')
+                    log_name = config.get('log', 'log_name')
                 except (configparser.NoSectionError, configparser.NoOptionError):
                     log_name = "%Y%m%d%H%M%S.log"
         except FileNotFoundError:
-            print(f"The file 'config.ini' does not exist.Never mind, we would use the default settings.")
             log_path = "reports/"
             log_name = "%Y%m%d%H%M%S.log"
 
         log_format = logging.Formatter('%(asctime)s - %(levelname)s - [ %(filename)s: %(lineno)d ] - %(message)s')
         log_directory = os.path.join(os.getcwd(), log_path)
         if not os.path.exists(log_directory):
             os.makedirs(log_directory)
@@ -59,13 +61,8 @@
         file_handler.setFormatter(log_format)
         logger.addHandler(file_handler)
 
         logger.debug("======Now LOG BEGIN=======")
         return logger
 
 
-# # Example usage
 Logger = LoggerUtils.get_logger()
-Logger.debug("This is a debug message.")
-Logger.info("This is an info message.")
-Logger.warning("This is a warning message.")
-Logger.error("This is an error message.")
```

## liveramp_automation/util_parsers.py

```diff
@@ -1,26 +1,30 @@
+from ctypes import cast
+from typing import Dict, Any
+
 from pytest_bdd.parsers import StepParser
 import parse as base_parse
 
 EXTRA_TYPES = {}
 
 
 class ParseUtils(StepParser):
     """parse step parser."""
 
+    # This is a Factory method pattern to parse the steps in the BDD scenarios
     def __init__(self, name, *args):
         """Compile parse expression."""
         super(ParseUtils, self).__init__(name)
         self.parser = base_parse.compile(self.name, *args, extra_types=EXTRA_TYPES)
 
-    def parse_arguments(self, name):
+    def parse_arguments(self, name: str) -> dict[str, Any]:
         """Get step arguments.
         :return: `dict` of step arguments
         """
-        return self.parser.parse(name).named
+        return cast(Dict[str, Any], self.parser.parse(name).named)
 
     def is_matching(self, name):
         """Match given name with the step name."""
         try:
             return bool(self.parser.parse(name))
         except ValueError:
-            return False
+            return False
```

## liveramp_automation/util_request.py

```diff
@@ -1,12 +1,15 @@
 import requests
 from liveramp_automation.util_allure import *
 from liveramp_automation.util_log import Logger
 
 
+# These are 7 types of methods to call the APIs.Each API allows to multiple parameters.
+# We also added some log/report_content while calling the APIs which would be helpful to check the errors.
+
 def request_post(url, headers, data=None, json=None, **kwargs):
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is POST")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is POST", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
@@ -33,15 +36,15 @@
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is GET", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
         allure_attach_json("The json in request body is:", json)
     try:
-        response = requests.get(url=url, data=data, json=json, headers=headers)
+        response = requests.get(url=url, data=data, json=json, headers=headers, **kwargs)
         Logger.info("The response infomation is {}".format(response.text))
     except requests.exceptions.HTTPError as error:
         Logger.info("HTTP error occurred {}".format(error))
     except requests.exceptions.Timeout as error:
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
@@ -103,46 +106,46 @@
     except requests.exceptions.Timeout as error:
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
-def request_put(url, headers, data=None, json=None):
+def request_put(url, headers, data=None, json=None, **kwargs):
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is PUT")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is PUT", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
         Logger.info("The json in request body is {}".format(json))
     try:
-        response = requests.put(url=url, data=data, json=json, headers=headers)
+        response = requests.put(url=url, data=data, json=json, headers=headers, **kwargs)
         Logger.info("The response infomation is {}".format(response.text))
     except requests.exceptions.HTTPError as error:
         Logger.info("HTTP error occurred {}".format(error))
     except requests.exceptions.Timeout as error:
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
-def request_patch(url, headers, data=None, json=None):
+def request_patch(url, headers, data=None, json=None, **kwargs):
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is PATCH")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is PATCH", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
         Logger.info("The json in request body is {}".format(json))
     try:
-        response = requests.patch(url=url, data=data, json=json, headers=headers)
+        response = requests.patch(url=url, data=data, json=json, headers=headers, **kwargs)
         Logger.info("The response infomation is {}".format(response.text))
     except requests.exceptions.HTTPError as error:
         Logger.info("HTTP error occurred {}".format(error))
     except requests.exceptions.Timeout as error:
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
```

## liveramp_automation/util_time.py

```diff
@@ -1,18 +1,22 @@
 import time
 from datetime import date, timedelta, datetime
 
+
+# The MACROS() API prepared some expected time format.
+# You could invole the time format like: yesterday.format(**MACROS) at any code snippet.
 MACROS = {
     "yesterday": (date.today() - timedelta(days=1)).strftime("%Y%m%d"),
     "today": date.today().strftime("%Y%m%d"),
     "dayOfYear": (date.today().timetuple()).tm_yday,
     "now": datetime.now().strftime("%Y%m%d%H%M%S"),
     "now_format": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
     "nowconnect": datetime.now().strftime("%Y%m%d-%H%M%S"),  # data ingestion must be in yyyymmdd-hhmmss format
     "three_days_ago": (date.today() - timedelta(days=0)).strftime("%Y%m%d"),
     "two_hours_from_now": (datetime.now() + timedelta(hours=2)).strftime("%Y%m%d-%H%M%S"),
     "24hours_before_now": (datetime.now() - timedelta(hours=24)).strftime("%Y%m%d%H%M%S")
 }
 
 
+# The fixed_wait() API defined the default=3 seconds wait time.
 def fixed_wait(value=3):
     time.sleep(value)
```

## Comparing `liveramp_automation-0.0.2.dist-info/METADATA` & `liveramp_automation-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-bdd
```

## Comparing `liveramp_automation-0.0.2.dist-info/RECORD` & `liveramp_automation-0.0.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 liveramp_automation/helper_bucket.py,sha256=C3x-5N536qGIVQRyDYDX4tLEtNwCwh7DJ7XXK22UyIU,1711
-liveramp_automation/helper_file.py,sha256=FBJ9uesQsEu72oyq3AZoxeeH9p4ItV4zY8bX-iiyvSg,2238
-liveramp_automation/helper_login.py,sha256=gaCtxlDO3a7Zau8P6Jp3F0W1nR8EcKuZj1CmYwD3PvA,3116
+liveramp_automation/helper_file.py,sha256=cjVEz_WEq4_TQBUirfslKTP6HmmOtuwkEAWAsFVtcoA,2320
+liveramp_automation/helper_login.py,sha256=FV9LEuKbgjBvzqfc02U6bsHoI9RinJ8EJhDD3_41TxU,3564
 liveramp_automation/helper_notification.py,sha256=9hYwVodMWn0y6z3trnkViClwg3berF60ipS5bLcxDB8,70
-liveramp_automation/util_allure.py,sha256=BebIEXUQ_8Xb27yA-hiyivgOZSNh6OUM7EAfGpREO1I,692
-liveramp_automation/util_log.py,sha256=ESv5AJBpJjDr4JkR21tZfCsvz9Pck__hF6Gr-1ogGI0,2541
-liveramp_automation/util_parsers.py,sha256=NNf44SSYXop1w6klQmtnJj7rsgKAqTLiyh5YBzD1DZg,723
+liveramp_automation/util_allure.py,sha256=EfFgEfVeO3mFyGyl01gbOsyvDtFGpLe021WYjfvzdl4,1057
+liveramp_automation/util_log.py,sha256=2xCVRXaSDkxtOiYUGPE7TlgDt1h_Th46ZwyOhO1Wlso,2516
+liveramp_automation/util_parsers.py,sha256=4_QLs-upSSiMVsophW648cdhoLznb_9aujD6Lk87m6E,902
 liveramp_automation/util_playwright.py,sha256=Kbwt6T_2LW9VIos_93V_Dc0hSpYQdUCP2PeyjZXs-mI,742
-liveramp_automation/util_request.py,sha256=NRVpgR437xwV7XWh1A8q96XBL8PCTEgS58AfA1Z_ySQ,7058
+liveramp_automation/util_request.py,sha256=8ztRhkkR1Bp5r_fAuW6f8MIlJbBJfWml_L0VcclCkWg,7304
 liveramp_automation/util_selenium.py,sha256=oW9DB6MZ1cqyqOg3PwtGqI-9kG2IJXUjaco1s31XTmI,743
-liveramp_automation/util_time.py,sha256=Pdc-mJnTw0x3PmqjF59PjpinJOxnDf42SrB9UhUETrQ,779
-liveramp_automation-0.0.2.dist-info/METADATA,sha256=EkY3dW9MMbF0GKNxEScdCCtgFULF-rOVuR50zS-9YJc,2431
-liveramp_automation-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-liveramp_automation-0.0.2.dist-info/top_level.txt,sha256=qRUeD1KGKo6cTZuEFDPYmXmkHqSsRq1qcGnhUgk6IHI,20
-liveramp_automation-0.0.2.dist-info/RECORD,,
+liveramp_automation/util_time.py,sha256=viI2-xq0Px2CAV9G-xNbmxVZ3dMiD5BN4P78LxkZWu8,988
+liveramp_automation-0.0.3.dist-info/METADATA,sha256=8m3l3WanKA4ZiS6tXiuilTTOi7BsO1XAiGlp21U-OGM,2431
+liveramp_automation-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+liveramp_automation-0.0.3.dist-info/top_level.txt,sha256=qRUeD1KGKo6cTZuEFDPYmXmkHqSsRq1qcGnhUgk6IHI,20
+liveramp_automation-0.0.3.dist-info/RECORD,,
```

