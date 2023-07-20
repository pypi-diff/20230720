# Comparing `tmp/pwforecast-1.1.3.tar.gz` & `tmp/pwforecast-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwforecast-1.1.3.tar", last modified: Sat Jul 15 21:47:03 2023, max compression
+gzip compressed data, was "pwforecast-1.1.4.tar", last modified: Thu Jul 20 08:14:06 2023, max compression
```

## Comparing `pwforecast-1.1.3.tar` & `pwforecast-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:47:03.624245 pwforecast-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-15 21:46:52.000000 pwforecast-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-15 21:47:03.624245 pwforecast-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-15 21:46:52.000000 pwforecast-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:47:03.624245 pwforecast-1.1.3/pwforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-15 21:47:03.000000 pwforecast-1.1.3/pwforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-15 21:47:03.000000 pwforecast-1.1.3/pwforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:47:03.000000 pwforecast-1.1.3/pwforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 21:47:03.000000 pwforecast-1.1.3/pwforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 21:47:03.000000 pwforecast-1.1.3/pwforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18399 2023-07-15 21:46:52.000000 pwforecast-1.1.3/pwforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 21:47:03.624245 pwforecast-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-15 21:46:52.000000 pwforecast-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:14:06.626301 pwforecast-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 08:13:51.000000 pwforecast-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-20 08:14:06.626301 pwforecast-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-20 08:13:51.000000 pwforecast-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:14:06.626301 pwforecast-1.1.4/pwforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 08:14:06.000000 pwforecast-1.1.4/pwforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-07-20 08:13:51.000000 pwforecast-1.1.4/pwforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:14:06.626301 pwforecast-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 08:13:51.000000 pwforecast-1.1.4/setup.py
```

### Comparing `pwforecast-1.1.3/LICENSE` & `pwforecast-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pwforecast-1.1.3/PKG-INFO` & `pwforecast-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python module to charge/discharge Tesla Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pwforecast-1.1.3/README.md` & `pwforecast-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pwforecast-1.1.3/pwforecast.egg-info/PKG-INFO` & `pwforecast-1.1.4/pwforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python module to charge/discharge Tesla Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pwforecast-1.1.3/pwforecast.py` & `pwforecast-1.1.4/pwforecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,16 +190,16 @@
         assert len(battery_list) == 1, 'More than one battery list returned!'
         battery = battery_list[0]
 
         battery_data = battery.get_battery_data()
         total_pack_energy = battery_data['total_pack_energy']
 
         # calculate available energy.
-        availability_factor = (self.visible_pack_energy
-                               + self.discharge_efficiency) / 2
+        factors = [self.visible_pack_energy, self.discharge_efficiency]
+        availability_factor = sum(factors) - (len(factors) - 1)
         available_pack_energy = total_pack_energy * availability_factor
 
         # fill the Powerwall until required energy is satisfied.
         available_energy = forecast_production
         charge_percent = self.min_reserve_off_peak_rate
         pack_energy_increment = available_pack_energy / 100
         while available_energy < self.required_energy_peak_rate:
```

### Comparing `pwforecast-1.1.3/setup.py` & `pwforecast-1.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # read the contents of README file
 this_directory = Path(__file__).parent
 readme = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pwforecast',
-    version='1.1.3',
+    version='1.1.4',
     author='Tim Hawker',
     license='MIT',
     url='https://github.com/timhawker/pwforecast',
     description=('A Python module to charge/discharge Tesla Powerwall based '
                  'on solar forecast and peak/off peak tariffs.'),
     long_description_content_type='text/markdown',
     long_description=readme,
```

