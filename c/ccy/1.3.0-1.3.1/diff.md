# Comparing `tmp/ccy-1.3.0.tar.gz` & `tmp/ccy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccy-1.3.0.tar", max compression
+gzip compressed data, was "ccy-1.3.1.tar", max compression
```

## Comparing `ccy-1.3.0.tar` & `ccy-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1488 2022-10-30 14:43:53.220468 ccy-1.3.0/LICENSE
--rw-r--r--   0        0        0     5287 2022-10-30 14:43:53.224468 ccy-1.3.0/README.rst
--rw-r--r--   0        0        0     1698 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/__init__.py
--rw-r--r--   0        0        0        0 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/core/__init__.py
--rw-r--r--   0        0        0     3094 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/core/country.py
--rw-r--r--   0        0        0     6205 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/core/currency.py
--rw-r--r--   0        0        0    10084 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/core/data.py
--rw-r--r--   0        0        0     1626 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/core/daycounter.py
--rw-r--r--   0        0        0        0 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/dates/__init__.py
--rw-r--r--   0        0        0     3446 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/dates/converters.py
--rw-r--r--   0        0        0      542 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/dates/futures.py
--rw-r--r--   0        0        0     4206 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/dates/period.py
--rw-r--r--   0        0        0      316 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/tradingcentres/__init__.py
--rw-r--r--   0        0        0     4299 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/tradingcentres/centres.py
--rw-r--r--   0        0        0      619 2022-10-30 14:43:53.224468 ccy-1.3.0/ccy/tradingcentres/holiday.py
--rw-r--r--   0        0        0      630 2022-10-30 14:43:53.224468 ccy-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5965 1970-01-01 00:00:00.000000 ccy-1.3.0/setup.py
--rw-r--r--   0        0        0     5681 1970-01-01 00:00:00.000000 ccy-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-07-20 19:57:03.636371 ccy-1.3.1/LICENSE
+-rw-r--r--   0        0        0     5287 2023-07-20 19:57:03.636371 ccy-1.3.1/README.rst
+-rw-r--r--   0        0        0     1698 2023-07-20 19:57:03.636371 ccy-1.3.1/ccy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 19:57:03.636371 ccy-1.3.1/ccy/core/__init__.py
+-rw-r--r--   0        0        0     3094 2023-07-20 19:57:03.636371 ccy-1.3.1/ccy/core/country.py
+-rw-r--r--   0        0        0     6205 2023-07-20 19:57:03.636371 ccy-1.3.1/ccy/core/currency.py
+-rw-r--r--   0        0        0    10084 2023-07-20 19:57:03.636371 ccy-1.3.1/ccy/core/data.py
+-rw-r--r--   0        0        0     1626 2023-07-20 19:57:03.636371 ccy-1.3.1/ccy/core/daycounter.py
+-rw-r--r--   0        0        0        0 2023-07-20 19:57:03.636371 ccy-1.3.1/ccy/dates/__init__.py
+-rw-r--r--   0        0        0     3446 2023-07-20 19:57:03.640371 ccy-1.3.1/ccy/dates/converters.py
+-rw-r--r--   0        0        0      542 2023-07-20 19:57:03.640371 ccy-1.3.1/ccy/dates/futures.py
+-rw-r--r--   0        0        0     4206 2023-07-20 19:57:03.640371 ccy-1.3.1/ccy/dates/period.py
+-rw-r--r--   0        0        0      316 2023-07-20 19:57:03.640371 ccy-1.3.1/ccy/tradingcentres/__init__.py
+-rw-r--r--   0        0        0     4299 2023-07-20 19:57:03.640371 ccy-1.3.1/ccy/tradingcentres/centres.py
+-rw-r--r--   0        0        0      619 2023-07-20 19:57:03.640371 ccy-1.3.1/ccy/tradingcentres/holiday.py
+-rw-r--r--   0        0        0      611 2023-07-20 19:57:03.640371 ccy-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5673 1970-01-01 00:00:00.000000 ccy-1.3.1/PKG-INFO
```

### Comparing `ccy-1.3.0/LICENSE` & `ccy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/README.rst` & `ccy-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/__init__.py` & `ccy-1.3.1/ccy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python currencies"""
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 
 from .core.country import (
     CountryError,
     countries,
     country,
     country_map,
```

### Comparing `ccy-1.3.0/ccy/core/country.py` & `ccy-1.3.1/ccy/core/country.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/core/currency.py` & `ccy-1.3.1/ccy/core/currency.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/core/data.py` & `ccy-1.3.1/ccy/core/data.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/core/daycounter.py` & `ccy-1.3.1/ccy/core/daycounter.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/dates/converters.py` & `ccy-1.3.1/ccy/dates/converters.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/dates/futures.py` & `ccy-1.3.1/ccy/dates/futures.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/dates/period.py` & `ccy-1.3.1/ccy/dates/period.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/tradingcentres/centres.py` & `ccy-1.3.1/ccy/tradingcentres/centres.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/ccy/tradingcentres/holiday.py` & `ccy-1.3.1/ccy/tradingcentres/holiday.py`

 * *Files identical despite different names*

### Comparing `ccy-1.3.0/pyproject.toml` & `ccy-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "ccy"
-version = "1.3.0"
+version = "1.3.1"
 description = "Python currencies"
 authors = ["Luca Sbardella <luca@quantmind.com>"]
 license = "BSD"
 readme = "README.rst"
 packages = [
     { include = "ccy" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 python-dateutil = "^2.8.2"
-pytz = "^2022.5"
+pytz = ">=2022.5"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
 coverage = "^6.5.0"
-codecov = "^2.1.12"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 mypy = "^0.982"
 flake8-blind-except = "^0.2.1"
 flake8-commas = "^2.1.0"
 
 [build-system]
```

### Comparing `ccy-1.3.0/setup.py` & `ccy-1.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,222 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ccy
+Version: 1.3.1
+Summary: Python currencies
+License: BSD
+Author: Luca Sbardella
+Author-email: luca@quantmind.com
+Requires-Python: >=3.8,<3.12
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: pytz (>=2022.5)
+Description-Content-Type: text/x-rst
+
+A python module for currencies. The module compiles a dictionary of
+currency objects containing information useful in financial analysis.
+Not all currencies in the world are supported yet. You are welcome to
+join and add more.
+
+:Package: |version| |license| |pyversions| |status| |downloads|
+:CI: |master-build| |coverage-master|
+:Dowloads: https://pypi.org/project/ccy/
+:Source: https://github.com/quantmind/ccy
+
+.. |version| image:: https://badge.fury.io/py/ccy.svg
+  :target: https://badge.fury.io/py/ccy
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/ccy.svg
+  :target: https://pypi.org/project/ccy/
+.. |license| image:: https://img.shields.io/pypi/l/ccy.svg
+  :target: https://pypi.org/project/ccy/
+.. |status| image:: https://img.shields.io/pypi/status/ccy.svg
+  :target: https://pypi.org/project/ccy/
+.. |downloads| image:: https://img.shields.io/pypi/dd/ccy.svg
+  :target: https://pypi.org/project/ccy/
+.. |master-build| image:: https://github.com/quantmind/ccy/workflows/build/badge.svg
+  :target: https://github.com/quantmind/ccy/actions?query=workflow%3Abuild
+.. |coverage-master| image:: https://codecov.io/gh/quantmind/ccy/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/quantmind/ccy
+
+
+.. contents::
+    :local:
+
+
+Currency object
+======================
+To use it::
+
+    >>> import ccy
+    >>> c = ccy.currency('aud')
+    >>> c.printinfo()
+    code: AUD
+    twoletterscode: AD
+    rounding: 4
+    default_country: AU
+    isonumber: 036
+    order: 3
+    name: Australian Dollar
+    >>> c.as_cross()
+    'AUDUSD'
+    >>> c.as_cross('/')
+    'AUD/USD'
+
+a currency object has the following properties:
+
+* *code*: the `ISO 4217`_ code.
+* *twoletterscode*: two letter code (can't remeber the ISO number). Very useful for financial data providers such as Bloomberg.
+* *default_country*: the default `ISO 3166-1 alpha-2`_ country code for the currency.
+* *isonumber*: the ISO 4217 number.
+* *name*: the name of the currency.
+* *order*: default ordering in currency pairs (more of this below).
+* *rounding*: number of decimal places
+
+Currency Crosses
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+You can create currency pairs by using the ``currency_pair`` function::
+
+    >>> import ccy
+    >>> p = ccy.currency_pair('eurusd')
+    >>> p
+    ccy_pair: EURUSD
+    >>> p.mkt()  # market convention pair
+    ccy_pair: EURUSD
+    >>> p = ccy.currency_pair('chfusd')
+    >>> p
+    ccy_pair: CHFUSD
+    >>> p.mkt()  # market convention pair
+    ccy_pair: USDCHF
+
+
+Some shortcuts::
+
+    >>> import ccy
+    >>> ccy.cross('aud')
+    'AUDUSD'
+    >>> ccy.crossover('eur')
+    'EUR/USD'
+    >>> ccy.crossover('chf')
+    'USD/CHF'
+
+Note, the Swiss franc cross is represented as 'USD/CHF', while the Aussie Dollar
+and Euro crosses are represented with the USD as denominator.
+This is the market convention which is handled by the **order** property
+of a currency object.
+
+Country information
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To use it::
+
+    >>> import ccy
+    >>> c = ccy.country('us')
+    >>> c
+    'United States'
+    >>> ccy.countryccy('us')
+    'USD'
+
+
+Not all the country codes are standard `ISO 3166-1 alpha-2`_.
+There is a function for adding extra pseudo-countries::
+
+    import ccy
+    ccy.set_new_country('EU','EUR','Eurozone')
+
+Set a new country with code 'EU', currency 'EUR' named 'Eurozone'.
+This pseudo country is set in the library already.
+
+Countries
+==============
+
+Country information is obtained via the pytz_ package which is strict
+requirement for ``ccy``::
+
+    >>> from ccy import country
+    >>> country('it')
+    'Italy'
+
+It knows about the 18 eurozone_ countries (European countries which share the
+euro as common currency)::
+
+    >>> from ccy import eurozone
+
+eurozone is tuple of country ISO codes::
+
+    >>> import ccy
+    >>> ccy.print_eurozone()
+    Austria
+    Belgium
+    Cyprus
+    Estonia
+    Finland
+    France
+    Germany
+    Greece
+    Ireland
+    Italy
+    Latvia
+    Lithuania
+    Luxembourg
+    Malta
+    Netherlands
+    Portugal
+    Slovakia
+    Slovenia
+    Spain
+
+
+Date and Periods
+===================
+
+The module is shipped with a ``date`` module for manipulating time periods and
+converting dates between different formats. The *period* function can be used
+to create ``Period`` instances::
+
+    >>> from ccy import period
+    >>> p = period('1m')
+    >>> p
+    1M
+    >>> p += '2w'
+    >>> p
+    1M2W
+    >>> P += '3m'
+    >>> p
+    4M2W
+
+
+Installation
+================
+This library works for Python 2.6 and higher, including Python 3.
+In addition, it requires:
+
+* pytz_ for Countries information.
+* dateutils_ for date calculations
+
+Install using ``pip``::
+
+    pip install ccy
+
+or from source::
+
+    python setup.py install
+
+
+Running tests
+~~~~~~~~~~~~~~~~~~~~~
+
+From within the package directory::
+
+    python setup.py test
+
+
+.. _pytz: http://pytz.sourceforge.net/
+.. _`ISO 3166-1 alpha-2`: http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2
+.. _`ISO 4217`: http://en.wikipedia.org/wiki/ISO_4217
+.. _dateutils: https://pypi.python.org/pypi/python-dateutil
+.. _eurozone: http://www.eurozone.europa.eu/euro-area/euro-area-member-states/
 
-packages = \
-['ccy', 'ccy.core', 'ccy.dates', 'ccy.tradingcentres']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['python-dateutil>=2.8.2,<3.0.0', 'pytz>=2022.5,<2023.0']
-
-setup_kwargs = {
-    'name': 'ccy',
-    'version': '1.3.0',
-    'description': 'Python currencies',
-    'long_description': "A python module for currencies. The module compiles a dictionary of\ncurrency objects containing information useful in financial analysis.\nNot all currencies in the world are supported yet. You are welcome to\njoin and add more.\n\n:Package: |version| |license| |pyversions| |status| |downloads|\n:CI: |master-build| |coverage-master|\n:Dowloads: https://pypi.org/project/ccy/\n:Source: https://github.com/quantmind/ccy\n\n.. |version| image:: https://badge.fury.io/py/ccy.svg\n  :target: https://badge.fury.io/py/ccy\n.. |pyversions| image:: https://img.shields.io/pypi/pyversions/ccy.svg\n  :target: https://pypi.org/project/ccy/\n.. |license| image:: https://img.shields.io/pypi/l/ccy.svg\n  :target: https://pypi.org/project/ccy/\n.. |status| image:: https://img.shields.io/pypi/status/ccy.svg\n  :target: https://pypi.org/project/ccy/\n.. |downloads| image:: https://img.shields.io/pypi/dd/ccy.svg\n  :target: https://pypi.org/project/ccy/\n.. |master-build| image:: https://github.com/quantmind/ccy/workflows/build/badge.svg\n  :target: https://github.com/quantmind/ccy/actions?query=workflow%3Abuild\n.. |coverage-master| image:: https://codecov.io/gh/quantmind/ccy/branch/master/graph/badge.svg\n  :target: https://codecov.io/gh/quantmind/ccy\n\n\n.. contents::\n    :local:\n\n\nCurrency object\n======================\nTo use it::\n\n    >>> import ccy\n    >>> c = ccy.currency('aud')\n    >>> c.printinfo()\n    code: AUD\n    twoletterscode: AD\n    rounding: 4\n    default_country: AU\n    isonumber: 036\n    order: 3\n    name: Australian Dollar\n    >>> c.as_cross()\n    'AUDUSD'\n    >>> c.as_cross('/')\n    'AUD/USD'\n\na currency object has the following properties:\n\n* *code*: the `ISO 4217`_ code.\n* *twoletterscode*: two letter code (can't remeber the ISO number). Very useful for financial data providers such as Bloomberg.\n* *default_country*: the default `ISO 3166-1 alpha-2`_ country code for the currency.\n* *isonumber*: the ISO 4217 number.\n* *name*: the name of the currency.\n* *order*: default ordering in currency pairs (more of this below).\n* *rounding*: number of decimal places\n\nCurrency Crosses\n~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nYou can create currency pairs by using the ``currency_pair`` function::\n\n    >>> import ccy\n    >>> p = ccy.currency_pair('eurusd')\n    >>> p\n    ccy_pair: EURUSD\n    >>> p.mkt()  # market convention pair\n    ccy_pair: EURUSD\n    >>> p = ccy.currency_pair('chfusd')\n    >>> p\n    ccy_pair: CHFUSD\n    >>> p.mkt()  # market convention pair\n    ccy_pair: USDCHF\n\n\nSome shortcuts::\n\n    >>> import ccy\n    >>> ccy.cross('aud')\n    'AUDUSD'\n    >>> ccy.crossover('eur')\n    'EUR/USD'\n    >>> ccy.crossover('chf')\n    'USD/CHF'\n\nNote, the Swiss franc cross is represented as 'USD/CHF', while the Aussie Dollar\nand Euro crosses are represented with the USD as denominator.\nThis is the market convention which is handled by the **order** property\nof a currency object.\n\nCountry information\n~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nTo use it::\n\n    >>> import ccy\n    >>> c = ccy.country('us')\n    >>> c\n    'United States'\n    >>> ccy.countryccy('us')\n    'USD'\n\n\nNot all the country codes are standard `ISO 3166-1 alpha-2`_.\nThere is a function for adding extra pseudo-countries::\n\n    import ccy\n    ccy.set_new_country('EU','EUR','Eurozone')\n\nSet a new country with code 'EU', currency 'EUR' named 'Eurozone'.\nThis pseudo country is set in the library already.\n\nCountries\n==============\n\nCountry information is obtained via the pytz_ package which is strict\nrequirement for ``ccy``::\n\n    >>> from ccy import country\n    >>> country('it')\n    'Italy'\n\nIt knows about the 18 eurozone_ countries (European countries which share the\neuro as common currency)::\n\n    >>> from ccy import eurozone\n\neurozone is tuple of country ISO codes::\n\n    >>> import ccy\n    >>> ccy.print_eurozone()\n    Austria\n    Belgium\n    Cyprus\n    Estonia\n    Finland\n    France\n    Germany\n    Greece\n    Ireland\n    Italy\n    Latvia\n    Lithuania\n    Luxembourg\n    Malta\n    Netherlands\n    Portugal\n    Slovakia\n    Slovenia\n    Spain\n\n\nDate and Periods\n===================\n\nThe module is shipped with a ``date`` module for manipulating time periods and\nconverting dates between different formats. The *period* function can be used\nto create ``Period`` instances::\n\n    >>> from ccy import period\n    >>> p = period('1m')\n    >>> p\n    1M\n    >>> p += '2w'\n    >>> p\n    1M2W\n    >>> P += '3m'\n    >>> p\n    4M2W\n\n\nInstallation\n================\nThis library works for Python 2.6 and higher, including Python 3.\nIn addition, it requires:\n\n* pytz_ for Countries information.\n* dateutils_ for date calculations\n\nInstall using ``pip``::\n\n    pip install ccy\n\nor from source::\n\n    python setup.py install\n\n\nRunning tests\n~~~~~~~~~~~~~~~~~~~~~\n\nFrom within the package directory::\n\n    python setup.py test\n\n\n.. _pytz: http://pytz.sourceforge.net/\n.. _`ISO 3166-1 alpha-2`: http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2\n.. _`ISO 4217`: http://en.wikipedia.org/wiki/ISO_4217\n.. _dateutils: https://pypi.python.org/pypi/python-dateutil\n.. _eurozone: http://www.eurozone.europa.eu/euro-area/euro-area-member-states/\n",
-    'author': 'Luca Sbardella',
-    'author_email': 'luca@quantmind.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

