# Comparing `tmp/ndbioimage-2023.7.2.tar.gz` & `tmp/ndbioimage-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2023.7.2.tar", max compression
+gzip compressed data, was "ndbioimage-2023.7.3.tar", max compression
```

## Comparing `ndbioimage-2023.7.2.tar` & `ndbioimage-2023.7.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2023.7.2/LICENSE
--rw-r--r--   0        0        0     2356 2023-07-04 14:24:16.158015 ndbioimage-2023.7.2/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2023.7.2/ndbioimage/.DS_Store
--rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2023.7.2/ndbioimage/AiryScan.xml
--rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2023.7.2/ndbioimage/Elyra_test.xml
--rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2023.7.2/ndbioimage/Elyra_test2.xml
--rwxr-xr-x   0        0        0    56839 2023-07-11 15:09:16.954915 ndbioimage-2023.7.2/ndbioimage/__init__.py
--rw-r--r--   0        0        0     7736 2022-08-01 13:44:51.766744 ndbioimage-2023.7.2/ndbioimage/bf.py
--rw-r--r--   0        0        0     1749 2023-06-29 11:31:54.170380 ndbioimage-2023.7.2/ndbioimage/jvm.py
--rw-r--r--   0        0        0     8677 2023-05-25 09:24:53.290471 ndbioimage-2023.7.2/ndbioimage/ntransforms.py
--rw-r--r--   0        0        0      191 2023-07-11 08:09:24.299786 ndbioimage-2023.7.2/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8234 2023-07-06 14:55:39.578133 ndbioimage-2023.7.2/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    22926 2023-07-11 14:07:47.789813 ndbioimage-2023.7.2/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     1990 2023-06-02 11:04:25.198511 ndbioimage-2023.7.2/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6113 2023-07-05 08:19:10.133201 ndbioimage-2023.7.2/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     2657 2023-06-12 12:28:43.438524 ndbioimage-2023.7.2/ndbioimage/readers/tifread.py
--rwxr-xr-x   0        0        0      245 2022-08-16 10:57:07.482485 ndbioimage-2023.7.2/ndbioimage/test.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2023.7.2/ndbioimage/transform.txt
--rw-r--r--   0        0        0     9609 2023-05-24 14:11:27.082389 ndbioimage-2023.7.2/ndbioimage/transforms.py
--rw-r--r--   0        0        0      837 2023-07-11 15:20:02.399013 ndbioimage-2023.7.2/pyproject.toml
--rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 ndbioimage-2023.7.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2023.7.3/LICENSE
+-rw-r--r--   0        0        0     2356 2023-07-04 14:24:16.158015 ndbioimage-2023.7.3/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2023.7.3/ndbioimage/.DS_Store
+-rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2023.7.3/ndbioimage/AiryScan.xml
+-rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2023.7.3/ndbioimage/Elyra_test.xml
+-rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2023.7.3/ndbioimage/Elyra_test2.xml
+-rwxr-xr-x   0        0        0    57073 2023-07-12 08:27:13.585201 ndbioimage-2023.7.3/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     7736 2022-08-01 13:44:51.766744 ndbioimage-2023.7.3/ndbioimage/bf.py
+-rw-r--r--   0        0        0     1749 2023-06-29 11:31:54.170380 ndbioimage-2023.7.3/ndbioimage/jvm.py
+-rw-r--r--   0        0        0     8677 2023-05-25 09:24:53.290471 ndbioimage-2023.7.3/ndbioimage/ntransforms.py
+-rw-r--r--   0        0        0      191 2023-07-11 08:09:24.299786 ndbioimage-2023.7.3/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8234 2023-07-06 14:55:39.578133 ndbioimage-2023.7.3/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    22926 2023-07-11 14:07:47.789813 ndbioimage-2023.7.3/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     1990 2023-06-02 11:04:25.198511 ndbioimage-2023.7.3/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6125 2023-07-20 08:22:48.530994 ndbioimage-2023.7.3/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     2657 2023-06-12 12:28:43.438524 ndbioimage-2023.7.3/ndbioimage/readers/tifread.py
+-rwxr-xr-x   0        0        0      245 2022-08-16 10:57:07.482485 ndbioimage-2023.7.3/ndbioimage/test.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2023.7.3/ndbioimage/transform.txt
+-rw-r--r--   0        0        0     9609 2023-05-24 14:11:27.082389 ndbioimage-2023.7.3/ndbioimage/transforms.py
+-rw-r--r--   0        0        0      837 2023-07-20 08:22:48.954994 ndbioimage-2023.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3411 1970-01-01 00:00:00.000000 ndbioimage-2023.7.3/PKG-INFO
```

### Comparing `ndbioimage-2023.7.2/LICENSE` & `ndbioimage-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/README.md` & `ndbioimage-2023.7.3/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/.DS_Store` & `ndbioimage-2023.7.3/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/AiryScan.xml` & `ndbioimage-2023.7.3/ndbioimage/AiryScan.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/Elyra_test.xml` & `ndbioimage-2023.7.3/ndbioimage/Elyra_test.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/Elyra_test2.xml` & `ndbioimage-2023.7.3/ndbioimage/Elyra_test2.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/__init__.py` & `ndbioimage-2023.7.3/ndbioimage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,14 +517,16 @@
         self.cyllens = ['None', 'None']
         self.duolink = 'None'
         self.detector = [0, 1]
         self.track = [0]
         self.cache = DequeDict(16)
         self._frame_decorator = None
         self.frameoffset = 0, 0  # how far apart the centers of frame and sensor are
+        self.flags = dict(C_CONTIGUOUS=False, F_CONTIGUOUS=False, OWNDATA=False, WRITEABLE=False,
+                          ALIGNED=False, WRITEBACKIFCOPY=False, UPDATEIFCOPY=False)
 
         self.open()
 
         # extract some metadata from ome
         instrument = self.ome.instruments[0] if self.ome.instruments else None
         image = self.ome.images[0]
         pixels = image.pixels
@@ -717,15 +719,15 @@
              f"series/pos:    {self.series}",
              f"reader:        {self.__class__.__module__.split('.')[-1]}",
              f"shape ({self.axes}):".ljust(15) + f"{' x '.join(str(i) for i in self.shape)}"]
         if self.pxsize_um:
             s.append(f'pixel size:    {1000 * self.pxsize_um:.2f} nm')
         if self.zstack and self.deltaz_um:
             s.append(f'z-interval:    {1000 * self.deltaz_um:.2f} nm')
-        if self.exposuretime_s:
+        if self.exposuretime_s and not all(e is None for e in self.exposuretime_s):
             s.append(f'exposuretime:  {self.exposuretime_s[0]:.2f} s')
         if self.timeseries and self.timeinterval:
             s.append(f'time interval: {self.timeinterval:.3f} s')
         if self.binning:
             s.append('binning:       {}x{}'.format(*self.binning))
         if self.laserwavelengths:
             s.append('laser colors:  ' + ' | '.join([' & '.join(len(w)*('{:.0f}',)).format(*w)
```

### Comparing `ndbioimage-2023.7.2/ndbioimage/bf.py` & `ndbioimage-2023.7.3/ndbioimage/bf.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/jvm.py` & `ndbioimage-2023.7.3/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/ntransforms.py` & `ndbioimage-2023.7.3/ndbioimage/ntransforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/readers/bfread.py` & `ndbioimage-2023.7.3/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/readers/cziread.py` & `ndbioimage-2023.7.3/ndbioimage/readers/cziread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/readers/ndread.py` & `ndbioimage-2023.7.3/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/readers/seqread.py` & `ndbioimage-2023.7.3/ndbioimage/readers/seqread.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 class Reader(Imread, ABC):
     priority = 10
 
     @staticmethod
     def _can_open(path):
-        return isinstance(path, Path) and path.suffix == ""
+        return isinstance(path, Path) and path.is_dir()
 
     @cached_property
     def ome(self):
         ome = model.OME()
         with tifffile.TiffFile(self.filedict[0, 0, 0]) as tif:
             metadata = {key: yaml.safe_load(value) for key, value in tif.pages[0].tags[50839].value.items()}
         ome.experimenters.append(
@@ -103,15 +103,15 @@
                     id=f"Channel:{c}", name=pattern_c.findall(self.filedict[c, 0, 0].stem)[0],
                     detector_settings=model.DetectorSettings(
                         id="Detector:0", binning=metadata["Info"]["Hamamatsu_sCMOS-Binning"]),
                     filter_set_ref=model.FilterSetRef(id='FilterSet:0')))
         return ome
 
     def open(self):
-        if not self.path.name.startswith("Pos"):
+        if re.match(r'(?:\d+\-)?Pos.*', self.path.name) is None:
             path = self.path / f"Pos{self.series}"
         else:
             path = self.path
 
         filelist = sorted([file for file in path.iterdir() if re.search(r'^img_\d{3,}.*\d{3,}.*\.tif$', file.name)])
         with tifffile.TiffFile(self.path / filelist[0]) as tif:
             metadata = {key: yaml.safe_load(value) for key, value in tif.pages[0].tags[50839].value.items()}
```

### Comparing `ndbioimage-2023.7.2/ndbioimage/readers/tifread.py` & `ndbioimage-2023.7.3/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/ndbioimage/transforms.py` & `ndbioimage-2023.7.3/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2023.7.2/pyproject.toml` & `ndbioimage-2023.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2023.7.2"
+version = "2023.7.3"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
```

### Comparing `ndbioimage-2023.7.2/PKG-INFO` & `ndbioimage-2023.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.8,<4.0
```

