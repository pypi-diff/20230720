# Comparing `tmp/tobler-0.8.2.tar.gz` & `tmp/tobler-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tobler-0.8.2.tar", last modified: Wed Jun 30 18:24:44 2021, max compression
+gzip compressed data, was "tobler-0.9.0.tar", last modified: Tue Feb 22 16:20:23 2022, max compression
```

## Comparing `tobler-0.8.2.tar` & `tobler-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 18:24:44.950864 tobler-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-06-30 18:24:17.000000 tobler-0.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-06-30 18:24:17.000000 tobler-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7274 2021-06-30 18:24:44.950864 tobler-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5789 2021-06-30 18:24:17.000000 tobler-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-06-30 18:24:18.000000 tobler-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-06-30 18:24:18.000000 tobler-0.8.2/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-06-30 18:24:18.000000 tobler-0.8.2/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-30 18:24:44.950864 tobler-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2021-06-30 18:24:18.000000 tobler-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 18:24:44.946864 tobler-0.8.2/tobler/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 18:24:44.950864 tobler-0.8.2/tobler/area_weighted/
--rw-r--r--   0 runner    (1001) docker     (121)      322 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/area_weighted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23775 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/area_weighted/_vectorized_raster_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)    22011 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/area_weighted/area_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/area_weighted/area_join.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 18:24:44.950864 tobler-0.8.2/tobler/dasymetric/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/dasymetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/dasymetric/masked_area_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/dasymetric/raster_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 18:24:44.950864 tobler-0.8.2/tobler/model/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7073 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/model/glm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 18:24:44.950864 tobler-0.8.2/tobler/pycno/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/pycno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10772 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/pycno/pycno.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 18:24:44.950864 tobler-0.8.2/tobler/util/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6994 2021-06-30 18:24:18.000000 tobler-0.8.2/tobler/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-30 18:24:44.946864 tobler-0.8.2/tobler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7274 2021-06-30 18:24:44.000000 tobler-0.8.2/tobler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-06-30 18:24:44.000000 tobler-0.8.2/tobler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-30 18:24:44.000000 tobler-0.8.2/tobler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-30 18:24:44.000000 tobler-0.8.2/tobler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-06-30 18:24:44.000000 tobler-0.8.2/tobler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-30 18:24:44.000000 tobler-0.8.2/tobler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 16:20:23.637615 tobler-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-02-22 16:19:58.000000 tobler-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-02-22 16:19:58.000000 tobler-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-02-22 16:20:23.641615 tobler-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5789 2022-02-22 16:19:58.000000 tobler-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-02-22 16:19:58.000000 tobler-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-22 16:19:58.000000 tobler-0.9.0/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-02-22 16:19:58.000000 tobler-0.9.0/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-02-22 16:20:23.641615 tobler-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-02-22 16:19:58.000000 tobler-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 16:20:23.641615 tobler-0.9.0/tobler/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-02-22 16:20:23.641615 tobler-0.9.0/tobler/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 16:20:23.637615 tobler-0.9.0/tobler/area_weighted/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/area_weighted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12400 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/area_weighted/area_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/area_weighted/area_join.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 16:20:23.637615 tobler-0.9.0/tobler/dasymetric/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/dasymetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3368 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/dasymetric/masked_area_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5300 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/dasymetric/raster_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 16:20:23.637615 tobler-0.9.0/tobler/model/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3742 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/model/glm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 16:20:23.637615 tobler-0.9.0/tobler/pycno/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/pycno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10807 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/pycno/pycno.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 16:20:23.637615 tobler-0.9.0/tobler/util/
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5005 2022-02-22 16:19:58.000000 tobler-0.9.0/tobler/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 16:20:23.637615 tobler-0.9.0/tobler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6713 2022-02-22 16:20:23.000000 tobler-0.9.0/tobler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2022-02-22 16:20:23.000000 tobler-0.9.0/tobler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 16:20:23.000000 tobler-0.9.0/tobler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 16:20:23.000000 tobler-0.9.0/tobler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-02-22 16:20:23.000000 tobler-0.9.0/tobler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-22 16:20:23.000000 tobler-0.9.0/tobler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    78254 2022-02-22 16:19:58.000000 tobler-0.9.0/versioneer.py
```

### Comparing `tobler-0.8.2/LICENSE.txt` & `tobler-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tobler-0.8.2/PKG-INFO` & `tobler-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,15 @@
 Metadata-Version: 2.1
 Name: tobler
-Version: 0.8.2
+Version: 0.9.0
 Summary: TOBLER: Areal Interpolation
 Home-page: https://github.com/pysal/tobler
 Maintainer: Serge Rey
 Maintainer-email: sjsrey@gmail.com
 License: 3-Clause BSD
-Description: <p align="center">
-        <img src="docs/figs/tobler_long.png" height="200px">
-        </p>
-        
-        ![CI Tests](https://github.com/pysal/tobler/workflows/Unit%20Tests/badge.svg)
-        [![codecov](https://codecov.io/gh/pysal/tobler/branch/master/graph/badge.svg?token=XO4SilfBEb)](https://codecov.io/gh/pysal/tobler)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tobler)
-        ![PyPI](https://img.shields.io/pypi/v/tobler)
-        ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/tobler)
-        ![GitHub commits since latest release (branch)](https://img.shields.io/github/commits-since/pysal/tobler/latest)
-        [![DOI](https://zenodo.org/badge/202220824.svg)](https://zenodo.org/badge/latestdoi/202220824)
-        
-        # PySAL `tobler`
-        
-        `tobler` is a python package for areal interpolation, dasymetric mapping, change of support, and small area estimation. It provides a suite of tools with a simple interface for transferring data from one polygonal representation to another. Common examples include standardizing census data from different time periods to a single representation (i.e. to overcome boundary changes in successive years), or the conversion of data collected at different spatial scales into shared units of analysis (e.g. converting zip code and neighborhood data into a regular grid). `tobler` is part of the [PySAL](https://pysal.org) family of packages for spatial data science and provides highly performant implementations of basic and advanced interpolation methods, leveraging [`pygeos`](https://pygeos.readthedocs.io/en/latest/) to optimize for multicore architecture. The package name is an homage to the legendary quantitative geographer [Waldo Tobler](https://en.wikipedia.org/wiki/Waldo_R._Tobler), a pioneer in geographic interpolation methods, spatial analysis, and computational social science.
-        
-        ![DC tracts to hexgrid](docs/_static/images/notebooks_census_to_hexgrid_25_1.png)
-        
-        ## Interpolation Methods
-        
-        `tobler` provides functionality for three families of spatial interpolation methods. The utility of each technique depends on the context of the problem and varies according to e.g. data availability, the properties of the interpolated variable, and the resolution of source and target geometries. For a further explanation of different interpolation techniques, please explore some of the field's [background literature](https://pysal.org/tobler/references.html)
-        
-        ### Area Weighted
-        
-        Areal interpolation uses the area of overlapping geometries to apportion variables. This is the simplest method with no additional data requirements, aside from input and output geometries, however this method is also most susceptible to the [modifiable areal unit problem](https://en.wikipedia.org/wiki/Modifiable_areal_unit_problem).
-        
-        ### Dasymetric
-        
-        Dasymetric interpolation uses auxiliary data to improve estimation, for example
-        by constraining the areal interpolation to areas that are known to be inhabited. Formally, `tobler` adopts a binary dasymetric approach, using auxiliary data to define which land is available or unavailable for interpolation. The package can incorporate additional sources such as
-        
-        * raster data such as satellite imagery that define land types
-        * vector features such as roads or water bodies that define habitable or inhabitable land
-        
-        either (or both) of which may be used to help ensure that variables from the source geometries are not allocated to inappropriate areas of the target geometries. Naturally, dasymetric approaches are sensitive to the quality of ancillary data and underlying assumptions used to guide the estimation.
-        
-        ### Model-based
-        
-        Model-based interpolation uses [spatial] statistical models to estimate a relationship between the target variable and a set of covariates such as physical features, administrative designations, or demographic and architectural characteristics. Model-based approaches offer the ability to incorporate the richest set of additional data, but they can also difficult to wield in practice because the true relationship between variables is never known. By definition, some formal assumptions of regression models are violated because the target variable is always predicted using data from a different spatial scale than it was estimated.
-        
-        ### Extensions
-        
-        `tobler` is under active development and will continue to incorporate emerging interpolation methods as they are introduced to the field. We welcome any and all contributions and if you would like to propose an additional method for adoption please raise an issue for discussion or open a new pull request!
-        
-        ![Charleston zipcodes to tracts](docs/_static/images/tobler3.png)
-        
-        ![raster example](docs/figs/raster_lattice_example.png)
-        
-        ## Installation
-        
-        ```bash
-        $ conda env create -f environment.yml
-        $ conda activate tobler 
-        $ python setup.py develop
-        ```
-        
-        ## Contribute
-        
-        PySAL-tobler is under active development and contributors are welcome.
-        
-        If you have any suggestion, feature request, or bug report, please open a new [issue](https://github.com/pysal/tobler/issues) on GitHub. To submit patches, please follow the PySAL development [guidelines](http://pysal.readthedocs.io/en/latest/developers/index.html) and open a [pull request](https://github.com/pysal/tobler). Once your changes get merged, you’ll automatically be added to the [Contributors List](https://github.com/pysal/tobler/graphs/contributors).
-        
-        ## License
-        
-        The project is licensed under the [BSD license](https://github.com/pysal/tobler/blob/master/LICENSE.txt).
-        
-        ## Funding
-        
-        <img src="docs/figs/nsf_logo.jpg" width="50"> 
-        
-        Award #1733705 [Neighborhoods in Space-Time Contexts](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1733705&HistoricalAwards=false)
-        
-         Award #1831615 [Scalable Geospatial Analytics for Social Science Research](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1831615)
-        
 Keywords: spatial statistics,interpolation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
@@ -92,7 +19,83 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
+License-File: LICENSE.txt
+
+<p align="center">
+<img src="docs/figs/tobler_long.png" height="200px">
+</p>
+
+![CI Tests](https://github.com/pysal/tobler/workflows/Unit%20Tests/badge.svg)
+[![codecov](https://codecov.io/gh/pysal/tobler/branch/master/graph/badge.svg?token=XO4SilfBEb)](https://codecov.io/gh/pysal/tobler)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tobler)
+![PyPI](https://img.shields.io/pypi/v/tobler)
+![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/tobler)
+![GitHub commits since latest release (branch)](https://img.shields.io/github/commits-since/pysal/tobler/latest)
+[![DOI](https://zenodo.org/badge/202220824.svg)](https://zenodo.org/badge/latestdoi/202220824)
+
+# PySAL `tobler`
+
+`tobler` is a python package for areal interpolation, dasymetric mapping, change of support, and small area estimation. It provides a suite of tools with a simple interface for transferring data from one polygonal representation to another. Common examples include standardizing census data from different time periods to a single representation (i.e. to overcome boundary changes in successive years), or the conversion of data collected at different spatial scales into shared units of analysis (e.g. converting zip code and neighborhood data into a regular grid). `tobler` is part of the [PySAL](https://pysal.org) family of packages for spatial data science and provides highly performant implementations of basic and advanced interpolation methods, leveraging [`pygeos`](https://pygeos.readthedocs.io/en/latest/) to optimize for multicore architecture. The package name is an homage to the legendary quantitative geographer [Waldo Tobler](https://en.wikipedia.org/wiki/Waldo_R._Tobler), a pioneer in geographic interpolation methods, spatial analysis, and computational social science.
+
+![DC tracts to hexgrid](docs/_static/images/notebooks_census_to_hexgrid_25_1.png)
+
+## Interpolation Methods
+
+`tobler` provides functionality for three families of spatial interpolation methods. The utility of each technique depends on the context of the problem and varies according to e.g. data availability, the properties of the interpolated variable, and the resolution of source and target geometries. For a further explanation of different interpolation techniques, please explore some of the field's [background literature](https://pysal.org/tobler/references.html)
+
+### Area Weighted
+
+Areal interpolation uses the area of overlapping geometries to apportion variables. This is the simplest method with no additional data requirements, aside from input and output geometries, however this method is also most susceptible to the [modifiable areal unit problem](https://en.wikipedia.org/wiki/Modifiable_areal_unit_problem).
+
+### Dasymetric
+
+Dasymetric interpolation uses auxiliary data to improve estimation, for example
+by constraining the areal interpolation to areas that are known to be inhabited. Formally, `tobler` adopts a binary dasymetric approach, using auxiliary data to define which land is available or unavailable for interpolation. The package can incorporate additional sources such as
+
+* raster data such as satellite imagery that define land types
+* vector features such as roads or water bodies that define habitable or inhabitable land
+
+either (or both) of which may be used to help ensure that variables from the source geometries are not allocated to inappropriate areas of the target geometries. Naturally, dasymetric approaches are sensitive to the quality of ancillary data and underlying assumptions used to guide the estimation.
+
+### Model-based
+
+Model-based interpolation uses [spatial] statistical models to estimate a relationship between the target variable and a set of covariates such as physical features, administrative designations, or demographic and architectural characteristics. Model-based approaches offer the ability to incorporate the richest set of additional data, but they can also difficult to wield in practice because the true relationship between variables is never known. By definition, some formal assumptions of regression models are violated because the target variable is always predicted using data from a different spatial scale than it was estimated.
+
+### Extensions
+
+`tobler` is under active development and will continue to incorporate emerging interpolation methods as they are introduced to the field. We welcome any and all contributions and if you would like to propose an additional method for adoption please raise an issue for discussion or open a new pull request!
+
+![Charleston zipcodes to tracts](docs/_static/images/tobler3.png)
+
+![raster example](docs/figs/raster_lattice_example.png)
+
+## Installation
+
+```bash
+$ conda env create -f environment.yml
+$ conda activate tobler 
+$ python setup.py develop
+```
+
+## Contribute
+
+PySAL-tobler is under active development and contributors are welcome.
+
+If you have any suggestion, feature request, or bug report, please open a new [issue](https://github.com/pysal/tobler/issues) on GitHub. To submit patches, please follow the PySAL development [guidelines](http://pysal.readthedocs.io/en/latest/developers/index.html) and open a [pull request](https://github.com/pysal/tobler). Once your changes get merged, you’ll automatically be added to the [Contributors List](https://github.com/pysal/tobler/graphs/contributors).
+
+## License
+
+The project is licensed under the [BSD license](https://github.com/pysal/tobler/blob/master/LICENSE.txt).
+
+## Funding
+
+<img src="docs/figs/nsf_logo.jpg" width="50"> 
+
+Award #1733705 [Neighborhoods in Space-Time Contexts](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1733705&HistoricalAwards=false)
+
+ Award #1831615 [Scalable Geospatial Analytics for Social Science Research](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1831615)
+
+
```

### Comparing `tobler-0.8.2/README.md` & `tobler-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tobler-0.8.2/setup.py` & `tobler-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """TOBLER: Areal Interpolation
 
 Tobler is a Python library for areal interpolation.
 """
+import os
+import versioneer
+from setuptools import setup, find_packages
+from distutils.command.build_py import build_py
 
 
 DOCLINES = __doc__.split("\n")
 
 with open("README.md", "r", encoding="utf8") as file:
     long_description = file.read()
 
 
-from setuptools import setup, find_packages
-from distutils.command.build_py import build_py
-import os
-
-# Get __version__ from tobler/__init__.py without importing the package
-# __version__ has to be defined in the first line
-with open("tobler/__init__.py", "r") as f:
-    exec(f.readline())
-
 # BEFORE importing distutils, remove MANIFEST. distutils doesn't properly
 # update it when the contents of directories change.
 if os.path.exists("MANIFEST"):
     os.remove("MANIFEST")
 
 
 def _get_requirements_from_files(groups_files):
@@ -45,15 +40,16 @@
 
     reqs = _get_requirements_from_files(_groups_files)
     install_reqs = reqs.pop("base")
     extras_reqs = reqs
 
     setup(
         name="tobler",  # name of package
-        version=__version__,
+        version=versioneer.get_version(),
+        cmdclass=versioneer.get_cmdclass({"build_py": build_py}),
         description=DOCLINES[0],
         # long_description="\n".join(DOCLINES[2:]),
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/pysal/tobler",
         maintainer="Serge Rey",
         maintainer_email="sjsrey@gmail.com",
@@ -74,13 +70,12 @@
             "Programming Language :: Python :: 3.9",
         ],
         license="3-Clause BSD",
         packages=find_packages(),
         install_requires=install_reqs,
         extras_require=extras_reqs,
         zip_safe=False,
-        cmdclass={"build.py": build_py},
     )
 
 
 if __name__ == "__main__":
     setup_package()
```

### Comparing `tobler-0.8.2/tobler/area_weighted/area_join.py` & `tobler-0.9.0/tobler/area_weighted/area_join.py`

 * *Files identical despite different names*

### Comparing `tobler-0.8.2/tobler/dasymetric/masked_area_interpolate.py` & `tobler-0.9.0/tobler/dasymetric/masked_area_interpolate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,91 @@
-from ..area_weighted import _slow_area_interpolate, _area_tables_raster
+import geopandas as gpd
 
-from ..area_weighted._vectorized_raster_interpolation import *
+from ..area_weighted import area_interpolate
+from .raster_tools import extract_raster_features
+from warnings import warn
 
 
 def masked_area_interpolate(
     source_df,
     target_df,
-    raster="nlcd_2011",
-    codes=None,
-    force_crs_match=True,
+    raster,
+    pixel_values,
     extensive_variables=None,
     intensive_variables=None,
+    categorical_variables=None,
     allocate_total=True,
-    tables=None,
+    nodata=255,
+    n_jobs=-1,
+    codes=None,
 ):
     """Interpolate data between two polygonal datasets using an auxiliary raster to mask out uninhabited land.
 
     Parameters
     ----------
     source_df : geopandas.GeoDataFrame
         source data to be converted to another geometric representation.
     target_df : geopandas.GeoDataFrame
         target geometries that will form the new representation of the input data
     raster : str
         path to raster file that contains ancillary data
-    codes : list of ints
-        list of pixel values that should be considered part of the mask (the default is None).
-        If no codes are passed, this defaults to  [21, 22, 23, 24] which are the developed land use
-        codes from the NLCD data
-    force_crs_match : bool
-        whether to force the input and target data to share the same CRS (the default is True).
+    pixel_values : list of ints
+        list of pixel values that should be considered part of the mask. For example if
+        using data from NLCD Land Cover Database <https://www.mrlc.gov/data>, a common
+        input might be [21,22,23,24], which match the "developed" land types in that dataset
     extensive_variables : list
         Columns of the input dataframe containing extensive variables to interpolate
     intensive_variables : list
         Columns of the input dataframe containing intensive variables to interpolate
+    categorical_variables : list
+        [Optional. Default=None] Columns in dataframes for categorical variables
     allocate_total : bool
         whether to allocate the total from the source geometries (the default is True).
-    tables : tuple of two numpy.array (optional)
-         As generated from `tobler.area_weighted.area_tables_raster` (the default is None).
+    nodata : int
+        value in raster that indicates null or missing values. Default is 255
+    n_jobs : int
+        [Optional. Default=-1] Number of processes to run in parallel to
+        generate the area allocation. If -1, this is set to the number of CPUs
+        available.
+
 
     Returns
     -------
     geopandas.GeoDataFrame
         GeoDataFrame with geometries matching the target_df and extensive and intensive
         variables as the columns
 
     """
-    if not codes:
-        codes = [21, 22, 23, 24]
-    if not raster:
-        raise IOError(
-            "You must pass the path to a raster that can be read with rasterio"
-        )
-
-    if not tables:
-        tables = _area_tables_raster(
-            source_df,
-            target_df.copy(),
-            raster_path=raster,
-            codes=codes,
-            force_crs_match=force_crs_match,
+    if codes:
+        warn(
+            "The `codes` keyword is deprecated and will be removed shortly. Please use `pixel_values` instead"
         )
+        pixel_values = codes
+    source_df = source_df.copy()
+    assert not any(
+        source_df.index.duplicated()
+    ), "The index of the source_df cannot contain duplicates."
+
+    #  create a vector mask from the raster data
+    raster_mask = extract_raster_features(
+        source_df, raster, pixel_values, nodata, n_jobs, collapse_values=True
+    )
+    #  create a column in the source_df to dissolve on
+    idx_name = source_df.index.name if source_df.index.name else "idx"
+    source_df[idx_name] = source_df.index
+
+    #  clip source_df by its mask (overlay/dissolve is faster than gpd.clip here)
+    source_df = gpd.overlay(
+        source_df, raster_mask.to_crs(source_df.crs), how="intersection"
+    ).dissolve(idx_name)
 
-    # In area_interpolate, the resulting variable has same length as target_df
-    interpolation = _slow_area_interpolate(
+    #  continue with standard areal interpolation using the clipped source
+    interpolation = area_interpolate(
         source_df,
         target_df.copy(),
         extensive_variables=extensive_variables,
         intensive_variables=intensive_variables,
+        n_jobs=n_jobs,
+        categorical_variables=categorical_variables,
         allocate_total=allocate_total,
-        tables=tables,
     )
-
     return interpolation
```

### Comparing `tobler-0.8.2/tobler/pycno/pycno.py` & `tobler-0.9.0/tobler/pycno/pycno.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 
 def pycno(
     gdf, value_field, cellsize, r=0.2, handle_null=True, converge=3, verbose=True
 ):
     try:
         from astropy.convolution import convolve as astro_convolve
-    except Exception:
-        raise ("Pycnophylactic interpolation requires the astropy package")
+    except (ImportError, ModuleNotFoundError):
+        raise ImportError("Pycnophylactic interpolation requires the astropy package")
 
     """Returns a smooth pycnophylactic interpolation raster for a given geodataframe
 
     Args:
     gdf (geopandas.geodataframe.GeoDataFrame): Input GeoDataFrame.
     value_field (str): Field name of values to be used to produce pycnophylactic surface
     cellsize (int): Pixel size of raster in planar units (i.e. metres, feet)
@@ -282,15 +282,15 @@
     Notes
     -----
     The formula is based on Tobler, W. R. (1979). Smooth pycnophylactic interpolation for geographical regions. Journal of the American Statistical Association, 74(367), 519–529. https://doi.org/10.1080/01621459.1979.10481647
 
     Original implementation written by @danlewis85 at <https://github.com/danlewis85/pycno/>
     and based in part on the R pycno package by Chris Brusndon (<https://cran.r-project.org/web/packages/pycno/index.html>)
 
-    References: :cite:`tobler_smooth_1979` 
+    References: :cite:`tobler_smooth_1979`
     """
     assert source_df.crs.equals(
         target_df.crs
     ), "source_df CRS and target_df CRS are not the same. Reproject into consistent systems before proceeding"
     output_vars = target_df.copy()[[target_df.geometry.name]]
     for variable in variables:
         pyc, trans, _ = pycno(
```

### Comparing `tobler-0.8.2/tobler.egg-info/PKG-INFO` & `tobler-0.9.0/tobler.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,15 @@
 Metadata-Version: 2.1
 Name: tobler
-Version: 0.8.2
+Version: 0.9.0
 Summary: TOBLER: Areal Interpolation
 Home-page: https://github.com/pysal/tobler
 Maintainer: Serge Rey
 Maintainer-email: sjsrey@gmail.com
 License: 3-Clause BSD
-Description: <p align="center">
-        <img src="docs/figs/tobler_long.png" height="200px">
-        </p>
-        
-        ![CI Tests](https://github.com/pysal/tobler/workflows/Unit%20Tests/badge.svg)
-        [![codecov](https://codecov.io/gh/pysal/tobler/branch/master/graph/badge.svg?token=XO4SilfBEb)](https://codecov.io/gh/pysal/tobler)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tobler)
-        ![PyPI](https://img.shields.io/pypi/v/tobler)
-        ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/tobler)
-        ![GitHub commits since latest release (branch)](https://img.shields.io/github/commits-since/pysal/tobler/latest)
-        [![DOI](https://zenodo.org/badge/202220824.svg)](https://zenodo.org/badge/latestdoi/202220824)
-        
-        # PySAL `tobler`
-        
-        `tobler` is a python package for areal interpolation, dasymetric mapping, change of support, and small area estimation. It provides a suite of tools with a simple interface for transferring data from one polygonal representation to another. Common examples include standardizing census data from different time periods to a single representation (i.e. to overcome boundary changes in successive years), or the conversion of data collected at different spatial scales into shared units of analysis (e.g. converting zip code and neighborhood data into a regular grid). `tobler` is part of the [PySAL](https://pysal.org) family of packages for spatial data science and provides highly performant implementations of basic and advanced interpolation methods, leveraging [`pygeos`](https://pygeos.readthedocs.io/en/latest/) to optimize for multicore architecture. The package name is an homage to the legendary quantitative geographer [Waldo Tobler](https://en.wikipedia.org/wiki/Waldo_R._Tobler), a pioneer in geographic interpolation methods, spatial analysis, and computational social science.
-        
-        ![DC tracts to hexgrid](docs/_static/images/notebooks_census_to_hexgrid_25_1.png)
-        
-        ## Interpolation Methods
-        
-        `tobler` provides functionality for three families of spatial interpolation methods. The utility of each technique depends on the context of the problem and varies according to e.g. data availability, the properties of the interpolated variable, and the resolution of source and target geometries. For a further explanation of different interpolation techniques, please explore some of the field's [background literature](https://pysal.org/tobler/references.html)
-        
-        ### Area Weighted
-        
-        Areal interpolation uses the area of overlapping geometries to apportion variables. This is the simplest method with no additional data requirements, aside from input and output geometries, however this method is also most susceptible to the [modifiable areal unit problem](https://en.wikipedia.org/wiki/Modifiable_areal_unit_problem).
-        
-        ### Dasymetric
-        
-        Dasymetric interpolation uses auxiliary data to improve estimation, for example
-        by constraining the areal interpolation to areas that are known to be inhabited. Formally, `tobler` adopts a binary dasymetric approach, using auxiliary data to define which land is available or unavailable for interpolation. The package can incorporate additional sources such as
-        
-        * raster data such as satellite imagery that define land types
-        * vector features such as roads or water bodies that define habitable or inhabitable land
-        
-        either (or both) of which may be used to help ensure that variables from the source geometries are not allocated to inappropriate areas of the target geometries. Naturally, dasymetric approaches are sensitive to the quality of ancillary data and underlying assumptions used to guide the estimation.
-        
-        ### Model-based
-        
-        Model-based interpolation uses [spatial] statistical models to estimate a relationship between the target variable and a set of covariates such as physical features, administrative designations, or demographic and architectural characteristics. Model-based approaches offer the ability to incorporate the richest set of additional data, but they can also difficult to wield in practice because the true relationship between variables is never known. By definition, some formal assumptions of regression models are violated because the target variable is always predicted using data from a different spatial scale than it was estimated.
-        
-        ### Extensions
-        
-        `tobler` is under active development and will continue to incorporate emerging interpolation methods as they are introduced to the field. We welcome any and all contributions and if you would like to propose an additional method for adoption please raise an issue for discussion or open a new pull request!
-        
-        ![Charleston zipcodes to tracts](docs/_static/images/tobler3.png)
-        
-        ![raster example](docs/figs/raster_lattice_example.png)
-        
-        ## Installation
-        
-        ```bash
-        $ conda env create -f environment.yml
-        $ conda activate tobler 
-        $ python setup.py develop
-        ```
-        
-        ## Contribute
-        
-        PySAL-tobler is under active development and contributors are welcome.
-        
-        If you have any suggestion, feature request, or bug report, please open a new [issue](https://github.com/pysal/tobler/issues) on GitHub. To submit patches, please follow the PySAL development [guidelines](http://pysal.readthedocs.io/en/latest/developers/index.html) and open a [pull request](https://github.com/pysal/tobler). Once your changes get merged, you’ll automatically be added to the [Contributors List](https://github.com/pysal/tobler/graphs/contributors).
-        
-        ## License
-        
-        The project is licensed under the [BSD license](https://github.com/pysal/tobler/blob/master/LICENSE.txt).
-        
-        ## Funding
-        
-        <img src="docs/figs/nsf_logo.jpg" width="50"> 
-        
-        Award #1733705 [Neighborhoods in Space-Time Contexts](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1733705&HistoricalAwards=false)
-        
-         Award #1831615 [Scalable Geospatial Analytics for Social Science Research](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1831615)
-        
 Keywords: spatial statistics,interpolation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
@@ -92,7 +19,83 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
+License-File: LICENSE.txt
+
+<p align="center">
+<img src="docs/figs/tobler_long.png" height="200px">
+</p>
+
+![CI Tests](https://github.com/pysal/tobler/workflows/Unit%20Tests/badge.svg)
+[![codecov](https://codecov.io/gh/pysal/tobler/branch/master/graph/badge.svg?token=XO4SilfBEb)](https://codecov.io/gh/pysal/tobler)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tobler)
+![PyPI](https://img.shields.io/pypi/v/tobler)
+![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/tobler)
+![GitHub commits since latest release (branch)](https://img.shields.io/github/commits-since/pysal/tobler/latest)
+[![DOI](https://zenodo.org/badge/202220824.svg)](https://zenodo.org/badge/latestdoi/202220824)
+
+# PySAL `tobler`
+
+`tobler` is a python package for areal interpolation, dasymetric mapping, change of support, and small area estimation. It provides a suite of tools with a simple interface for transferring data from one polygonal representation to another. Common examples include standardizing census data from different time periods to a single representation (i.e. to overcome boundary changes in successive years), or the conversion of data collected at different spatial scales into shared units of analysis (e.g. converting zip code and neighborhood data into a regular grid). `tobler` is part of the [PySAL](https://pysal.org) family of packages for spatial data science and provides highly performant implementations of basic and advanced interpolation methods, leveraging [`pygeos`](https://pygeos.readthedocs.io/en/latest/) to optimize for multicore architecture. The package name is an homage to the legendary quantitative geographer [Waldo Tobler](https://en.wikipedia.org/wiki/Waldo_R._Tobler), a pioneer in geographic interpolation methods, spatial analysis, and computational social science.
+
+![DC tracts to hexgrid](docs/_static/images/notebooks_census_to_hexgrid_25_1.png)
+
+## Interpolation Methods
+
+`tobler` provides functionality for three families of spatial interpolation methods. The utility of each technique depends on the context of the problem and varies according to e.g. data availability, the properties of the interpolated variable, and the resolution of source and target geometries. For a further explanation of different interpolation techniques, please explore some of the field's [background literature](https://pysal.org/tobler/references.html)
+
+### Area Weighted
+
+Areal interpolation uses the area of overlapping geometries to apportion variables. This is the simplest method with no additional data requirements, aside from input and output geometries, however this method is also most susceptible to the [modifiable areal unit problem](https://en.wikipedia.org/wiki/Modifiable_areal_unit_problem).
+
+### Dasymetric
+
+Dasymetric interpolation uses auxiliary data to improve estimation, for example
+by constraining the areal interpolation to areas that are known to be inhabited. Formally, `tobler` adopts a binary dasymetric approach, using auxiliary data to define which land is available or unavailable for interpolation. The package can incorporate additional sources such as
+
+* raster data such as satellite imagery that define land types
+* vector features such as roads or water bodies that define habitable or inhabitable land
+
+either (or both) of which may be used to help ensure that variables from the source geometries are not allocated to inappropriate areas of the target geometries. Naturally, dasymetric approaches are sensitive to the quality of ancillary data and underlying assumptions used to guide the estimation.
+
+### Model-based
+
+Model-based interpolation uses [spatial] statistical models to estimate a relationship between the target variable and a set of covariates such as physical features, administrative designations, or demographic and architectural characteristics. Model-based approaches offer the ability to incorporate the richest set of additional data, but they can also difficult to wield in practice because the true relationship between variables is never known. By definition, some formal assumptions of regression models are violated because the target variable is always predicted using data from a different spatial scale than it was estimated.
+
+### Extensions
+
+`tobler` is under active development and will continue to incorporate emerging interpolation methods as they are introduced to the field. We welcome any and all contributions and if you would like to propose an additional method for adoption please raise an issue for discussion or open a new pull request!
+
+![Charleston zipcodes to tracts](docs/_static/images/tobler3.png)
+
+![raster example](docs/figs/raster_lattice_example.png)
+
+## Installation
+
+```bash
+$ conda env create -f environment.yml
+$ conda activate tobler 
+$ python setup.py develop
+```
+
+## Contribute
+
+PySAL-tobler is under active development and contributors are welcome.
+
+If you have any suggestion, feature request, or bug report, please open a new [issue](https://github.com/pysal/tobler/issues) on GitHub. To submit patches, please follow the PySAL development [guidelines](http://pysal.readthedocs.io/en/latest/developers/index.html) and open a [pull request](https://github.com/pysal/tobler). Once your changes get merged, you’ll automatically be added to the [Contributors List](https://github.com/pysal/tobler/graphs/contributors).
+
+## License
+
+The project is licensed under the [BSD license](https://github.com/pysal/tobler/blob/master/LICENSE.txt).
+
+## Funding
+
+<img src="docs/figs/nsf_logo.jpg" width="50"> 
+
+Award #1733705 [Neighborhoods in Space-Time Contexts](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1733705&HistoricalAwards=false)
+
+ Award #1831615 [Scalable Geospatial Analytics for Social Science Research](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1831615)
+
+
```

### Comparing `tobler-0.8.2/tobler.egg-info/SOURCES.txt` & `tobler-0.9.0/tobler.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 requirements.txt
 requirements_docs.txt
 requirements_tests.txt
+setup.cfg
 setup.py
+versioneer.py
 tobler/__init__.py
+tobler/_version.py
 tobler.egg-info/PKG-INFO
 tobler.egg-info/SOURCES.txt
 tobler.egg-info/dependency_links.txt
 tobler.egg-info/not-zip-safe
 tobler.egg-info/requires.txt
 tobler.egg-info/top_level.txt
 tobler/area_weighted/__init__.py
-tobler/area_weighted/_vectorized_raster_interpolation.py
 tobler/area_weighted/area_interpolate.py
 tobler/area_weighted/area_join.py
 tobler/dasymetric/__init__.py
 tobler/dasymetric/masked_area_interpolate.py
 tobler/dasymetric/raster_tools.py
 tobler/model/__init__.py
 tobler/model/glm.py
```

