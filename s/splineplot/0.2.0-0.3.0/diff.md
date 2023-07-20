# Comparing `tmp/splineplot-0.2.0.tar.gz` & `tmp/splineplot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splineplot-0.2.0.tar", max compression
+gzip compressed data, was "splineplot-0.3.0.tar", max compression
```

## Comparing `splineplot-0.2.0.tar` & `splineplot-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-07-20 11:43:07.546254 splineplot-0.2.0/LICENSE
--rw-r--r--   0        0        0      256 2023-07-20 12:06:34.656029 splineplot-0.2.0/README.md
--rw-r--r--   0        0        0      437 2023-07-20 12:28:09.374689 splineplot-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1224 2023-07-20 12:05:06.408220 splineplot-0.2.0/splineplot/__init__.py
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 splineplot-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-20 11:43:07.546254 splineplot-0.3.0/LICENSE
+-rw-r--r--   0        0        0      256 2023-07-20 12:06:34.656029 splineplot-0.3.0/README.md
+-rw-r--r--   0        0        0      437 2023-07-20 12:34:48.768693 splineplot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1526 2023-07-20 12:34:33.125706 splineplot-0.3.0/splineplot/__init__.py
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 splineplot-0.3.0/PKG-INFO
```

### Comparing `splineplot-0.2.0/LICENSE` & `splineplot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splineplot-0.2.0/splineplot/__init__.py` & `splineplot-0.3.0/splineplot/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 def splineplot(
     x,
     y,
     df: int = 5,
     degree: int = 3,
     alpha: int = 0,
     scatter: bool = True,
+    scatter_kws: dict[str, Any] = {},
+    line_kws: dict[str, Any] = {},
     **kwargs: Any,
 ) -> None:
     """Fit a spline and plot it with some data
 
     Parameters
     ----------
     x : numpy.typing.ArrayLike
@@ -29,14 +31,18 @@
         Y data
     df : int = 5
         Degrees of freedom of the fitted spline
     degree : int = 3
         Degree of the fitted spline polynomial
     alpha : int = 0
         Penalization term to prevent overfitting
+    scatter_kws : dict[str, Any] = {}
+        Additional keyword arguments to pass to `plt.scatter`
+    line_kws : dict[str, Any] = {}
+        Additional keyword arguments to pass to `plt.line`
     scatter : bool = True
         Plot the scatter data
     """
     ax = plt.gca()
 
     spline = BSplines(x, df=df, degree=degree, include_intercept=True)
     gam = GLMGam(
@@ -45,17 +51,18 @@
         alpha=alpha,
     )
     res = gam.fit()
 
     x_basis = np.linspace(x.min(), x.max(), 1000)
 
     if scatter:
-        ax.scatter(x, y, **kwargs)
+        ax.scatter(x, y, **kwargs, **scatter_kws)
 
     label = kwargs.pop("label", "")
 
     ax.plot(
         x_basis,
         spline.transform(x_basis) @ res.params,
         label=f"{label} Spline".strip(),
+        **line_kws,
         **kwargs,
     )
```

### Comparing `splineplot-0.2.0/PKG-INFO` & `splineplot-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splineplot
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: Apache 2.0
 Author: Matthew Badger
 Author-email: matt@branchenergy.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

