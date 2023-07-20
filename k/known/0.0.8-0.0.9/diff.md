# Comparing `tmp/known-0.0.8.tar.gz` & `tmp/known-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "known-0.0.8.tar", last modified: Fri Jul  7 20:49:50 2023, max compression
+gzip compressed data, was "known-0.0.9.tar", last modified: Thu Jul 20 14:17:27 2023, max compression
```

## Comparing `known-0.0.8.tar` & `known-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 20:49:50.420099 known-0.0.8/
--rw-rw-rw-   0        0        0     1102 2023-01-13 14:13:36.000000 known-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      263 2023-07-07 20:49:50.420099 known-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-03-31 14:51:15.000000 known-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-07 20:49:50.404453 known-0.0.8/module/
-drwxrwxrwx   0        0        0        0 2023-07-07 20:49:50.404453 known-0.0.8/module/known/
--rw-rw-rw-   0        0        0      453 2023-07-07 20:48:30.000000 known-0.0.8/module/known/__init__.py
--rw-rw-rw-   0        0        0    26381 2023-07-07 20:43:11.000000 known-0.0.8/module/known/basic.py
--rw-rw-rw-   0        0        0     4988 2023-07-07 20:47:33.000000 known-0.0.8/module/known/imgu.py
--rw-rw-rw-   0        0        0    10284 2023-07-01 18:24:41.000000 known-0.0.8/module/known/mailer.py
--rw-rw-rw-   0        0        0     5849 2023-06-24 16:36:17.000000 known-0.0.8/module/known/store.py
-drwxrwxrwx   0        0        0        0 2023-07-07 20:49:50.420099 known-0.0.8/module/known.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-07 20:49:50.000000 known-0.0.8/module/known.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-07 20:49:50.000000 known-0.0.8/module/known.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 20:49:50.000000 known-0.0.8/module/known.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 20:49:50.000000 known-0.0.8/module/known.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 20:49:50.420099 known-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-07-07 20:48:08.000000 known-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:17:27.293120 known-0.0.9/
+-rw-rw-rw-   0        0        0     1102 2023-01-13 14:13:36.000000 known-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-20 14:17:27.293120 known-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-03-31 14:51:15.000000 known-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-20 14:17:27.266487 known-0.0.9/module/
+drwxrwxrwx   0        0        0        0 2023-07-20 14:17:27.290972 known-0.0.9/module/known/
+-rw-rw-rw-   0        0        0      453 2023-07-20 14:15:40.000000 known-0.0.9/module/known/__init__.py
+-rw-rw-rw-   0        0        0    26381 2023-07-07 20:43:11.000000 known-0.0.9/module/known/basic.py
+-rw-rw-rw-   0        0        0     6695 2023-07-08 08:36:04.000000 known-0.0.9/module/known/imgu.py
+-rw-rw-rw-   0        0        0    10365 2023-07-08 07:57:05.000000 known-0.0.9/module/known/mailer.py
+-rw-rw-rw-   0        0        0     5849 2023-06-24 16:36:17.000000 known-0.0.9/module/known/store.py
+drwxrwxrwx   0        0        0        0 2023-07-20 14:17:27.293120 known-0.0.9/module/known.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-20 14:17:27.000000 known-0.0.9/module/known.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-20 14:17:27.000000 known-0.0.9/module/known.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 14:17:27.000000 known-0.0.9/module/known.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 14:17:27.000000 known-0.0.9/module/known.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 14:17:27.293120 known-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-07-20 14:15:45.000000 known-0.0.9/setup.py
```

### Comparing `known-0.0.8/LICENSE` & `known-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `known-0.0.8/module/known/basic.py` & `known-0.0.9/module/known/basic.py`

 * *Files identical despite different names*

### Comparing `known-0.0.8/module/known/imgu.py` & `known-0.0.9/module/known/imgu.py`

 * *Files 23% similar despite different names*

```diff
@@ -49,26 +49,40 @@
         b,g,r,a = (self.i[row, col, :]/255 if normalize else self.i[row, col, :])
         return (r, g, b, a)
     
     def set_color_at(self, row:int, col:int, rgba:tuple, normalize=False): 
         if normalize: rgba = [int(x*255) for x in rgba]
         r,g,b,a = rgba
         self.i[row, col, :] = (b, r, g, a) 
-    
+
+    def set_color_in(self, start_row:int, start_col:int, n_rows:int, n_cols:int, rgba:tuple, normalize=False): 
+        if normalize: rgba = [int(x*255) for x in rgba]
+        r,g,b,a = rgba
+        self.i[start_row:start_row+n_rows, start_col:start_col+n_cols, :] = (b, r, g, a) 
 
     def set_hex_at(self, row:int, col:int, hex:str):
         if hex.startswith('#'): hex = hex[1:]
         hex = hex.upper()
         lenhex = len(hex)
         assert lenhex==6 or lenhex==8, f'expecting 6 or 8 chars but got {lenhex} :: {hex}'
         if lenhex==6: hex = 'FF' + hex # max alpha
         B,G,R,A = tuple(BaseConvert.int2base(num=BaseConvert.to_base_10(BaseConvert.SYM_HEX, hex), base=256, digs=4))
         return self.set_color_at(row,col,(R,G,B,A))
-    
-    
+
+    def set_hex_in(self, start_row:int, start_col:int, n_rows:int, n_cols:int, hex:str):
+        if hex.startswith('#'): hex = hex[1:]
+        hex = hex.upper()
+        lenhex = len(hex)
+        assert lenhex==6 or lenhex==8, f'expecting 6 or 8 chars but got {lenhex} :: {hex}'
+        if lenhex==6: hex = 'FF' + hex # max alpha
+        B,G,R,A = tuple(BaseConvert.int2base(num=BaseConvert.to_base_10(BaseConvert.SYM_HEX, hex), base=256, digs=4))
+        return self.set_color_in(start_row,start_col,n_rows,n_cols,(R,G,B,A))
+
+
+
     @staticmethod
     def save(pix, path):  
         return cv2.imwrite(path, pix.i)
 
     @staticmethod
     def load(path): 
         img =  cv2.imread(path, cv2.IMREAD_UNCHANGED)
@@ -93,14 +107,33 @@
         plt.figure(figsize=fs)
         plt.yticks([], [])
         plt.title(f'{rgba=}')
         plt.bar([f'{hexc}'], [1], color=color)
         plt.show()
         plt.close()
 
+    @staticmethod
+    def region(from_pix, start_row, start_col, n_rows, n_cols):
+        r""" creates a new class object from a rectangular region with upper left corner at (x,y) and size (w,h)"""
+        pix = __class__(n_rows, n_cols, False)
+        pix.i = np.copy(from_pix.i[start_row:start_row+n_rows, start_col:start_col+n_cols,  :])
+        return pix
+
+    @staticmethod
+    def copy_region(pix_from, start_row, start_col, n_rows, n_cols, pix_to, start_row_to, start_col_to):
+        pix_to.i[start_row_to:start_row_to+n_rows, start_col_to:start_col_to+n_cols,  :] = pix_from.i[start_row:start_row+n_rows, start_col:start_col+n_cols,  :]
+
+    @staticmethod
+    def copy(pix_from, pix_to): pix_to.i[:, :, :] = pix_from.i[:, :, :]
+
+    def clone(self):
+        pix = self.__class__(self.h, self.w, create=False)
+        pix.i = np.copy(self.i)
+        return pix
+        
 
 def graphfromimage(img_path:str, pixel_choice:str='first', dtype=None) -> ndarray:
     r""" 
     Covert an image to an array (1-Dimensional)
 
     :param img_path:        path of input image 
     :param pixel_choice:    choose from ``[ 'first', 'last', 'mid', 'mean' ]``
```

### Comparing `known-0.0.8/module/known/mailer.py` & `known-0.0.9/module/known/mailer.py`

 * *Files 5% similar despite different names*

```diff
@@ -218,18 +218,18 @@
     @staticmethod
     def load_pickle(path:str):
         r""" load pickle file to object """
         with open(path, 'rb') as f: o = pickle.load(f)
         return o
 
     @staticmethod
-    def str2bytes(s:str, encoding:str='raw_unicode_escape')->list: return [b for b in bytes(s, encoding)]
+    def str2bytes(s:str, encoding:str='raw_unicode_escape')->list: return [i+b+1 for i,b in enumerate(bytearray(s, encoding))] #list(bytearray(s, encoding))
 
     @staticmethod
-    def bytes2str(s, encoding:str='raw_unicode_escape')->str: return bytes.decode(bytes(s), encoding)
+    def bytes2str(s, encoding:str='raw_unicode_escape')->str: return bytes.decode(bytes([b-i-1 for i,b in enumerate(s)]), encoding)
 
     @staticmethod
     def save_login(path):
         r""" save your login credentials as pickle """
         __class__.save_pickle((  __class__.str2bytes(input('Enter Username')), __class__.str2bytes(input('Enter Password'))  ), path)
     
     @staticmethod
```

### Comparing `known-0.0.8/module/known/store.py` & `known-0.0.9/module/known/store.py`

 * *Files identical despite different names*

### Comparing `known-0.0.8/setup.py` & `known-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name =                      'known',
-    version =                   '0.0.8',
+    version =                   '0.0.9',
     url =                       'https://github.com/Nelson-iitp/known',
     author =                    'Nelson.S',
     author_email =              'mail.nelsonsharma@gmail.com',
     description =               'Module :: known',
     packages =                  ['known'],
     classifiers=                ['License :: OSI Approved :: MIT License'],
     package_dir =               { '' : 'module'},
```

