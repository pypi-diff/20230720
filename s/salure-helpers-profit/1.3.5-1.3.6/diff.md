# Comparing `tmp/salure_helpers_profit-1.3.5.tar.gz` & `tmp/salure_helpers_profit-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-1.3.5.tar", last modified: Thu Jun 29 12:21:53 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-1.3.6.tar", last modified: Thu Jul 20 16:21:17 2023, max compression
```

## Comparing `salure_helpers_profit-1.3.5.tar` & `salure_helpers_profit-1.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   138891 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 12:21:53.000000 salure_helpers_profit-1.3.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-29 12:21:30.000000 salure_helpers_profit-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   139049 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:21:17.000000 salure_helpers_profit-1.3.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-20 16:21:02.000000 salure_helpers_profit-1.3.6/setup.py
```

### Comparing `salure_helpers_profit-1.3.5/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-1.3.6/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.5/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-1.3.6/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.5/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-1.3.6/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-1.3.5/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-1.3.6/salure_helpers/profit/profit_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1300,15 +1300,15 @@
         allowed_fields_contract = ['end_date_contract', 'seniority_date', 'date_in_service_original', 'probation_period_code', 'end_date_probation_period', 'contract_chain_code', 'start_date_contract_chain']
 
         # function fields
         required_fields_function = ['organizational_unit', 'date_effective', 'function_id', 'costcenter', 'costcarrier']
 
         # schedule fields
         required_fields_schedule = ['weekly_hours', 'parttime_percentage']
-        allowed_fields_schedule = ['changing_work_pattern', 'days_per_week', 'fte', 'type_of_schedule']
+        allowed_fields_schedule = ['changing_work_pattern', 'days_per_week', 'fte', 'type_of_schedule', 'on-call_contract']
 
         # salary fields
         required_fields_salary = ['type_of_salary']
         allowed_fields_salary = ['step', 'salary_scale', 'salary_scale_type', 'function_scale', 'function_scale_type', 'salary_year',
                                  'net_salary', 'apply_timetable', 'amount']
 
         allowed_fields = allowed_fields_person + allowed_fields_salary + allowed_fields_schedule + allowed_fields_contract + allowed_fields_address
@@ -1504,14 +1504,15 @@
 
         # Add overload fields to the base of the schedule data
         fields_to_update_schedule = {}
         fields_to_update_schedule.update({"StPa": data['changing_work_pattern']}) if 'changing_work_pattern' in data else fields_to_update_schedule
         fields_to_update_schedule.update({"DyWk": data['days_per_week']}) if 'days_per_week' in data else fields_to_update_schedule
         fields_to_update_schedule.update({"Ft": data['fte']}) if 'fte' in data else fields_to_update_schedule
         fields_to_update_schedule.update({"EtTy": data['type_of_schedule']}) if 'type_of_schedule' in data else fields_to_update_schedule
+        fields_to_update_schedule.update({"ClAg": data['on-call_contract']}) if 'on-call_contract' in data else fields_to_update_schedule
         if overload_fields is not None and 'schedule' in overload_fields.keys():
             fields_to_update_schedule.update(overload_fields['schedule'])
         # Update the request body with update fields
         body['AfasEmployee']['Element']['Objects']['AfasTimeTable']['Element']['Fields'].update(fields_to_update_schedule)
 
         # Add fields that you want to update a dict (adding to body itself is too much text)
         fields_to_update_organisational_unit = {}
```

### Comparing `salure_helpers_profit-1.3.5/setup.py` & `salure_helpers_profit-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='1.3.5',
+    version='1.3.6',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

