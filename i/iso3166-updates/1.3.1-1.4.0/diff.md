# Comparing `tmp/iso3166-updates-1.3.1.tar.gz` & `tmp/iso3166-updates-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-1.3.1.tar", last modified: Sat Jun 24 13:15:40 2023, max compression
+gzip compressed data, was "iso3166-updates-1.4.0.tar", last modified: Thu Jul 20 19:26:12 2023, max compression
```

## Comparing `iso3166-updates-1.3.1.tar` & `iso3166-updates-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35367 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-24 13:15:40.000000 iso3166-updates-1.3.1/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-24 13:15:40.728347 iso3166-updates-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-24 13:15:14.000000 iso3166-updates-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21765 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/iso3166_updates/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/iso3166_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/iso3166_updates/iso3166_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/iso3166_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21765 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:26:11.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 19:26:12.000000 iso3166-updates-1.4.0/iso3166_updates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-20 19:26:12.312900 iso3166-updates-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-20 19:25:42.000000 iso3166-updates-1.4.0/setup.py
```

### Comparing `iso3166-updates-1.3.1/LICENSE` & `iso3166-updates-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.3.1/PKG-INFO` & `iso3166-updates-1.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,25 @@
-Metadata-Version: 2.1
-Name: iso3166-updates
-Version: 1.3.1
-Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
-Home-page: https://github.com/amckenna41/iso3166-updates
-Author: AJ McKenna, https://github.com/amckenna41
-Author-email: amckenna41@qub.ac.uk
-Maintainer: AJ McKenna
-License: MIT
-Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
-Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: Free For Educational Use
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
-
 # iso3166-updates
 
 [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
 [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/amckenna41/iso3166-updates/tree/main.svg?style=svg&circle-token=9b0c0a9f6cc032f255dc28842c95600401aa4426)](https://dl.circleci.com/status-badge/redirect/gh/amckenna41/iso3166-updates/tree/main)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
+<!-- [![codecov](https://codecov.io/gh/amckenna41/iso3166-updates/branch/main/graph/badge.svg?token=XOBSBVH8XA)](https://codecov.io/gh/amckenna41/iso3166-updates) -->
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-<!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
 [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
-[![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
+<!-- [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates) -->
 <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
   <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
 </div>
 
-> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
   * [API](#api)
   * [Staying up to date](#staying-up-to-date)
   * [Requirements](#requirements)
@@ -94,39 +60,36 @@
 
 * The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
 
 * Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
 
 * If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
-The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g. the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>.
+
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
 
 Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
-Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
+Ultimately, this Cloud Run microservice ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
-* [python][python] >= 3.7
-* [pandas][pandas] >= 1.4.3
-* [numpy][numpy] >= 1.23.2
-* [requests][requests] >= 2.28.1
-* [beautifulsoup4][beautifulsoup4] >= 4.11.1
-* [iso3166][iso3166] >= 2.1.1
+* [python][python] >= 3.8
+* [iso3166][iso3166] >= 2.1.1 
 
 Installation
 ------------
 Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-updates --upgrade
@@ -135,21 +98,75 @@
 Installation from source:
 ```bash
 git clone -b master https://github.com/amckenna41/iso3166-updates.git
 cd iso3166_updates
 python3 setup.py install
 ```
 
-Usage
------
+Usage (iso3166-updates Python package)
+--------------------------------------
+Below are some examples of using the custom-built iso3166-updates Python package. 
+
 **Import package:**
 ```python
-import iso3166_updates as iso3166_updates
+import iso3166_updates as iso
+```
+
+**Get all listed changes/updates for all countries and years:**
+```python
+iso.updates.all
 ```
 
+**Get all listed ISO 3166-2 changes/updates for Andorra (AD):**
+```python
+iso.updates.AD
+```
+
+**Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY:**
+```python
+iso.updates["BA","DE","FR","HU","PY"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
+```python
+iso.updates.year("2012-2021")["IE"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015":**
+```python
+iso.updates.year(">2015")["TA"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
+```python
+iso.updates.year("<2010")["YE"]
+```
+Usage get_all_iso3166_updates.py script
+---------------------------------------
+Below are some examples of using the get_all_iso3166_updates.py script which is used to pull all the ISO 3166 updates
+from the various data sources.
+
+**Requirements:**
+* [python][python] >= 3.8
+* [iso3166-updates][iso3166-updates] >= 1.3.0
+* [pandas][pandas] >= 1.4.3
+* [numpy][numpy] >= 1.23.2
+* [requests][requests] >= 2.28.1
+* [beautifulsoup4][beautifulsoup4] >= 4.11.1
+* [iso3166][iso3166] >= 2.1.1
+* [google-auth][google-auth] >= 2.17.3
+* [google-cloud-storage][google-cloud-storage] >= 2.8.0
+* [google-api-python-client][google-api-python-client] >= 2.86.0
+* [emoji-country-flag][emoji-country-flag] == 1.3.0
+* [selenium][seleniumn] >= 4.10.0
+* [flask][flask] >= 2.3.2
+* [gunicorn][gunicorn] >= 21.2.0
+<!-- * [webdriver-manager][webdriver-manager] >= 3.8.6 -->
+<!-- * [lxml][lxml] >=  4.9.3 -->
+
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
   #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
@@ -159,26 +176,34 @@
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
   #                       Selected year/years, year ranges or year to check for updates greater
   #                       than or less than specified year
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
+  # -verbose, --verbose
+  #                       Set to 1 to print out progress of updates function, 0 will not print progress.
+  # -use_selenium, --use_selenium
+  #                       Gather all data for each country from its official page on the ISO website which 
+  #                       requires Python Selenium and chromedriver. If False then just use country data
+  #                       from its wiki page.
 ```
+**Get all the latest updates for all ISO 3166 countries**
+```bash
+./get_all_updates.sh 
 
-**Get all listed changes/updates for all countries and years which happens by default if no alpha-2 codes or years specified in input paramaters, export csv and json to folder "iso3166-updates", print progress via verbose flag:**
-```python
-iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1, verbose=1)
-#exported files: /iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
+'''
+--export_filename     Filename for exported JSON/CSVs files containing updates data (default="iso3166-updates.json").
+--export_folder       Folder name to store exported JSON/CSVs files containing updates data (default="test-iso3166-updates).
+'''
 ```
 
-**Get all listed ISO 3166-2 changes/updates for Andorra, export csv and json to folder "iso3166-updates":**
+**Import module:**
 ```python
-iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
+import get_all_iso3166_updates as iso3166_updates
 ```
 
 **Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```python
 iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0, verbose=1)
 #exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
@@ -202,27 +227,14 @@
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ```
-## Terminal/Command Line
-
-The software functions can also be run from the cmd/terminal interface, when the script is called the get_updates() function will be called. The script accepts the same parameter names as the get_updates() function.
-
-**Get all listed ISO 3166-2 changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose flag:** 
-```bash
-python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
-```
-
-**Get all listed ISO 3166-2 changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose flag:**
-```bash
-python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
-```
 
 The output to the above functions for the updates/changes to an ISO 3166-2 country returns 4 columns: 
 <b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
 * Edition/Newsletter: Name and or edition of newsletter that the ISO 3166-2 change/update was communicated in.
 * Date Issued: Date that the change was communicated.
 * Code/Subdivision change: Overall summary of change/update made.
@@ -265,42 +277,53 @@
 Directories
 -----------
 * `/docs` - documentation for `iso3166-updates` Python package.
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
 * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
 * `/tests` - unit and integration tests for `iso3166-updates`.
+* `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
+* `get_all_iso3166-updates.sh` - shell script created to call the get_all..py script to introduce some pseudo randomness required when using Python Selenium. 
 
 Issues
 ------
-Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
+Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository.
 
 Contact
 -------
 If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
 
 References
 ----------
-\[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
-\[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
+\[1\]: ISO 3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
+\[2\]: ISO 3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
 \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
 \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
-\[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
-\[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
+\[5\]: ISO 3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
+\[6\]: ISO 3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
 
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
 [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [python]: https://www.python.org/downloads/release/python-360/
+[iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
+[google-auth]: https://cloud.google.com/python/docs/reference
+[google-cloud-storage]: https://cloud.google.com/python/docs/reference
+[google-api-python-client]: https://cloud.google.com/python/docs/reference
+[flask]: https://flask.palletsprojects.com/en/2.3.x/
+[emoji-country-flag]: https://pypi.org/project/emoji-country-flag/
+[gunicorn]: https://pypi.org/project/gunicorn/
+[selenium]: https://selenium-python.readthedocs.io/index.html
+[webdriver-manager]: https://pypi.org/project/webdriver-manager/
+[lxml]: https://lxml.de/
 [iso3166]: https://github.com/deactivated/python-iso3166
 [PyPi]: https://pypi.org/project/iso3166-updates/
-[Issues]: https://github.com/amckenna41/iso3166-updates/issues
-
+[Issues]: https://github.com/amckenna41/iso3166-updates/issues
```

### Comparing `iso3166-updates-1.3.1/README.md` & `iso3166-updates-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,60 @@
+Metadata-Version: 2.1
+Name: iso3166-updates
+Version: 1.4.0
+Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
+Home-page: https://github.com/amckenna41/iso3166-updates
+Author: AJ McKenna, https://github.com/amckenna41
+Author-email: amckenna41@qub.ac.uk
+Maintainer: AJ McKenna
+License: MIT
+Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
+Keywords: iso,iso3166,beautifulsoup,python,pypi,countries,country codes,csv,iso3166-2,iso3166-1,alpha-2,alpha-3
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Free For Educational Use
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: docs
+License-File: LICENSE
+
 # iso3166-updates
 
 [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
 [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/amckenna41/iso3166-updates/tree/main.svg?style=svg&circle-token=9b0c0a9f6cc032f255dc28842c95600401aa4426)](https://dl.circleci.com/status-badge/redirect/gh/amckenna41/iso3166-updates/tree/main)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
+<!-- [![codecov](https://codecov.io/gh/amckenna41/iso3166-updates/branch/main/graph/badge.svg?token=XOBSBVH8XA)](https://codecov.io/gh/amckenna41/iso3166-updates) -->
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-<!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
 [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
-[![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
+<!-- [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates) -->
 <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
   <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
 </div>
 
-> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
   * [API](#api)
   * [Staying up to date](#staying-up-to-date)
   * [Requirements](#requirements)
@@ -59,39 +95,36 @@
 
 * The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
 
 * Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
 
 * If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
-The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g. the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>.
+
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
 
 Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
-Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
+Ultimately, this Cloud Run microservice ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
-* [python][python] >= 3.7
-* [pandas][pandas] >= 1.4.3
-* [numpy][numpy] >= 1.23.2
-* [requests][requests] >= 2.28.1
-* [beautifulsoup4][beautifulsoup4] >= 4.11.1
-* [iso3166][iso3166] >= 2.1.1
+* [python][python] >= 3.8
+* [iso3166][iso3166] >= 2.1.1 
 
 Installation
 ------------
 Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-updates --upgrade
@@ -100,21 +133,75 @@
 Installation from source:
 ```bash
 git clone -b master https://github.com/amckenna41/iso3166-updates.git
 cd iso3166_updates
 python3 setup.py install
 ```
 
-Usage
------
+Usage (iso3166-updates Python package)
+--------------------------------------
+Below are some examples of using the custom-built iso3166-updates Python package. 
+
 **Import package:**
 ```python
-import iso3166_updates as iso3166_updates
+import iso3166_updates as iso
+```
+
+**Get all listed changes/updates for all countries and years:**
+```python
+iso.updates.all
 ```
 
+**Get all listed ISO 3166-2 changes/updates for Andorra (AD):**
+```python
+iso.updates.AD
+```
+
+**Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY:**
+```python
+iso.updates["BA","DE","FR","HU","PY"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
+```python
+iso.updates.year("2012-2021")["IE"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015":**
+```python
+iso.updates.year(">2015")["TA"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
+```python
+iso.updates.year("<2010")["YE"]
+```
+Usage get_all_iso3166_updates.py script
+---------------------------------------
+Below are some examples of using the get_all_iso3166_updates.py script which is used to pull all the ISO 3166 updates
+from the various data sources.
+
+**Requirements:**
+* [python][python] >= 3.8
+* [iso3166-updates][iso3166-updates] >= 1.3.0
+* [pandas][pandas] >= 1.4.3
+* [numpy][numpy] >= 1.23.2
+* [requests][requests] >= 2.28.1
+* [beautifulsoup4][beautifulsoup4] >= 4.11.1
+* [iso3166][iso3166] >= 2.1.1
+* [google-auth][google-auth] >= 2.17.3
+* [google-cloud-storage][google-cloud-storage] >= 2.8.0
+* [google-api-python-client][google-api-python-client] >= 2.86.0
+* [emoji-country-flag][emoji-country-flag] == 1.3.0
+* [selenium][seleniumn] >= 4.10.0
+* [flask][flask] >= 2.3.2
+* [gunicorn][gunicorn] >= 21.2.0
+<!-- * [webdriver-manager][webdriver-manager] >= 3.8.6 -->
+<!-- * [lxml][lxml] >=  4.9.3 -->
+
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
   #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
@@ -124,26 +211,34 @@
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
   #                       Selected year/years, year ranges or year to check for updates greater
   #                       than or less than specified year
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
+  # -verbose, --verbose
+  #                       Set to 1 to print out progress of updates function, 0 will not print progress.
+  # -use_selenium, --use_selenium
+  #                       Gather all data for each country from its official page on the ISO website which 
+  #                       requires Python Selenium and chromedriver. If False then just use country data
+  #                       from its wiki page.
 ```
+**Get all the latest updates for all ISO 3166 countries**
+```bash
+./get_all_updates.sh 
 
-**Get all listed changes/updates for all countries and years which happens by default if no alpha-2 codes or years specified in input paramaters, export csv and json to folder "iso3166-updates", print progress via verbose flag:**
-```python
-iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1, verbose=1)
-#exported files: /iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
+'''
+--export_filename     Filename for exported JSON/CSVs files containing updates data (default="iso3166-updates.json").
+--export_folder       Folder name to store exported JSON/CSVs files containing updates data (default="test-iso3166-updates).
+'''
 ```
 
-**Get all listed ISO 3166-2 changes/updates for Andorra, export csv and json to folder "iso3166-updates":**
+**Import module:**
 ```python
-iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
+import get_all_iso3166_updates as iso3166_updates
 ```
 
 **Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```python
 iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0, verbose=1)
 #exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
@@ -167,27 +262,14 @@
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ```
-## Terminal/Command Line
-
-The software functions can also be run from the cmd/terminal interface, when the script is called the get_updates() function will be called. The script accepts the same parameter names as the get_updates() function.
-
-**Get all listed ISO 3166-2 changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose flag:** 
-```bash
-python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
-```
-
-**Get all listed ISO 3166-2 changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose flag:**
-```bash
-python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
-```
 
 The output to the above functions for the updates/changes to an ISO 3166-2 country returns 4 columns: 
 <b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
 * Edition/Newsletter: Name and or edition of newsletter that the ISO 3166-2 change/update was communicated in.
 * Date Issued: Date that the change was communicated.
 * Code/Subdivision change: Overall summary of change/update made.
@@ -230,41 +312,54 @@
 Directories
 -----------
 * `/docs` - documentation for `iso3166-updates` Python package.
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
 * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
 * `/tests` - unit and integration tests for `iso3166-updates`.
+* `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
+* `get_all_iso3166-updates.sh` - shell script created to call the get_all..py script to introduce some pseudo randomness required when using Python Selenium. 
 
 Issues
 ------
-Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
+Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository.
 
 Contact
 -------
 If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
 
 References
 ----------
-\[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
-\[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
+\[1\]: ISO 3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
+\[2\]: ISO 3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
 \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
 \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
-\[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
-\[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
+\[5\]: ISO 3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
+\[6\]: ISO 3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
 
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
 [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [python]: https://www.python.org/downloads/release/python-360/
+[iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
+[google-auth]: https://cloud.google.com/python/docs/reference
+[google-cloud-storage]: https://cloud.google.com/python/docs/reference
+[google-api-python-client]: https://cloud.google.com/python/docs/reference
+[flask]: https://flask.palletsprojects.com/en/2.3.x/
+[emoji-country-flag]: https://pypi.org/project/emoji-country-flag/
+[gunicorn]: https://pypi.org/project/gunicorn/
+[selenium]: https://selenium-python.readthedocs.io/index.html
+[webdriver-manager]: https://pypi.org/project/webdriver-manager/
+[lxml]: https://lxml.de/
 [iso3166]: https://github.com/deactivated/python-iso3166
 [PyPi]: https://pypi.org/project/iso3166-updates/
-[Issues]: https://github.com/amckenna41/iso3166-updates/issues
+[Issues]: https://github.com/amckenna41/iso3166-updates/issues
+
```

### Comparing `iso3166-updates-1.3.1/iso3166_updates.egg-info/PKG-INFO` & `iso3166-updates-1.4.0/iso3166_updates.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.3.1
+Version: 1.4.0
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -33,27 +33,28 @@
 Provides-Extra: docs
 License-File: LICENSE
 
 # iso3166-updates
 
 [![iso3166_updates](https://img.shields.io/pypi/v/iso3166-updates)](https://pypi.org/project/iso3166-updates/)
 [![pytest](https://github.com/amckenna41/iso3166-updates/workflows/Building%20and%20Testing/badge.svg)](https://github.com/amckenna41/iso3166-updates/actions?query=workflowBuilding%20and%20Testing)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/amckenna41/iso3166-updates/tree/main.svg?style=svg&circle-token=9b0c0a9f6cc032f255dc28842c95600401aa4426)](https://dl.circleci.com/status-badge/redirect/gh/amckenna41/iso3166-updates/tree/main)
 [![Platforms](https://img.shields.io/badge/platforms-linux%2C%20macOS%2C%20Windows-green)](https://pypi.org/project/iso3166-updates/)
+<!-- [![codecov](https://codecov.io/gh/amckenna41/iso3166-updates/branch/main/graph/badge.svg?token=XOBSBVH8XA)](https://codecov.io/gh/amckenna41/iso3166-updates) -->
 [![License: MIT](https://img.shields.io/github/license/amckenna41/iso3166-updates)](https://opensource.org/licenses/MIT)
-<!-- [![CircleCI](https://circleci.com/gh/amckenna41/iso3166-updates.svg?style=svg&circle-token=d860bb64668be19d44f106841b80eb47a8b7e7e8)](https://app.circleci.com/pipelines/github/amckenna41/iso3166-updates) -->
 [![Issues](https://img.shields.io/github/issues/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates/issues)
-[![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates)
+<!-- [![Size](https://img.shields.io/github/repo-size/amckenna41/iso3166-updates)](https://github.com/amckenna41/iso3166-updates) -->
 <!-- [![Commits](https://img.shields.io/github/commit-activity/w/amckenna41/iso3166-updates)](https://github.com/iso3166-updates) -->
 
 <div alt="images" style="justify-content: center; display:flex; margin-left=50px;">
   <img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Flag-map_of_the_world_%282017%29.png" alt="globe" height="200" width="500"/>
   <img src="https://upload.wikimedia.org/wikipedia/commons/e/e3/ISO_Logo_%28Red_square%29.svg" alt="iso" height="200" width="300"/>
 </div>
 
-> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
+> Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a lightweight Python software package and API; a demo of both is available [here][demo].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
   * [API](#api)
   * [Staying up to date](#staying-up-to-date)
   * [Requirements](#requirements)
@@ -94,39 +95,36 @@
 
 * The year parameter can be a specific year, year range, or a cut-off year to get updates less than/more than a year (e.g "/year/2017", "2010-2015", "<2009", ">2002"). 
 
 * Finally, the months parameter will gather all updates for 1 or more alpha-2 codes from a number of months from the present day (e.g "?months=2", "/months/6", "/months/48").
 
 * If no input parameter values specified then all ISO 3166-2 updates for all countries and years will be gotten.
 
-The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure the hosting was switched to Vercel (https://vercel.com/).
+The API was hosted and built using GCP, with a Cloud Function being used in the backend which is fronted by an api gateway and load balancer. The function calls a GCP Storage bucket to access the back-end JSON where all ISO 3166 updates are stored. A complete diagram of the architecture is shown below. Although, due to the cost of infrastructure, the hosting was switched to Vercel (https://vercel.com/).
 
 The API documentation and usage with all useful commands and examples to the API is available on the [README](https://github.com/amckenna41/iso3166-updates/blob/main/iso3166-updates-api/README.md) of the iso3166-updates-api folder. 
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/amckenna41/iso3166-updates/main/iso3166-updates-api/gcp_arch.png" alt="gcp_arch" height="200" width="400"/>
 </p>
 
 Staying up to date
 ------------------
-The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>. 
-The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Function ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The function uses the `iso3166-updates` Python software to pull all the latest updates/changes from all ISO 3166-2 wiki's to check for the latest updates within a certain period e.g. the past 3-6 months. The function compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data.
+The list of ISO 3166-2 updates was last updated on <strong>Nov 2022</strong>.
+
+The object storing all updates, both locally (iso3166-updates.json) and on the API, are consistenly checked for the latest updates using a Google Cloud Run microservice ([iso3166-check-for-updates](https://github.com/amckenna41/iso3166-updates/tree/main/iso3166-check-for-updates)). The application is built using a custom Docker container that uses the `iso3166-updates` Python software to pull all the latest updates/changes, from all ISO 3166-2 wiki's and each country's ISO website page, to check for the latest updates within a certain period e.g. the past 3-6 months. The app compares the generated output with that of the updates json currently in the Google Cloud Storage bucket and will replace this json to integrate the latest updates found such that the API will have the most up-to-date data. A Cloud Scheduler is used to periodically call the application.
 
 Additionally, a GitHub Issue in the custom-built `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` repositories will be automatically created that outlines all updates/changes that need to be implemented into the `iso3166-updates`, `iso3166-2` and `iso3166-flag-icons` JSONs and repos.
 
-Ultimately, this Cloud Function ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
+Ultimately, this Cloud Run microservice ensures that the software and assoicated APIs are up-to-date with the latest ISO 3166-2 information for all countries/territories/subdivisions etc.
 
 Requirements
 ------------
-* [python][python] >= 3.7
-* [pandas][pandas] >= 1.4.3
-* [numpy][numpy] >= 1.23.2
-* [requests][requests] >= 2.28.1
-* [beautifulsoup4][beautifulsoup4] >= 4.11.1
-* [iso3166][iso3166] >= 2.1.1
+* [python][python] >= 3.8
+* [iso3166][iso3166] >= 2.1.1 
 
 Installation
 ------------
 Install the latest version of `iso3166-updates` via [PyPi][PyPi] using pip:
 
 ```bash
 pip3 install iso3166-updates --upgrade
@@ -135,21 +133,75 @@
 Installation from source:
 ```bash
 git clone -b master https://github.com/amckenna41/iso3166-updates.git
 cd iso3166_updates
 python3 setup.py install
 ```
 
-Usage
------
+Usage (iso3166-updates Python package)
+--------------------------------------
+Below are some examples of using the custom-built iso3166-updates Python package. 
+
 **Import package:**
 ```python
-import iso3166_updates as iso3166_updates
+import iso3166_updates as iso
+```
+
+**Get all listed changes/updates for all countries and years:**
+```python
+iso.updates.all
 ```
 
+**Get all listed ISO 3166-2 changes/updates for Andorra (AD):**
+```python
+iso.updates.AD
+```
+
+**Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY:**
+```python
+iso.updates["BA","DE","FR","HU","PY"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Ireland, between years 2012 and 2021:**
+```python
+iso.updates.year("2012-2021")["IE"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Tanzania, with updates with year >=2015":**
+```python
+iso.updates.year(">2015")["TA"]
+```
+
+**Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010:**
+```python
+iso.updates.year("<2010")["YE"]
+```
+Usage get_all_iso3166_updates.py script
+---------------------------------------
+Below are some examples of using the get_all_iso3166_updates.py script which is used to pull all the ISO 3166 updates
+from the various data sources.
+
+**Requirements:**
+* [python][python] >= 3.8
+* [iso3166-updates][iso3166-updates] >= 1.3.0
+* [pandas][pandas] >= 1.4.3
+* [numpy][numpy] >= 1.23.2
+* [requests][requests] >= 2.28.1
+* [beautifulsoup4][beautifulsoup4] >= 4.11.1
+* [iso3166][iso3166] >= 2.1.1
+* [google-auth][google-auth] >= 2.17.3
+* [google-cloud-storage][google-cloud-storage] >= 2.8.0
+* [google-api-python-client][google-api-python-client] >= 2.86.0
+* [emoji-country-flag][emoji-country-flag] == 1.3.0
+* [selenium][seleniumn] >= 4.10.0
+* [flask][flask] >= 2.3.2
+* [gunicorn][gunicorn] >= 21.2.0
+<!-- * [webdriver-manager][webdriver-manager] >= 3.8.6 -->
+<!-- * [lxml][lxml] >=  4.9.3 -->
+
 **Input parameters to get_updates function:**
 ```python
   # -alpha2 ALPHA2, --alpha2 ALPHA2
   #                       Alpha-2 code/s of ISO 3166 countries to check for updates.
   # -export_filename EXPORT_FILENAME, --export_filename EXPORT_FILENAME
   #                       Filename for exported ISO 3166 updates for CSV and JSON files.
   # -export_folder EXPORT_FOLDER, --export_folder EXPORT_FOLDER
@@ -159,26 +211,34 @@
   # -export_csv, --export_csv
   #                       Whether to export all found updates to csv files in export folder.
   # -year YEAR, --year YEAR
   #                       Selected year/years, year ranges or year to check for updates greater
   #                       than or less than specified year
   # -concat_updates, --concat_updates
   #                       Whether to concatenate updates of individual countrys into the same json file or seperate.
+  # -verbose, --verbose
+  #                       Set to 1 to print out progress of updates function, 0 will not print progress.
+  # -use_selenium, --use_selenium
+  #                       Gather all data for each country from its official page on the ISO website which 
+  #                       requires Python Selenium and chromedriver. If False then just use country data
+  #                       from its wiki page.
 ```
+**Get all the latest updates for all ISO 3166 countries**
+```bash
+./get_all_updates.sh 
 
-**Get all listed changes/updates for all countries and years which happens by default if no alpha-2 codes or years specified in input paramaters, export csv and json to folder "iso3166-updates", print progress via verbose flag:**
-```python
-iso3166_updates.get_updates(export_folder="iso3166-updates", export_json=1, export_csv=1, verbose=1)
-#exported files: /iso3166-updates.json and /iso3166-updates/iso3166-updates.csv
+'''
+--export_filename     Filename for exported JSON/CSVs files containing updates data (default="iso3166-updates.json").
+--export_folder       Folder name to store exported JSON/CSVs files containing updates data (default="test-iso3166-updates).
+'''
 ```
 
-**Get all listed ISO 3166-2 changes/updates for Andorra, export csv and json to folder "iso3166-updates":**
+**Import module:**
 ```python
-iso3166_updates.get_updates("AD", export_folder="iso3166-updates", export_json=1, export_csv=1)
-#exported files: /iso3166-updates-AD.json and /iso3166-updates/iso3166-updates-AD.csv
+import get_all_iso3166_updates as iso3166_updates
 ```
 
 **Get all listed ISO 3166-2 changes/updates for BA, DE, FR, HU, PY, export only JSON of updates to export folder "iso3166-updates", print progress using verbose flag:**
 ```python
 iso3166_updates.get_updates(["BA","DE","FR","HU","PY"], export_folder="iso3166-updates", export_json=1, export_csv=0, verbose=1)
 #exported files: /iso3166-updates/iso3166-updates-BA,DE,FR,HU,PY.json
 ```
@@ -202,27 +262,14 @@
 ```
 
 **Get any listed ISO 3166-2 changes/updates for Yemen, with updates with year < 2010, use default parameters (export to json but not csv):**
 ```python
 iso3166_updates.get_updates("YE", year="<2010")
 #exported files: /iso3166-updates/iso3166-output-YE_<2010.json
 ```
-## Terminal/Command Line
-
-The software functions can also be run from the cmd/terminal interface, when the script is called the get_updates() function will be called. The script accepts the same parameter names as the get_updates() function.
-
-**Get all listed ISO 3166-2 changes/updates for all countries, export csv and json to folder "iso3166-updates", print progress using verbose flag:** 
-```bash
-python3 iso3166_updates.py --export_folder="iso3166-updates" --export_csv --export_json --verbose
-```
-
-**Get all listed ISO 3166-2 changes/updates for BY, DJ, ET, LY, PA for year range 2005-2010, export only CSV of updates to export folder "iso3166-updates", print progress using verbose flag:**
-```bash
-python3 iso3166_updates.py --alpha2="BY, DJ, ET, LY, PA" --year="2005-2010" --export_folder="iso3166-updates" --export_csv --no-export_json --verbose
-```
 
 The output to the above functions for the updates/changes to an ISO 3166-2 country returns 4 columns: 
 <b>Edition/Newsletter, Date Issued, Code/Subdivision change</b> and <b>Description of change in newsletter.</b> For the CSV export, if more than one country input, then an additional primary key column <b>Country Code</b> will be prepended to the first column, which will be the 2 letter ISO 3166-1 country code. 
 
 * Edition/Newsletter: Name and or edition of newsletter that the ISO 3166-2 change/update was communicated in.
 * Date Issued: Date that the change was communicated.
 * Code/Subdivision change: Overall summary of change/update made.
@@ -265,42 +312,54 @@
 Directories
 -----------
 * `/docs` - documentation for `iso3166-updates` Python package.
 * `/iso3166_updates` - source code for `iso3166-updates` Python package.
 * `/iso3166-updates-api` - all code and files related to the serverless Google Cloud Function for the `iso3166-updates` API, including the main.py, requirements.txt and API config file.
 * `/iso3166-check-for-updates` - all code and files related to the serverless Google Cloud Function for the check-for-updates function which is a periodically called Cloud Function that uses the Python software to check for the latest updates for all country's, ensuring the API and jsons are reliable and up-to-date. Includes the main.py and requirements.txt files.
 * `/tests` - unit and integration tests for `iso3166-updates`.
+* `get_all_iso3166_updates.py` - python module that pulls and exports all the latest ISO 3166 data from the various data sources.
+* `get_all_iso3166-updates.sh` - shell script created to call the get_all..py script to introduce some pseudo randomness required when using Python Selenium. 
 
 Issues
 ------
-Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository. Also if there are any missing or incorrect data in the updates json, this should also be raised by creating an issue. 
+Any issues, errors or bugs can be raised via the [Issues](Issues) tab in the repository.
 
 Contact
 -------
 If you have any questions or comments, please contact amckenna41@qub.ac.uk or raise an issue on the [Issues][Issues] tab. <br><br>
 [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adam-mckenna-7a5b22151/)
 
 References
 ----------
-\[1\]: ISO3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
-\[2\]: ISO3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
+\[1\]: ISO 3166-1: https://en.wikipedia.org/wiki/ISO_3166-1 <br>
+\[2\]: ISO 3166-2: https://en.wikipedia.org/wiki/ISO_3166-2 <br>
 \[3\]: ISO Country Codes Collection: https://www.iso.org/publication/PUB500001 <br>
 \[4\]: ISO Country Codes: https://www.iso.org/iso-3166-country-codes.html <br>
-\[5\]: ISO3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
-\[6\]: ISO3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
+\[5\]: ISO 3166-1 flag-icons repo: https://github.com/lipis/flag-icons <br>
+\[6\]: ISO 3166-2 flag-icons repo: https://github.com/amckenna41/iso3166-flag-icons <br>
 
 Support
 -------
 <a href="https://www.buymeacoffee.com/amckenna41" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 [Back to top](#TOP)
 
 [demo]: https://colab.research.google.com/drive/1oGF3j3_9b_g2qAmBtv3n-xO2GzTYRJjf?usp=sharing
 [python]: https://www.python.org/downloads/release/python-360/
+[iso3166-updates]: https://github.com/amckenna41/iso3166-updates
 [pandas]: https://pandas.pydata.org/
 [numpy]: https://numpy.org/
 [requests]: https://requests.readthedocs.io/
 [beautifulsoup4]: https://www.crummy.com/software/BeautifulSoup/bs4/doc/
+[google-auth]: https://cloud.google.com/python/docs/reference
+[google-cloud-storage]: https://cloud.google.com/python/docs/reference
+[google-api-python-client]: https://cloud.google.com/python/docs/reference
+[flask]: https://flask.palletsprojects.com/en/2.3.x/
+[emoji-country-flag]: https://pypi.org/project/emoji-country-flag/
+[gunicorn]: https://pypi.org/project/gunicorn/
+[selenium]: https://selenium-python.readthedocs.io/index.html
+[webdriver-manager]: https://pypi.org/project/webdriver-manager/
+[lxml]: https://lxml.de/
 [iso3166]: https://github.com/deactivated/python-iso3166
 [PyPi]: https://pypi.org/project/iso3166-updates/
 [Issues]: https://github.com/amckenna41/iso3166-updates/issues
```

### Comparing `iso3166-updates-1.3.1/setup.cfg` & `iso3166-updates-1.4.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-updates
-version = 1.3.1
+version = 1.4.0
 description = A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 url = https://github.com/amckenna41/iso3166-updates
 download_url = https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -19,14 +19,16 @@
 	countries
 	country codes
 	csv
 	iso3166-2
 	iso3166-1
 	alpha2
 	alpha3
+	selenium
+	chromedriver
 classifiers = 
 	Development Status :: 3 - Alpha,
 	Environment :: Console,
 	Intended Audience :: Developers,
 	Intended Audience :: Science/Research,
 	Intended Audience :: Information Technology,
 	License :: OSI Approved :: MIT License,
```

### Comparing `iso3166-updates-1.3.1/setup.py` & `iso3166-updates-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pathlib
 from setuptools import setup, find_packages
 import sys
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.3.1"
+__version__ = "1.4.0"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Development'
```

