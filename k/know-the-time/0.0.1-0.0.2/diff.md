# Comparing `tmp/know_the_time-0.0.1.tar.gz` & `tmp/know_the_time-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "know_the_time-0.0.1.tar", last modified: Sun Jun 18 16:10:02 2023, max compression
+gzip compressed data, was "know_the_time-0.0.2.tar", last modified: Thu Jul 20 17:23:14 2023, max compression
```

## Comparing `know_the_time-0.0.1.tar` & `know_the_time-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:10:02.901276 know_the_time-0.0.1/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:12:34.000000 know_the_time-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       82 2023-01-17 17:17:39.000000 know_the_time-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1118 2023-06-18 16:10:02.900041 know_the_time-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-18 16:02:11.000000 know_the_time-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 16:10:02.891524 know_the_time-0.0.1/know_the_time/
--rw-rw-rw-   0        0        0      773 2023-06-18 16:04:01.000000 know_the_time-0.0.1/know_the_time/__init__.py
--rw-rw-rw-   0        0        0    12152 2023-06-18 16:00:06.000000 know_the_time-0.0.1/know_the_time/know_the_time.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:10:02.898022 know_the_time-0.0.1/know_the_time.egg-info/
--rw-rw-rw-   0        0        0     1118 2023-06-18 16:10:02.000000 know_the_time-0.0.1/know_the_time.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-18 16:10:02.000000 know_the_time-0.0.1/know_the_time.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:10:02.000000 know_the_time-0.0.1/know_the_time.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-18 16:10:02.000000 know_the_time-0.0.1/know_the_time.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 16:10:02.901276 know_the_time-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1217 2023-06-18 16:02:15.000000 know_the_time-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:23:14.295453 know_the_time-0.0.2/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:12:34.000000 know_the_time-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       82 2023-01-17 17:17:39.000000 know_the_time-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1118 2023-07-20 17:23:14.294453 know_the_time-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-18 16:02:11.000000 know_the_time-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 17:23:14.283424 know_the_time-0.0.2/know_the_time/
+-rw-rw-rw-   0        0        0      781 2023-07-20 17:22:25.000000 know_the_time-0.0.2/know_the_time/__init__.py
+-rw-rw-rw-   0        0        0    12701 2023-07-17 23:07:38.000000 know_the_time-0.0.2/know_the_time/know_the_time.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:23:14.292455 know_the_time-0.0.2/know_the_time.egg-info/
+-rw-rw-rw-   0        0        0     1118 2023-07-20 17:23:14.000000 know_the_time-0.0.2/know_the_time.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-20 17:23:14.000000 know_the_time-0.0.2/know_the_time.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 17:23:14.000000 know_the_time-0.0.2/know_the_time.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-20 17:23:14.000000 know_the_time-0.0.2/know_the_time.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 17:23:14.295453 know_the_time-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2023-07-20 17:22:17.000000 know_the_time-0.0.2/setup.py
```

### Comparing `know_the_time-0.0.1/LICENSE` & `know_the_time-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `know_the_time-0.0.1/PKG-INFO` & `know_the_time-0.0.2/know_the_time.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: know_the_time
-Version: 0.0.1
+Name: know-the-time
+Version: 0.0.2
 Summary: Get the time in different formats. Quickly available time stamps, dates, etc. are available useing functions. - makes `datetime` more available.
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `know_the_time-0.0.1/know_the_time/__init__.py` & `know_the_time-0.0.2/know_the_time/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .know_the_time import (
-    time_delta_prettystring,
-    time_delta_prettystring2,
+    get_time_delta_prettystring,
+    get_time_delta_prettystring2,
     get_year,
     get_month,
     get_month_3_characters_eng,
     get_month_name_eng,
     get_years_day,
     get_months_day,
     get_weaks_day,
@@ -25,8 +25,8 @@
     get_time_stamp_s,
     get_time_stamp_date,
     date_to_total_seconds,
     total_seconds_to_date,
 )
 
 
-__version__ = "0.0.8"
+__version__ = "0.0.2"
```

### Comparing `know_the_time-0.0.1/know_the_time/know_the_time.py` & `know_the_time-0.0.2/know_the_time/know_the_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from math import floor
 from time import time, localtime
 
 
-def time_delta_prettystring(
+def get_time_delta_prettystring(
     start: float,
     end: float = None,
     start_is_delta: bool = False,
     include_milliseconds: bool = False,
 ):
     """Get the time difference in the form of hours:minutes:seconds{:milliseconds}
 
@@ -51,15 +51,15 @@
 
     if not include_milliseconds:
         return f"{hours}:{minutes}:{seconds}"
     else:
         return f"{hours}:{minutes}:{seconds}:{milliseconds}"
 
 
-def time_delta_prettystring2(
+def get_time_delta_prettystring2(
     start: float,
     end: float = None,
     start_is_delta: bool = False,
     include_milliseconds: bool = False,
     zeros: bool = True,
     long_units: bool = False,
 ):
@@ -269,22 +269,26 @@
         str_minute = "0" + str_minute
     while len(str_second) < 2:
         str_second = "0" + str_second
     return f"{str_hour}:{str_minute}:{str_second}"
 
 
 def get_time_stamp(
-    point_of_time: float,
+    point_of_time: float = None,
     zeros: bool = True,
+    seperator: str = "-",
+    date_time_seperator: str = " - ",
 ) -> str:
     """
     Get a time stamp formated like: 'year-month-day - hour-minute-second-millisecond' for example '2023-06-18 - 17-52-42-446'
 
     0 before the number (e.g. june -> 06) can be trashed by setting zeros to `False`
     """
+    if point_of_time == None:
+        point_of_time = time()
     str_months_day, str_month = str(get_months_day(point_of_time)), str(
         get_month(point_of_time)
     )
     if zeros:
         while len(str_months_day) < 2:
             str_months_day = "0" + str_months_day
         while len(str_month) < 2:
@@ -300,26 +304,30 @@
             str_hour = "0" + str_hour
         while len(str_minute) < 2:
             str_minute = "0" + str_minute
         while len(str_second) < 2:
             str_second = "0" + str_second
         while len(str_millisecond) < 3:
             str_millisecond = "0" + str_millisecond
-    return f"{get_year(point_of_time)}-{str_month}-{str_months_day} - {str_hour}-{str_minute}-{str_second}-{str_millisecond}"
+    return str(get_year(point_of_time)) + seperator + str_month + seperator + str_months_day + date_time_seperator + str_hour + seperator + str_minute + seperator + str_second + seperator + str_millisecond
 
 
 def get_time_stamp_s(
-    point_of_time: float,
+    point_of_time: float = None,
     zeros: bool = True,
+    seperator: str = "-",
+    date_time_seperator: str = " - ",
 ) -> str:
     """
     Get a time stamp formated like: 'year-month-day - hour-minute-second' for example '2023-06-18 - 17-52-42'
 
     0 before the number (e.g. june -> 06) can be trashed by setting zeros to `False`
     """
+    if point_of_time == None:
+        point_of_time = time()
     str_months_day, str_month = str(get_months_day(point_of_time)), str(
         get_month(point_of_time)
     )
     if zeros:
         while len(str_months_day) < 2:
             str_months_day = "0" + str_months_day
         while len(str_month) < 2:
@@ -332,26 +340,29 @@
     if zeros:
         while len(str_hour) < 2:
             str_hour = "0" + str_hour
         while len(str_minute) < 2:
             str_minute = "0" + str_minute
         while len(str_second) < 2:
             str_second = "0" + str_second
-    return f"{get_year(point_of_time)}-{str_month}-{str_months_day} - {str_hour}-{str_minute}-{str_second}"
+    return str(get_year(point_of_time)) + seperator + str_month + seperator + str_months_day + date_time_seperator + str_hour + seperator + str_minute + seperator + str_second
 
 
 def get_time_stamp_date(
-    point_of_time: float,
+    point_of_time: float = None,
     zeros: bool = True,
+    seperator: str = "-",
 ) -> str:
     """
     Get a time stamp formated like: 'year-month-day' for example '2023-06-18'
 
     0 before the number (e.g. june -> 06) can be trashed by setting zeros to `False`
     """
+    if point_of_time == None:
+        point_of_time = time()
     str_months_day, str_month = str(get_months_day(point_of_time)), str(
         get_month(point_of_time)
     )
     if zeros:
         while len(str_months_day) < 2:
             str_months_day = "0" + str_months_day
         while len(str_month) < 2:
@@ -364,15 +375,15 @@
     if zeros:
         while len(str_hour) < 2:
             str_hour = "0" + str_hour
         while len(str_minute) < 2:
             str_minute = "0" + str_minute
         while len(str_second) < 2:
             str_second = "0" + str_second
-    return f"{get_year(point_of_time)}-{str_month}-{str_months_day}"
+    return str(get_year(point_of_time)) + seperator + str_month + seperator + str_months_day
 
 
 def date_to_total_seconds(day, month, year, hour, minute, second):
     dt = datetime.datetime(year, month, day, hour, minute, second)
     return dt.timestamp()
```

### Comparing `know_the_time-0.0.1/know_the_time.egg-info/PKG-INFO` & `know_the_time-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: know-the-time
-Version: 0.0.1
+Name: know_the_time
+Version: 0.0.2
 Summary: Get the time in different formats. Quickly available time stamps, dates, etc. are available useing functions. - makes `datetime` more available.
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `know_the_time-0.0.1/setup.py` & `know_the_time-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 DESCRIPTION = (
     "Get the time in different formats. Quickly available time stamps, dates, etc. are available useing functions. - makes `datetime` more available."
 )
 
 # Setting up
 setup(
     name="know_the_time",
-    version="0.0.1",
+    version="0.0.2",
     author="André Herber",
     author_email="andre.herber.programming@gmail.com",
     # url="https://github.com/ICreedenI/know_the_time",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

