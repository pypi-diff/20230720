# Comparing `tmp/jampy-7.1.0.tar.gz` & `tmp/jampy-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jampy-7.1.0.tar", last modified: Mon Jun  5 17:20:37 2023, max compression
+gzip compressed data, was "jampy-7.2.0.tar", last modified: Thu Jul 20 18:41:23 2023, max compression
```

## Comparing `jampy-7.1.0.tar` & `jampy-7.2.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:20:37.984359 jampy-7.1.0/
--rw-rw-rw-   0        0        0    50165 2023-06-05 17:20:37.984359 jampy-7.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-05 17:20:37.921410 jampy-7.1.0/jampy/
--rw-rw-rw-   0        0        0    12746 2023-06-05 16:56:47.000000 jampy-7.1.0/jampy/CHANGELOG.rst
--rw-rw-rw-   0        0        0      442 2022-12-26 20:25:49.000000 jampy-7.1.0/jampy/LICENSE.txt
--rw-rw-rw-   0        0        0     3564 2022-10-02 22:25:04.000000 jampy-7.1.0/jampy/README.rst
--rw-rw-rw-   0        0        0       23 2023-06-05 17:20:30.000000 jampy-7.1.0/jampy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:20:37.984359 jampy-7.1.0/jampy/examples/
--rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.1.0/jampy/examples/__init__.py
--rw-rw-rw-   0        0        0     1019 2022-02-07 11:29:21.000000 jampy-7.1.0/jampy/examples/cappellari2020_table1.txt
--rw-rw-rw-   0        0        0     3060 2023-06-04 08:12:29.000000 jampy-7.1.0/jampy/examples/jam_axi_intr_example.py
--rw-rw-rw-   0        0        0     4517 2023-06-01 10:17:18.000000 jampy-7.1.0/jampy/examples/jam_axi_proj_example.py
--rw-rw-rw-   0        0        0     6915 2023-06-05 17:03:23.000000 jampy-7.1.0/jampy/examples/jam_black_hole_bayes_example.py
--rw-rw-rw-   0        0        0    10298 2023-06-05 17:02:41.000000 jampy-7.1.0/jampy/examples/jam_dark_halo_bayes_example.py
--rw-rw-rw-   0        0        0    10196 2023-06-04 08:26:08.000000 jampy-7.1.0/jampy/examples/jam_hernquist_model_example.py
--rw-rw-rw-   0        0        0     8544 2018-05-01 13:45:20.000000 jampy-7.1.0/jampy/examples/jam_mock_kinematics_black_hole.txt
--rw-rw-rw-   0        0        0     8592 2021-12-21 19:35:32.000000 jampy-7.1.0/jampy/examples/jam_mock_kinematics_dark_halo.txt
--rw-rw-rw-   0        0        0     2592 2023-05-31 18:23:57.000000 jampy-7.1.0/jampy/examples/jam_sph_proj_example.py
--rw-rw-rw-   0        0        0     2195 2023-06-05 17:01:53.000000 jampy-7.1.0/jampy/examples/mge_vcirc_example.py
--rw-rw-rw-   0        0        0    37662 2023-06-05 17:18:24.000000 jampy-7.1.0/jampy/jam_axi_intr.py
--rw-rw-rw-   0        0        0    48571 2023-06-05 17:18:24.000000 jampy-7.1.0/jampy/jam_axi_proj.py
--rw-rw-rw-   0        0        0     8141 2023-05-31 18:20:50.000000 jampy-7.1.0/jampy/jam_sph_intr.py
--rw-rw-rw-   0        0        0    29072 2023-05-31 18:20:50.000000 jampy-7.1.0/jampy/jam_sph_proj.py
--rw-rw-rw-   0        0        0     6547 2022-10-09 17:30:15.000000 jampy-7.1.0/jampy/mge_half_light_isophote.py
--rw-rw-rw-   0        0        0     3568 2019-10-24 18:03:59.000000 jampy-7.1.0/jampy/mge_radial_density.py
--rw-rw-rw-   0        0        0     3173 2019-06-12 10:26:52.000000 jampy-7.1.0/jampy/mge_radial_mass.py
--rw-rw-rw-   0        0        0     6845 2023-01-01 15:05:41.000000 jampy-7.1.0/jampy/mge_vcirc.py
--rw-rw-rw-   0        0        0    18603 2023-06-04 08:26:08.000000 jampy-7.1.0/jampy/quad1d.py
--rw-rw-rw-   0        0        0    12204 2023-01-01 15:01:54.000000 jampy-7.1.0/jampy/quad2d.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:20:37.953084 jampy-7.1.0/jampy.egg-info/
--rw-rw-rw-   0        0        0    50165 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      933 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-05 17:20:37.984359 jampy-7.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1750 2021-06-24 13:30:54.000000 jampy-7.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:41:23.656146 jampy-7.2.0/
+-rw-rw-rw-   0        0        0    50553 2023-07-20 18:41:23.656146 jampy-7.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 18:41:23.598747 jampy-7.2.0/jampy/
+-rw-rw-rw-   0        0        0    13168 2023-07-20 18:41:14.000000 jampy-7.2.0/jampy/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      398 2023-07-07 13:06:09.000000 jampy-7.2.0/jampy/LICENSE.txt
+-rw-rw-rw-   0        0        0     3564 2022-10-02 22:25:04.000000 jampy-7.2.0/jampy/README.rst
+-rw-rw-rw-   0        0        0       23 2023-07-20 18:40:10.000000 jampy-7.2.0/jampy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:41:23.656146 jampy-7.2.0/jampy/examples/
+-rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.2.0/jampy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1019 2022-02-07 11:29:21.000000 jampy-7.2.0/jampy/examples/cappellari2020_table1.txt
+-rw-rw-rw-   0        0        0     3060 2023-06-15 16:06:10.000000 jampy-7.2.0/jampy/examples/jam_axi_intr_example.py
+-rw-rw-rw-   0        0        0     4524 2023-07-16 14:17:21.000000 jampy-7.2.0/jampy/examples/jam_axi_proj_example.py
+-rw-rw-rw-   0        0        0     6915 2023-06-05 17:03:23.000000 jampy-7.2.0/jampy/examples/jam_black_hole_bayes_example.py
+-rw-rw-rw-   0        0        0    10298 2023-06-05 17:02:41.000000 jampy-7.2.0/jampy/examples/jam_dark_halo_bayes_example.py
+-rw-rw-rw-   0        0        0    10196 2023-06-21 10:58:03.000000 jampy-7.2.0/jampy/examples/jam_hernquist_model_example.py
+-rw-rw-rw-   0        0        0     8544 2018-05-01 13:45:20.000000 jampy-7.2.0/jampy/examples/jam_mock_kinematics_black_hole.txt
+-rw-rw-rw-   0        0        0     8592 2021-12-21 19:35:32.000000 jampy-7.2.0/jampy/examples/jam_mock_kinematics_dark_halo.txt
+-rw-rw-rw-   0        0        0     2592 2023-05-31 18:23:57.000000 jampy-7.2.0/jampy/examples/jam_sph_proj_example.py
+-rw-rw-rw-   0        0        0     2195 2023-06-05 17:01:53.000000 jampy-7.2.0/jampy/examples/mge_vcirc_example.py
+-rw-rw-rw-   0        0        0    35745 2023-06-21 12:51:09.000000 jampy-7.2.0/jampy/jam_axi_intr.py
+-rw-rw-rw-   0        0        0    48705 2023-06-18 18:06:40.000000 jampy-7.2.0/jampy/jam_axi_proj.py
+-rw-rw-rw-   0        0        0     5438 2023-07-05 09:54:32.000000 jampy-7.2.0/jampy/jam_axi_sersic_mass.py
+-rw-rw-rw-   0        0        0     8141 2023-05-31 18:20:50.000000 jampy-7.2.0/jampy/jam_sph_intr.py
+-rw-rw-rw-   0        0        0    29072 2023-05-31 18:20:50.000000 jampy-7.2.0/jampy/jam_sph_proj.py
+-rw-rw-rw-   0        0        0     6547 2022-10-09 17:30:15.000000 jampy-7.2.0/jampy/mge_half_light_isophote.py
+-rw-rw-rw-   0        0        0     3568 2019-10-24 18:03:59.000000 jampy-7.2.0/jampy/mge_radial_density.py
+-rw-rw-rw-   0        0        0     3173 2019-06-12 10:26:52.000000 jampy-7.2.0/jampy/mge_radial_mass.py
+-rw-rw-rw-   0        0        0     6845 2023-01-01 15:05:41.000000 jampy-7.2.0/jampy/mge_vcirc.py
+-rw-rw-rw-   0        0        0    19470 2023-06-13 12:02:24.000000 jampy-7.2.0/jampy/quad1d.py
+-rw-rw-rw-   0        0        0    13046 2023-06-18 17:52:36.000000 jampy-7.2.0/jampy/quad2d.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:41:23.630007 jampy-7.2.0/jampy.egg-info/
+-rw-rw-rw-   0        0        0    50553 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 18:41:23.000000 jampy-7.2.0/jampy.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-20 18:41:23.656146 jampy-7.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1750 2021-06-24 13:30:54.000000 jampy-7.2.0/setup.py
```

### Comparing `jampy-7.1.0/PKG-INFO` & `jampy-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jampy
-Version: 7.1.0
+Version: 7.2.0
 Summary: JamPy: Jeans Anisotropic Models for Galactic Dynamics
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -437,15 +437,15 @@
     PSF convolution is not performed.
 plot: bool
     When ``data is not None`` setting this keyword produces a plot with the
     data/model comparison at the end of the calculation.
 quiet: bool
     Set this keyword to avoid printing values on the console.
 rbh: float, optional
-    This keyword is ignored unless ``align='cyl'`` and `analytic_los=True`.
+    This keyword is ignored unless ``align='cyl'`` and ``analytic_los=True``.
     In all other cases JAM assume a point-like central black hole.
     This scalar gives the sigma in arcsec of the Gaussian approximating the
     central black hole of mass MBH [See Section 3.1.2 of `Cappellari (2008)`_]
     The gravitational potential is indistinguishable from a point source
     for ``radii > 2*rbh``, so the default ``rbh=0.01`` arcsec is appropriate
     in most current situations.
 
@@ -467,18 +467,18 @@
     with a first call to ``jam_axi_proj`` with PSF convolution, and the
     model predictions at large radii with a second call to ``jam_axi_proj``
     without PSF convolution.
 step: float, optional
     Spatial step for the model calculation and PSF convolution in arcsec.
     This value is automatically computed by default as
     ``step=max(sigmapsf,pixsize/2)/4``. It is assumed that when ``pixsize``
-    or ``sigmapsf`` are large, high-resolution calculations are not needed. In
-    some cases, however, e.g. to accurately estimate the central Vrms in a
-    very cuspy galaxy inside a large aperture, one may want to override the
-    default value to force smaller spatial pixels using this keyword.
+    or ``sigmapsf`` are large, high-resolution calculations are not needed.
+    In some cases, however, e.g. to accurately estimate the central Vrms in
+    a very cuspy galaxy inside a large aperture, one may want to override
+    the default value to force smaller spatial pixels using this keyword.
 vmax: float, optional
     Maximum value of the ``data`` to plot.
 vmin: float, optional
     Minimum value of the ``data`` to plot.
 
 Output Parameters
 -----------------
@@ -789,36 +789,43 @@
 License
 =======
 
 Other/Proprietary License
 
 Copyright (c) 2003-2023 Michele Cappellari
 
-This software is provided as is without any warranty whatsoever.
-Permission to use, for non-commercial purposes is granted.
-Permission to modify for personal or internal use is granted,
-provided this copyright and disclaimer are included in all 
-copies of the software. All other rights are reserved.
-In particular, redistribution of the code is not allowed.
+This software is provided as is with no warranty. You may use it for
+non-commercial purposes and modify it for personal or internal use, as long
+as you include this copyright and disclaimer in all copies. You may not
+redistribute the code.
+
+###########################################################################
 
 Changelog
 =========
 
-V7.1.0: MC, Oxford, 1 June 2023
+V7.2.0: MC, Oxford, 20 July 2023
+    - ``jam_axi_intr``: Integrate all velocity components at the same time with
+      a single call to the updated ``quad1d`` and ``quad2d``. Significant speedup.
+    - ``quad1d``, ``quad2d``: Allow for integration of vector functions.
+      All components are integrated over the same set of evaluation points.
+    - ``jam_axi_proj``: Updated verbose output with more information.
+
+V7.1.0: MC, Oxford, 5 June 2023
     - Separated computation for the black hole kinematics for both the
       cylindrically and spherically-aligned solutions. In both cases this
       removed one numerical quadrature. This is useful in extreme situations,
       when the minimum radius one wants to model around the black hole is orders
       of magnitude smaller than the smallest MGE Gaussian. This change
       eliminated the need for the ``rbh`` keyword in ``jam_axi_intr``, which I
       removed. The only case where the black hole is still approximated with a
       small Gaussian is in ``jam_axi_proj`` when both ``align='cyl'`` and
       ``analytic_los=True``.
-    - Adopted consistent minimum radius, based on ``step``, for both the
-      intrinsic and projected interpolation grids.
+    - Adopted minimum radius based on ``step`` for the intrinsic interpolation
+      grid as already done for the projected one.
     - Simplified minimum-inclination test.
     - Removed ``legacy`` folder with old redundant procedures.
     - Moved the formalism for the LOS analytic integrand with ``align='cyl'``
       into ``jam_axi_proj``.
     - ``jam_axi_proj``, ``jam_axi_intr``, ``jam_sph_proj``, ``jam_sph_intr``:
       New keyword ``logistic`` to specify when JAM should interpret the input
       anisotropy parameters ``beta`` and ``gamma`` as defining a logistic
```

### Comparing `jampy-7.1.0/jampy/CHANGELOG.rst` & `jampy-7.2.0/jampy/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+
 Changelog
 =========
 
-V7.1.0: MC, Oxford, 1 June 2023
+V7.2.0: MC, Oxford, 20 July 2023
+    - ``jam_axi_intr``: Integrate all velocity components at the same time with
+      a single call to the updated ``quad1d`` and ``quad2d``. Significant speedup.
+    - ``quad1d``, ``quad2d``: Allow for integration of vector functions.
+      All components are integrated over the same set of evaluation points.
+    - ``jam_axi_proj``: Updated verbose output with more information.
+
+V7.1.0: MC, Oxford, 5 June 2023
     - Separated computation for the black hole kinematics for both the
       cylindrically and spherically-aligned solutions. In both cases this
       removed one numerical quadrature. This is useful in extreme situations,
       when the minimum radius one wants to model around the black hole is orders
       of magnitude smaller than the smallest MGE Gaussian. This change
       eliminated the need for the ``rbh`` keyword in ``jam_axi_intr``, which I
       removed. The only case where the black hole is still approximated with a
       small Gaussian is in ``jam_axi_proj`` when both ``align='cyl'`` and
       ``analytic_los=True``.
-    - Adopted consistent minimum radius, based on ``step``, for both the
-      intrinsic and projected interpolation grids.
+    - Adopted minimum radius based on ``step`` for the intrinsic interpolation
+      grid as already done for the projected one.
     - Simplified minimum-inclination test.
     - Removed ``legacy`` folder with old redundant procedures.
     - Moved the formalism for the LOS analytic integrand with ``align='cyl'``
       into ``jam_axi_proj``.
     - ``jam_axi_proj``, ``jam_axi_intr``, ``jam_sph_proj``, ``jam_sph_intr``:
       New keyword ``logistic`` to specify when JAM should interpret the input
       anisotropy parameters ``beta`` and ``gamma`` as defining a logistic
```

### Comparing `jampy-7.1.0/jampy/README.rst` & `jampy-7.2.0/jampy/README.rst`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/cappellari2020_table1.txt` & `jampy-7.2.0/jampy/examples/cappellari2020_table1.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/jam_axi_intr_example.py` & `jampy-7.2.0/jampy/examples/jam_axi_intr_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/jam_axi_proj_example.py` & `jampy-7.2.0/jampy/examples/jam_axi_proj_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
 def jam_axi_proj_example():
     """
     Usage example for jam_axi_proj.
     It takes about 2s on a 3GHz CPU
 
     """
-    np.random.seed(123)
-    xbin, ybin = np.random.uniform(low=[-55, -40], high=[55, 40], size=[500, 2]).T
+    rng = np.random.default_rng(123)
+    xbin, ybin = rng.uniform(low=[-55, -40], high=[55, 40], size=[500, 2]).T
 
     inc = 60.                                                # Assumed galaxy inclination
     r = np.sqrt(xbin**2 + (ybin/np.cos(np.radians(inc)))**2) # Radius in the plane of the disk
     a = 40                                                   # Scale length in arcsec
     vr = 2000*np.sqrt(r)/(r + a)                             # Assumed velocity profile (v_c of Hernquist 1990)
     vel = vr * np.sin(np.radians(inc))*xbin/r                # Projected velocity field
     sig = 8700/(r + a)                                       # Assumed velocity dispersion profile
```

### Comparing `jampy-7.1.0/jampy/examples/jam_black_hole_bayes_example.py` & `jampy-7.2.0/jampy/examples/jam_black_hole_bayes_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/jam_dark_halo_bayes_example.py` & `jampy-7.2.0/jampy/examples/jam_dark_halo_bayes_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/jam_hernquist_model_example.py` & `jampy-7.2.0/jampy/examples/jam_hernquist_model_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/jam_mock_kinematics_black_hole.txt` & `jampy-7.2.0/jampy/examples/jam_mock_kinematics_black_hole.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/jam_mock_kinematics_dark_halo.txt` & `jampy-7.2.0/jampy/examples/jam_mock_kinematics_dark_halo.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/jam_sph_proj_example.py` & `jampy-7.2.0/jampy/examples/jam_sph_proj_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/examples/mge_vcirc_example.py` & `jampy-7.2.0/jampy/examples/mge_vcirc_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/jam_axi_intr.py` & `jampy-7.2.0/jampy/jam_axi_intr.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,165 +53,202 @@
     """ Density for each luminous Gaussian at (R, z) """
 
     nu = dens*np.exp(-0.5/sigma**2*(R**2 + (z/qintr)**2))  # Cappellari (2008) eq.(13)
 
     return nu
 
 ##############################################################################
-def intrinsic_moments_cyl_bh(R, z, dens_lum, sigma_lum, qintr_lum, mbh, beta, gamma):
-    """
-    Compute analytic intrinsic moments for the black hole alone
 
-    """
+def intrinsic_moments_cyl_bh(R, z, dens_lum, sigma_lum, qintr_lum, mbh, beta, gamma, all_mom):
+    """ Compute analytic intrinsic moments for the black hole alone """
+
     G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
     h = sigma_lum*qintr_lum*np.sqrt(2)
     r = np.sqrt(R**2 + z**2)
     nu = density(R, z, dens_lum, sigma_lum, qintr_lum)
     nu /= nu.sum()
-    sig2z = G*mbh*nu*(1/r - special.erfcx(r/h)*np.sqrt(np.pi)/h)
-
     bani = 1/(1 - beta)  # Anisotropy ratio b = (sig_R/sig_z)**2
-    sig2R = bani*sig2z
-    sig2phi = (1 - gamma)*sig2R
-    v2phi = G*mbh*R**2/r**3*(1 - bani)*nu \
-            + bani*(1 + (1 - qintr_lum**2)*(R/(sigma_lum*qintr_lum))**2)*sig2z
 
-    return sig2R.sum(), sig2z.sum(), sig2phi.sum(), v2phi.sum()
+    sig2z = G*mbh*nu*(1/r - special.erfcx(r/h)*np.sqrt(np.pi)/h)
+    v2phi = G*mbh*R**2/r**3*(1 - bani)*nu + (
+            1 + (1 - qintr_lum**2)*(R/(sigma_lum*qintr_lum))**2)*bani*sig2z
+    arr = [sig2z, v2phi]
+
+    if all_mom:
+        sig2R = bani*sig2z
+        sig2phi = (1 - gamma)*sig2R
+        arr.extend([sig2R, sig2phi])
+
+    return np.sum(arr, 1)
 
 ##############################################################################
 
 def integrand_cyl(u, R, z,
                   dens_lum, sigma_lum, qintr_lum,
                   dens_pot, sigma_pot, qintr_pot,
-                  beta, gamma, logistic, component):
+                  beta, gamma, logistic, all_mom):
     """
     Compute all the non-zero JAM first and second intrinsic velocity moments
     using the formulas from Cappellari (2008, MNRAS, 390, 71; hereafter C08).
     https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
 
     """
-    if logistic:        # Variable anisotropy, same for all Gaussians
-        zab, beta0, betainf, alpha = beta
-        beta = (beta0 + betainf*(abs(z)/zab)**alpha)/(1 + (abs(z)/zab)**alpha)
-        bani = 1/(1 - beta)
-    else:               # Constant anisotropy, different per Gaussian
-        bani = 1/(1 - beta[:, None, None]) if np.ptp(beta) else 1/(1 - beta[0])  # Anisotropy ratio b = (sig_R/sig_z)**2
-
     dens_lum = dens_lum[:, None, None]
     sigma_lum = sigma_lum[:, None, None]
     qintr_lum = qintr_lum[:, None, None]
 
     dens_pot = dens_pot[None, :, None]
     sigma_pot = sigma_pot[None, :, None]
     qintr_pot = qintr_pot[None,:, None]
 
-    # DE Change of variables for Chandrasekhar u-integral
+    # DE Change of variables for Chandrasekhar u-integral (Sec.6.2 of Cappellari 2020)
     # np.arcsinh(np.log([rmin, rmax])*2/np.pi) -> [0, inf]
     x = np.exp(np.sinh(u)*np.pi/2)
     duds = x*np.cosh(u)*np.pi/2
     u = x[None, None, :]
 
-    # Tracer
+    if logistic:  # Variable anisotropy, same for all Gaussians
+        zab, beta0, betainf, alpha = beta
+        beta = (beta0 + betainf*(abs(z)/zab)**alpha)/(1 + (abs(z)/zab)**alpha)
+        bani = 1/(1 - beta)  # Anisotropy ratio b = (sig_R/sig_z)**2
+    else:  # Constant anisotropy, different per Gaussian
+        bani = 1/(1 - beta[:, None, None]) if np.ptp(beta) else 1/(1 - beta[0])
+
+    # Tracer Gaussians
     R2, z2 = R**2, z**2
     a = -1/(2*sigma_lum**2)
     b = a/qintr_lum**2
     exp1 = dens_lum*np.exp(a*R2 + b*z2)
 
-    # Mass
+    # Mass Gaussians
     G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
     u1, qu = 1 + u, qintr_pot**2 + u
     tmp = -1/(2*sigma_pot**2)
     c, d = tmp/u1, tmp/qu
-    upot = 2*np.pi*G*dens_pot*qintr_pot*sigma_pot**2/(u1*np.sqrt(qu))
-    exp2 = upot*np.exp(c*R2 + d*z2)
+    cst = 2*np.pi*G*dens_pot*qintr_pot*sigma_pot**2
+    exp2 = cst*np.exp(c*R2 + d*z2)/(u1*np.sqrt(qu))
 
     bd = d/(b + d)
     sig2z = exp1*exp2*bd
+    v2phi = (bani + 2*R2*((a + c)*bani - c/bd))*sig2z
+    arr = [sig2z, v2phi]
 
-    if component == 'sig2R':
-        sig2z *= bani
-    elif component == 'sig2phi':
-        if logistic:        # Variable anisotropy, same for all Gaussians
-            zag, gamma0, gammainf, alpha = gamma
-            gamma = (gamma0 + gammainf*(abs(z)/zag)**alpha)/(1 + (abs(z)/zag)**alpha)
-        else:               # Constant anisotropy, different per Gaussian
-            gamma = gamma[:, None, None] if np.ptp(gamma) else gamma[0]  # Anisotropy gamma = 1 - (sig_phi/sig_R)**2
-        sig2z *= (1 - gamma)*bani
-    elif component == 'v2phi':
-        sig2z *= bani + 2*R2*((a + c)*bani - c/bd)
+    if all_mom:
+        gamma = gamma[:, None, None] if np.ptp(gamma) else gamma[0]
+        sig2R = bani*sig2z
+        sig2phi = (1 - gamma)*sig2R
+        arr.extend([sig2R, sig2phi])
 
-    return duds*sig2z.sum((0, 1))
+    return duds*np.sum(arr, (1, 2))
 
 ##############################################################################
+
 def intrinsic_moments_cyl(R, z,
                           dens_lum, sigma_lum, qintr_lum,
                           dens_pot, sigma_pot, qintr_pot,
                           mbh, beta, gamma, logistic, epsrel):
     """ Numerical quadratures of the Jeans solution """
 
     mds, mxs = np.median(sigma_lum), np.max(sigma_lum)
     xlim = np.arcsinh(np.log([1e-7*mds, 1e3*mxs])*2/np.pi)
-
-    args = [R, z, dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot, beta, gamma, logistic]
     nu = density(R, z, dens_lum, sigma_lum, qintr_lum).sum()
-    sig2z = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args+['sig2z']).integ/nu
-    v2phi = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args+['v2phi']).integ/nu
 
-    if (not logistic) and (np.ptp(beta) or np.ptp(gamma)):
-        sig2R = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args+['sig2R']).integ/nu
-        sig2phi = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args+['sig2phi']).integ/nu
+    all_mom = True if (not logistic) and (np.ptp(beta) or np.ptp(gamma)) else False
+    args = [R, z, dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
+            beta, gamma, logistic, all_mom]
+    mom = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args).integ/nu
+
+    if logistic:
+        zab, beta0, betainf, alpha = beta
+        beta = (beta0 + betainf*(abs(z)/zab)**alpha)/(1 + (abs(z)/zab)**alpha)
+        zag, gamma0, gammainf, alpha = gamma
+        gamma = (gamma0 + gammainf*(abs(z)/zag)**alpha)/(1 + (abs(z)/zag)**alpha)
     else:
-        if logistic:
-            zab, beta0, betainf, alpha = beta
-            beta = (beta0 + betainf*(abs(z)/zab)**alpha)/(1 + (abs(z)/zab)**alpha)
-            zag, gamma0, gammainf, alpha = gamma
-            gamma = (gamma0 + gammainf*(abs(z)/zag)**alpha)/(1 + (abs(z)/zag)**alpha)
-        else:
-            beta = beta[0]
-            gamma = gamma[0]
-        sig2R = sig2z/(1 - beta)
-        sig2phi = sig2R*(1 - gamma)
+        if not np.ptp(beta): beta = beta[0]
+        if not np.ptp(gamma): gamma = gamma[0]
 
     if mbh > 0:
-        sig2R_bh, sig2z_bh, sig2phi_bh, v2phi_bh = intrinsic_moments_cyl_bh(
-            R, z, dens_lum, sigma_lum, qintr_lum, mbh, beta, gamma)
-        sig2R += sig2R_bh
-        sig2z += sig2z_bh
-        sig2phi += sig2phi_bh
-        v2phi += v2phi_bh
+        mom += intrinsic_moments_cyl_bh(
+            R, z, dens_lum, sigma_lum, qintr_lum, mbh, beta, gamma, all_mom)
+
+    if all_mom:
+        sig2z, v2phi, sig2R, sig2phi = mom
+    else:
+        sig2z, v2phi = mom
+        sig2R = sig2z/(1 - beta)
+        sig2phi = sig2R*(1 - gamma)
 
     return sig2R, sig2z, sig2phi, v2phi, nu
 
 ##############################################################################
-def integand_tan_dth_pot(u, R2, z2, dens_pot, sigma_pot, qintr_pot):
+
+def integrand_sph_bh(t, r, th, dens_lum, sigma_lum, qintr_lum, beta, gamma, logistic, mbh, all_mom):
+    """ Solution of the spherically-aligned Jeans equations for a black hole alone """
+
+    # TANH Change of variables for Jeans r-integral (Sec.6.2 of Cappellari 2020)
+    # np.log([rmin, rmax]) -> [r, inf]
+    drdt = np.exp(t)
+    r1 = r + drdt[:, None]
+
+    if logistic:    # Variable anisotropy, same for all Gaussians
+        rab, beta0, betainf, alpha = beta
+        fun = (r1/r)**(2*beta0)
+        fun *= ((1 + (r1/rab)**alpha)/(1 + (r/rab)**alpha))**(2*(betainf - beta0)/alpha)
+        beta = beta0 + (betainf - beta0)/(1 + (rab/r)**alpha)
+    else:           # Constant anisotropy, different per Gaussian
+        fun = (r1/r)**(2*beta)
+
+    # Tracer Gaussians
+    s2_lum = sigma_lum**2
+    q2_lum = qintr_lum**2
+    rs = fun*(r*np.sin(th))**2
+    aa = -r1**2/(2*q2_lum*s2_lum)
+    bb = (1 - q2_lum)/(2*q2_lum*s2_lum)*rs
+    ex1 = dens_lum*np.exp(aa + bb)
+
+    G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
+    sig2r = G*fun*ex1*mbh/r1**2
+    v2phi = (1 - beta)*(1 + 2*bb)*sig2r
+    arr = [sig2r, v2phi]
+
+    if all_mom:
+        sig2th = (1 - beta)*sig2r       # Anisotropy beta = 1 - (sig_th/sig_r)**2
+        sig2phi = (1 - gamma)*sig2r     # Anisotropy gamma = 1 - (sig_phi/sig_r)**2
+        arr.extend([sig2th, sig2phi])
+
+    return drdt*np.sum(arr, 2)
+
+##############################################################################
+
+def integrand_tan_dth_pot(u, R2, z2, dens_pot, sigma_pot, qintr_pot):
     """
     Returns the integrand of the tan(th)*d(pot)/dth derivative
     of the MGE potential at (r, th).
     This is equation (51) of Cappellari (2020, MNRAS, 494, 4819)
     https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C
 
     """
-    # DE Change of variables for Chandrasekhar u-integral
+    # DE Change of variables for Chandrasekhar u-integral (Sec.6.2 of Cappellari 2020)
     # np.arcsinh(np.log([rmin, rmax])*2/np.pi) -> [0, inf]
     x = np.exp(np.sinh(u)*np.pi/2)
     duds = x*np.cosh(u)*np.pi/2
     u = x[:, None]
 
     G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
-    qu = qintr_pot**2 + u
-    u1 = 1 + u
+    u1, qu = 1 + u, qintr_pot**2 + u
     d = 2*np.pi*G*dens_pot*qintr_pot*(qintr_pot**2 - 1)*R2
     e = np.exp(-0.5/sigma_pot**2*(R2/u1 + z2/qu))
     tan_dth_pot = d*e/(u1**2*qu**1.5)
 
     return duds*tan_dth_pot.sum(1)   # u.size
 
 ##############################################################################
+
 def integrand_sph(s, t, r, th, dens_lum, sigma_lum, qintr_lum, beta, gamma,
-                  logistic, dens_pot, sigma_pot, qintr_pot, component):
+                  logistic, dens_pot, sigma_pot, qintr_pot, all_mom):
     """
     Solution of the spherically-aligned Jeans equations for an MGE
     from eq.(52)-(54) of Cappellari (2020, MNRAS, 494, 4819)
     https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C
 
     """
     dens_lum = dens_lum[:, None, None]
@@ -246,147 +283,89 @@
     rs = fun*(r*np.sin(th))**2
     aa = -r1**2/(2*q2_lum*s2_lum)
     bb = (1 - q2_lum)/(2*q2_lum*s2_lum)*rs
     ex1 = dens_lum*np.exp(aa + bb)
 
     # Mass Gaussians
     G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
-    qu = qintr_pot**2 + u
-    u1 = 1 + u
+    u1, qu = 1 + u, qintr_pot**2 + u
     cc = -r1**2/(2*qu*s2_pot)
     dd = (u1 - qu)/(2*qu*s2_pot*u1)*rs
     cst = 2*np.pi*G*dens_pot*qintr_pot*r1
     ex2 = cst*np.exp(cc + dd)/(u1*qu**1.5)
 
-    psi = fun*ex1*ex2
+    sig2r = fun*ex1*ex2
+    v2phi = (1 - beta)*(1 + 2*(bb + dd))*sig2r
+    arr = [sig2r, v2phi]
+
+    if all_mom:
+        gamma = gamma[:, None, None] if np.ptp(gamma) else gamma[0]
+        sig2th = (1 - beta)*sig2r       # Anisotropy beta = 1 - (sig_th/sig_r)**2
+        sig2phi = (1 - gamma)*sig2r     # Anisotropy gamma = 1 - (sig_phi/sig_r)**2
+        arr.extend([sig2th, sig2phi])
 
-    if component == 'sig2r':
-        integ = psi
-    elif component == 'sig2th':
-        integ = psi*(1 - beta)
-    elif component == 'sig2phi':
-        if logistic:    # Variable anisotropy, same for all Gaussians
-            rag, gamma0, gammainf, alpha = gamma
-            gamma = gamma0 + (gammainf - gamma0)/(1 + (rag/r)**alpha)
-        else:           # Constant anisotropy, different per Gaussian
-            gamma = gamma[:, None, None] if np.ptp(gamma) else gamma[0]  # Anisotropy gamma = 1 - (sig_phi/sig_R)**2
-        integ = psi*(1 - gamma)
-    elif component == 'v2phi':
-        integ = psi*(1 - beta)*(1 + 2*(bb + dd))
-
-    return duds*drdt*integ.sum((0, 1))    # u.size == t.size
+    return duds*drdt*np.sum(arr, (1, 2))
 
 ##############################################################################
-def integrand_sph_bh(t, r, th, dens_lum, sigma_lum, qintr_lum, beta, gamma, logistic, mbh, component):
-    """
-    Solution of the spherically-aligned Jeans equations for a black hole alone
 
-    """
-    # TANH Change of variables for Jeans r-integral (Sec.6.2 of Cappellari 2020)
-    # np.log([rmin, rmax]) -> [r, inf]
-    drdt = np.exp(t)
-    r1 = r + drdt[:, None]
-
-    if logistic:    # Variable anisotropy, same for all Gaussians
-        rab, beta0, betainf, alpha = beta
-        fun = (r1/r)**(2*beta0)
-        fun *= ((1 + (r1/rab)**alpha)/(1 + (r/rab)**alpha))**(2*(betainf - beta0)/alpha)
-        beta = beta0 + (betainf - beta0)/(1 + (rab/r)**alpha)
-    else:           # Constant anisotropy, different per Gaussian
-        fun = (r1/r)**(2*beta)
-
-    # Tracer Gaussians
-    s2_lum = sigma_lum**2
-    q2_lum = qintr_lum**2
-    rs = fun*(r*np.sin(th))**2
-    aa = -r1**2/(2*q2_lum*s2_lum)
-    bb = (1 - q2_lum)/(2*q2_lum*s2_lum)*rs
-    ex1 = dens_lum*np.exp(aa + bb)
-
-    G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
-    psi = G*fun*ex1*mbh/r1**2
-
-    if component == 'sig2r':
-        integ = psi
-    elif component == 'sig2th':
-        integ = psi*(1 - beta)
-    elif component == 'sig2phi':
-        if logistic:    # Variable anisotropy, same for all Gaussians
-            rag, gamma0, gammainf, alpha = gamma
-            gamma = gamma0 + (gammainf - gamma0)/(1 + (rag/r)**alpha)
-        integ = psi*(1 - gamma)
-    elif component == 'v2phi':
-        integ = psi*(1 - beta)*(1 + 2*bb)
-
-    return drdt*integ.sum(1)
-
-##############################################################################
 def intrinsic_moments_sph(R, z,
                           dens_lum, sigma_lum, qintr_lum,
                           dens_pot, sigma_pot, qintr_pot,
                           mbh, beta, gamma, logistic, epsrel):
     """ Numerical quadratures of the Jeans solution """
 
     r = np.sqrt(R**2 + z**2)
     th = np.arctan2(R, z)  # Angle from symmetry axis z
 
     mds, mxs = np.median(sigma_lum), np.max(sigma_lum)
     xlim = np.arcsinh(np.log([1e-7*mds, 1e3*mxs])*2/np.pi)
     ylim = np.log([1e-6*mds, 3*mxs])
     args = [r, th, dens_lum, sigma_lum, qintr_lum, beta, gamma, logistic]
-    args_mge = args + [dens_pot, sigma_pot, qintr_pot]
     nu = density(R, z, dens_lum, sigma_lum, qintr_lum).sum()
 
-    sig2r = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge+['sig2r']).integ/nu
-    v2phi = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge+['v2phi']).integ/nu
-
+    all_mom = True if (not logistic) and (np.ptp(beta) or np.ptp(gamma)) else False
+    args_mge = args + [dens_pot, sigma_pot, qintr_pot, all_mom]
+    mom = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge).integ
     if mbh > 0:
-        args_bh = args + [mbh]
-        sig2r += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args_bh+['sig2r']).integ/nu
-        v2phi += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args_bh+['v2phi']).integ/nu
-
-    if (not logistic) and (np.ptp(beta) or np.ptp(gamma)):
-        sig2th = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge+['sig2th']).integ/nu
-        sig2phi = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge+['sig2phi']).integ/nu
-        if mbh > 0:
-            sig2th += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args_bh+['sig2th']).integ/nu
-            sig2phi += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args_bh+['sig2phi']).integ/nu
+        mom += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args+[mbh, all_mom]).integ
+
+    if all_mom:
+        sig2r, v2phi, sig2th, sig2phi = mom/nu
     else:
+        sig2r, v2phi = mom/nu
         if logistic:
             rab, beta0, betainf, alpha = beta
             beta = beta0 + (betainf - beta0)/(1 + (rab/r)**alpha)
             rag, gamma0, gammainf, alpha = gamma
             gamma = gamma0 + (gammainf - gamma0)/(1 + (rag/r)**alpha)
         else:
             beta = beta[0]
             gamma = gamma[0]
         sig2th = sig2r*(1 - beta)
         sig2phi = sig2r*(1 - gamma)
 
-    v2phi += quad1d(integand_tan_dth_pot, xlim, epsrel=epsrel,
-                     args=(R**2, z**2, dens_pot, sigma_pot, qintr_pot)).integ
+    v2phi += quad1d(integrand_tan_dth_pot, xlim, epsrel=epsrel,
+                    args=(R**2, z**2, dens_pot, sigma_pot, qintr_pot)).integ
 
     return sig2r, sig2th, sig2phi, v2phi, nu
 
 ##############################################################################
+
 def intrinsic_moments(Rbin, zbin, dens_lum, sigma_lum, qintr_lum, dens_pot,
                       sigma_pot, qintr_pot, mbh, beta, gamma, logistic, nrad,
                       nang, epsrel, interp, proj_cyl, align):
 
     fun = intrinsic_moments_cyl if align == 'cyl' else intrinsic_moments_sph
 
     if nrad*nang > Rbin.size or (not interp):  # Just calculate values
-        print("Just compute values")
-        sig2r, sig2th, sig2phi, v2phi, nu = np.empty((5, Rbin.size))
-        for j, (Rj, zj) in enumerate(zip(Rbin, zbin)):  # loop over coordinates
-            sig2r[j], sig2th[j], sig2phi[j], v2phi[j], nu[j] = fun(Rj, zj,
-                dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
-                mbh, beta, gamma, logistic, epsrel)
+        mom = [fun(Rj, zj, dens_lum, sigma_lum, qintr_lum, dens_pot,
+                   sigma_pot, qintr_pot, mbh, beta, gamma, logistic, epsrel)
+               for (Rj, zj) in zip(Rbin, zbin)]
+        sig2r, sig2th, sig2phi, v2phi, nu = np.array(mom).T
     else:
-        print("Perform interpolation")
         irp = mom_interp(Rbin, zbin, dens_lum, sigma_lum, qintr_lum, dens_pot,
                          sigma_pot, qintr_pot, mbh, beta, gamma, logistic, nrad,
                          nang, epsrel=epsrel, align=align)
         sig2r, sig2th, sig2phi, v2phi, nu = irp.get_moments(Rbin, zbin)
 
     # Project the velocity dispersion tensor to cylindrical coordinates
     if proj_cyl and (align == 'sph'):
@@ -402,18 +381,16 @@
 class mom_interp:
 
     def __init__(self, xbin, ybin,
                  dens_lum, sigma_lum, qintr_lum,
                  dens_pot, sigma_pot, qintr_pot,
                  mbh, beta, gamma, logistic, nrad, nang, epsrel=1e-2,
                  rmin=None, rmax=None, align='cyl'):
-        """
-        Initializes model values on a grid for subsequent interpolation
+        """ Initializes model values on a grid for subsequent interpolation """
 
-        """
         fun = intrinsic_moments_cyl if align == 'cyl' else intrinsic_moments_sph
 
         # Define parameters of polar grid for interpolation
         w = sigma_lum < np.max(np.abs(xbin))  # Characteristic MGE axial ratio in observed range
         self.qmed = np.median(qintr_lum) if w.sum() < 3 else np.median(qintr_lum[w])
 
         if rmin is None or rmax is None:
@@ -426,24 +403,19 @@
         rad =  np.geomspace(self.rmin, self.rmax, nrad)
         self.logRad = np.log(rad)
         self.ang = np.linspace(0, np.pi/2, nang)
         rellGrid, eccGrid = map(np.ravel, np.meshgrid(rad, self.ang))
         R = rellGrid*np.cos(eccGrid)
         z = rellGrid*np.sin(eccGrid)*self.qmed  # ecc=0 on equatorial plane
 
-        sig2r, sig2th, sig2phi, v2phi, nu = np.empty((5, R.size))
-        for j, (Rj, zj) in enumerate(zip(R, z)):
-            sig2r[j], sig2th[j], sig2phi[j], v2phi[j], nu[j] = fun(Rj, zj,
-                dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
-                mbh, beta, gamma, logistic, epsrel)
-
-        self.sig2r = sig2r.reshape(nang, nrad)
-        self.sig2th = sig2th.reshape(nang, nrad)
-        self.sig2phi = sig2phi.reshape(nang, nrad)
-        self.v2phi = v2phi.reshape(nang, nrad)
+        mom = [fun(Rj, zj, dens_lum, sigma_lum, qintr_lum, dens_pot,
+                   sigma_pot, qintr_pot, mbh, beta, gamma, logistic, epsrel)
+               for (Rj, zj) in zip(R, z)]
+
+        self.sig2r, self.sig2th, self.sig2phi, self.v2phi, nu = np.array(mom).T.reshape((5, nang, nrad))
         self.dens_lum = dens_lum
         self.sigma_lum = sigma_lum
         self.qintr_lum = qintr_lum
 
 ##############################################################################
 
     def get_moments(self, R, z):
@@ -452,18 +424,16 @@
         of (R, z) coordinates from pre-computed values.
         Interpolation of non-weighted kinematics for accuracy.
         The returned density is analytic, not interpolated.
 
         """
         r1 = 0.5*np.log((R**2 + (z/self.qmed)**2).clip(self.rmin**2))  # Log elliptical radius of input (R,z)
         e1 = np.arctan2(np.abs(z/self.qmed), np.abs(R))  # Eccentric anomaly of input (R,z)
-        sig2r = bilinear_interpolate(self.logRad, self.ang, self.sig2r, r1, e1)
-        sig2th = bilinear_interpolate(self.logRad, self.ang, self.sig2th, r1, e1)
-        sig2phi = bilinear_interpolate(self.logRad, self.ang, self.sig2phi, r1, e1)
-        v2phi = bilinear_interpolate(self.logRad, self.ang, self.v2phi, r1, e1)
+        bint = lambda x: bilinear_interpolate(self.logRad, self.ang, x, r1, e1)
+        sig2r, sig2th, sig2phi, v2phi = map(bint, [self.sig2r, self.sig2th, self.sig2phi, self.v2phi])
         nu = density(R[:, None], z[:, None], self.dens_lum, self.sigma_lum, self.qintr_lum).sum(-1)
 
         return sig2r, sig2th, sig2phi, v2phi, nu
 
 ##############################################################################
 
 class jam_axi_intr:
@@ -765,14 +735,18 @@
 
         # model contains [sig2r, sig2th, sig2phi, v2phi]
         *model, nu = intrinsic_moments(Rbin, zbin, dens_lum, sigma_lum,
             qintr_lum, dens_pot, sigma_pot, qintr_pot, mbh, beta, gamma,
             logistic, nrad, nang, epsrel, interp, proj_cyl, align)
 
         if not quiet:
+            if nrad*nang > Rbin.size or (not interp):
+                print("Just computed values")
+            else:
+                print("Performed interpolation")
             print(f'jam_axi_intr_{align} elapsed time (sec): {clock() - t:.2f}')
 
         if data is None:
             chi2 = None
             if ml is None:
                 ml = 1.
         else:
```

### Comparing `jampy-7.1.0/jampy/jam_axi_proj.py` & `jampy-7.2.0/jampy/jam_axi_proj.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,23 @@
 
 ##############################################################################
 def integrand_cyl_los(u1,
                       dens_lum, sigma_lum, q_lum,
                       dens_pot, sigma_pot, q_pot,
                       x1, y1, inc, beta, tensor):
     """
-    This routine computes the integrand of Eq.(28) of Cappellari (2008; C08) for
-    a model with constant anisotropy sigma_R**2 = b*sigma_z**2 and <V_R*V_z> = 0.
+    Computes the integrand of Eq.(28) of Cappellari (2008 MNRAS; C08
+    https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C) for a model with
+    constant anisotropy per Gaussian sigma_R**2 = b*sigma_z**2 and <V_R*V_z> = 0.
     The components of the proper motion dispersions tensor are calculated as
-    described in note 5 of C08.
-    See Cappellari (2012; C12 http://arxiv.org/abs/1211.7009)
-    for explicit formulas for the proper motion tensor.
-    The formulas are also given in Appendix A3 of Cappellari (2020, C20)
+    described in note 5 of C08. I later gave explicit formulas in
+    Cappellari (2012; C12 http://arxiv.org/abs/1211.7009).
+    I collected all formulas in Appendix A3 of Cappellari (2020 MNRAS, C20)
     https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C
 
-
     """
     dens_lum = dens_lum[:, None, None]
     sigma_lum = sigma_lum[:, None, None]
     q_lum = q_lum[:, None, None]
     beta = beta[:, None, None]
 
     dens_pot = dens_pot[None, :, None]
@@ -109,24 +108,21 @@
     return 4*np.pi**1.5*G*arr.sum((0, 1))
 
 ##############################################################################
 def surf_v2los_cyl(x1, y1, inc,
                    dens_lum, sigma_lum, qintr_lum,
                    dens_pot, sigma_pot, qintr_pot,
                    beta, tensor):
-    """
-    This routine gives the projected weighted second moment Sigma*<V^2_los>
+    """ Compute the projected weighted second moment Sigma*<V^2_los> """
 
-    """
-    sb_mu2 = np.empty_like(x1)
-    for j, (xj, yj) in enumerate(zip(x1, y1)):
-        sb_mu2[j] = quad1d(integrand_cyl_los, [0., 1.], singular=1,
-                           args=(dens_lum, sigma_lum, qintr_lum,
-                                  dens_pot, sigma_pot, qintr_pot,
-                                  xj, yj, inc, beta, tensor)).integ
+    sb_mu2 = [quad1d(integrand_cyl_los, [0., 1.], singular=1,
+                     args=(dens_lum, sigma_lum, qintr_lum,
+                           dens_pot, sigma_pot, qintr_pot,
+                           xj, yj, inc, beta, tensor)).integ
+              for (xj, yj) in zip(x1, y1)]
 
     return sb_mu2
 
 ##############################################################################
 def vmom_proj(x1, y1, inc, mbh, beta, gamma, logistic,
               dens_lum, sigma_lum, qintr_lum,
               dens_pot, sigma_pot, qintr_pot,
@@ -268,14 +264,15 @@
 
     psf_convolution = (np.max(sigmaPsf) > 0) and (pixSize > 0)
 
     if not interp or ((nrad*nang > x.size) and (not psf_convolution)):  # Just calculate values
 
         assert np.all((x != 0) | (y != 0)), "One must avoid the singularity at `(xbin, ybin) = (0, 0)`"
 
+        interp = False
         x_pol = x
         y_pol = y
         step = np.min(rell)  # Minimum radius
 
     else:  # Interpolate values on polar grid
 
         # Kernel step is 1/4 of largest between sigma(min) and 1/2 pixel side.
@@ -384,15 +381,15 @@
             if moment in ('xy', 'xz'):
                 mu *= np.sign(x*y)
             elif moment in ('y', 'z'):
                 mu *= np.sign(x)
             elif moment == 'x':
                 mu *= np.sign(y)
 
-    return mu, psf_convolution, vel, vel2
+    return mu, psf_convolution, interp, vel, vel2
 
 ##############################################################################
 
 class jam_axi_proj:
     """
     jam_axi_proj
     ============
@@ -720,15 +717,15 @@
         PSF convolution is not performed.
     plot: bool
         When ``data is not None`` setting this keyword produces a plot with the
         data/model comparison at the end of the calculation.
     quiet: bool
         Set this keyword to avoid printing values on the console.
     rbh: float, optional
-        This keyword is ignored unless ``align='cyl'`` and `analytic_los=True`.
+        This keyword is ignored unless ``align='cyl'`` and ``analytic_los=True``.
         In all other cases JAM assume a point-like central black hole.
         This scalar gives the sigma in arcsec of the Gaussian approximating the
         central black hole of mass MBH [See Section 3.1.2 of `Cappellari (2008)`_]
         The gravitational potential is indistinguishable from a point source
         for ``radii > 2*rbh``, so the default ``rbh=0.01`` arcsec is appropriate
         in most current situations.
 
@@ -750,18 +747,18 @@
         with a first call to ``jam_axi_proj`` with PSF convolution, and the
         model predictions at large radii with a second call to ``jam_axi_proj``
         without PSF convolution.
     step: float, optional
         Spatial step for the model calculation and PSF convolution in arcsec.
         This value is automatically computed by default as
         ``step=max(sigmapsf,pixsize/2)/4``. It is assumed that when ``pixsize``
-        or ``sigmapsf`` are large, high-resolution calculations are not needed. In
-        some cases, however, e.g. to accurately estimate the central Vrms in a
-        very cuspy galaxy inside a large aperture, one may want to override the
-        default value to force smaller spatial pixels using this keyword.
+        or ``sigmapsf`` are large, high-resolution calculations are not needed.
+        In some cases, however, e.g. to accurately estimate the central Vrms in
+        a very cuspy galaxy inside a large aperture, one may want to override
+        the default value to force smaller spatial pixels using this keyword.
     vmax: float, optional
         Maximum value of the ``data`` to plot.
     vmin: float, optional
         Minimum value of the ``data`` to plot.
 
     Output Parameters
     -----------------
@@ -885,25 +882,25 @@
         # Add a Gaussian with small sigma and the same total mass as the BH.
         # The Gaussian provides an excellent representation of the second moments
         # of a point-like mass, to 1% accuracy out to a radius 2*sigmaBH.
         # The error increases to 14% at 1*sigmaBH, independently of the BH mass.
         if mbh > 0 and analytic_los:
             tmp = np.concatenate([sigmapsf, [pixsize], sigma_lum])
             assert rbh > 0.01*np.min(tmp[tmp > 0]), "`rbh` is too small"
-            sigmaBH_pc = rbh*pc # Adopt for the BH just a very small size
+            sigmaBH_pc = rbh*pc     # Adopt for the BH just a very small size
             surfBH_pc = mbh/(2*np.pi*sigmaBH_pc**2)
             surf_pot_pc = np.append(surfBH_pc, surf_pot_pc) # Add Gaussian to potential only!
             sigma_pot_pc = np.append(sigmaBH_pc, sigma_pot_pc)
             qobs_pot = np.append(1., qobs_pot)  # Make sure vectors do not have extra dimensions
 
         qobs_lum = qobs_lum.clip(0, 0.999999)
         qobs_pot = qobs_pot.clip(0, 0.999999)
 
         t = clock()
-        model, psfConvolution, vel, vel2 = psf_conv(
+        model, psfConvolution, interp, vel, vel2 = psf_conv(
             xbin_pc, ybin_pc, inc,
             surf_lum_pc, sigma_lum_pc, qobs_lum,
             surf_pot_pc, sigma_pot_pc, qobs_pot,
             mbh, beta, gamma, logistic, moment, align, sigmaPsf_pc, normpsf,
             pixSize_pc, pixang, step_pc, nrad, nang, nlos, epsrel,
             interp, analytic_los)
 
@@ -939,18 +936,16 @@
                     model *= kappa
 
         else:
 
             d, m = (data/errors)[goodbins], (model/errors)[goodbins]
 
             if moment in str2[:3]:
-
                 if ml is None:
                     ml = ((d @ m)/(m @ m))**2   # eq. (51) of Cappellari (2008, MNRAS)
-
                 scale, kappa = np.sqrt(ml), 1.0
 
             else:
 
                 if kappa is None:
 
                     # Scale by having the same angular momentum in the model and
@@ -965,29 +960,30 @@
                 scale, ml = kappa, 1.0
 
             model *= scale
             m *= scale
             chi2 = ((d - m)**2).sum()/goodbins.sum()
 
         if not quiet:
-            print(f'jam_axi_proj_{align}_{moment} (analytic_los={analytic_los}) '
-                  f'elapsed time sec: {clock() - t:.2f}')
+            const_anis = not (np.ptp(beta) or np.ptp(gamma))
+            print(f"jam_axi_proj(align='{align}', moment='{moment}') -- elapsed time sec: {clock() - t:.2f}\n"
+                  f"analytic_los={analytic_los:d} logistic={logistic:d} constant_anisotropy={const_anis:d}")
             if (not psfConvolution) or (not interp):
-                txt = "No PSF/pixel convolution:"
+                txt = "No PSF/pixel convolution because"
                 if np.max(sigmapsf) == 0:
-                    txt += " sigmapsf == 0;"
+                    txt += " sigmapsf=0"
                 if pixsize == 0:
-                    txt += " pixsize == 0;"
+                    txt += " pixsize=0"
                 if not interp:
-                    txt += " interp == False;"
+                    txt += " interp=0"
                 print(txt)
             print(f'inc={inc:#.3g}; beta[1]={beta[1]:#.2g}; kappa={kappa:#.3g}; '
                   f'M/L={ml:#.3g}; BH={mbh*ml:#.2g}; chi2/DOF={chi2:#.3g}')
             mass = 2*np.pi*surf_pot_pc*qobs_pot*sigma_pot_pc**2
-            print(f'Total mass MGE (MSun): {(mass*ml).sum():#.4g}')
+            print(f'Total mass MGE (MSun): {(mass*ml).sum():#.4g}\n')
 
         self.xbin = xbin
         self.ybin = ybin
         self.goodbins = goodbins
         self.data = data
         self.model = model
         self.ml = ml
```

### Comparing `jampy-7.1.0/jampy/jam_sph_intr.py` & `jampy-7.2.0/jampy/jam_sph_intr.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/jam_sph_proj.py` & `jampy-7.2.0/jampy/jam_sph_proj.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/mge_half_light_isophote.py` & `jampy-7.2.0/jampy/mge_half_light_isophote.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/mge_radial_density.py` & `jampy-7.2.0/jampy/mge_radial_density.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/mge_radial_mass.py` & `jampy-7.2.0/jampy/mge_radial_mass.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/mge_vcirc.py` & `jampy-7.2.0/jampy/mge_vcirc.py`

 * *Files identical despite different names*

### Comparing `jampy-7.1.0/jampy/quad1d.py` & `jampy-7.2.0/jampy/quad1d.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,19 @@
           transforming the coordinates of the integrand. This is useful
           when one wants to transform the coordinates outside ``quad1d``.
         MC, Oxford, 4 February 2022
 
     V3.1.0: Change defaults to `singular=False` and `epsabs=0` like `quad2d`.
         MC, Oxford, 3 January 2023
 
+    V4.0.0: Allow for quadrature of vector functions. Uses the same set of
+        evaluation points for all components of the function and ensures that
+        the convergence criterion is satisfied for all.
+        MC, Oxford, 11 June 2023
+
 """
 import numpy as np
 import matplotlib.pyplot as plt
 
 EPS = 100*np.finfo(float).eps
 
 ################################################################################
@@ -185,80 +190,83 @@
     # Initialize partial sums.
     IfxOK = errOK = 0
 
     # Initialize main loop
     OK = first = converged = True
     Ifx = errbnd = fcall = vfcall = 0
 
-    if plot:
-        plt.figure('quad1d')
-        plt.clf()
-        plt.xlabel('x')
-        plt.ylabel('y')
-        xall = yall = []
-
     while True:
         # SUBS contains subintervals of [a,b] where the integral is not
         # sufficiently accurate.  The first row of SUBS holds the left end
         # points and the second row, the corresponding right end points.
-        midpt = np.sum(subs, axis=1)/2      # midpoints of the subintervals
+        midpt = subs.sum(1)/2      # midpoints of the subintervals
         halfh = np.diff(subs, axis=1)/2     # half the lengths of the subintervals
         x = nodes*halfh + midpt[:, None]    # broadcasting midpt
         halfh = halfh.ravel()
         x = x.ravel()
 
         fx, too_close = f(fun, x, a, b, args)
-        fcall += fx.size
+        fcall += x.size
         vfcall += 1
 
         # Quit if mesh points are too close or too close to a
         # singular point or got into trouble on first evaluation.
         not_finite = np.any(np.isinf(fx))
         if too_close or not_finite:
             break
 
         if plot:
+            if first:
+                plt.figure('quad1d')
+                plt.clf()
+                plt.xlabel('x')
+                plt.ylabel('y')
+                xall, yall = x, fx
+            else:
+                yall = np.column_stack([yall, fx])
+                xall = np.append(xall, x)
             plt.figure('quad1d')
-            plt.plot(x, fx, '+')
-            xall = np.append(xall, x)
-            yall = np.append(yall, fx)
+            plt.plot(x, fx.T, '+')
 
-        fx = fx.reshape(-1, samples)
+        if fx.ndim == 1:
+            fx = fx[None, :]
+
+        fx = fx.reshape(len(fx), -1, samples)
 
         # Quantities for subintervals.
         Ifxsubs = fx @ wt * halfh
         errsubs = fx @ ewt * halfh
 
         # Quantities for all of [a, b].
-        Ifx = np.sum(Ifxsubs) + IfxOK
-        errbnd = abs(np.sum(errsubs) + errOK)
+        Ifx = Ifxsubs.sum(1) + IfxOK
+        errbnd = abs(errsubs.sum(1) + errOK)
 
         # Test for convergence:
-        tol = max(atol, rtol*np.abs(Ifx))
-        if errbnd <= tol:
+        tol = np.maximum(atol, rtol*np.abs(Ifx))
+        if np.all(errbnd <= tol):
             converged = True
             break
 
         # Locate subintervals where the approximate integrals are
         # sufficiently accurate and use them to update partial sums.
-        good = np.abs(errsubs) <= (2/tbma)*halfh*tol
-        errOK += np.sum(errsubs[good])
-        IfxOK += np.sum(Ifxsubs[good])
+        good = np.all(np.abs(errsubs) <= (2/tbma)*halfh*tol[:, None], 0)
+        errOK += np.sum(errsubs[:, good])
+        IfxOK += np.sum(Ifxsubs[:, good])
         # Only keep subintervals which are not yet sufficiently accurate
         subs = subs[~good, :]
         if subs.size == 0:  # all intervals are accurate
             converged = True
             break
 
         # Split the remaining subintervals in half. Quit if splitting
         # results in too many subintervals.
         many_subint = 2*subs.size > 650  # multiplied limit by 10x MC 26/FEB/2008
         if many_subint:
             break
-        midpt = np.sum(subs, axis=1)/2
+        midpt = subs.sum(1)/2
         tmp = np.column_stack([subs[:, 0], midpt, midpt, subs[:, 1]])
         subs = tmp.reshape(-1, 2)  # ---> subs[n, 2]
         first = False
 
     if first and not converged:
         if too_close:
             print('***Sub intervals too close.')
@@ -267,15 +275,15 @@
         elif many_subint:
             print('***Too many sub intervals.')
         OK = False
 
     if plot:
         plt.figure('quad1d')
         w = np.argsort(xall)
-        plt.plot(xall[w], yall[w])
+        plt.plot(xall[w], yall.T[w])
 
     return Ifx, errbnd, OK, fcall, vfcall
 
 ################################################################################
 
 class quad1d:
     """
@@ -284,17 +292,23 @@
     ``q.integ`` and ``q.errbnd`` will contain the value of the integral 
     and the corresponding estimate of the error bound.
 
     When ``INTERVAL = [A,B]``, computes the integral of a continuous function
     ``f(x)`` from A to B for A < B.  A can be ``-np.inf`` and/or B can be
     ``np.inf``.
 
-    FUN accepts a row vector X and returns a vector Y with ``Y(m) = f(X(m))``
+    FUN accepts a row vector X and returns a vector Y with ``Y[m] = f(X[m])``
     for ``m = 1,...,len(X)``.
 
+    FUN can also be a vector function. In this case the function must return a
+    matrix, where every row ``matrix[j, m] = f(X[m])``. In this case the
+    procedure returns the integral of all components, computed using the same
+    set of evaluation points. The convergence criterion ensures that all
+    components satisfy the required tolerance.
+
     quad1d returns an approximation Ifx to the integral and optionally an
     approximate bound, ERRBND, on the error ``|integral - Ifx|``. It attempts
     to compute Ifx such that ``|Ifx - integral| <= max(ABSTOL,RELTOL*|Ifx|)``.
     If quad1d is unsuccessful, Ifx and ERRBND are still meaningful, so a
     warning is issued that includes ERRBND.
 
     If the interval is infinite, say ``[a, np.inf)``, then for the integral to
@@ -416,14 +430,18 @@
         else:
 
             tinterval = np.linspace(-1, 1, 11)
             Ifx, errbnd, OK, fcall, vfcall = _qva_Vadapt(
                 _qva_f5, tinterval, rtol, atol, samples, nodes, wt, ewt,
                 fun, a, b, args, plot)
 
+        if len(Ifx) == 1:
+            Ifx = Ifx[0]
+            errbnd = errbnd[0]
+
         if OK:
             status = 0  # success   
         else:
             print('***Integral does not satisfy error test.')
             print('***Approximate bound on error is', errbnd)
             status = 1
```

### Comparing `jampy-7.1.0/jampy/quad2d.py` & `jampy-7.2.0/jampy/quad2d.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 #############################################################################
 
-    Copyright (C) 2019, Michele Cappellari
+    Copyright (C) 2019-2023, Michele Cappellari
 
     E-mail: michele.cappellari_at_physics.ox.ac.uk
 
     Updated versions of the software are available from PyPi
     https://pypi.org/project/jampy
 
 
@@ -18,15 +18,20 @@
     provided this copyright and disclaimer are included unchanged
     at the beginning of the file. All other rights are reserved.
     In particular, redistribution of the code is not allowed.
 
 #############################################################################
 
 V1.0.0: Ported to Python from Shampine's MATLAB version
-        by Michele Cappellari, Oxford, 4 June 2019
+    by Michele Cappellari, Oxford, 4 June 2019
+
+V2.0.0: Allow for quadrature of vector functions. Uses the same set of
+    evaluation points for all components of the function and ensures that
+    the convergence criterion is satisfied for all.
+    MC, Oxford, 11 June 2023
 
 """
 import numpy as np
 import matplotlib.pyplot as plt
 
 ################################################################################
 
@@ -40,14 +45,16 @@
     It implements the algorithm described in
     `Shampine (2008) <https://doi.org/10.1016/j.amc.2008.02.012>`_
 
     Calling Sequence
     ----------------
 
     .. code-block:: python
+    
+        from jampy.quad2d import quad2d
 
         res = quad2d(fun, [a, b], [c, d], epsrel=0, epsabs=1e-5,  args=())
         print(f"integral = {res.integ} +/- {res.errbnd}")
         print("function calls:", res.fcall)
 
     approximates the integral
 
@@ -62,28 +69,36 @@
         Evaluates ``f(x,y)``.  It must accept arrays X and Y and return an
         array ``Z = f(X,Y)`` of corresponding values. These arrays are all 14x14.
         The region is a generalized rectangle which is described in Cartesian
         coordinates (x,y) by ``a <= x <= b`` -- A and B must be constants and
         ``c <= y <= d`` -- C and D can be constants or functions of x that
         describe the lower and upper boundaries. Functions must be vectorized.
         ``res.integ`` is an approximation to the integral with an estimated
-        bound ``ERRBND`` on the error that satisfies  ``ERRBND <= 1e-5``.
+        bound ``res.errbnd`` on the error that satisfies  ``res.errbnd <= 1e-5``.
+
+        ``fun`` can also be a vector function ``fun = [f_1, f_2,... f_n]``.
+        In this case the ``fun`` must return a ``matrix[j, :] = f_j(X, Y)``.
+        In this case the procedure returns the integral of all components,
+        computed using the same set of evaluation points. The convergence
+        criterion ensures that all components satisfy the required tolerance.
+
     epsabs:
         Absolute error tolerance
     epsrel:
         Relative error tolerance
 
         quad2d attempts to satisfy ERRBND <= max(epsabs, epsrel*|Q|).
         This is absolute error control when |Q| is sufficiently small and
         relative error control when |Q| is larger. A default tolerance
         value is used when a tolerance is not specified. The default value
         of 'epsrel' is 1e-5. The default value of 'epsabs' is 0.
-    singular: quad2d can be applied to f(x,y) that are singular on a
-       boundary. With value True, this option causes quad2d to use
-       transformations to weaken singularities for better performance.
+    singular: 
+       quad2d can be applied to f(x,y) that are singular on a boundary. 
+       With value True, this option causes quad2d to use transformations 
+       to weaken singularities for better performance.
     args:
         Parameters to pass to the user function ``fun``
 
     """
     def __init__(self, fun, xlim, ylim, epsrel=1e-5, epsabs=0,
                  plot=False, verbose=False, singular=False, args=()):
 
@@ -139,23 +154,22 @@
                         0.1046562260264672])
 
         # Compute initial approximations on four subrectangles.  Initialize LIST
         # of information about subrectangles for which the approximations are
         # not sufficiently accurate.  NLIST is the number of subrectangles that
         # remain to be processed.  ERRBND is a bound on the error.
         Qsub, esub = self.tensor(a, b, thetaL, thetaR, phiB, phiT, WT3, WT7, args)
-        self.integ = Qsub.sum()
+        self.integ = Qsub.sum(1)
         # Use an artificial value of TOL to force the program to refine.
         self.TOL = self.EPS*np.abs(self.integ)
         self.ERR_OK = 0
-        self.ADJUST = 1
-        self.LIST = np.zeros((200, 7))
-        self.NLIST = -1
+        self.ADJUST = np.ones_like(self.integ)
+        self.LIST = []
         self.Save2LIST(Qsub, esub, thetaL, thetaR, phiB, phiT)
-        if self.NLIST < 0 or self.errbnd <= self.TOL:
+        if len(self.LIST) < 0 or np.all(self.errbnd <= self.TOL):
             return
 
         while True:
             # Get entries from LIST corresponding to the biggest (adjusted) error.
             q, e, thetaL, thetaR, phiB, phiT = self.NextEntry()
 
             # Approximate integral over four subrectangles.
@@ -165,31 +179,35 @@
             # approximation "q" of the integral over a rectangle.  Newq = sum(Qsub)
             # is a much better approximation to the integral.  It is used here to
             # estimate the error in "q" and thereby determine that the estimator is
             # conservative by a factor of "ADJUST".  This factor is applied to the
             # estimate of the error in "Newq" to get a more realistic estimate.
             # This scheme loses the sign of the error, so a conservative local test
             # is used to decide convergence.
-            Newq = Qsub.sum()
-            self.ADJUST = min(1, abs(q - Newq)/e)
+            Newq = Qsub.sum(1)
+            self.ADJUST = np.minimum(1, abs(q - Newq)/e)
             self.integ += Newq - q
-            TOL = max(epsabs, epsrel*abs(self.integ))/8
-            TOL = max(TOL, self.EPS*abs(self.integ))
+            TOL = np.maximum(epsabs, epsrel*abs(self.integ))/8
+            TOL = np.maximum(TOL, self.EPS*abs(self.integ))
             self.Save2LIST(Qsub, esub, thetaL, thetaR, phiB, phiT)
 
             # Test for convergence and failures.
-            if self.NLIST < 0 or self.errbnd <= TOL:
+            if len(self.LIST) < 0 or np.all(self.errbnd <= TOL):
                 break
-            elif self.NLIST >= 2000:
-                if self.errbnd > max(epsabs, max(self.EPS, epsrel)*abs(self.integ)):
-                    raise ValueError(f'Maximum number of subintervals {self.NLIST}: Q does NOT pass error test.')
+            elif len(self.LIST) >= 2000:
+                if np.all(self.errbnd > np.maximum(epsabs, max(self.EPS, epsrel)*abs(self.integ))):
+                    raise ValueError(f'Maximum number of subintervals {len(self.LIST)}: Q does NOT pass error test.')
                 else:
-                    print(f'Maximum number of subintervals {self.NLIST}: Q appears to pass error test.')
+                    print(f'Maximum number of subintervals {len(self.LIST)}: Q appears to pass error test.')
                 break
 
+        if len(self.integ) == 1:
+            self.integ = self.integ[0]
+            self.errbnd = self.errbnd[0]
+
         if verbose:
             print(f"Integral: {self.integ} +/- {self.errbnd}")
             print(f"Function calls: {self.fcall} Function evaluations: {self.fcall*14**2}")
 
         if self.plot:
             self.axis[1].tricontourf(self.xall, self.yall, self.zall)
             self.axis[1].plot(self.xall, self.yall, 'w,')
@@ -217,29 +235,33 @@
         if self.singular:
             t = 0.5 + 0.5*np.cos(phi)
         else:
             t = phi
         x = np.tile(xx, (2*n, 1))
         y = bottom + t*dydt
         z = self.FUN(x.ravel(), y.ravel(), *args)
-        z = z.reshape(x.shape)
+
+        if z.ndim == 1:
+            z = z[None, :]
+
+        z = z.reshape(len(z), *x.shape)
         self.fcall += 1
         if self.singular:
             z *= 0.25*(b - a)*np.sin(phi)*(dydt*np.sin(theta))
         else:
             z *= dydt
 
-        # Split array into four n*n quadrants
-        zz = z.reshape(2, n, 2, n).swapaxes(1, 2).reshape(4, n, n)
+        # For each component, split array into four n*n quadrants
+        zz = z.reshape(len(z), 2, n, 2, n).swapaxes(2, 3).reshape(len(z), 4, n, n)
 
-        # Four tensor products: Gauss 3 point formula
+        # Four tensor products per component: Gauss 3 point formula
         esub = WT3 @ zz @ WT3
         esub = (esub/4)*(dtheta/2)*(dphi/2)
 
-        # Four tensor products: Kronrod 7 point formula
+        # Four tensor products per component: Kronrod 7 point formula
         Qsub = WT7 @ zz @ WT7
         Qsub = (Qsub/4)*(dtheta/2)*(dphi/2)
 
         esub = np.abs(esub - Qsub)
 
         if self.plot:
             self.axis[0].plot(x.ravel(), y.ravel(), '+')
@@ -252,59 +274,53 @@
 ################################################################################
 
     def NextEntry(self):
         """
         Take entries from LIST corresponding to the biggest adjusted error
 
         """
-        index = np.argmax(np.abs(self.LIST[:self.NLIST + 1, 6]))
-        row = self.LIST[index, :6]
-        self.LIST = np.delete(self.LIST, index, axis=0)
-        self.NLIST -= 1
+        adjerr = [a[6] for a in self.LIST]
+        index = np.argmax(np.max(np.abs(adjerr), 1))
+        row = self.LIST.pop(index)
 
-        return row
+        return row[:6]
 
 ################################################################################
 
     def Save2LIST(self, Qsub, esub, thetaL, thetaR, phiB, phiT):
         """
         Save to the list information about subrectangles for which the
         integral is not sufficiently accurate. NLIST is the number of
         subrectangles to be processed.
 
         """
         dtheta = thetaR - thetaL
         dphi = phiT - phiB
         localtol = self.TOL*(dtheta/2)*(dphi/2)/self.AREA
-        localtol = max(localtol, self.EPS*abs(Qsub.sum()))
+        localtol = np.maximum(localtol, self.EPS*abs(Qsub.sum(1)))
+
+        adjerr = self.ADJUST[:, None]*esub
 
-        adjerr = self.ADJUST*esub
-        if self.NLIST + 5 > len(self.LIST):
-            self.LIST = np.vstack([self.LIST, np.zeros((100, 7))])
-
-        if adjerr[0] > localtol:
-            self.NLIST += 1
-            self.LIST[self.NLIST] = [Qsub[0], esub[0], thetaL, thetaL + dtheta/2, phiB, phiB + dphi/2, adjerr[0]]
+        if np.all(adjerr[:, 0] > localtol):
+            self.LIST.append([Qsub[:, 0], esub[:, 0], thetaL, thetaL + dtheta/2, phiB, phiB + dphi/2, adjerr[:, 0]])
         else:
-            self.ERR_OK += adjerr[0]
+            self.ERR_OK += adjerr[:, 0]
 
-        if adjerr[1] > localtol:
-            self.NLIST += 1
-            self.LIST[self.NLIST] = [Qsub[1], esub[1], thetaL + dtheta/2, thetaR, phiB, phiB + dphi/2, adjerr[1]]
+        if np.all(adjerr[:, 1] > localtol):
+            self.LIST.append([Qsub[:, 1], esub[:, 1], thetaL + dtheta/2, thetaR, phiB, phiB + dphi/2, adjerr[:, 1]])
         else:
-            self.ERR_OK += adjerr[1]
+            self.ERR_OK += adjerr[:, 1]
 
-        if adjerr[2] > localtol:
-            self.NLIST += 1
-            self.LIST[self.NLIST] = [Qsub[2], esub[2], thetaL, thetaL + dtheta/2, phiB + dphi/2, phiT, adjerr[2]]
+        if np.all(adjerr[:, 2] > localtol):
+            self.LIST.append([Qsub[:, 2], esub[:, 2], thetaL, thetaL + dtheta/2, phiB + dphi/2, phiT, adjerr[:, 2]])
         else:
-            self.ERR_OK += adjerr[2]
+            self.ERR_OK += adjerr[:, 2]
 
-        if adjerr[3] > localtol:
-            self.NLIST += 1
-            self.LIST[self.NLIST] = [Qsub[3], esub[3], thetaL + dtheta/2, thetaR, phiB + dphi/2, phiT, adjerr[3]]
+        if np.all(adjerr[:, 3] > localtol):
+            self.LIST.append([Qsub[:, 3], esub[:, 3], thetaL + dtheta/2, thetaR, phiB + dphi/2, phiT, adjerr[:, 3]])
         else:
-            self.ERR_OK += adjerr[3]
+            self.ERR_OK += adjerr[:, 3]
 
-        self.errbnd = self.ERR_OK + self.LIST[:, 6].sum()
+        adjerr = [a[6] for a in self.LIST]
+        self.errbnd = self.ERR_OK + np.sum(adjerr, 0)
 
 ################################################################################
```

### Comparing `jampy-7.1.0/jampy.egg-info/PKG-INFO` & `jampy-7.2.0/jampy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jampy
-Version: 7.1.0
+Version: 7.2.0
 Summary: JamPy: Jeans Anisotropic Models for Galactic Dynamics
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -437,15 +437,15 @@
     PSF convolution is not performed.
 plot: bool
     When ``data is not None`` setting this keyword produces a plot with the
     data/model comparison at the end of the calculation.
 quiet: bool
     Set this keyword to avoid printing values on the console.
 rbh: float, optional
-    This keyword is ignored unless ``align='cyl'`` and `analytic_los=True`.
+    This keyword is ignored unless ``align='cyl'`` and ``analytic_los=True``.
     In all other cases JAM assume a point-like central black hole.
     This scalar gives the sigma in arcsec of the Gaussian approximating the
     central black hole of mass MBH [See Section 3.1.2 of `Cappellari (2008)`_]
     The gravitational potential is indistinguishable from a point source
     for ``radii > 2*rbh``, so the default ``rbh=0.01`` arcsec is appropriate
     in most current situations.
 
@@ -467,18 +467,18 @@
     with a first call to ``jam_axi_proj`` with PSF convolution, and the
     model predictions at large radii with a second call to ``jam_axi_proj``
     without PSF convolution.
 step: float, optional
     Spatial step for the model calculation and PSF convolution in arcsec.
     This value is automatically computed by default as
     ``step=max(sigmapsf,pixsize/2)/4``. It is assumed that when ``pixsize``
-    or ``sigmapsf`` are large, high-resolution calculations are not needed. In
-    some cases, however, e.g. to accurately estimate the central Vrms in a
-    very cuspy galaxy inside a large aperture, one may want to override the
-    default value to force smaller spatial pixels using this keyword.
+    or ``sigmapsf`` are large, high-resolution calculations are not needed.
+    In some cases, however, e.g. to accurately estimate the central Vrms in
+    a very cuspy galaxy inside a large aperture, one may want to override
+    the default value to force smaller spatial pixels using this keyword.
 vmax: float, optional
     Maximum value of the ``data`` to plot.
 vmin: float, optional
     Minimum value of the ``data`` to plot.
 
 Output Parameters
 -----------------
@@ -789,36 +789,43 @@
 License
 =======
 
 Other/Proprietary License
 
 Copyright (c) 2003-2023 Michele Cappellari
 
-This software is provided as is without any warranty whatsoever.
-Permission to use, for non-commercial purposes is granted.
-Permission to modify for personal or internal use is granted,
-provided this copyright and disclaimer are included in all 
-copies of the software. All other rights are reserved.
-In particular, redistribution of the code is not allowed.
+This software is provided as is with no warranty. You may use it for
+non-commercial purposes and modify it for personal or internal use, as long
+as you include this copyright and disclaimer in all copies. You may not
+redistribute the code.
+
+###########################################################################
 
 Changelog
 =========
 
-V7.1.0: MC, Oxford, 1 June 2023
+V7.2.0: MC, Oxford, 20 July 2023
+    - ``jam_axi_intr``: Integrate all velocity components at the same time with
+      a single call to the updated ``quad1d`` and ``quad2d``. Significant speedup.
+    - ``quad1d``, ``quad2d``: Allow for integration of vector functions.
+      All components are integrated over the same set of evaluation points.
+    - ``jam_axi_proj``: Updated verbose output with more information.
+
+V7.1.0: MC, Oxford, 5 June 2023
     - Separated computation for the black hole kinematics for both the
       cylindrically and spherically-aligned solutions. In both cases this
       removed one numerical quadrature. This is useful in extreme situations,
       when the minimum radius one wants to model around the black hole is orders
       of magnitude smaller than the smallest MGE Gaussian. This change
       eliminated the need for the ``rbh`` keyword in ``jam_axi_intr``, which I
       removed. The only case where the black hole is still approximated with a
       small Gaussian is in ``jam_axi_proj`` when both ``align='cyl'`` and
       ``analytic_los=True``.
-    - Adopted consistent minimum radius, based on ``step``, for both the
-      intrinsic and projected interpolation grids.
+    - Adopted minimum radius based on ``step`` for the intrinsic interpolation
+      grid as already done for the projected one.
     - Simplified minimum-inclination test.
     - Removed ``legacy`` folder with old redundant procedures.
     - Moved the formalism for the LOS analytic integrand with ``align='cyl'``
       into ``jam_axi_proj``.
     - ``jam_axi_proj``, ``jam_axi_intr``, ``jam_sph_proj``, ``jam_sph_intr``:
       New keyword ``logistic`` to specify when JAM should interpret the input
       anisotropy parameters ``beta`` and ``gamma`` as defining a logistic
```

### Comparing `jampy-7.1.0/jampy.egg-info/SOURCES.txt` & `jampy-7.2.0/jampy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 setup.py
 jampy/CHANGELOG.rst
 jampy/LICENSE.txt
 jampy/README.rst
 jampy/__init__.py
 jampy/jam_axi_intr.py
 jampy/jam_axi_proj.py
+jampy/jam_axi_sersic_mass.py
 jampy/jam_sph_intr.py
 jampy/jam_sph_proj.py
 jampy/mge_half_light_isophote.py
 jampy/mge_radial_density.py
 jampy/mge_radial_mass.py
 jampy/mge_vcirc.py
 jampy/quad1d.py
```

### Comparing `jampy-7.1.0/setup.py` & `jampy-7.2.0/setup.py`

 * *Files identical despite different names*

