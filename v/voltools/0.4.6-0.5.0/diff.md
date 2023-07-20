# Comparing `tmp/voltools-0.4.6.tar.gz` & `tmp/voltools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/voltools-0.4.6.tar", last modified: Thu Jun 10 10:03:31 2021, max compression
+gzip compressed data, was "voltools-0.5.0.tar", last modified: Thu Jul 20 14:18:47 2023, max compression
```

## Comparing `voltools-0.4.6.tar` & `voltools-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-10 10:03:31.000000 voltools-0.4.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2021-06-10 10:03:08.000000 voltools-0.4.6/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       42 2021-06-10 10:03:08.000000 voltools-0.4.6/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     6507 2021-06-10 10:03:31.000000 voltools-0.4.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5869 2021-06-10 10:03:08.000000 voltools-0.4.6/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-10 10:03:31.000000 voltools-0.4.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2021-06-10 10:03:08.000000 voltools-0.4.6/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-10 10:03:31.000000 voltools-0.4.6/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2614 2021-06-10 10:03:08.000000 voltools-0.4.6/tests/benchmark.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2188 2021-06-10 10:03:08.000000 voltools-0.4.6/tests/test_devices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2021-06-10 10:03:08.000000 voltools-0.4.6/tests/test_scripts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2021-06-10 10:03:08.000000 voltools-0.4.6/tests/test_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2021-06-10 10:03:08.000000 voltools-0.4.6/tests/test_transforms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2021-06-10 10:03:08.000000 voltools-0.4.6/tests/test_volume.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools/
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools/kernels/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4483 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/kernels/bspline.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3070 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/kernels/helper_interpolation.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    37970 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/kernels/helper_math.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    12038 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/transforms.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)      349 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4444 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/utils/general.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5116 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/utils/matrices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      389 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/utils/mrc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6151 2021-06-10 10:03:08.000000 voltools-0.4.6/voltools/volume.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6507 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      623 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-06-10 10:03:31.000000 voltools-0.4.6/voltools.egg-info/top_level.txt
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.826735 voltools-0.5.0/
+-rw-r--r--   0 ilya       (501) staff       (20)     1050 2022-03-11 21:56:02.000000 voltools-0.5.0/LICENSE.md
+-rw-r--r--   0 ilya       (501) staff       (20)       42 2022-03-11 21:56:02.000000 voltools-0.5.0/MANIFEST.in
+-rw-r--r--   0 ilya       (501) staff       (20)     6501 2023-07-20 14:18:47.826595 voltools-0.5.0/PKG-INFO
+-rw-r--r--   0 ilya       (501) staff       (20)     5869 2022-03-11 21:56:02.000000 voltools-0.5.0/README.md
+-rw-r--r--   0 ilya       (501) staff       (20)       38 2023-07-20 14:18:47.826778 voltools-0.5.0/setup.cfg
+-rw-r--r--   0 ilya       (501) staff       (20)     1073 2023-07-20 13:38:18.000000 voltools-0.5.0/setup.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.824139 voltools-0.5.0/tests/
+-rw-r--r--   0 ilya       (501) staff       (20)     2614 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/benchmark.py
+-rw-r--r--   0 ilya       (501) staff       (20)     2188 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_devices.py
+-rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_scripts.py
+-rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_tools.py
+-rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_transforms.py
+-rw-r--r--   0 ilya       (501) staff       (20)      127 2022-03-11 21:56:02.000000 voltools-0.5.0/tests/test_volume.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.824843 voltools-0.5.0/voltools/
+-rw-r--r--   0 ilya       (501) staff       (20)      196 2023-07-20 14:14:08.000000 voltools-0.5.0/voltools/__init__.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.825999 voltools-0.5.0/voltools/kernels/
+-rw-r--r--   0 ilya       (501) staff       (20)     4483 2022-03-11 21:56:02.000000 voltools-0.5.0/voltools/kernels/bspline.h
+-rw-r--r--   0 ilya       (501) staff       (20)     3070 2022-03-11 21:56:02.000000 voltools-0.5.0/voltools/kernels/helper_interpolation.h
+-rw-r--r--   0 ilya       (501) staff       (20)    37970 2022-03-11 21:56:02.000000 voltools-0.5.0/voltools/kernels/helper_math.h
+-rw-r--r--   0 ilya       (501) staff       (20)    11599 2023-07-20 13:36:34.000000 voltools-0.5.0/voltools/transforms.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.826430 voltools-0.5.0/voltools/utils/
+-rw-r--r--   0 ilya       (501) staff       (20)      316 2023-07-20 13:34:11.000000 voltools-0.5.0/voltools/utils/__init__.py
+-rw-r--r--   0 ilya       (501) staff       (20)     4075 2023-07-20 13:34:11.000000 voltools-0.5.0/voltools/utils/general.py
+-rw-r--r--   0 ilya       (501) staff       (20)     5116 2022-03-11 21:56:02.000000 voltools-0.5.0/voltools/utils/matrices.py
+-rw-r--r--   0 ilya       (501) staff       (20)     6219 2023-07-20 13:34:11.000000 voltools-0.5.0/voltools/volume.py
+drwxr-xr-x   0 ilya       (501) staff       (20)        0 2023-07-20 14:18:47.825595 voltools-0.5.0/voltools.egg-info/
+-rw-r--r--   0 ilya       (501) staff       (20)     6501 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/PKG-INFO
+-rw-r--r--   0 ilya       (501) staff       (20)      601 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/SOURCES.txt
+-rw-r--r--   0 ilya       (501) staff       (20)        1 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/dependency_links.txt
+-rw-r--r--   0 ilya       (501) staff       (20)        1 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/not-zip-safe
+-rw-r--r--   0 ilya       (501) staff       (20)       19 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/requires.txt
+-rw-r--r--   0 ilya       (501) staff       (20)        9 2023-07-20 14:18:47.000000 voltools-0.5.0/voltools.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `voltools-0.4.6/LICENSE.md` & `voltools-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voltools-0.4.6/PKG-INFO` & `voltools-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: voltools
-Version: 0.4.6
+Version: 0.5.0
 Summary: CUDA-accelerated 3D affine transformations for NumPy and CuPy
 Home-page: https://github.com/the-lay/voltools
 Author: the-lay
 Author-email: ilja.gubin@gmail.com
 License: MIT
 Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -113,9 +113,7 @@
                    scipy      np_transform   np_transform_out  cp_transform  cp_transform_out  static_vol  static_vol_out
 5, 5, 5           0.201232      4.528787          0.207631      0.195885          0.163193    0.109361         0.059611
 25, 25, 25        5.240529      0.332447          0.238356      0.217309          0.194111    0.138756         0.09321
 50, 50, 50       43.515086      0.804508          0.632981      0.560689          0.527334    0.474820         0.416062
 100, 100, 100   375.886700      4.232868          4.114524      3.454444          3.390018    3.091396         2.999451
 250, 250, 250  6189.052927     95.083083         94.479406     85.200392         84.435548    81.808363       80.959284
 ```
-
-
```

### Comparing `voltools-0.4.6/README.md` & `voltools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `voltools-0.4.6/setup.py` & `voltools-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         'gputil'
     ],
     packages=setuptools.find_packages(),
     include_package_data=True,
     zip_safe=False,
     test_suite='tests',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
     ]
 )
```

### Comparing `voltools-0.4.6/tests/benchmark.py` & `voltools-0.5.0/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `voltools-0.4.6/tests/test_devices.py` & `voltools-0.5.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `voltools-0.4.6/voltools/kernels/bspline.h` & `voltools-0.5.0/voltools/kernels/bspline.h`

 * *Files identical despite different names*

### Comparing `voltools-0.4.6/voltools/kernels/helper_interpolation.h` & `voltools-0.5.0/voltools/kernels/helper_interpolation.h`

 * *Files identical despite different names*

### Comparing `voltools-0.4.6/voltools/kernels/helper_math.h` & `voltools-0.5.0/voltools/kernels/helper_math.h`

 * *Files identical despite different names*

### Comparing `voltools-0.4.6/voltools/transforms.py` & `voltools-0.5.0/voltools/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,16 @@
               rotation: Union[Tuple[float, float, float], np.ndarray] = None,
               rotation_units: str = 'deg', rotation_order: str = 'rzxz',
               translation: Union[Tuple[float, float, float], np.ndarray] = None,
               center: Union[Tuple[float, float, float], np.ndarray] = None,
               interpolation: str = 'linear',
               reshape: bool = False,
               profile: bool = False,
-              output = None, device: str = 'cpu'):
+              output=None,
+              device: str = 'cpu'):
 
     if center is None:
         center = np.divide(np.subtract(volume.shape, 1), 2, dtype=np.float32)
 
     # passing just one float is uniform scaling
     if isinstance(scale, float):
         scale = (scale, scale, scale)
@@ -48,41 +49,44 @@
 
 
 def translate(volume: np.ndarray,
               translation: Tuple[float, float, float],
               interpolation: str = 'linear',
               reshape: bool = False,
               profile: bool = False,
-              output = None, device: str = 'cpu'):
+              output=None,
+              device: str = 'cpu'):
 
     m = translation_matrix(translation)
     return affine(volume, m, interpolation, reshape, profile, output, device)
 
 
 def shear(volume: np.ndarray,
           coefficients: Union[float, Tuple[float, float, float]],
           interpolation: str = 'linear',
           reshape: bool = False,
           profile: bool = False,
-          output = None, device: str = 'cpu'):
+          output=None,
+          device: str = 'cpu'):
 
     # passing just one float is uniform scaling
     if isinstance(coefficients, float):
         coefficients = (coefficients, coefficients, coefficients)
 
     m = shear_matrix(coefficients)
     return affine(volume, m, interpolation, reshape, profile, output, device)
 
 
 def scale(volume: np.ndarray,
           coefficients: Union[float, Tuple[float, float, float]],
           interpolation: str = 'linear',
           reshape: bool = False,
           profile: bool = False,
-          output = None, device: str = 'cpu'):
+          output=None,
+          device: str = 'cpu'):
 
     # passing just one float is uniform scaling
     if isinstance(coefficients, float):
         coefficients = (coefficients, coefficients, coefficients)
 
     m = scale_matrix(coefficients)
     return affine(volume, m, interpolation, reshape, profile, output, device)
@@ -91,26 +95,27 @@
 def rotate(volume: np.ndarray,
            rotation: Tuple[float, float, float],
            rotation_units: str = 'deg',
            rotation_order: str = 'rzxz',
            interpolation: str = 'linear',
            reshape: bool = False,
            profile: bool = False,
-           output = None, device: str = 'cpu'):
+           output=None,
+           device: str = 'cpu'):
 
     m = rotation_matrix(rotation=rotation, rotation_units=rotation_units, rotation_order=rotation_order)
     return affine(volume, m, interpolation, reshape, profile, output, device)
 
 
 def affine(volume: np.ndarray,
            transform_m: np.ndarray,
            interpolation: str = 'linear',
            reshape: bool = False,
            profile: bool = False,
-           output = None,
+           output=None,
            device: str = 'cpu'):
 
     if device not in AVAILABLE_DEVICES:
         raise ValueError(f'Unknown device ({device}), must be one of {AVAILABLE_DEVICES}')
 
     if device == 'cpu':
 
@@ -135,15 +140,20 @@
             # but we need to apply pad_before offset to transform_m get full volume
             transform_m = np.dot(transform_m, translation_matrix(pad_before, transform_m.dtype))
 
         else:
             output_shape = volume.shape
 
         # run affine transformation
-        output_vol = affine_transform(volume, transform_m, output_shape=output_shape, output=output, order=order, prefilter=prefilter)
+        output_vol = affine_transform(volume,
+                                      transform_m,
+                                      output_shape=output_shape,
+                                      output=output,
+                                      order=order,
+                                      prefilter=prefilter)
 
         if profile:
             t_end = time.time()
             time_took = (t_end - t_start) * 1000
             print(f'transform finished in {time_took:.3f}ms')
 
         if output is not None:
@@ -175,15 +185,15 @@
         arr = cp.cuda.texture.CUDAarray(ch, *volume_shape[::-1])  # CUDAArray: last dimension=fastest changing dimension
         res = cp.cuda.texture.ResourceDescriptor(cp.cuda.runtime.cudaResourceTypeArray, cuArr=arr)
         tex = cp.cuda.texture.TextureDescriptor((cp.cuda.runtime.cudaAddressModeBorder,
                                                  cp.cuda.runtime.cudaAddressModeBorder,
                                                  cp.cuda.runtime.cudaAddressModeBorder),
                                                 cp.cuda.runtime.cudaFilterModeLinear,
                                                 cp.cuda.runtime.cudaReadModeElementType)
-        texobj = cp.cuda.texture.TextureObject(res, tex)
+        tex_obj = cp.cuda.texture.TextureObject(res, tex)
 
         # prefilter if required and upload to texture
         if interpolation.startswith('filt_bspline'):
             volume = _bspline_prefilter(volume)
             arr.copy_from(volume)
         else:
             arr.copy_from(volume)
@@ -195,51 +205,34 @@
         dim_grid, dim_blocks = utils.compute_elementwise_launch_dims(volume_shape)
 
         if output is None:
             volume.fill(0.0)  # reuse input array
         else:
             volume = output
 
-        kernel(dim_grid, dim_blocks, (volume, texobj, xform, dims))
+        kernel(dim_grid, dim_blocks, (volume, tex_obj, xform, dims))
 
         if profile:
             t_end = stream.record()
             t_end.synchronize()
 
             time_took = cp.cuda.get_elapsed_time(t_start, t_end)
             print(f'transform finished in {time_took:.3f}ms')
 
         if output is None:
-            del texobj, xform, dims
+            del tex_obj, xform, dims
             return volume.get()
         else:
-            del texobj, xform, dims
+            del tex_obj, xform, dims
             return None
 
     else:
         raise ValueError(f'No instructions for {device}.')
 
 
-def oob_affine(volume: np.ndarray,
-               transform_m: np.ndarray,
-               interpolation: str = 'linear',
-               reshape: bool = False,
-               profile: bool = False,
-               output = None,
-               device: str = 'cpu'):
-
-    # oob affine is needed only for gpu
-    if device == 'cpu':
-        return affine(volume, transform_m, interpolation, reshape, profile, output, device)
-
-    # compute how big the volume will be after the transform
-    pad_before, pad_after, new_dims = utils.compute_post_transform_dimensions(volume.shape, transform_m)
-    memory_required = np.product(new_dims) * volume.itemsize * 2.1
-    # available_memory =
-
 def _get_transform_kernel(interpolation: str = 'linear'):
 
     if interpolation not in AVAILABLE_INTERPOLATIONS:
         raise ValueError(f'Interpolation must be one of {interpolation}')
 
     code = f'''
         #include "helper_math.h"
@@ -289,14 +282,15 @@
             }}
         }}
     '''
     incl_path = str((Path(__file__).parent / 'kernels').absolute())
     kernel = cp.RawKernel(code=code, name='transform', options=('-I', incl_path))
     return kernel
 
+
 def _bspline_prefilter(volume):
 
     code = f'''
         #include "helper_math.h"
         #include "bspline.h"
     '''
     incl_path = str((Path(__file__).parent / 'kernels').absolute())
```

### Comparing `voltools-0.4.6/voltools/utils/general.py` & `voltools-0.5.0/voltools/utils/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import string
-import random
-import sys
 import numpy as np
 from typing import Tuple
 import GPUtil
 try:
     import cupy
 except ImportError:
     pass
@@ -33,23 +30,14 @@
     dim_blocks = ((dim_x, dim_y, 1),
                   (dim_x, dim_y, 1),
                   (dim_x, dim_y, 1))
 
     return dim_grid, dim_blocks
 
 
-def compute_pervoxel_workgroup_dims(shape: Tuple[int, int, int]) -> Tuple[Tuple, Tuple]:
-    dim_grid = (shape[0] // 8 + 1 * (shape[0] % 8 != 0),
-                shape[1] // 8 + 1 * (shape[1] % 8 != 0),
-                shape[2] // 8 + 1 * (shape[2] % 8 != 0))
-    dim_blocks = (8, 8, 8)
-    return dim_grid, dim_blocks
-
-
-# @cupy.memoize()
 def compute_elementwise_launch_dims(shape: Tuple[int, int, int]) -> Tuple[Tuple[int, int, int], Tuple[int, int, int]]:
     device = cupy.cuda.device.Device()
     min_threads = device.attributes['WarpSize']
     max_threads = 128
     thread_blocks_per_mp = 8
     max_blocks = 4 * thread_blocks_per_mp * device.attributes['MultiProcessorCount']
     n = np.prod(shape).item()
@@ -71,24 +59,24 @@
     return (block_count, 1, 1), (threads_per_block, 1, 1)
 
 
 def get_available_devices():
 
     available_devices = ['cpu']
 
-    # get all available gpus
-    gpu_ids = GPUtil.getAvailable()
-
     # check if cupy is installed
     try:
         import cupy
 
         # add auto gpu
         available_devices.append('gpu')
 
+        # get all available gpus
+        gpu_ids = GPUtil.getAvailable()
+
         # add gpus to list of available devices
         for i in gpu_ids:
             available_devices.append(f'gpu:{i}')
 
     except ImportError:
         print('Warning: cupy is not found. Therefore, the only available device is "cpu".\n'
               'Please install cupy>=7.0.0b4:\npip install cupy>=7.0.0b4')
@@ -105,15 +93,15 @@
 
 
 # computes required padding before, after and new volume dimensions after transformation
 def compute_post_transform_dimensions(shape: Tuple[int, int, int], transform_m: np.ndarray) \
         -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
 
     # constructing volume bbox vertices matrix
-    a, b, c = shape # not using xyz to avoid confusion with axes
+    a, b, c = shape  # not using xyz to avoid confusion with axes
     boundaries = [[0, a, 0, a, 0, a, 0, a],
                   [0, 0, b, b, 0, 0, b, b],
                   [0, 0, 0, 0, c, c, c, c],
                   [1, 1, 1, 1, 1, 1, 1, 1]]
 
     # inverting transformation matrix to map from output to input
     try:
```

### Comparing `voltools-0.4.6/voltools/utils/matrices.py` & `voltools-0.5.0/voltools/utils/matrices.py`

 * *Files identical despite different names*

### Comparing `voltools-0.4.6/voltools/volume.py` & `voltools-0.5.0/voltools/volume.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     scale_matrix, shear_matrix, rotation_matrix, translation_matrix, transform_matrix, get_available_devices
 
 try:
     import cupy as cp
 except ImportError:
     pass
 
+
 class StaticVolume:
 
     def __init__(self, data: np.ndarray, interpolation: str = 'linear', device: str = 'gpu'):
 
         if data.ndim != 3:
             raise ValueError('Expected a 3D array')
 
@@ -92,59 +93,64 @@
 
     def transform(self, scale: Union[float, Tuple[float, float, float], np.ndarray] = None,
                   shear: Union[float, Tuple[float, float, float], np.ndarray] = None,
                   rotation: Union[Tuple[float, float, float], np.ndarray] = None,
                   rotation_units: str = 'deg', rotation_order: str = 'rzxz',
                   translation: Union[Tuple[float, float, float], np.ndarray] = None,
                   center: Union[Tuple[float, float, float], np.ndarray] = None,
-                  profile: bool = False, output = None) -> Union[np.ndarray, None]:
+                  profile: bool = False,
+                  output=None) -> Union[np.ndarray, None]:
 
         if center is None:
-            center = np.divide(np.subtract(volume.shape, 1), 2, dtype=np.float32)
+            center = np.divide(np.subtract(self.shape, 1), 2, dtype=np.float32)
 
         # passing just one float is uniform scaling
         if isinstance(scale, float):
             scale = (scale, scale, scale)
         if isinstance(shear, float):
             shear = (shear, shear, shear)
 
         m = transform_matrix(scale, shear, rotation, rotation_units, rotation_order,
                              translation, center)
         return self.affine(m, profile, output)
 
     def translate(self,
                   translation: Tuple[float, float, float],
-                  profile: bool = False, output = None) -> Union[np.ndarray, None]:
+                  profile: bool = False,
+                  output=None) -> Union[np.ndarray, None]:
 
         m = translation_matrix(translation)
         return self.affine(m, profile, output)
 
     def shear(self,
               coefficients: Union[float, Tuple[float, float, float]],
-              profile: bool = False, output = None) -> Union[np.ndarray, None]:
+              profile: bool = False,
+              output=None) -> Union[np.ndarray, None]:
 
         # passing just one float is uniform scaling
         if isinstance(coefficients, float):
             coefficients = (coefficients, coefficients, coefficients)
 
         m = shear_matrix(coefficients)
         return self.affine(m, profile, output)
 
     def scale(self,
               coefficients: Union[float, Tuple[float, float, float]],
-              profile: bool = False, output = None) -> Union[np.ndarray, None]:
+              profile: bool = False,
+              output=None) -> Union[np.ndarray, None]:
 
         # passing just one float is uniform scaling
         if isinstance(coefficients, float):
             coefficients = (coefficients, coefficients, coefficients)
 
         m = scale_matrix(coefficients)
         return self.affine(m, profile, output)
 
     def rotate(self,
                rotation: Tuple[float, float, float],
                rotation_units: str = 'deg',
                rotation_order: str = 'rzxz',
-               profile: bool = False, output = None) -> Union[np.ndarray, None]:
+               profile: bool = False,
+               output=None) -> Union[np.ndarray, None]:
 
         m = rotation_matrix(rotation=rotation, rotation_units=rotation_units, rotation_order=rotation_order)
         return self.affine(m, profile, output)
```

### Comparing `voltools-0.4.6/voltools.egg-info/PKG-INFO` & `voltools-0.5.0/voltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: voltools
-Version: 0.4.6
+Version: 0.5.0
 Summary: CUDA-accelerated 3D affine transformations for NumPy and CuPy
 Home-page: https://github.com/the-lay/voltools
 Author: the-lay
 Author-email: ilja.gubin@gmail.com
 License: MIT
 Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -113,9 +113,7 @@
                    scipy      np_transform   np_transform_out  cp_transform  cp_transform_out  static_vol  static_vol_out
 5, 5, 5           0.201232      4.528787          0.207631      0.195885          0.163193    0.109361         0.059611
 25, 25, 25        5.240529      0.332447          0.238356      0.217309          0.194111    0.138756         0.09321
 50, 50, 50       43.515086      0.804508          0.632981      0.560689          0.527334    0.474820         0.416062
 100, 100, 100   375.886700      4.232868          4.114524      3.454444          3.390018    3.091396         2.999451
 250, 250, 250  6189.052927     95.083083         94.479406     85.200392         84.435548    81.808363       80.959284
 ```
-
-
```

### Comparing `voltools-0.4.6/voltools.egg-info/SOURCES.txt` & `voltools-0.5.0/voltools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 voltools.egg-info/requires.txt
 voltools.egg-info/top_level.txt
 voltools/kernels/bspline.h
 voltools/kernels/helper_interpolation.h
 voltools/kernels/helper_math.h
 voltools/utils/__init__.py
 voltools/utils/general.py
-voltools/utils/matrices.py
-voltools/utils/mrc.py
+voltools/utils/matrices.py
```

