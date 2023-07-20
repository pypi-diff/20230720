# Comparing `tmp/circular-dict-1.5.tar.gz` & `tmp/circular-dict-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circular-dict-1.5.tar", last modified: Tue Jun 20 08:15:53 2023, max compression
+gzip compressed data, was "circular-dict-1.6.tar", last modified: Thu Jul 20 08:21:57 2023, max compression
```

## Comparing `circular-dict-1.5.tar` & `circular-dict-1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:15:53.700155 circular-dict-1.5/
--rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.5/LICENSE
--rw-rw-rw-   0        0        0     5925 2023-06-20 08:15:53.699152 circular-dict-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4258 2023-06-20 08:15:45.000000 circular-dict-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 08:15:53.666321 circular-dict-1.5/circular_dict/
--rw-rw-rw-   0        0        0     4798 2023-06-19 23:50:27.000000 circular-dict-1.5/circular_dict/CircularDict.py
--rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.5/circular_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:15:53.696617 circular-dict-1.5/circular_dict.egg-info/
--rw-rw-rw-   0        0        0     5925 2023-06-20 08:15:53.000000 circular-dict-1.5/circular_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-20 08:15:53.000000 circular-dict-1.5/circular_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:15:53.000000 circular-dict-1.5/circular_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-20 08:15:53.000000 circular-dict-1.5/circular_dict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 08:15:53.701152 circular-dict-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1863 2023-06-20 08:15:45.000000 circular-dict-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:21:57.339483 circular-dict-1.6/
+-rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.6/LICENSE
+-rw-rw-rw-   0        0        0     5925 2023-07-20 08:21:57.338034 circular-dict-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4258 2023-06-20 08:15:45.000000 circular-dict-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 08:21:57.289039 circular-dict-1.6/circular_dict/
+-rw-rw-rw-   0        0        0     4955 2023-07-20 07:40:50.000000 circular-dict-1.6/circular_dict/CircularDict.py
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.6/circular_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:21:57.335916 circular-dict-1.6/circular_dict.egg-info/
+-rw-rw-rw-   0        0        0     5925 2023-07-20 08:21:57.000000 circular-dict-1.6/circular_dict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-20 08:21:57.000000 circular-dict-1.6/circular_dict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:21:57.000000 circular-dict-1.6/circular_dict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-20 08:21:57.000000 circular-dict-1.6/circular_dict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 08:21:57.339483 circular-dict-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1863 2023-07-20 08:20:16.000000 circular-dict-1.6/setup.py
```

### Comparing `circular-dict-1.5/LICENSE` & `circular-dict-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `circular-dict-1.5/PKG-INFO` & `circular-dict-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular-dict
-Version: 1.5
+Version: 1.6
 Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
 Home-page: https://github.com/Eric-Canas/CircularDict
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `circular-dict-1.5/README.md` & `circular-dict-1.6/README.md`

 * *Files identical despite different names*

### Comparing `circular-dict-1.5/circular_dict/CircularDict.py` & `circular-dict-1.6/circular_dict/CircularDict.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,21 @@
             assert self.current_size <= self.maxsize_bytes, f"currentsize must be less than or equal to maxsize. currentsize={self.current_size}, maxsize={self.maxsize_bytes}"
 
         if self.maxlen is not None:
             assert len(self) <= self.maxlen, f"len(self) must be less than or equal to self.maxlen. len(self)={len(self)}, self.maxlen={self.maxlen}"
 
         return (self.maxlen is not None and len(self) == self.maxlen) or (self.maxsize_bytes is not None and self.current_size == self.maxsize_bytes)
 
+    def clear(self):
+        """
+        Remove all items from the dictionary.
+        """
+        super().clear()
+        self.current_size = 0
+
     def __setitem__(self, key: Any, value: Any):
         """
         Set an item in the dictionary. If the key already exists, it will update the value.
         If the dictionary exceeds maxlen or maxsize, it will remove the oldest item until it no longer does.
 
         :param key: Any. Key to set or update. (It must be hashable)
         :param value: Any. Value to associate with the key.
@@ -99,8 +106,9 @@
         Delete an item from the dictionary.
 
         :param key: Any. The key of the item to delete.
         """
         if key in self:
             value = self[key]
             self.current_size -= sys.getsizeof(key) + sys.getsizeof(value)
-            OrderedDict.__delitem__(self, key)
+            OrderedDict.__delitem__(self, key)
+
```

### Comparing `circular-dict-1.5/circular_dict.egg-info/PKG-INFO` & `circular-dict-1.6/circular_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular-dict
-Version: 1.5
+Version: 1.6
 Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
 Home-page: https://github.com/Eric-Canas/CircularDict
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `circular-dict-1.5/setup.py` & `circular-dict-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='circular-dict',
-    version='1.5',
+    version='1.6',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/CircularDict',
     description='CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. '
                 'Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. '
                 'This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor '
                 'the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. ',
```

