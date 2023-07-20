# Comparing `tmp/ltsfit-5.0.20.tar.gz` & `tmp/ltsfit-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltsfit-5.0.20.tar", last modified: Mon Oct  3 16:57:26 2022, max compression
+gzip compressed data, was "ltsfit-6.0.1.tar", last modified: Thu Jul 20 11:20:32 2023, max compression
```

## Comparing `ltsfit-5.0.20.tar` & `ltsfit-6.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-10-03 16:57:26.677032 ltsfit-5.0.20/
--rw-rw-rw-   0        0        0    12885 2022-10-03 16:57:26.675984 ltsfit-5.0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-03 16:57:26.636550 ltsfit-5.0.20/ltsfit/
--rw-rw-rw-   0        0        0     3215 2022-10-03 16:26:15.000000 ltsfit-5.0.20/ltsfit/CHANGELOG.rst
--rw-rw-rw-   0        0        0      442 2022-10-03 15:42:50.000000 ltsfit-5.0.20/ltsfit/LICENSE.txt
--rw-rw-rw-   0        0        0     2654 2022-10-03 16:55:01.000000 ltsfit-5.0.20/ltsfit/README.rst
--rw-rw-rw-   0        0        0       24 2022-10-03 16:57:15.000000 ltsfit-5.0.20/ltsfit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-03 16:57:26.673720 ltsfit-5.0.20/ltsfit/examples/
--rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 ltsfit-5.0.20/ltsfit/examples/__init__.py
--rw-rw-rw-   0        0        0     2543 2020-02-17 19:17:41.000000 ltsfit-5.0.20/ltsfit/examples/lts_fits_python_reference_output.txt
--rw-rw-rw-   0        0        0     1980 2022-09-20 10:15:55.000000 ltsfit-5.0.20/ltsfit/examples/lts_linefit_example.py
--rw-rw-rw-   0        0        0     2131 2022-05-20 17:12:50.000000 ltsfit-5.0.20/ltsfit/examples/lts_planefit_example.py
--rw-rw-rw-   0        0        0    14472 2022-10-03 16:55:01.000000 ltsfit-5.0.20/ltsfit/lts_linefit.py
--rw-rw-rw-   0        0        0    17481 2022-10-03 16:55:01.000000 ltsfit-5.0.20/ltsfit/lts_planefit.py
-drwxrwxrwx   0        0        0        0 2022-10-03 16:57:26.664207 ltsfit-5.0.20/ltsfit.egg-info/
--rw-rw-rw-   0        0        0    12885 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-03 16:57:26.000000 ltsfit-5.0.20/ltsfit.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2022-10-03 16:57:26.678455 ltsfit-5.0.20/setup.cfg
--rw-rw-rw-   0        0        0     1723 2022-10-03 16:48:21.000000 ltsfit-5.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:20:32.757317 ltsfit-6.0.1/
+-rw-rw-rw-   0        0        0    13646 2023-07-20 11:20:32.757317 ltsfit-6.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-20 11:20:32.726063 ltsfit-6.0.1/ltsfit/
+-rw-rw-rw-   0        0        0     3961 2023-07-20 10:55:57.000000 ltsfit-6.0.1/ltsfit/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      398 2023-07-07 13:04:21.000000 ltsfit-6.0.1/ltsfit/LICENSE.txt
+-rw-rw-rw-   0        0        0     2751 2023-07-07 13:18:09.000000 ltsfit-6.0.1/ltsfit/README.rst
+-rw-rw-rw-   0        0        0       23 2023-07-20 10:56:06.000000 ltsfit-6.0.1/ltsfit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:20:32.757317 ltsfit-6.0.1/ltsfit/examples/
+-rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 ltsfit-6.0.1/ltsfit/examples/__init__.py
+-rw-rw-rw-   0        0        0     6416 2023-07-20 11:18:04.000000 ltsfit-6.0.1/ltsfit/examples/ltsfit_examples.py
+-rw-rw-rw-   0        0        0     4151 2023-07-20 10:53:10.000000 ltsfit-6.0.1/ltsfit/examples/ltsfit_python_reference_output.txt
+-rw-rw-rw-   0        0        0      710 2023-07-18 06:10:19.000000 ltsfit-6.0.1/ltsfit/lts_linefit.py
+-rw-rw-rw-   0        0        0      980 2023-07-18 06:12:24.000000 ltsfit-6.0.1/ltsfit/lts_planefit.py
+-rw-rw-rw-   0        0        0    21941 2023-07-20 11:19:29.000000 ltsfit-6.0.1/ltsfit/ltsfit.py
+drwxrwxrwx   0        0        0        0 2023-07-20 11:20:32.757317 ltsfit-6.0.1/ltsfit.egg-info/
+-rw-rw-rw-   0        0        0    13646 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 11:20:32.000000 ltsfit-6.0.1/ltsfit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-20 11:20:32.757317 ltsfit-6.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1652 2023-07-20 10:57:13.000000 ltsfit-6.0.1/setup.py
```

### Comparing `ltsfit-5.0.20/PKG-INFO` & `ltsfit-6.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltsfit
-Version: 5.0.20
+Version: 6.0.1
 Summary: LtsFit: Least Trimmed Squares Fitting
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,38 +12,38 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 
 The LtsFit Package
 ==================
 
-**Robust Linear Regression with Scatter in One or Two Dimensions**
+**Robust Least Squares Regression with Uncertainties and Scatter in Any Dimension**
 
 .. image:: https://img.shields.io/pypi/v/ltsfit.svg
     :target: https://pypi.org/project/ltsfit/
 .. image:: https://img.shields.io/badge/arXiv-1208.3522-orange.svg
     :target: https://arxiv.org/abs/1208.3522
 .. image:: https://img.shields.io/badge/DOI-10.1093/mnras/stt562-green.svg
     :target: https://doi.org/10.1093/mnras/stt562
 
-LtsFit is a Python implementation of the method described in Section 3.2 of
+LtsFit is a Python package for **very robust** hyperplane fitting in N dimensions,
+with uncertainties in all coordinates and intrinsic scatter. It implements the
+method described in Section 3.2 of
 `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-to perform **very robust** fits of lines or planes to data with errors in all
-coordinates, while allowing for possible intrinsic scatter.
-Outliers are iteratively clipped using the robust Least Trimmed Squares (LTS)
-technique by `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+and uses the Least Trimmed Squares (LTS) technique to iteratively clip outliers
+`(Rousseeuw & van Driessen 2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
 
 .. contents:: :depth: 2
 
 Attribution
 -----------
 
-If you use this software for your research, please also cite
-`Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-where the implementation was described. The BibTeX entry for the paper is::
+Please also cite `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+if you use this software for your research. This is the paper where the
+implementation was described. The BibTeX entry for the paper is::
 
     @ARTICLE{Cappellari2013a,
         author = {{Cappellari}, M. and {Scott}, N. and {Alatalo}, K. and
             {Blitz}, L. and {Bois}, M. and {Bournaud}, F. and {Bureau}, M. and
             {Crocker}, A.~F. and {Davies}, R.~L. and {Davis}, T.~A. and {de Zeeuw},
             P.~T. and {Duc}, P.-A. and {Emsellem}, E. and {Khochfar}, S. and
             {Krajnovi{\'c}}, D. and {Kuntschner}, H. and {McDermid}, R.~M. and
@@ -67,241 +67,215 @@
 
     pip install ltsfit
 
 Without writing access to the global ``site-packages`` directory, use::
 
     pip install --user ltsfit
 
+To upgrade the package to the latest version use::
+
+    pip install --upgrade ltsfit
+
 Documentation
 -------------
 
 See ``ltsfit/examples`` and the files docstrings.
 They are copied by ``pip`` within the global folder
 `site-packages <https://stackoverflow.com/a/46071447>`_.
 
 ###########################################################################
 
-lts_linefit
-===========
+ltsfit
+======
 
 Purpose
 -------
 
-Best straight-line *robust* fit to data with errors in
-both coordinates while fitting for the intrinsic scatter.
-See `Cappellari et al. (2013a, Sec.3.2)
-<https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+Fit a linear function of the form::
 
-Explanation
------------
+    y = a + b1*x1 + b2*x2 +...+ bm*xm,
 
-Linear Least-squares approximation in one-dimension (y = a + b*x),
-when both x and y data have errors and allowing for intrinsic
-scatter in the relation.
-
-Outliers are iteratively clipped using the extremely robust
-FAST-LTS technique by
-`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
+to data with errors in all coordinates and intrinsic scatter, using a robust
+method that clips outliers. The function can handle lines in 2-dim, planes in
+3-dim, or hyperplanes in N-dim, where ``x1, x2,..., xm`` are the independent
+variables and ``y`` is the dependent variable. The method was introduced in
+Sec. 3.2 of `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+and the treatment of outliers is is based on the FAST-LTS technique by
+`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_.
 
 Calling Sequence
 ----------------
 
 .. code-block:: python
 
-    p = lts_linefit(x, y, sigx, sigy, clip=2.6, epsy=True, corr=True,
-                  frac=None, pivot=None, plot=True, text=True)
+    from ltsfit.ltsfit import ltsfit
 
-The output values are stored as attributes of "p".
-See usage example at the bottom of this file.
+    p = ltsfit(x, y, sigx, sigy, clip=2.6, corr=True, epsy=True,
+               frac=None, label='Fitted', label_clip='Clipped',
+               legend=True, pivot=None, plot=True, text=True)
 
-Input Parameters
-----------------
-
-x, y:
-    vectors of size N with the measured values.
-sigx, sigy:
-    vectors of size N with the 1sigma errors in x and y.
-clip:
-    values deviating more than clip*sigma from the best fit are
-    considered outliers and are excluded from the linear fit.
-epsy:
-    if True, the intrinsic scatter is printed on the plot.
-corr:
-    if True, the correlation coefficients are printed on the plot.
-frac:
-    fractions of values to include in the LTS stage.
-    Up to a fraction "frac" of the values can be outliers.
-    One must have 0.5 < frac < 1  (default frac=0.5).
-
-    NOTE: Set frac=1, to turn off outliers detection.
-label:
-    optional string label to create a legend outside the procedure.
-pivot:
-    if this is not None, then lts_linefit fits the relation::
-
-        y = a + b*(x - pivot)
-
-    pivot is called x_0 in eq.(6) of Cappellari et al. (2013)
-    Use of this keyword is *strongly* recommended and a suggested
-    value is pivot ~ np.mean(x). This keyword is important to
-    reduce the covariance between a and b.
-plot:
-    if True a plot of the fit is produced.
-text:
-    if True, the best fitting parameters are printed on the plot.
+    print(f"Best fitting parameters: {p.coeff}")
 
-Output Parameters
------------------
+The output values are stored as attributes of the ``p`` object.
 
-The output values are stored as attributed of the lts_linefit class.
-
-p.ab:
-    best fitting parameters [a, b]
-p.ab_err:
-    1*sigma formal errors [a_err, b_err] on a and b.
-p.mask:
-    boolean vector with the same size of x and y.
-    It contains True  for the elements of (x, y) which were included in
-    the fit and False for the outliers which were automatically clipped.
-p.rms:
-    rms = np.std(fit - y) beteween the data and the fitted relation.
-p.sig_int:
-    intrinsic scatter around the linear relation.
-    sig_int is called epsilon_y in eq.(6) of Cappellari et al. (2013).
-p.sig_int_err:
-    1*sigma formal error on sig_int.
-
-###########################################################################
-
-
-lts_planefit
-============
-
-Purpose
--------
-
-Best plane *robust* fit to data with errors in all
-three coordinates and fitting for the intrinsic scatter.
-See `Cappellari et al. (2013a, Sec.3.2)
-<https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-
-Explanation
------------
-
-Linear Least-squares approximation in two-dimension (z = a + b*x + c*y),
-when x, y and z data have errors, and allowing for intrinsic
-scatter in the relation.
-
-Outliers are iteratively clipped using the extremely robust
-FAST-LTS technique by
-`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
-
-Calling Sequence
+Input Parameters
 ----------------
 
-.. code-block:: python
-
-    p = lts_planefit(x, y, z, sigx, sigy, sigz, clip=2.6, epsz=True,
-                    frac=None, pivotx=None, pivoty=None, plot=True, text=True)
+x: array_like with shape (n, m)
+    Array of ``n`` independent variables for ``m`` dimensions.
 
-The output values are stored as attributes of "p".
-See usage example at the bottom of this file.
+    EXAMPLE: To fit a line in 2-dim, one has a single vector ``x`` of
+    length ``n`` with the independent variable and a corresponding vector of
+    dependent variable ``y``.
+
+    EXAMPLE: To fit a plane in 3-dim, one has two vectors of length ``n`` of
+    independent variables ``(x1, x2)``. In this case,
+    ``x = np.column_stack([x1, x2])``.
+
+    EXAMPLE: To fit a hyperplane in 4-dim, one has three vectors of
+    independent variables ``(x1, x2, x3)``. In this case,
+    ``x = np.column_stack([x1, x2, x3])``.
+y: array_like with shape (n,)
+    Vector of measured values for each set of ``x`` variables.
+sigx: array_like with shape (n, m)
+    Array of ``1sigma`` uncertainties for each ``x`` coordinate for ``m``
+    dimensions. This has the same shape as ``x``.
+sigy: array_like with shape (n,)
+    Vector of ``1sigma`` uncertainties for each ``y`` value.
 
-Input Parameters
-----------------
+Optional Keywords
+-----------------
 
-x, y, z:
-    vectors of size N with the measured values.
-sigx, sigy, sigz:
-    vectors of size N with the 1sigma errors in x , y and z.
-clip:
-    values deviating more than clip*sigma from the best fit are
-    considered outliers and are excluded from the plane fit.
-epsz:
-    if True, the intrinsic scatter is printed on the plot.
-frac:
-    fractions of values to include in the LTS stage.
-    Up to a fraction "frac" of the values can be outliers.
-    One must have 0.5 <= frac <= 1  (default frac=0.5).
-
-    NOTE: Set frac=1, to turn off outliers detection.
-pivotx, pivoty:
-    if these are not None, then lts_planefit fits the plane::
-
-        z = a + b*(x - pivotx) + c*(y - pivoty)
-
-    pivotx, pivoty are called x_0, y_0 in eq.(7) of Cappellari et al. (2013)
-    Use of these keywords is *strongly* recommended, and suggested
-    values are ``pivotx=np.median(x), pivoty=np.median(y)``.
-    This keyword is important to reduce the covariance between a, b and c.
-plot:
-    if True a plot of the fit is produced.
-text:
-    if True, the best fitting parameters are printed on the plot.
+clip: float
+    Clipping threshold in ``sigma`` units. Values deviating more than
+    ``clip*sigma`` from the best fit are considered outliers and are
+    excluded from the fit. Default is ``clip=2.6``, which would include
+    99% of the values for a Gaussian distribution.
+corr: bool
+    if ``True``, the correlation coefficients are printed on the plot.
+    Default is ``True``.
+epsy: bool
+    If ``True``, the intrinsic scatter is printed on the output plot.
+    Default is ``True``.
+frac: float
+    Fraction of values to include in the LTS stage.
+    Up to a fraction ``frac`` of the values can be outliers.
+    One must have ``0.5 <= frac <= 1``. Default is ``0.5``.
+
+    NOTE: Set ``frac=1`` to turn off outlier detection.
+pivot: array_like with shape (m,)
+    If nonzero, then ``ltsfit`` fits the following line, plane or hyperplane::
+
+        y = a + b0*(x0 - pivot[0]) + b1*(x1 - pivot[1]) + ...
+
+    ``pivot`` are called ``x_0``, ``y_0`` in eq.(7) of `Cappellari et al. (2013a)`_.
+    Use of this keyword is strongly recommended, and suggested values are
+    ``pivot = np.median(x, 0)``. This keyword has no effect on the best fit
+    but is important to reduce the covariance and uncertainty in the
+    intercept ``a``.  However, the covariance is weakly dependent on the
+    precise value of the ``pivot``. For this reason, it is generally better
+    to round the ``pivot`` values to nice numbers. Default is ``0``.
+plot: bool
+    If ``True``, a plot of the fit is produced. Default is ``True``.
+text: bool
+    If ``True``, the best fitting parameters are printed on the plot.
+    Default is ``True``.
 
 Output Parameters
 -----------------
 
-The output values are stored as attributed of the lts_linefit class.
+The output values are stored as attributes of the ``ltsfit`` class.
 
-p.abc:
-    best fitting parameters [a, b, c]
-p.abc_err:
-    1*sigma formal errors [a_err, b_err, c_err] on a, b and c.
-p.mask:
-    boolean vector with the same size of x, y and z.
-    It contains True for the elements of (x, y, z) which were included in
-    the fit and False for the outliers which were automatically clipped.
-p.rms:
-    rms = np.std(fit - z) beteween the data and the fitted relation.
-p.sig_int:
-    intrinsic scatter in the z direction around the plane.
-    sig_int is called epsilon_z in eq.(7) of Cappellari et al. (2013).
-p.sig_int_err:
-    1*sigma formal error on sig_int.
+p.coef: array_like with shape (m+1,)
+    Best fitting parameters ``[a, b1, b2,..., bm]``.
+p.coef_err: array_like with shape (m+1,)
+    ``1*sigma`` formal uncertainties ``[a_err, b1_err, b2_err,..., bm_err]``.
+p.mask: array_like with shape (n,) and dtype bool
+    Boolean vector indicating which elements of ``z`` were included in
+    the fit (``True``) and which were clipped as outliers (``False``).
+p.rms: float
+    RMS deviation between the data and the fitted relation.
+p.sig_int: float
+    Intrinsic scatter in the ``y`` direction around the line/plane/hyperplane.
+    ``sig_int`` is called ``epsilon_y`` in eq.(6) of `Cappellari et al. (2013a)`_.
+p.sig_int_err: float
+    ``1*sigma`` formal error on ``sig_int``.
+p.xx: array_like with shape (n,)
+    Values plotted along the x-axis. This is the linear combination of the
+    ``x`` variables that represents the plane/hyperplane edge-on::
+
+        xx = a + b1*(x1 - pivot[0]) + b2*(x2 - pivot[1]) + ...
+
+    For line fitting, these are just the ``x`` values.
+p.yy: array_like with shape (n,)
+    The input ``y`` values plotted along the y-axis.
+p.xerr: array_like with shape (n,)
+    ``1*sigma`` uncertainties for ``p.xx`` in the x-axis of the plot.
+p.yerr: array_like with shape (n,)
+    ``1*sigma`` uncertainties for ``p.yy`` in the y-axis of the plot.
+p.xline: array_like with shape (2,)
+    ``x`` coordinates of the best fitting relation as shown on the plot.
+p.yline: array_like with shape (2,)
+    ``y`` coordinates of the best fitting relation as shown on the plot.
+p.spearmanr: array_like with shape (2,)
+    Spearman ``r`` coefficient and probability ``p`` between ``(p.xx, p.yy)``
+    without clipping outliers.
+p.pearsonr: array_like with shape (2,)
+    Pearson ``r`` coefficient and probability ``p`` between ``(p.xx, p.yy)``
+    without clipping outliers.
 
 ###########################################################################
 
 
 
 License
 =======
 
 Other/Proprietary License
 
-Copyright (c) 2012-2022 Michele Cappellari
+Copyright (c) 2012-2023 Michele Cappellari
 
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
 
-V2.0.20: MC, Oxford, 3 October 2022
+V6.0.1: MC, Oxford, 20 July 2023
+  - New function ``ltsfit`` to fit hyperplanes in N-dim. This procedure
+    generalizes and replaces both ``lts_linefit`` and ``lts_planefit``, which
+    are now deprecated wrappers for ``ltsfit``. This change was suggested and
+    motivated by Francesco D'Eugenio (cam.ac.uk), who shared his own 4-dim
+    ``lts_hyperfit`` and his paper on a useful application.
+  - ``ltsfit``: When fitting planes/hyperplanes, plot the independent variable
+    on the y-axis to be consistent with line fitting. Also plot a legend.
+  - Updated all ``ltsfit_examples``.
+  - Fixed inconsistency between the version number on PyPi and in the Changelog.
+
+V5.0.20: MC, Oxford, 3 October 2022
   - Fixed program stop due to Matplotlib change.
     Thanks to Hitesh Lala (Heidelberg) for the report.
   - Extract documentation from docstrings and show it on PyPi.
 
-V2.0.19: MC, Oxford, 22 January 2021
+V5.0.19: MC, Oxford, 22 January 2021
   - Fixed incorrect plot ranges due to a Matplotlib change.
     Thanks to Davide Bevacqua (unibo.it) for the report.
 
-V2.0.18: MC, Oxford, 17 February 2020
+V5.0.18: MC, Oxford, 17 February 2020
   - Properly print significant trailing zeros in results.
 
-V2.0.17: MC, Oxford, 22 January 2020
+V5.0.17: MC, Oxford, 22 January 2020
   - Formatted documentation as docstring.
   - Included p.rms output.
-
+  - Published on PyPi. Increased major version number by mistake.
 
 V2.0.16: MC, Oxford, 27 September 2018
   - Fixed clock DeprecationWarning in Python 3.7.
 
 V2.0.15: MC, Oxford, 12 May 2018
   - Dropped Python 2.7 support.
```

### Comparing `ltsfit-5.0.20/ltsfit/README.rst` & `ltsfit-6.0.1/ltsfit/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 The LtsFit Package
 ==================
 
-**Robust Linear Regression with Scatter in One or Two Dimensions**
+**Robust Least Squares Regression with Uncertainties and Scatter in Any Dimension**
 
 .. image:: https://img.shields.io/pypi/v/ltsfit.svg
     :target: https://pypi.org/project/ltsfit/
 .. image:: https://img.shields.io/badge/arXiv-1208.3522-orange.svg
     :target: https://arxiv.org/abs/1208.3522
 .. image:: https://img.shields.io/badge/DOI-10.1093/mnras/stt562-green.svg
     :target: https://doi.org/10.1093/mnras/stt562
 
-LtsFit is a Python implementation of the method described in Section 3.2 of
+LtsFit is a Python package for **very robust** hyperplane fitting in N dimensions,
+with uncertainties in all coordinates and intrinsic scatter. It implements the
+method described in Section 3.2 of
 `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-to perform **very robust** fits of lines or planes to data with errors in all
-coordinates, while allowing for possible intrinsic scatter.
-Outliers are iteratively clipped using the robust Least Trimmed Squares (LTS)
-technique by `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+and uses the Least Trimmed Squares (LTS) technique to iteratively clip outliers
+`(Rousseeuw & van Driessen 2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
 
 .. contents:: :depth: 2
 
 Attribution
 -----------
 
-If you use this software for your research, please also cite
-`Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-where the implementation was described. The BibTeX entry for the paper is::
+Please also cite `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+if you use this software for your research. This is the paper where the
+implementation was described. The BibTeX entry for the paper is::
 
     @ARTICLE{Cappellari2013a,
         author = {{Cappellari}, M. and {Scott}, N. and {Alatalo}, K. and
             {Blitz}, L. and {Bois}, M. and {Bournaud}, F. and {Bureau}, M. and
             {Crocker}, A.~F. and {Davies}, R.~L. and {Davis}, T.~A. and {de Zeeuw},
             P.~T. and {Duc}, P.-A. and {Emsellem}, E. and {Khochfar}, S. and
             {Krajnovi{\'c}}, D. and {Kuntschner}, H. and {McDermid}, R.~M. and
@@ -52,14 +52,18 @@
 
     pip install ltsfit
 
 Without writing access to the global ``site-packages`` directory, use::
 
     pip install --user ltsfit
 
+To upgrade the package to the latest version use::
+
+    pip install --upgrade ltsfit
+
 Documentation
 -------------
 
 See ``ltsfit/examples`` and the files docstrings.
 They are copied by ``pip`` within the global folder
 `site-packages <https://stackoverflow.com/a/46071447>`_.
```

### Comparing `ltsfit-5.0.20/ltsfit/lts_planefit.py` & `ltsfit-6.0.1/ltsfit/ltsfit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # ###############################################################################
 #
-# Copyright (C) 2012-2021, Michele Cappellari
+# Copyright (C) 2012-2023, Michele Cappellari
 # E-mail: michele.cappellari_at_physics.ox.ac.uk
 #
 # Updated versions of the software are available from my web page
 # http://purl.org/cappellari/software
 #
 # If you have found this software useful for your research, I would
-# appreciate an acknowledgement to the use of the "LTS_PLANEFIT program
+# appreciate an acknowledgement to the use of the "LtsFit package
 # described in Cappellari et al. (2013, MNRAS, 432, 1709), which
 # combines the Least Trimmed Squares robust technique of Rousseeuw &
 # van Driessen (2006) into a least-squares fitting algorithm which
 # allows for errors in all variables and intrinsic scatter."
 #
 # This software is provided as is without any warranty whatsoever.
 # Permission to use, for non-commercial purposes is granted.
@@ -35,15 +35,15 @@
 #           MC, Baltimore, 8 June 2014
 #       V2.0.5: Text plotting changes. MC, Oxford, 26 June 2014
 #       V3.0.0: Converted from IDL into Python. MC, Oxford, 5 November 2014
 #       V3.0.1: Updated documentation. MC, Baltimore, 9 June 2015
 #       V3.0.2: Fixed potential program stop without outliers.
 #           Thanks to Masato Onodera for a clear report of the problem.
 #         - Output boolean mask instead of good/bad indices.
-#         - Removed lts_planefit_example from this file.
+#         - Removed lts_linefit_example from this file.
 #           MC, Oxford, 6 July 2015
 #       V3.0.3: Fixed potential program stop without outliers.
 #           MC, Oxford, 1 October 2015
 #       V3.0.4: Fixed potential program stop without outliers in Matplotlib 1.5.
 #           MC, Oxford, 9 December 2015
 #       V3.0.5: Use LimeGreen for outliers. MC, Oxford, 8 January 2016
 #       V3.0.6: Check for non finite values in input.
@@ -71,367 +71,448 @@
 #       Vx.x.x: Additional changes are documented in the CHANGELOG of the LtsFit package.
 #
 #------------------------------------------------------------------------------
 
 from time import perf_counter as clock
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy import optimize
+from scipy import optimize, stats
 
 #----------------------------------------------------------------------------
 
-def _planefit(x, y, z, sigz=None, weights=None):
-    """
-    Fit a plane z = a + b*x + c*y to a set of points (x, y, z)
-    by minimizing chi2 = np.sum(((z - zfit)/sigz)**2)
-
-    """
-    v1 = np.ones_like(x)
-    if weights is None:
-        if sigz is None:
-            sw = v1
-        else:
-            sw = v1/sigz
-    else:
-        sw = np.sqrt(weights)
+def _display_errors(par, sig_par, epsy):
+    """ Print parameters rounded according to their uncertainties """
 
-    a = np.column_stack([v1, x, y])
-    abc = np.linalg.lstsq(a*sw[:, None], z*sw, rcond=None)[0]
-
-    return abc
-
-#----------------------------------------------------------------------------
-
-def _display_errors(par, sig_par, epsz):
-    """
-    Print parameters rounded according to their errors
-
-    """
     prec = np.zeros_like(par)
     w = (sig_par != 0) & (par != 0)
     prec[w] = np.ceil(np.log10(np.abs(par[w]))) - np.floor(np.log10(sig_par[w])) + 1
-    prec = prec.clip(0)  # negative precisions not allowed
+    prec = prec.clip(0)  # negative precisions aren't allowed
     dg = list(map(str, prec.astype(int)))
 
-    # print on the terminal and save as string
+    txt = ['a = '] + [f'b_{j} = ' for j in range(len(par) - 2)]
 
-    txt = ['intercept: ', 'slopeX: ', 'slopeY: ', 'scatter: ']
+    txt1 = txt + ['scatter = ']
+    str_txt = ''
+    for t, d, p, s in zip(txt1, dg, par, sig_par):
+        str_txt += f"\n{t:>12} {p:#.{d}g} +/- {s:#.2g}"
+
+    if epsy:
+        txt += ['\\varepsilon_y=']
+    str_tex = ''
     for t, d, p, s in zip(txt, dg, par, sig_par):
-        print(f"{t:>{12}} {p:#.{d}g} +/- {s:#.2g}")
+        str_tex += f"${t} {p:#.{d}g} \\pm {s:#.2g}$\n"
 
-    txt = ['a=', 'b=', 'c=', '\\varepsilon_z=']
-    if not epsz:
-        txt = txt[:-1]
-    string = ''
-    for t, d, p, s in zip(txt, dg, par, sig_par):
-        string += f"${t} {p:#.{d}g} \\pm {s:#.2g}$\n"
+    return str_tex, str_txt
 
-    return string
-
-#------------------------------------------------------------------------------
+#----------------------------------------------------------------------------
 
-def _residuals(abc, x, y, z, sigx, sigy, sigz):
+def _hyperfit(x, y, sigy=None):
     """
-    See equation (7) of Cappellari et al. (2013, MNRAS, 432, 1709)
+    Fit a hyperplane yfit = a + b1*x1 + b2*x2 + ...
+    to a set of points (x1, x2,... , y)
+    by minimizing chi2 = np.sum(((y - yfit)/sigy)**2)
 
     """
-    res = (abc[0] + abc[1]*x + abc[2]*y - z) \
-        / np.sqrt((abc[1]*sigx)**2 + (abc[2]*sigy)**2 + sigz**2)
+    if sigy is None:
+        coef = np.linalg.lstsq(x, y, rcond=None)[0]
+    else:
+        coef = np.linalg.lstsq(x/sigy[:, None], y/sigy, rcond=None)[0]
 
-    return res
+    return coef
+
+#------------------------------------------------------------------------------
+
+def _residuals(coef, x, y, sigx, sigy):
+    """ See equation (7) of Cappellari et al. (2013, MNRAS, 432, 1709) """
+
+    return (x @ coef - y)/np.sqrt(sigx**2 @ coef[1:]**2 + sigy**2)
 
 #----------------------------------------------------------------------------
 
-def _fitting(x, y, z, sigx, sigy, sigz, abc):
+def _fitting(x, y, sigx, sigy, coef):
 
-    abc, pcov, infodict, errmsg, success = optimize.leastsq(
-        _residuals, abc, args=(x, y, z, sigx, sigy, sigz), full_output=1)
+    coef, pcov, infodict, errmsg, success = optimize.leastsq(
+        _residuals, coef, args=(x, y, sigx, sigy), full_output=True)
 
     if pcov is None or np.any(np.diag(pcov) < 0):
-        sig_ABC = np.full(3, np.inf)
+        sig_coef = np.full(x.shape[1], np.inf)
         chi2 = np.inf
     else:
         chi2 = np.sum(infodict['fvec']**2)
-        sig_ABC = np.sqrt(np.diag(pcov))  # ignore covariance
+        sig_coef = np.sqrt(np.diag(pcov))  # ignore covariance
 
-    return abc, sig_ABC, chi2
+    return coef, sig_coef, chi2
 
 #----------------------------------------------------------------------------
 
-def _fast_algorithm(x, y, z, sigx, sigy, sigz, h):
+def _fast_algorithm(x, y, sigx, sigy, h):
 
     # Robust least trimmed squares regression.
     # Pg. 38 of Rousseeuw & van Driessen (2006)
     # http://dx.doi.org/10.1007/s10618-005-0024-4
     #
     m = 500 # Number of random starting points
-    abcv = np.empty((m, 3))
+    ndim = x.shape[1]
+    coefv = np.empty((m, ndim))
     chi2v = np.empty(m)
     for j in range(m):  # Draw m random starting points
-        w = np.random.choice(x.size, 3, replace=False)
-        abc = _planefit(x[w], y[w], z[w])  # Find a plane going trough three random points
+        w = np.random.choice(y.size, ndim, replace=False)
+        coef = _hyperfit(x[w], y[w])  # Find a plane going through three random points
         for k in range(3):  # Run C-steps up to H_3
-            res = _residuals(abc, x, y, z, sigx, sigy, sigz)
-            good = np.argsort(np.abs(res))[:h]  # Fit the h points with smallest errors
-            abc, sig_abc, chi_sq = _fitting(x[good], y[good], z[good], sigx[good], sigy[good], sigz[good], abc)
-        abcv[j, :] = abc
+            res = _residuals(coef, x, y, sigx, sigy)
+            good = np.argsort(np.abs(res))[:h]  # Fit the h points with the smallest errors
+            coef, sig_coef, chi_sq = _fitting(x[good], y[good], sigx[good], sigy[good], coef)
+        coefv[j, :] = coef
         chi2v[j] = chi_sq
 
     # Perform full C-steps only for the 10 best results
     #
     w = np.argsort(chi2v)
     nbest = 10
     chi_sq = np.inf
     for j in range(nbest):
-        abc1 = abcv[w[j], :]
+        coef1 = coefv[w[j], :]
         while True:  # Run C-steps to convergence
-            abcOld = abc1
-            res = _residuals(abc1, x, y, z, sigx, sigy, sigz)
-            good1 = np.argsort(np.abs(res))[:h]  # Fit the h points with smallest errors
-            abc1, sig_ab1, chi1_sq = _fitting(x[good1], y[good1], z[good1], sigx[good1], sigy[good1], sigz[good1], abc1)
-            if np.allclose(abcOld, abc1):
+            coefOld = coef1
+            res = _residuals(coef1, x, y, sigx, sigy)
+            good1 = np.argsort(np.abs(res))[:h]  # Fit the h points with the smallest errors
+            coef1, sig_ab1, chi1_sq = _fitting(x[good1], y[good1], sigx[good1], sigy[good1], coef1)
+            if np.allclose(coefOld, coef1):
                 break
         if chi_sq > chi1_sq:
-            abc = abc1  # Save best solution
+            coef = coef1  # Save best solution
             good = good1
             chi_sq = chi1_sq
 
-    mask = np.zeros_like(x, dtype=bool)
+    mask = np.zeros_like(y, dtype=bool)
     mask[good] = True
 
-    return abc, mask
+    return coef, mask
 
 #------------------------------------------------------------------------------
 
-class lts_planefit:
+class ltsfit:
     """
-    lts_planefit
-    ============
+    ltsfit
+    ======
 
     Purpose
     -------
 
-    Best plane *robust* fit to data with errors in all
-    three coordinates and fitting for the intrinsic scatter.
-    See `Cappellari et al. (2013a, Sec.3.2)
-    <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-
-    Explanation
-    -----------
-
-    Linear Least-squares approximation in two-dimension (z = a + b*x + c*y),
-    when x, y and z data have errors, and allowing for intrinsic
-    scatter in the relation.
-
-    Outliers are iteratively clipped using the extremely robust
-    FAST-LTS technique by
-    `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-    See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
+    Fit a linear function of the form::
+
+        y = a + b1*x1 + b2*x2 +...+ bm*xm,
 
+    to data with errors in all coordinates and intrinsic scatter, using a robust
+    method that clips outliers. The function can handle lines in 2-dim, planes in
+    3-dim, or hyperplanes in N-dim, where ``x1, x2,..., xm`` are the independent
+    variables and ``y`` is the dependent variable. The method was introduced in
+    Sec. 3.2 of `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+    and the treatment of outliers is is based on the FAST-LTS technique by
+    `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+    See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_.
+    
     Calling Sequence
     ----------------
 
     .. code-block:: python
 
-        p = lts_planefit(x, y, z, sigx, sigy, sigz, clip=2.6, epsz=True,
-                        frac=None, pivotx=None, pivoty=None, plot=True, text=True)
+        from ltsfit.ltsfit import ltsfit
+
+        p = ltsfit(x, y, sigx, sigy, clip=2.6, corr=True, epsy=True,
+                   frac=None, label='Fitted', label_clip='Clipped',
+                   legend=True, pivot=None, plot=True, text=True)
+
+        print(f"Best fitting parameters: {p.coeff}")
 
-    The output values are stored as attributes of "p".
-    See usage example at the bottom of this file.
+    The output values are stored as attributes of the ``p`` object.
 
     Input Parameters
     ----------------
 
-    x, y, z:
-        vectors of size N with the measured values.
-    sigx, sigy, sigz:
-        vectors of size N with the 1sigma errors in x , y and z.
-    clip:
-        values deviating more than clip*sigma from the best fit are
-        considered outliers and are excluded from the plane fit.
-    epsz:
-        if True, the intrinsic scatter is printed on the plot.
-    frac:
-        fractions of values to include in the LTS stage.
-        Up to a fraction "frac" of the values can be outliers.
-        One must have 0.5 <= frac <= 1  (default frac=0.5).
-
-        NOTE: Set frac=1, to turn off outliers detection.
-    pivotx, pivoty:
-        if these are not None, then lts_planefit fits the plane::
-
-            z = a + b*(x - pivotx) + c*(y - pivoty)
-
-        pivotx, pivoty are called x_0, y_0 in eq.(7) of Cappellari et al. (2013)
-        Use of these keywords is *strongly* recommended, and suggested
-        values are ``pivotx=np.median(x), pivoty=np.median(y)``.
-        This keyword is important to reduce the covariance between a, b and c.
-    plot:
-        if True a plot of the fit is produced.
-    text:
-        if True, the best fitting parameters are printed on the plot.
+    x: array_like with shape (n, m)
+        Array of ``n`` independent variables for ``m`` dimensions.
+
+        EXAMPLE: To fit a line in 2-dim, one has a single vector ``x`` of
+        length ``n`` with the independent variable and a corresponding vector of
+        dependent variable ``y``.
+
+        EXAMPLE: To fit a plane in 3-dim, one has two vectors of length ``n`` of
+        independent variables ``(x1, x2)``. In this case,
+        ``x = np.column_stack([x1, x2])``.
+
+        EXAMPLE: To fit a hyperplane in 4-dim, one has three vectors of
+        independent variables ``(x1, x2, x3)``. In this case,
+        ``x = np.column_stack([x1, x2, x3])``.
+    y: array_like with shape (n,)
+        Vector of measured values for each set of ``x`` variables.
+    sigx: array_like with shape (n, m)
+        Array of ``1sigma`` uncertainties for each ``x`` coordinate for ``m``
+        dimensions. This has the same shape as ``x``.
+    sigy: array_like with shape (n,)
+        Vector of ``1sigma`` uncertainties for each ``y`` value.
+
+    Optional Keywords
+    -----------------
+
+    clip: float
+        Clipping threshold in ``sigma`` units. Values deviating more than
+        ``clip*sigma`` from the best fit are considered outliers and are
+        excluded from the fit. Default is ``clip=2.6``, which would include
+        99% of the values for a Gaussian distribution.
+    corr: bool
+        if ``True``, the correlation coefficients are printed on the plot.
+        Default is ``True``.
+    epsy: bool
+        If ``True``, the intrinsic scatter is printed on the output plot.
+        Default is ``True``.
+    frac: float
+        Fraction of values to include in the LTS stage.
+        Up to a fraction ``frac`` of the values can be outliers.
+        One must have ``0.5 <= frac <= 1``. Default is ``0.5``.
+
+        NOTE: Set ``frac=1`` to turn off outlier detection.
+    pivot: array_like with shape (m,)
+        If nonzero, then ``ltsfit`` fits the following line, plane or hyperplane::
+
+            y = a + b0*(x0 - pivot[0]) + b1*(x1 - pivot[1]) + ...
+
+        ``pivot`` are called ``x_0``, ``y_0`` in eq.(7) of `Cappellari et al. (2013a)`_.
+        Use of this keyword is strongly recommended, and suggested values are
+        ``pivot = np.median(x, 0)``. This keyword has no effect on the best fit
+        but is important to reduce the covariance and uncertainty in the
+        intercept ``a``.  However, the covariance is weakly dependent on the
+        precise value of the ``pivot``. For this reason, it is generally better
+        to round the ``pivot`` values to nice numbers. Default is ``0``.
+    plot: bool
+        If ``True``, a plot of the fit is produced. Default is ``True``.
+    text: bool
+        If ``True``, the best fitting parameters are printed on the plot.
+        Default is ``True``.
 
     Output Parameters
     -----------------
 
-    The output values are stored as attributed of the lts_linefit class.
+    The output values are stored as attributes of the ``ltsfit`` class.
 
-    p.abc:
-        best fitting parameters [a, b, c]
-    p.abc_err:
-        1*sigma formal errors [a_err, b_err, c_err] on a, b and c.
-    p.mask:
-        boolean vector with the same size of x, y and z.
-        It contains True for the elements of (x, y, z) which were included in
-        the fit and False for the outliers which were automatically clipped.
-    p.rms:
-        rms = np.std(fit - z) beteween the data and the fitted relation.
-    p.sig_int:
-        intrinsic scatter in the z direction around the plane.
-        sig_int is called epsilon_z in eq.(7) of Cappellari et al. (2013).
-    p.sig_int_err:
-        1*sigma formal error on sig_int.
+    p.coef: array_like with shape (m+1,)
+        Best fitting parameters ``[a, b1, b2,..., bm]``.
+    p.coef_err: array_like with shape (m+1,)
+        ``1*sigma`` formal uncertainties ``[a_err, b1_err, b2_err,..., bm_err]``.
+    p.mask: array_like with shape (n,) and dtype bool
+        Boolean vector indicating which elements of ``z`` were included in
+        the fit (``True``) and which were clipped as outliers (``False``).
+    p.rms: float
+        RMS deviation between the data and the fitted relation.
+    p.sig_int: float
+        Intrinsic scatter in the ``y`` direction around the line/plane/hyperplane.
+        ``sig_int`` is called ``epsilon_y`` in eq.(6) of `Cappellari et al. (2013a)`_.
+    p.sig_int_err: float
+        ``1*sigma`` formal error on ``sig_int``.
+    p.xx: array_like with shape (n,)
+        Values plotted along the x-axis. This is the linear combination of the
+        ``x`` variables that represents the plane/hyperplane edge-on::
+
+            xx = a + b1*(x1 - pivot[0]) + b2*(x2 - pivot[1]) + ...
+
+        For line fitting, these are just the ``x`` values.
+    p.yy: array_like with shape (n,)
+        The input ``y`` values plotted along the y-axis.
+    p.xerr: array_like with shape (n,)
+        ``1*sigma`` uncertainties for ``p.xx`` in the x-axis of the plot.
+    p.yerr: array_like with shape (n,)
+        ``1*sigma`` uncertainties for ``p.yy`` in the y-axis of the plot.
+    p.xline: array_like with shape (2,)
+        ``x`` coordinates of the best fitting relation as shown on the plot.
+    p.yline: array_like with shape (2,)
+        ``y`` coordinates of the best fitting relation as shown on the plot.
+    p.spearmanr: array_like with shape (2,)
+        Spearman ``r`` coefficient and probability ``p`` between ``(p.xx, p.yy)``
+        without clipping outliers.
+    p.pearsonr: array_like with shape (2,)
+        Pearson ``r`` coefficient and probability ``p`` between ``(p.xx, p.yy)``
+        without clipping outliers.
 
     ###########################################################################
 
     """
+    def __init__(self, x0, y, sigx, sigy, clip=2.6, corr=True, epsy=True,
+                 frac=None, label='Fitted', label_clip='Clipped', legend=True,
+                 pivot=None, plot=True, text=True):
+
+        if x0.ndim == 1:
+            x0, sigx = x0[:, None], sigx[:, None]
+
+        n, ndim = x0.shape
+        assert x0.shape == sigx.shape, 'x and sigx must have the same shape'
+        assert n == y.size == sigy.size, 'y, sigy must have length x.shape[0]'
+        assert np.all(np.isfinite(np.column_stack([x0, y, sigx, sigy]))), \
+            'Input contains non finite values'
+
+        if pivot is None:
+            print('WARNING: Using a nonzero `pivot` keyword is always reccomended')
+            pivot = np.zeros(ndim)
+        else:
+            pivot = np.atleast_1d(pivot)
+
+        t = clock()
+
+        p = ndim + 1  # space dimension
+        n = y.size
+        h = int((n + p + 1)/2) if frac is None else int(max(round(frac*n), (n + p + 1)/2))
+
+        x = np.column_stack([np.ones_like(y), x0 - pivot])
+        self._single_fit(x, y, sigx, sigy, h, clip)
+        self.rms = np.std(x[self.mask] @ self.coef - y[self.mask], ddof=p)
+
+        par = np.append(self.coef, self.sig_int)
+        sig_par = np.append(self.coef_err, self.sig_int_err)
+        str_tex, str_txt = _display_errors(par, sig_par, epsy)
+        ylabel0 = 'a + ' + ' + '.join([f'(x_{j} - p_{j}) b_{j}' for j in range(ndim)])
+
+        if p == 2:
+            xx = x0.ravel()
+            xerr = sigx.ravel()
+            xlabel = '$x_0$'
+            ylabel = '$y,\quad y_{\\rm fit} = a + (x_0 - p_{0}) b_0$'
+        else:
+            xx = x @ par[:-1]
+            xerr = np.sqrt(sigx**2 @ par[1:-1]**2)
+            xlabel = '$' + ylabel0 + '$'
+            ylabel = 'y'
+
+        self.spearmanr = stats.spearmanr(xx, y)
+        self.pearsonr = stats.pearsonr(xx, y)
+        self.xx = xx
+        self.yy = y
+        self.xerr = xerr
+        self.yerr = sigy
+
+        print('\n################# Values and formal errors ################')
+        print(str_txt)
+        print(f'Observed rms scatter: {self.rms:#.2g}')
+        print('y = ' + ylabel0)
+        for j, piv in enumerate(pivot):
+            print(f'   p_{j} = {pivot[j]:#.4g}')
+        print(f"Adopted clip = {clip:#.2f}*sigma")
+        print('Non-clipped Spearman r = %#.2g and p = %#.2g' % self.spearmanr)
+        print('Non-clipped Pearson r = %#.2g and p = %#.2g' % self.pearsonr)
+        print(f'Execution time {clock() - t:.2f} s')
+        print('\n###########################################################\n')
 
-    def _find_outliers(self, sig_int, x, y, z, sigx, sigy, sigz1, h, offs, clip):
+        if plot:
+            plt.errorbar(xx[self.mask], y[self.mask], xerr=xerr[self.mask],
+                         yerr=sigy[self.mask], fmt='ob', capthick=0, capsize=0,
+                         label=label)
+            plt.errorbar(xx[~self.mask], y[~self.mask], xerr=xerr[~self.mask],
+                         yerr=sigy[~self.mask], fmt='d', color='LimeGreen',
+                         capthick=0, capsize=0, label=label_clip)
+            ax = plt.gca()
+            xlim = np.array(ax.get_xlim())
+            ylim = np.array(ax.get_ylim())
+            y1 = par[0] + par[1]*(xlim - pivot) if p == 2 else xlim
+            self.xline = xlim
+            self.yline = y1
+
+            plt.plot(xlim, y1, '-k', linewidth=2, zorder=1, label='Fit')
+            plt.plot(xlim, y1 + self.rms, '--r', lw=2, zorder=1, label="1$\sigma$")
+            plt.plot(xlim, y1 - self.rms, '--r', lw=2, zorder=1)
+            plt.plot(xlim, y1 + clip*self.rms, ':r', lw=2, zorder=1, label=f"{clip:#.1f}$\sigma$")
+            plt.plot(xlim, y1 - clip*self.rms, ':r', lw=2, zorder=1)
+            plt.xlabel(xlabel)
+            plt.ylabel(ylabel)
+            plt.xlim(xlim)
+            plt.ylim(ylim)
+            ax.minorticks_on()
+
+            if legend:
+                plt.legend(loc=4)
+
+            if text:
+                str_tex += f'$\Delta={self.rms:#.2g}$\n'
+                if np.any(pivot):
+                    for j, piv in enumerate(pivot):
+                        str_tex += f'$(p_{j}={piv:#.4g})$\n'
+                ax.text(0.02, 0.98, str_tex, horizontalalignment='left',
+                        verticalalignment='top', transform=ax.transAxes)
+
+            if corr:
+                txt = '${\\rm Spearman/Pearson}$\n'
+                txt += '$r=%#.2g\, p=%#.2g$\n' % self.spearmanr
+                txt += '$r=%#.2g\, p=%#.2g$\n' % self.pearsonr
+                ax.text(0.98, 0.98, txt, horizontalalignment='right',
+                        verticalalignment='top', transform=ax.transAxes)
 
-        sigz = np.sqrt(sigz1**2 + sig_int**2) # Gaussian intrinsic scatter
+# ------------------------------------------------------------------------------
+    def _find_outliers(self, sig_int, x, y, sigx, sigy1, h, offs, clip):
 
-        if h == x.size: # No outliers detection
+        sigy = np.sqrt(sigy1**2 + sig_int**2) # Gaussian intrinsic scatter
 
-            abc = _planefit(x, y, z, sigz=sigz)  # quick initial guess
-            abc, sig_abc, chi_sq = _fitting(x, y, z, sigx, sigy, sigz, abc)
-            mask = np.ones_like(x, dtype=bool)  # No outliers
+        if h == len(x):     # No outliers detection
 
-        else: # Robust fit and outliers detection
+            coef = _hyperfit(x, y, sigy=sigy)  # quick initial guess
+            coef, sig_coef, chi_sq = _fitting(x, y, sigx, sigy, coef)
+            mask = np.ones_like(y, dtype=bool)  # No outliers
 
-            # Initial estimate using the maximum breakdown of
-            # the method of 50% but minimum efficiency
+        else:   # Robust fit and outliers detection
+
+            # Initial estimate using the maximum breakdown
+            # of 50% for the method but the lowest efficiency
             #
-            abc, mask = _fast_algorithm(x, y, z, sigx, sigy, sigz, h)
+            coef, mask = _fast_algorithm(x, y, sigx, sigy, h)
 
             # inside-out outliers removal
             #
             while True:
-                res = _residuals(abc, x, y, z, sigx, sigy, sigz)
-                sig = np.std(res[mask], ddof=3)
+                res = _residuals(coef, x, y, sigx, sigy)
+                sig = np.std(res[mask], ddof=coef.size)
                 maskOld = mask
                 mask = np.abs(res) < clip*sig
-                abc, sig_abc, chi_sq = _fitting(x[mask], y[mask], z[mask], sigx[mask], sigy[mask], sigz[mask], abc)
+                coef, sig_coef, chi_sq = _fitting(x[mask], y[mask], sigx[mask], sigy[mask], coef)
                 if np.array_equal(mask, maskOld):
                     break
 
         # To determine 1sigma error on the intrinsic scatter the chi2
-        # is decreased by 1sigma=sqrt(2(h-3)) while optimizing (a,b,c)
+        # is decreased by 1sigma=sqrt(2(h-ndim)) while optimizing coef
         #
         h = mask.sum()
-        dchi = np.sqrt(2*(h - 3)) if offs else 0.
+        dchi = np.sqrt(2*(h - coef.size)) if offs else 0.
 
-        self.abc = abc
-        self.abc_err = sig_abc
+        self.coef = coef
+        self.coef_err = sig_coef
         self.mask = mask
 
-        err = (chi_sq + dchi)/(h - 3.) - 1
+        err = (chi_sq + dchi)/(h - coef.size) - 1
         print('sig_int: %10.4f  %10.4f' % (sig_int, err))
 
         return err
 
 #------------------------------------------------------------------------------
 
-    def _single_fit(self, x, y, z, sigx, sigy, sigz, h, clip):
+    def _single_fit(self, x, y, sigx, sigy, h, clip):
 
-        if self._find_outliers(0, x, y, z, sigx, sigy, sigz, h, 0, clip) < 0:
+        if self._find_outliers(0, x, y, sigx, sigy, h, 0, clip) < 0:
             print('No intrinsic scatter or errors overestimated')
             sig_int = 0.
             sig_int_err = 0.
         else:
             sig1 = 0.
-            res = self.abc[0] + self.abc[1]*x + self.abc[2]*y - z  # Total residuals ignoring measurement errors
-            std = np.std(res[self.mask], ddof=3)
+            ndim = x.shape[1]
+            res = x @ self.coef - y  # Total residuals ignoring measurement errors
+            std = np.std(res[self.mask], ddof=ndim)
             sig2 = std*(1 + 3/np.sqrt(2*self.mask.sum()))  # Observed scatter + 3sigma error
             print('Computing sig_int')
             sig_int = optimize.brentq(self._find_outliers, sig1, sig2,
-                                      args=(x, y, z, sigx, sigy, sigz, h, 0, clip), rtol=1e-3)
-            print('Computing sig_int error') # chi2 can always decrease
+                                      args=(x, y, sigx, sigy, h, 0, clip), rtol=1e-3)
+            print('Computing sig_int error')    # chi2 can always decrease
             sigMax_int = optimize.brentq(self._find_outliers, sig_int, sig2,
-                                         args=(x, y, z, sigx, sigy, sigz, h, 1, clip), rtol=1e-3)
+                                         args=(x, y, sigx, sigy, h, 1, clip), rtol=1e-3)
             sig_int_err = sigMax_int - sig_int
 
         self.sig_int = sig_int
         self.sig_int_err = sig_int_err
 
         print('Repeat at best fitting solution')
-        self._find_outliers(sig_int, x, y, z, sigx, sigy, sigz, h, 0, clip)
+        self._find_outliers(sig_int, x, y, sigx, sigy, h, 0, clip)
 
 #------------------------------------------------------------------------------
 
-    def __init__(self, x0, y0, z, sigx, sigy, sigz, clip=2.6, epsz=True,
-                  frac=None, pivotx=0, pivoty=0, plot=True, text=True):
-
-        assert x0.size == y0.size == z.size == sigx.size == sigy.size == sigz.size, '[X, Y, Z, SIGX, SIGY, SIGZ] must have the same size'
-
-        if not np.all(np.isfinite(np.hstack([x0, y0, z, sigx, sigy, sigz]))):
-            raise ValueError('Input contains non finite values')
-
-        t = clock()
-
-        x = x0 - pivotx
-        y = y0 - pivoty
-
-        p = 3  # three dimensions
-        n = x.size
-        h = int((n + p + 1)/2) if frac is None else int(max(round(frac*n), (n + p + 1)/2))
-
-        self._single_fit(x, y, z, sigx, sigy, sigz, h, clip)
-        self.rms = np.std(self.abc[0] + self.abc[1]*x[self.mask] + self.abc[2]*y[self.mask] - z[self.mask], ddof=3)
-
-        par = np.append(self.abc, self.sig_int)
-        sig_par = np.append(self.abc_err, self.sig_int_err)
-        print('################# Values and formal errors ################')
-        string = _display_errors(par, sig_par, epsz)
-        print(f'Observed rms scatter: {self.rms:#.2g}')
-        if pivotx or pivoty:
-            print('z = a + b*(x - pivotx) + c*(y - pivoty)')
-            print('with pivotx = %.4g & pivoty = %.4g' % (pivotx, pivoty))
-        else:
-            print('WARNING: pivotx=0 or pivoty=0. Using `pivotx` and `pivoty` keywords is always reccomended')
-
-        print('##########################################################')
-
-        print('seconds %.2f' % (clock() - t))
-
-        if plot:
-
-            z1 = par[0] + x*par[1] + y*par[2]
-            sigz1 = np.sqrt((sigx*par[1])**2 + (sigy*par[2])**2)
-
-            plt.errorbar(z[self.mask], z1[self.mask], xerr=sigz[self.mask], yerr=sigz1[self.mask],
-                         fmt='ob', capthick=0, capsize=0)
-            if not np.all(self.mask):
-                plt.errorbar(z[~self.mask], z1[~self.mask], xerr=sigz[~self.mask], yerr=sigz1[~self.mask],
-                             fmt='d', color='LimeGreen', capthick=0, capsize=0)
-            xlim = plt.gca().get_xlim()
-            plt.title('Best fit, 1$\sigma$ (68%) and 2.6$\sigma$ (99%)')
-
-            plt.plot(xlim, xlim, '-k',
-                     xlim, xlim + self.rms, '--r',
-                     xlim, xlim - self.rms, '--r',
-                     xlim, xlim + 2.6*self.rms, ':r',
-                     xlim, xlim - 2.6*self.rms, ':r', linewidth=2, zorder=1)
-
-            ax = plt.gca()
-            if text:
-                string += f'$\Delta={self.rms:#.2g}$\n'
-                if pivotx:
-                    string += '$(x_0=%.4g)$\n' % pivotx
-                if pivoty:
-                    string += '$(y_0=%.4g)$' % pivoty
-                ax.text(0.05, 0.95, string, horizontalalignment='left',
-                        verticalalignment='top', transform=ax.transAxes)
-
-            ax.minorticks_on()
-            plt.xlim(xlim)
-
-#------------------------------------------------------------------------------
```

### Comparing `ltsfit-5.0.20/ltsfit.egg-info/PKG-INFO` & `ltsfit-6.0.1/ltsfit.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltsfit
-Version: 5.0.20
+Version: 6.0.1
 Summary: LtsFit: Least Trimmed Squares Fitting
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,38 +12,38 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 
 The LtsFit Package
 ==================
 
-**Robust Linear Regression with Scatter in One or Two Dimensions**
+**Robust Least Squares Regression with Uncertainties and Scatter in Any Dimension**
 
 .. image:: https://img.shields.io/pypi/v/ltsfit.svg
     :target: https://pypi.org/project/ltsfit/
 .. image:: https://img.shields.io/badge/arXiv-1208.3522-orange.svg
     :target: https://arxiv.org/abs/1208.3522
 .. image:: https://img.shields.io/badge/DOI-10.1093/mnras/stt562-green.svg
     :target: https://doi.org/10.1093/mnras/stt562
 
-LtsFit is a Python implementation of the method described in Section 3.2 of
+LtsFit is a Python package for **very robust** hyperplane fitting in N dimensions,
+with uncertainties in all coordinates and intrinsic scatter. It implements the
+method described in Section 3.2 of
 `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-to perform **very robust** fits of lines or planes to data with errors in all
-coordinates, while allowing for possible intrinsic scatter.
-Outliers are iteratively clipped using the robust Least Trimmed Squares (LTS)
-technique by `Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+and uses the Least Trimmed Squares (LTS) technique to iteratively clip outliers
+`(Rousseeuw & van Driessen 2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
 
 .. contents:: :depth: 2
 
 Attribution
 -----------
 
-If you use this software for your research, please also cite
-`Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-where the implementation was described. The BibTeX entry for the paper is::
+Please also cite `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+if you use this software for your research. This is the paper where the
+implementation was described. The BibTeX entry for the paper is::
 
     @ARTICLE{Cappellari2013a,
         author = {{Cappellari}, M. and {Scott}, N. and {Alatalo}, K. and
             {Blitz}, L. and {Bois}, M. and {Bournaud}, F. and {Bureau}, M. and
             {Crocker}, A.~F. and {Davies}, R.~L. and {Davis}, T.~A. and {de Zeeuw},
             P.~T. and {Duc}, P.-A. and {Emsellem}, E. and {Khochfar}, S. and
             {Krajnovi{\'c}}, D. and {Kuntschner}, H. and {McDermid}, R.~M. and
@@ -67,241 +67,215 @@
 
     pip install ltsfit
 
 Without writing access to the global ``site-packages`` directory, use::
 
     pip install --user ltsfit
 
+To upgrade the package to the latest version use::
+
+    pip install --upgrade ltsfit
+
 Documentation
 -------------
 
 See ``ltsfit/examples`` and the files docstrings.
 They are copied by ``pip`` within the global folder
 `site-packages <https://stackoverflow.com/a/46071447>`_.
 
 ###########################################################################
 
-lts_linefit
-===========
+ltsfit
+======
 
 Purpose
 -------
 
-Best straight-line *robust* fit to data with errors in
-both coordinates while fitting for the intrinsic scatter.
-See `Cappellari et al. (2013a, Sec.3.2)
-<https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+Fit a linear function of the form::
 
-Explanation
------------
+    y = a + b1*x1 + b2*x2 +...+ bm*xm,
 
-Linear Least-squares approximation in one-dimension (y = a + b*x),
-when both x and y data have errors and allowing for intrinsic
-scatter in the relation.
-
-Outliers are iteratively clipped using the extremely robust
-FAST-LTS technique by
-`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
+to data with errors in all coordinates and intrinsic scatter, using a robust
+method that clips outliers. The function can handle lines in 2-dim, planes in
+3-dim, or hyperplanes in N-dim, where ``x1, x2,..., xm`` are the independent
+variables and ``y`` is the dependent variable. The method was introduced in
+Sec. 3.2 of `Cappellari et al. (2013a) <https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
+and the treatment of outliers is is based on the FAST-LTS technique by
+`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_.
+See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_.
 
 Calling Sequence
 ----------------
 
 .. code-block:: python
 
-    p = lts_linefit(x, y, sigx, sigy, clip=2.6, epsy=True, corr=True,
-                  frac=None, pivot=None, plot=True, text=True)
+    from ltsfit.ltsfit import ltsfit
 
-The output values are stored as attributes of "p".
-See usage example at the bottom of this file.
+    p = ltsfit(x, y, sigx, sigy, clip=2.6, corr=True, epsy=True,
+               frac=None, label='Fitted', label_clip='Clipped',
+               legend=True, pivot=None, plot=True, text=True)
 
-Input Parameters
-----------------
-
-x, y:
-    vectors of size N with the measured values.
-sigx, sigy:
-    vectors of size N with the 1sigma errors in x and y.
-clip:
-    values deviating more than clip*sigma from the best fit are
-    considered outliers and are excluded from the linear fit.
-epsy:
-    if True, the intrinsic scatter is printed on the plot.
-corr:
-    if True, the correlation coefficients are printed on the plot.
-frac:
-    fractions of values to include in the LTS stage.
-    Up to a fraction "frac" of the values can be outliers.
-    One must have 0.5 < frac < 1  (default frac=0.5).
-
-    NOTE: Set frac=1, to turn off outliers detection.
-label:
-    optional string label to create a legend outside the procedure.
-pivot:
-    if this is not None, then lts_linefit fits the relation::
-
-        y = a + b*(x - pivot)
-
-    pivot is called x_0 in eq.(6) of Cappellari et al. (2013)
-    Use of this keyword is *strongly* recommended and a suggested
-    value is pivot ~ np.mean(x). This keyword is important to
-    reduce the covariance between a and b.
-plot:
-    if True a plot of the fit is produced.
-text:
-    if True, the best fitting parameters are printed on the plot.
+    print(f"Best fitting parameters: {p.coeff}")
 
-Output Parameters
------------------
+The output values are stored as attributes of the ``p`` object.
 
-The output values are stored as attributed of the lts_linefit class.
-
-p.ab:
-    best fitting parameters [a, b]
-p.ab_err:
-    1*sigma formal errors [a_err, b_err] on a and b.
-p.mask:
-    boolean vector with the same size of x and y.
-    It contains True  for the elements of (x, y) which were included in
-    the fit and False for the outliers which were automatically clipped.
-p.rms:
-    rms = np.std(fit - y) beteween the data and the fitted relation.
-p.sig_int:
-    intrinsic scatter around the linear relation.
-    sig_int is called epsilon_y in eq.(6) of Cappellari et al. (2013).
-p.sig_int_err:
-    1*sigma formal error on sig_int.
-
-###########################################################################
-
-
-lts_planefit
-============
-
-Purpose
--------
-
-Best plane *robust* fit to data with errors in all
-three coordinates and fitting for the intrinsic scatter.
-See `Cappellari et al. (2013a, Sec.3.2)
-<https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C>`_
-
-Explanation
------------
-
-Linear Least-squares approximation in two-dimension (z = a + b*x + c*y),
-when x, y and z data have errors, and allowing for intrinsic
-scatter in the relation.
-
-Outliers are iteratively clipped using the extremely robust
-FAST-LTS technique by
-`Rousseeuw & van Driessen (2006) <http://doi.org/10.1007/s10618-005-0024-4>`_
-See also `Rousseeuw (1987) <http://books.google.co.uk/books?id=woaH_73s-MwC&pg=PA15>`_
-
-Calling Sequence
+Input Parameters
 ----------------
 
-.. code-block:: python
-
-    p = lts_planefit(x, y, z, sigx, sigy, sigz, clip=2.6, epsz=True,
-                    frac=None, pivotx=None, pivoty=None, plot=True, text=True)
+x: array_like with shape (n, m)
+    Array of ``n`` independent variables for ``m`` dimensions.
 
-The output values are stored as attributes of "p".
-See usage example at the bottom of this file.
+    EXAMPLE: To fit a line in 2-dim, one has a single vector ``x`` of
+    length ``n`` with the independent variable and a corresponding vector of
+    dependent variable ``y``.
+
+    EXAMPLE: To fit a plane in 3-dim, one has two vectors of length ``n`` of
+    independent variables ``(x1, x2)``. In this case,
+    ``x = np.column_stack([x1, x2])``.
+
+    EXAMPLE: To fit a hyperplane in 4-dim, one has three vectors of
+    independent variables ``(x1, x2, x3)``. In this case,
+    ``x = np.column_stack([x1, x2, x3])``.
+y: array_like with shape (n,)
+    Vector of measured values for each set of ``x`` variables.
+sigx: array_like with shape (n, m)
+    Array of ``1sigma`` uncertainties for each ``x`` coordinate for ``m``
+    dimensions. This has the same shape as ``x``.
+sigy: array_like with shape (n,)
+    Vector of ``1sigma`` uncertainties for each ``y`` value.
 
-Input Parameters
-----------------
+Optional Keywords
+-----------------
 
-x, y, z:
-    vectors of size N with the measured values.
-sigx, sigy, sigz:
-    vectors of size N with the 1sigma errors in x , y and z.
-clip:
-    values deviating more than clip*sigma from the best fit are
-    considered outliers and are excluded from the plane fit.
-epsz:
-    if True, the intrinsic scatter is printed on the plot.
-frac:
-    fractions of values to include in the LTS stage.
-    Up to a fraction "frac" of the values can be outliers.
-    One must have 0.5 <= frac <= 1  (default frac=0.5).
-
-    NOTE: Set frac=1, to turn off outliers detection.
-pivotx, pivoty:
-    if these are not None, then lts_planefit fits the plane::
-
-        z = a + b*(x - pivotx) + c*(y - pivoty)
-
-    pivotx, pivoty are called x_0, y_0 in eq.(7) of Cappellari et al. (2013)
-    Use of these keywords is *strongly* recommended, and suggested
-    values are ``pivotx=np.median(x), pivoty=np.median(y)``.
-    This keyword is important to reduce the covariance between a, b and c.
-plot:
-    if True a plot of the fit is produced.
-text:
-    if True, the best fitting parameters are printed on the plot.
+clip: float
+    Clipping threshold in ``sigma`` units. Values deviating more than
+    ``clip*sigma`` from the best fit are considered outliers and are
+    excluded from the fit. Default is ``clip=2.6``, which would include
+    99% of the values for a Gaussian distribution.
+corr: bool
+    if ``True``, the correlation coefficients are printed on the plot.
+    Default is ``True``.
+epsy: bool
+    If ``True``, the intrinsic scatter is printed on the output plot.
+    Default is ``True``.
+frac: float
+    Fraction of values to include in the LTS stage.
+    Up to a fraction ``frac`` of the values can be outliers.
+    One must have ``0.5 <= frac <= 1``. Default is ``0.5``.
+
+    NOTE: Set ``frac=1`` to turn off outlier detection.
+pivot: array_like with shape (m,)
+    If nonzero, then ``ltsfit`` fits the following line, plane or hyperplane::
+
+        y = a + b0*(x0 - pivot[0]) + b1*(x1 - pivot[1]) + ...
+
+    ``pivot`` are called ``x_0``, ``y_0`` in eq.(7) of `Cappellari et al. (2013a)`_.
+    Use of this keyword is strongly recommended, and suggested values are
+    ``pivot = np.median(x, 0)``. This keyword has no effect on the best fit
+    but is important to reduce the covariance and uncertainty in the
+    intercept ``a``.  However, the covariance is weakly dependent on the
+    precise value of the ``pivot``. For this reason, it is generally better
+    to round the ``pivot`` values to nice numbers. Default is ``0``.
+plot: bool
+    If ``True``, a plot of the fit is produced. Default is ``True``.
+text: bool
+    If ``True``, the best fitting parameters are printed on the plot.
+    Default is ``True``.
 
 Output Parameters
 -----------------
 
-The output values are stored as attributed of the lts_linefit class.
+The output values are stored as attributes of the ``ltsfit`` class.
 
-p.abc:
-    best fitting parameters [a, b, c]
-p.abc_err:
-    1*sigma formal errors [a_err, b_err, c_err] on a, b and c.
-p.mask:
-    boolean vector with the same size of x, y and z.
-    It contains True for the elements of (x, y, z) which were included in
-    the fit and False for the outliers which were automatically clipped.
-p.rms:
-    rms = np.std(fit - z) beteween the data and the fitted relation.
-p.sig_int:
-    intrinsic scatter in the z direction around the plane.
-    sig_int is called epsilon_z in eq.(7) of Cappellari et al. (2013).
-p.sig_int_err:
-    1*sigma formal error on sig_int.
+p.coef: array_like with shape (m+1,)
+    Best fitting parameters ``[a, b1, b2,..., bm]``.
+p.coef_err: array_like with shape (m+1,)
+    ``1*sigma`` formal uncertainties ``[a_err, b1_err, b2_err,..., bm_err]``.
+p.mask: array_like with shape (n,) and dtype bool
+    Boolean vector indicating which elements of ``z`` were included in
+    the fit (``True``) and which were clipped as outliers (``False``).
+p.rms: float
+    RMS deviation between the data and the fitted relation.
+p.sig_int: float
+    Intrinsic scatter in the ``y`` direction around the line/plane/hyperplane.
+    ``sig_int`` is called ``epsilon_y`` in eq.(6) of `Cappellari et al. (2013a)`_.
+p.sig_int_err: float
+    ``1*sigma`` formal error on ``sig_int``.
+p.xx: array_like with shape (n,)
+    Values plotted along the x-axis. This is the linear combination of the
+    ``x`` variables that represents the plane/hyperplane edge-on::
+
+        xx = a + b1*(x1 - pivot[0]) + b2*(x2 - pivot[1]) + ...
+
+    For line fitting, these are just the ``x`` values.
+p.yy: array_like with shape (n,)
+    The input ``y`` values plotted along the y-axis.
+p.xerr: array_like with shape (n,)
+    ``1*sigma`` uncertainties for ``p.xx`` in the x-axis of the plot.
+p.yerr: array_like with shape (n,)
+    ``1*sigma`` uncertainties for ``p.yy`` in the y-axis of the plot.
+p.xline: array_like with shape (2,)
+    ``x`` coordinates of the best fitting relation as shown on the plot.
+p.yline: array_like with shape (2,)
+    ``y`` coordinates of the best fitting relation as shown on the plot.
+p.spearmanr: array_like with shape (2,)
+    Spearman ``r`` coefficient and probability ``p`` between ``(p.xx, p.yy)``
+    without clipping outliers.
+p.pearsonr: array_like with shape (2,)
+    Pearson ``r`` coefficient and probability ``p`` between ``(p.xx, p.yy)``
+    without clipping outliers.
 
 ###########################################################################
 
 
 
 License
 =======
 
 Other/Proprietary License
 
-Copyright (c) 2012-2022 Michele Cappellari
+Copyright (c) 2012-2023 Michele Cappellari
 
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
 
-V2.0.20: MC, Oxford, 3 October 2022
+V6.0.1: MC, Oxford, 20 July 2023
+  - New function ``ltsfit`` to fit hyperplanes in N-dim. This procedure
+    generalizes and replaces both ``lts_linefit`` and ``lts_planefit``, which
+    are now deprecated wrappers for ``ltsfit``. This change was suggested and
+    motivated by Francesco D'Eugenio (cam.ac.uk), who shared his own 4-dim
+    ``lts_hyperfit`` and his paper on a useful application.
+  - ``ltsfit``: When fitting planes/hyperplanes, plot the independent variable
+    on the y-axis to be consistent with line fitting. Also plot a legend.
+  - Updated all ``ltsfit_examples``.
+  - Fixed inconsistency between the version number on PyPi and in the Changelog.
+
+V5.0.20: MC, Oxford, 3 October 2022
   - Fixed program stop due to Matplotlib change.
     Thanks to Hitesh Lala (Heidelberg) for the report.
   - Extract documentation from docstrings and show it on PyPi.
 
-V2.0.19: MC, Oxford, 22 January 2021
+V5.0.19: MC, Oxford, 22 January 2021
   - Fixed incorrect plot ranges due to a Matplotlib change.
     Thanks to Davide Bevacqua (unibo.it) for the report.
 
-V2.0.18: MC, Oxford, 17 February 2020
+V5.0.18: MC, Oxford, 17 February 2020
   - Properly print significant trailing zeros in results.
 
-V2.0.17: MC, Oxford, 22 January 2020
+V5.0.17: MC, Oxford, 22 January 2020
   - Formatted documentation as docstring.
   - Included p.rms output.
-
+  - Published on PyPi. Increased major version number by mistake.
 
 V2.0.16: MC, Oxford, 27 September 2018
   - Fixed clock DeprecationWarning in Python 3.7.
 
 V2.0.15: MC, Oxford, 12 May 2018
   - Dropped Python 2.7 support.
```

### Comparing `ltsfit-5.0.20/setup.py` & `ltsfit-6.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     docstring = re.search(rex, main_file).group(1)
     return docstring.replace("\n    ", "\n")
 
 setup(name=package,
       version=find_version(package),
       description='LtsFit: Least Trimmed Squares Fitting',
       long_description=open(package + "/README.rst").read()
-                       + read_docstring(package, "lts_linefit")
-                       + read_docstring(package, "lts_planefit")
+                       + read_docstring(package, "ltsfit")
                        + "\n\nLicense\n=======\n\n"
                        + open(package + "/LICENSE.txt").read()
                        + open(package + "/CHANGELOG.rst").read(),
       long_description_content_type='text/x-rst',
       url="https://purl.org/cappellari/software",
       author="Michele Cappellari",
       author_email="michele.cappellari@physics.ox.ac.uk",
```

