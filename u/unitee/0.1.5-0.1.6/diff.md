# Comparing `tmp/unitee-0.1.5.tar.gz` & `tmp/unitee-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitee-0.1.5.tar", max compression
+gzip compressed data, was "unitee-0.1.6.tar", max compression
```

## Comparing `unitee-0.1.5.tar` & `unitee-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      448 2021-03-06 17:23:39.880698 unitee-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       36 2021-03-06 14:38:16.226561 unitee-0.1.5/unitee/__init__.py
--rw-r--r--   0        0        0      116 2021-02-25 22:29:45.498717 unitee-0.1.5/unitee/base_units.csv
--rw-r--r--   0        0        0      142 2021-02-27 14:32:51.442769 unitee-0.1.5/unitee/consts.csv
--rw-r--r--   0        0        0      717 2021-03-06 16:54:03.752144 unitee-0.1.5/unitee/derived_units.csv
--rw-r--r--   0        0        0      310 2021-02-13 16:45:27.482700 unitee-0.1.5/unitee/prefixes.csv
--rw-r--r--   0        0        0    18691 2021-03-06 17:21:10.163849 unitee-0.1.5/unitee/unitee.py
--rw-r--r--   0        0        0      510 2021-03-06 17:24:13.619764 unitee-0.1.5/setup.py
--rw-r--r--   0        0        0      423 2021-03-06 17:24:13.619764 unitee-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      448 2023-07-20 13:35:02.439057 unitee-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       36 2021-03-07 11:47:43.175048 unitee-0.1.6/unitee/__init__.py
+-rw-r--r--   0        0        0      116 2021-03-07 11:47:43.178040 unitee-0.1.6/unitee/base_units.csv
+-rw-r--r--   0        0        0      142 2021-03-07 11:47:43.179038 unitee-0.1.6/unitee/consts.csv
+-rw-r--r--   0        0        0      718 2023-07-20 11:53:40.514525 unitee-0.1.6/unitee/derived_units.csv
+-rw-r--r--   0        0        0      310 2021-03-07 11:47:43.181350 unitee-0.1.6/unitee/prefixes.csv
+-rw-r--r--   0        0        0    18699 2023-07-20 11:53:40.522513 unitee-0.1.6/unitee/unitee.py
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 unitee-0.1.6/PKG-INFO
```

### Comparing `unitee-0.1.5/unitee/derived_units.csv` & `unitee-0.1.6/unitee/derived_units.csv`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 lumen,lm,1.0,cd
 lux,lx,1.0,m-2.cd
 becquerel,Bq,1.0,s-1
 gray,Gy,1.0,m2.s-2
 sievert,Sv,1.0,m2.s-2
 katal,kat,1.0,s-1.mol
 gram,g,1e-3,kg
-electron volt,eV,1.602176565e-19,m.kg.s-2
+electron volt,eV,1.602176565e-19,m2.kg.s-2
 minute,min,60,s
 hour,h,3600,s
 day,d,86400,s
 litre,l,1e-3,m3
 astronomical unit,au,149597870700,m
 miles,mi,1609.344,m
```

### Comparing `unitee-0.1.5/unitee/unitee.py` & `unitee-0.1.6/unitee/unitee.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     base: _Quantity = None
     base_unit: bool = None
 
     def __init__(self, prefix: str=''):
         self.prefix = self.unit_system.prefixes[prefix]
         
     @property
-    def is_base(self):
+    def is_base(self) -> bool:
         return self.__class__.base_unit and self.prefix.symbol == ''
 
     @property
     def prefix_val(self) -> float:
         return self.prefix.val
         
     def as_quantity(self) -> _Quantity:
```

