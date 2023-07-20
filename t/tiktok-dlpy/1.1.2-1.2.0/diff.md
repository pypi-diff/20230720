# Comparing `tmp/tiktok-dlpy-1.1.2.tar.gz` & `tmp/tiktok-dlpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok-dlpy-1.1.2.tar", last modified: Wed Jul 19 23:52:18 2023, max compression
+gzip compressed data, was "tiktok-dlpy-1.2.0.tar", last modified: Thu Jul 20 15:26:47 2023, max compression
```

## Comparing `tiktok-dlpy-1.1.2.tar` & `tiktok-dlpy-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-19 23:52:18.101547 tiktok-dlpy-1.1.2/
--rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.1.2/LICENSE
--rw-r--r--   0 becky      (501) staff       (20)      506 2023-07-19 23:52:18.101599 tiktok-dlpy-1.1.2/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      487 2023-06-12 14:02:52.000000 tiktok-dlpy-1.1.2/README.md
--rw-r--r--   0 becky      (501) staff       (20)       79 2023-07-19 23:52:18.101762 tiktok-dlpy-1.1.2/setup.cfg
--rw-r--r--   0 becky      (501) staff       (20)      766 2023-07-19 23:46:49.000000 tiktok-dlpy-1.1.2/setup.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-19 23:52:18.100337 tiktok-dlpy-1.1.2/tiktok_dlpy.egg-info/
--rw-r--r--   0 becky      (501) staff       (20)      506 2023-07-19 23:52:18.000000 tiktok-dlpy-1.1.2/tiktok_dlpy.egg-info/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      333 2023-07-19 23:52:18.000000 tiktok-dlpy-1.1.2/tiktok_dlpy.egg-info/SOURCES.txt
--rw-r--r--   0 becky      (501) staff       (20)        1 2023-07-19 23:52:18.000000 tiktok-dlpy-1.1.2/tiktok_dlpy.egg-info/dependency_links.txt
--rw-r--r--   0 becky      (501) staff       (20)       40 2023-07-19 23:52:18.000000 tiktok-dlpy-1.1.2/tiktok_dlpy.egg-info/requires.txt
--rw-r--r--   0 becky      (501) staff       (20)        9 2023-07-19 23:52:18.000000 tiktok-dlpy-1.1.2/tiktok_dlpy.egg-info/top_level.txt
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-19 23:52:18.101325 tiktok-dlpy-1.1.2/tiktokdl/
--rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.1.2/tiktokdl/__init__.py
--rw-r--r--   0 becky      (501) staff       (20)    11988 2023-07-19 23:44:55.000000 tiktok-dlpy-1.1.2/tiktokdl/download_video.py
--rw-r--r--   0 becky      (501) staff       (20)      434 2023-07-19 23:43:36.000000 tiktok-dlpy-1.1.2/tiktokdl/exceptions.py
--rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.1.2/tiktokdl/image_processing.py
--rw-r--r--   0 becky      (501) staff       (20)      443 2023-06-11 17:49:11.000000 tiktok-dlpy-1.1.2/tiktokdl/video_data.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-20 15:26:47.782496 tiktok-dlpy-1.2.0/
+-rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.2.0/LICENSE
+-rw-r--r--   0 becky      (501) staff       (20)      506 2023-07-20 15:26:47.782556 tiktok-dlpy-1.2.0/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      487 2023-06-12 14:02:52.000000 tiktok-dlpy-1.2.0/README.md
+-rw-r--r--   0 becky      (501) staff       (20)       79 2023-07-20 15:26:47.782733 tiktok-dlpy-1.2.0/setup.cfg
+-rw-r--r--   0 becky      (501) staff       (20)      766 2023-07-20 15:25:54.000000 tiktok-dlpy-1.2.0/setup.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-20 15:26:47.781441 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/
+-rw-r--r--   0 becky      (501) staff       (20)      506 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      333 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 becky      (501) staff       (20)        1 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 becky      (501) staff       (20)       40 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/requires.txt
+-rw-r--r--   0 becky      (501) staff       (20)        9 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/top_level.txt
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-20 15:26:47.782397 tiktok-dlpy-1.2.0/tiktokdl/
+-rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.2.0/tiktokdl/__init__.py
+-rw-r--r--   0 becky      (501) staff       (20)    13722 2023-07-20 15:24:21.000000 tiktok-dlpy-1.2.0/tiktokdl/download_video.py
+-rw-r--r--   0 becky      (501) staff       (20)      434 2023-07-19 23:43:36.000000 tiktok-dlpy-1.2.0/tiktokdl/exceptions.py
+-rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.2.0/tiktokdl/image_processing.py
+-rw-r--r--   0 becky      (501) staff       (20)      443 2023-06-11 17:49:11.000000 tiktok-dlpy-1.2.0/tiktokdl/video_data.py
```

### Comparing `tiktok-dlpy-1.1.2/LICENSE` & `tiktok-dlpy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.1.2/setup.py` & `tiktok-dlpy-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tiktok-dlpy",
-    version="1.1.2",
+    version="1.2.0",
     url="https://github.com/Fluxticks/TikTokDL",
-    download_url="https://github.com/Fluxticks/TikTokDL/archive/v1.1.2.tar.gz",
+    download_url="https://github.com/Fluxticks/TikTokDL/archive/v1.2.0.tar.gz",
     author="Fluxticks",
     packages=find_packages(),
     install_requires=[
         "bs4",
         "lxml",
         "playwright",
         "numpy",
```

### Comparing `tiktok-dlpy-1.1.2/tiktokdl/download_video.py` & `tiktok-dlpy-1.2.0/tiktokdl/download_video.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import json
 from datetime import datetime
 import random
 import time
 from typing import Literal
 from urllib.parse import parse_qs, urlparse
 
@@ -174,31 +175,49 @@
         await button.click()
 
     await playwright_page.get_by_role("button", name="Decline all").click()
     await __random_timeout_duration(playwright_page, 500, 900)
     return len(close_buttons) + 1
 
 
+def __filter_kwargs(function: callable, all_kwargs: dict):
+    all_args = inspect.getfullargspec(function)
+    allowed_args = all_args.kwonlyargs
+
+    valid_kwargs = {}
+    for key, value in all_kwargs.items():
+        if key in allowed_args:
+            valid_kwargs[key] = value
+
+    return valid_kwargs
+
+
 async def get_video(
     url: str,
     download: bool = True,
+    force_download_strategy: Literal["primary",
+                                     "secondary"] | None = None,
+    proxy: dict | None = None,
     download_timeout: float = 5000,
     browser: Literal["firefox",
                      "chromium",
                      "chrome",
                      "safari",
                      "webkit"] = "firefox",
     headless: bool | None = None,
-    slow_mo: float | None = None
+    slow_mo: float | None = None,
+    **kwargs: dict
 ) -> TikTokVideo:
     """Get the information about a given video URL. If the `download` param is set to True, also download the video as an mp4 file.
 
     Args:
         url (str): The URL to get the information of.
         download (bool, optional): If the video should be downloaded locally. Defaults to True.
+        force_download_strategy (Literal[&quot;primary&quot;, &quot;secondary&quot;] | None, optional): Force a specific download strategy to use. Defaults to None which will auto-select the strategy to use.
+        proxy (dict | None, optional): The proxy settings to use for the request. Defaults to None.
         download_timeout (float, optional): The number of ms the download will wait to start before timing out.
         browser (Literal[&quot;firefox&quot;, &quot;chromium&quot;, &quot;chrome&quot;, &quot;safari&quot;, &quot;webkit&quot;], optional): The browser to use to scrape the content. Defaults to "firefox".
         headless (bool | None, optional): If the browser should be headless. Defaults to None.
         slow_mo (float | None, optional): Slow the browser down, useful when not headless. Defaults to None.
 
     Raises:
         TypeError: If the given browser is not a valid browser.
@@ -219,16 +238,20 @@
             case "safari":
                 browser_instance = playwright.webkit
             case "webkit":
                 browser_instance = playwright.webkit
             case _:
                 raise TypeError(f"Invalid browser given. Browser {browser} is not valid.")
 
-        browser_instance = await browser_instance.launch(headless=headless, slow_mo=slow_mo)
-        browser_context = await browser_instance.new_context()
+        instance_extra_kwargs = __filter_kwargs(browser_instance.launch, kwargs)
+        browser_instance = await browser_instance.launch(headless=headless, slow_mo=slow_mo, **instance_extra_kwargs)
+
+        context_extra_kwargs = __filter_kwargs(browser_instance.new_context, kwargs)
+        browser_context = await browser_instance.new_context(proxy=proxy, **context_extra_kwargs)
+
         await browser_context.clear_cookies()
 
         video_page = await browser_context.new_page()
         await video_page.goto(url)
 
         try:
             page_source = await video_page.content()
@@ -241,14 +264,30 @@
 
         captcha_success_result = await __handle_captcha(video_page)
         if not captcha_success_result:
             raise CaptchaFailedException(url)
 
         await __close_popups(video_page)
 
+        if force_download_strategy:
+            try:
+                match force_download_strategy:
+                    case "primary":
+                        await primary_download_strategy(browser_context, video_page, video_info, download_timeout)
+                    case "secondary":
+                        await alternate_download_strategy(video_page, video_info, download_timeout)
+                    case _:
+                        raise ValueError(
+                            "Invalid download strategy provided. Strategy must be \"primary\", \"secondary\" or None."
+                        )
+            except:
+                raise DownloadFailedException(url=url)
+
+            return video_info
+
         try:
             if video_info.video_download_setting == 0:
                 await primary_download_strategy(browser_context, video_page, video_info, download_timeout)
             else:
                 await alternate_download_strategy(video_page, video_info, download_timeout)
         except PlaywrightTimeoutError:
             raise DownloadFailedException(url=url)
```

### Comparing `tiktok-dlpy-1.1.2/tiktokdl/image_processing.py` & `tiktok-dlpy-1.2.0/tiktokdl/image_processing.py`

 * *Files identical despite different names*

