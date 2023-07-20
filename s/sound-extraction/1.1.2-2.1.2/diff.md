# Comparing `tmp/sound-extraction-1.1.2.tar.gz` & `tmp/sound-extraction-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sound-extraction-1.1.2.tar", last modified: Mon Jun 19 20:04:09 2023, max compression
+gzip compressed data, was "dist\sound-extraction-2.1.2.tar", last modified: Thu Jul 20 13:02:59 2023, max compression
```

## Comparing `sound-extraction-1.1.2.tar` & `sound-extraction-2.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 20:04:09.809977 sound-extraction-1.1.2/
--rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     7109 2023-06-19 20:04:09.806985 sound-extraction-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6603 2023-06-19 19:59:46.000000 sound-extraction-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 20:04:09.809977 sound-extraction-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1131 2023-06-19 20:04:03.000000 sound-extraction-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:04:09.789434 sound-extraction-1.1.2/sound_extraction.egg-info/
--rw-rw-rw-   0        0        0     7109 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      153 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 20:04:09.804990 sound-extraction-1.1.2/src/
--rw-rw-rw-   0        0        0    18042 2023-06-19 20:03:52.000000 sound-extraction-1.1.2/src/sound_extraction.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:02:59.863448 sound-extraction-2.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-2.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     8537 2023-07-20 13:02:59.861407 sound-extraction-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8031 2023-07-20 12:50:30.000000 sound-extraction-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 13:02:59.864400 sound-extraction-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1334 2023-07-20 13:02:20.000000 sound-extraction-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:02:59.849439 sound-extraction-2.1.2/sound_extraction.egg-info/
+-rw-rw-rw-   0        0        0     8537 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      219 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-20 13:02:59.000000 sound-extraction-2.1.2/sound_extraction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 13:02:59.858418 sound-extraction-2.1.2/src/
+-rw-rw-rw-   0        0        0        0 2023-07-18 16:09:50.000000 sound-extraction-2.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0    10907 2023-07-19 20:33:31.000000 sound-extraction-2.1.2/src/recording_times_generator.py
+-rw-rw-rw-   0        0        0    18955 2023-07-20 12:53:44.000000 sound-extraction-2.1.2/src/sound_extraction.py
```

### Comparing `sound-extraction-1.1.2/LICENSE.txt` & `sound-extraction-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sound-extraction-1.1.2/PKG-INFO` & `sound-extraction-2.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,50 @@
-Metadata-Version: 2.1
-Name: sound-extraction
-Version: 1.1.2
-Home-page: https://github.com/prayagnshah/Sound-Extraction
-Author: Prayag Shah
-Author-email: prayagshah07@gmail.com
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Audio-File Extraction
 
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://pypi.org/project/sound-extraction/)
+
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
-## Types of Installation
+## Types of Installation and you only have to use *one* of them
 
 1. Download the python package:
     
     `pip install sound-extraction`
 
     a. After the installation you can use the following command to run the program or use `--help` to see the arguments list:
 
-    `sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
+    `sound_extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
 
-and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#Arguments) OR
+and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#arguments) OR
 
 2. If you want to run the program thorugh Docker then follow the steps below: [Docker](#using-dockerfile) OR
 
-3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup).
+3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup-windows).
 
 <b>Note: You can use any one of the installation above to run the program.</b>
 
 ## Using Dockerfile
 
 1. Download the Docker application: [Docker](https://www.docker.com/products/docker-desktop).
 
-2. Download `Dockerfile` and `requirements.txt` files: [Docker-File](https://github.com/prayagnshah/Sound-Extraction/blob/main/Dockerfile) and [Requirements](https://github.com/prayagnshah/Sound-Extraction/blob/main/requirements.txt).
+2. Open the terminal and make sure docker package is installed on your system. If not then run the following two commands:
+
+    `pip install docker`
+    `docker pull prayagshah/sound-extraction`
 
-3. Open the terminal and go to the directory where you have downloaded the `Dockerfile` and `requirements.txt` files. Run the following command:
+3. Once the docker is installed and the package is pulled then run the following command to run the program:
 
-    `docker build -t sound-extraction .`
     `docker run sound-extraction`
 
+4. After running the above command you will be asked to enter the arguments. Follow the instructions below to enter the arguments:
+
+    `docker run prayagshah/sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
+
 ## Setup (Windows)
 
 Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     venv\Scripts\Activate
     pip install -r requirements.txt
@@ -125,7 +119,23 @@
 2. Original files should be in the format `20220611T202300.wav` or `20220611T202300.flac`. Sample files in CSV should be in the format `20220611_202300.wav` or `20220611_202300.flac` under the heading `sampleFile`. For instance,
 
    ![Sample Image](data/image.png)
 
 ## Changelog
 
 1. All the version changes are mentioned in the [CHANGELOG.md](https://github.com/prayagnshah/Sound-Extraction/blob/main/CHANGELOG.md) file.
+
+## Contributing
+
+Contributions are welcomed and appreciated. Here are some ways to get involved:
+    * Submitting bug reports.
+    * Feature requests or suggestions.
+    * Improving the documentation or providing examples.
+    * Writing code to add optimizations or new features.
+
+Please use the [GitHub issue tracker](https://github.com/prayagnshah/Sound-Extraction/issues) to raise any bugs or to submit feature requests. If something does not work as you might expect, please let us know. If there are features that you feel are missing, please let us know.
+
+Code submissions should be submitted as a pull request.
+
+If you are stuck or need help, raising an issue is a good place to start. This helps us keep common issues in public view.
+
+Please note that we adhere to [code of conduct](https://github.com/prayagnshah/Sound-Extraction/blob/main/CODE_OF_CONDUCT.md)
```

### Comparing `sound-extraction-1.1.2/README.md` & `sound-extraction-2.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,64 @@
+Metadata-Version: 2.1
+Name: sound-extraction
+Version: 2.1.2
+Home-page: https://github.com/prayagnshah/Sound-Extraction
+Author: Prayag Shah
+Author-email: prayagshah07@gmail.com
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Audio-File Extraction
 
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://pypi.org/project/sound-extraction/)
+
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
-## Types of Installation
+## Types of Installation and you only have to use *one* of them
 
 1. Download the python package:
     
     `pip install sound-extraction`
 
     a. After the installation you can use the following command to run the program or use `--help` to see the arguments list:
 
-    `sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
+    `sound_extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
 
-and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#Arguments) OR
+and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#arguments) OR
 
 2. If you want to run the program thorugh Docker then follow the steps below: [Docker](#using-dockerfile) OR
 
-3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup).
+3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup-windows).
 
 <b>Note: You can use any one of the installation above to run the program.</b>
 
 ## Using Dockerfile
 
 1. Download the Docker application: [Docker](https://www.docker.com/products/docker-desktop).
 
-2. Download `Dockerfile` and `requirements.txt` files: [Docker-File](https://github.com/prayagnshah/Sound-Extraction/blob/main/Dockerfile) and [Requirements](https://github.com/prayagnshah/Sound-Extraction/blob/main/requirements.txt).
+2. Open the terminal and make sure docker package is installed on your system. If not then run the following two commands:
+
+    `pip install docker`
+    `docker pull prayagshah/sound-extraction`
 
-3. Open the terminal and go to the directory where you have downloaded the `Dockerfile` and `requirements.txt` files. Run the following command:
+3. Once the docker is installed and the package is pulled then run the following command to run the program:
 
-    `docker build -t sound-extraction .`
     `docker run sound-extraction`
 
+4. After running the above command you will be asked to enter the arguments. Follow the instructions below to enter the arguments:
+
+    `docker run prayagshah/sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
+
 ## Setup (Windows)
 
 Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     venv\Scripts\Activate
     pip install -r requirements.txt
@@ -111,7 +133,23 @@
 2. Original files should be in the format `20220611T202300.wav` or `20220611T202300.flac`. Sample files in CSV should be in the format `20220611_202300.wav` or `20220611_202300.flac` under the heading `sampleFile`. For instance,
 
    ![Sample Image](data/image.png)
 
 ## Changelog
 
 1. All the version changes are mentioned in the [CHANGELOG.md](https://github.com/prayagnshah/Sound-Extraction/blob/main/CHANGELOG.md) file.
+
+## Contributing
+
+Contributions are welcomed and appreciated. Here are some ways to get involved:
+    * Submitting bug reports.
+    * Feature requests or suggestions.
+    * Improving the documentation or providing examples.
+    * Writing code to add optimizations or new features.
+
+Please use the [GitHub issue tracker](https://github.com/prayagnshah/Sound-Extraction/issues) to raise any bugs or to submit feature requests. If something does not work as you might expect, please let us know. If there are features that you feel are missing, please let us know.
+
+Code submissions should be submitted as a pull request.
+
+If you are stuck or need help, raising an issue is a good place to start. This helps us keep common issues in public view.
+
+Please note that we adhere to [code of conduct](https://github.com/prayagnshah/Sound-Extraction/blob/main/CODE_OF_CONDUCT.md)
```

### Comparing `sound-extraction-1.1.2/setup.py` & `sound-extraction-2.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sound-extraction",
-    version="1.1.2",
+    version="2.1.2",
     packages=["src"],
     install_requires=[
         "certifi==2023.5.7",
         "cffi==1.15.1",
         "load-dotenv==0.1.0",
         "numpy==1.24.3",
         "pycparser==2.21",
         "python-dotenv==1.0.0",
         "sentry-sdk==1.25.1",
         "soundfile==0.12.1",
         "urllib3==2.0.3",
+        "astral==3.2",
+        "backports.zoneinfo==0.2.1",
+        "pytz==2023.3",
+        "tzdata==2023.3",
+        
     ],
     entry_points={
         "console_scripts": [
-            "sound-extraction = src.sound_extraction:main",
+            "sound_extraction = src.sound_extraction:main",
+            "recording_times_generator = src.recording_times_generator:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
```

### Comparing `sound-extraction-1.1.2/sound_extraction.egg-info/PKG-INFO` & `sound-extraction-2.1.2/sound_extraction.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 Metadata-Version: 2.1
 Name: sound-extraction
-Version: 1.1.2
+Version: 2.1.2
 Home-page: https://github.com/prayagnshah/Sound-Extraction
 Author: Prayag Shah
 Author-email: prayagshah07@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Audio-File Extraction
 
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/pypromice.svg)](https://pypi.org/project/sound-extraction/)
+
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
-## Types of Installation
+## Types of Installation and you only have to use *one* of them
 
 1. Download the python package:
     
     `pip install sound-extraction`
 
     a. After the installation you can use the following command to run the program or use `--help` to see the arguments list:
 
-    `sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
+    `sound_extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
 
-and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#Arguments) OR
+and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#arguments) OR
 
 2. If you want to run the program thorugh Docker then follow the steps below: [Docker](#using-dockerfile) OR
 
-3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup).
+3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup-windows).
 
 <b>Note: You can use any one of the installation above to run the program.</b>
 
 ## Using Dockerfile
 
 1. Download the Docker application: [Docker](https://www.docker.com/products/docker-desktop).
 
-2. Download `Dockerfile` and `requirements.txt` files: [Docker-File](https://github.com/prayagnshah/Sound-Extraction/blob/main/Dockerfile) and [Requirements](https://github.com/prayagnshah/Sound-Extraction/blob/main/requirements.txt).
+2. Open the terminal and make sure docker package is installed on your system. If not then run the following two commands:
+
+    `pip install docker`
+    `docker pull prayagshah/sound-extraction`
 
-3. Open the terminal and go to the directory where you have downloaded the `Dockerfile` and `requirements.txt` files. Run the following command:
+3. Once the docker is installed and the package is pulled then run the following command to run the program:
 
-    `docker build -t sound-extraction .`
     `docker run sound-extraction`
 
+4. After running the above command you will be asked to enter the arguments. Follow the instructions below to enter the arguments:
+
+    `docker run prayagshah/sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
+
 ## Setup (Windows)
 
 Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     venv\Scripts\Activate
     pip install -r requirements.txt
@@ -125,7 +133,23 @@
 2. Original files should be in the format `20220611T202300.wav` or `20220611T202300.flac`. Sample files in CSV should be in the format `20220611_202300.wav` or `20220611_202300.flac` under the heading `sampleFile`. For instance,
 
    ![Sample Image](data/image.png)
 
 ## Changelog
 
 1. All the version changes are mentioned in the [CHANGELOG.md](https://github.com/prayagnshah/Sound-Extraction/blob/main/CHANGELOG.md) file.
+
+## Contributing
+
+Contributions are welcomed and appreciated. Here are some ways to get involved:
+    * Submitting bug reports.
+    * Feature requests or suggestions.
+    * Improving the documentation or providing examples.
+    * Writing code to add optimizations or new features.
+
+Please use the [GitHub issue tracker](https://github.com/prayagnshah/Sound-Extraction/issues) to raise any bugs or to submit feature requests. If something does not work as you might expect, please let us know. If there are features that you feel are missing, please let us know.
+
+Code submissions should be submitted as a pull request.
+
+If you are stuck or need help, raising an issue is a good place to start. This helps us keep common issues in public view.
+
+Please note that we adhere to [code of conduct](https://github.com/prayagnshah/Sound-Extraction/blob/main/CODE_OF_CONDUCT.md)
```

### Comparing `sound-extraction-1.1.2/src/sound_extraction.py` & `sound-extraction-2.1.2/src/sound_extraction.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 load_dotenv()
 
 # Get the sentry DSN from the environment variables
 sentry_dsn = os.getenv("sentry_dsn")
 
 sentry_sdk.init(
     dsn=sentry_dsn,
-    release="v1.1.2",
+    release="v2.1.2",
     # Set traces_sample_rate to 1.0 to capture 100%
     # of transactions for performance monitoring.
     traces_sample_rate=1.0,
 )
 
-
 def main():
     def get_directories(root_directory):
         """
         Getting the directories and files from the root directory
         logging messages if no files or no extension files are found
         """
         all_files = []
@@ -46,110 +45,124 @@
             if ext_found:
                 directory.append(root)
 
         return directory, all_files
 
     def read_csv_file(csv_file_path, sampleFile, categories_col):
         """
-        Reads data from a CSV file and filters it based on a column name which has sample audio files and categories column
+        Reads data from a CSV file and filters it based on a column name which has sample audio files and categories column. It returns sample recordings and
+        a dictionary with sample recordings as keys and categories as values.
+
+        Args:
+            csv_file_path (str): The path to the CSV file to be read.
+            sampleFile (str): The name of the column containing sample audio files.
+            categories_col (str): The name of the column containing categories.
+
+        Returns:
+            tuple: A tuple containing two elements:
+                - list: A list of sample recordings.
+                - dict: A dictionary with sample recordings as keys and categories as values.
+
+        Steps:
+            1. Open the CSV file and read its content.
+            2. Find the indices of the sampleFile and categories_col columns.
+            3. Extract the relevant data from the CSV file.
+            4. Create a dictionary with sample recordings as keys and categories as values.
         """
         with open(csv_file_path, "r") as files:
             csv_reader = csv.reader(files)
 
             header = next(csv_reader)
 
             sampleFile_index = header.index(sampleFile)
 
-            # Checking if the categories column is present in the CSV file
-
             categories_bool = False
             if categories_col not in header:
                 logging.info(
                     "Categories column not found in CSV file, so there is no folder named Nocturnal, Daytime, etc."
                 )
 
                 categories_bool = True
 
             else:
                 categories_index = header.index(categories_col)
 
-            # storing the values in list so that it can be used once the file is closed
-
             rows = list(csv_reader)
 
-        # Filtering the sample recordings
-
         sample_recordings = [row[sampleFile_index] for row in rows]
 
-        # Checking if no column present then it will be empty string
-
         if categories_bool:
             categories = ["" for row in rows]
 
         else:
             categories = [row[categories_index] for row in rows]
 
-        # Creating a dictionary with sample recordings as keys and categories as values
-
         categories_dict = {k: v for k, v in zip(sample_recordings, categories)}
 
         return sample_recordings, categories_dict
 
     def process_recordings(all_files, sample_recordings):
-        # Filtering in actual recordings
+        """
+            Processes long recordings and matches them with the corresponding sample
+            recordings based on their timestamps. Returns a dictionary with long
+            recordings as keys and lists of associated sample recordings as values.
+
+        Args:
+            all_files (list): A list of all long recordings files.
+            sample_recordings (list): A list of sample recordings files.
+
+        Returns:
+            dict: A dictionary with long recordings as keys and lists of associated
+                    sample recordings as values.
+
+        Steps:
+            1. Filter and sort long recordings.
+            2. Iterate through long recordings and create a dictionary to store the
+                associated sample recordings.
+            3. Check if a sample recording falls within a long recording's time frame.
+            4. Filter the dictionary to remove empty lists and format the keys.
+        """
 
         long_recordings = [file for file in all_files if "T" in file]
 
         long_recordings.sort()
         recordings_dict = {}
 
         for long_recording in long_recordings:
-            # Splitting the .flac extension from the filename so datetime can be parsed
-
             filename, extension = os.path.splitext(long_recording)
 
-            # Get the start and end datetime of the long recording
             # Putting try and except handling because there will be backup file with .flac and we need to avoid it
 
             long_start_datetime = datetime.datetime.strptime(filename, "%Y%m%dT%H%M%S")
 
-            # Getting the duration of the recording by checking the next long recording's start time and if there is one then,
-
             try:
                 next_long_recording = long_recordings[
                     long_recordings.index(long_recording) + 1
                 ]
                 next_filename, next_extension = os.path.splitext(next_long_recording)
 
                 duration = (
                     datetime.datetime.strptime(next_filename, "%Y%m%dT%H%M%S")
                     - long_start_datetime
                 )
 
-            # Assuming the last recording of 3 hours
-
             except IndexError:
                 duration = datetime.timedelta(hours=3)
 
             long_end_datetime = long_start_datetime + duration
 
             # Create an empty list to hold sample recordings that fall within this long recording's time frame
 
             recordings_dict[long_start_datetime] = []
 
-            # Using if condition to check that sample recording falls into long recording
-            # Finally producing the output: sample_recording
-
             for sample_recording in sample_recordings:
                 file, ext = os.path.splitext(sample_recording)
 
-                # Get the datetime of the sample recording
                 sample_datetime = datetime.datetime.strptime(file, "%Y%m%d_%H%M%S")
 
-                # Check if the sample recording falls within the current long recording's time frame
                 if long_start_datetime <= sample_datetime <= long_end_datetime:
                     recordings_dict[long_start_datetime].append(sample_recording)
 
         # Storing the user input for the extension
 
         extension = args.extension
 
@@ -171,93 +184,84 @@
         user_input = input("Enter the subdirectory name: ")
 
         return f"{user_input}"
 
     def extract_audio_segments(
         filtered_recordings_dict, output_directory, site_name, categories_dict
     ):
-        # Generating the subdirectory name
+        """
+        This function extracts audio segments from a dictionary of filtered recordings
+        and saves them into a specified output directory. If flag -span is used
+
+        Args:
+            filtered_recordings_dict (dict): A dictionary of filtered audio recordings.
+            output_directory (str): The directory path where extracted segments will be saved.
+            site_name (str): The name of the site where the recordings were taken.
+            categories_dict (dict): A dictionary containing the categories of recordings.
+
+        Steps:
+            1. Generate the subdirectory name for the output directory.
+            2. Create the output subdirectory.
+            3. Set the duration of the audio segments to be extracted.
+            4. Get the directories and files within the root directory.
+            5. Loop through each directory and extract the audio segments.
+        """
+
         subdir_name = generate_subdir_name()
 
-        # Creating the subdirectory
         output_subdirectory = os.path.join(output_directory, subdir_name)
         os.makedirs(output_subdirectory, exist_ok=True)
 
-        # Set the duration for the portion of the audio file to extract
-
         duration = datetime.timedelta(minutes=args.duration)
 
-        # Calling the function to get the directories
-
         directories, all_files = get_directories(root_directory)
 
         for directory in directories:
-            # Calling the function to get the original audio files
-
             recording_keys = sorted(os.listdir(directory))
 
-            # Looping through each key-value pair
-
             for key, value in filtered_recordings_dict.items():
-                # Checking if the key is in the original audio files
-
                 if key not in recording_keys:
                     continue
 
                 # Trying to put in the exception handler if corrupted audio file comes up then it prints in the console and it will still continue the code instead of breaking up
 
                 try:
                     # Loading the original audio recording file while samplefile produces array and samplerate together
 
                     audio_file, samplerate = sf.read(os.path.join(directory, key))
 
                 except Exception as e:
                     logging.error(f"Error reading audio file {key}: {e}")
                     continue
 
-                # Splitting the key values into datetime
-
                 split_key = os.path.splitext(key)[0]
-                # Getting the start time of the audio file from the actual recordings
 
                 start_time_parent = datetime.datetime.strptime(
                     split_key, "%Y%m%dT%H%M%S"
                 )
 
-                # Loop through each specified snippet in the value
-
                 for snippet in value:
                     start_time_str = os.path.splitext(snippet)[0]
 
-                    # Extract the start and end time for the snippet and parsing string as datetime object
-
                     start_time = datetime.datetime.strptime(
                         start_time_str, "%Y%m%d_%H%M%S"
                     )
 
-                    # Getting the actual start time of the snippet in the audio file
-
                     snippet_start_time = start_time - start_time_parent
 
-                    # Calculate the start and end frame indices for the portion of the audio file to extract into seconds
-
                     start_frame = int(snippet_start_time.total_seconds() * samplerate)
                     end_frame = int(
                         (snippet_start_time + duration).total_seconds() * samplerate
                     )
 
-                    # Checking the index of the current key
-
                     current_key_index = recording_keys.index(key)
 
                     # Due to the fact that the audio files are not of 3 mins duration so we need to check if the duration is less than 3 mins then we need to add the next audio file to it
 
                     if current_key_index + 1 < len(recording_keys):
-                        # Setting the duration of the snippet
-
                         duration_new = datetime.timedelta(minutes=args.duration)
 
                         next_key = recording_keys[current_key_index + 1]
 
                         # Adding error handling for the next key if it is corrupted
 
                         try:
@@ -267,150 +271,149 @@
                         except ValueError:
                             logging.error(
                                 f"Error parsing next key {next_key} for snippet {snippet}"
                             )
                             continue
 
                         # Checking if the duration of the snippet is greater than the next key's start time and flag "-span" is used then it won't concatenate the audio files
-                        # It will calculate the exact duration of the files and then it will concatenate
 
                         if (
                             not args.span
                             and start_time + duration_new > next_key_start_time
                         ):
                             parent_duration_time = len(audio_file) / samplerate
                             time_duration_second = (
                                 parent_duration_time
                                 - snippet_start_time.total_seconds()
                             )
                             time_duration = datetime.timedelta(
                                 seconds=time_duration_second
                             )
 
-                            # Loading the next audio file
-
                             next_audio_file, next_samplerate = sf.read(
                                 os.path.join(directory, next_key)
                             )
 
-                            # Getting the remaining duration of the snippet
-
                             remaining_duration = duration_new - time_duration
 
-                            # Getting the remaining audio from the next audio file
-
                             remaining_audio = next_audio_file[
                                 : int(
                                     remaining_duration.total_seconds() * next_samplerate
                                 )
                                 + 1
                             ]
 
-                            # Concatenating the audio files
-
                             snippet_data = np.concatenate(
                                 (audio_file[start_frame:], remaining_audio)
                             )
 
                         else:
                             snippet_data = audio_file[start_frame:end_frame]
 
                     else:
                         # Extract the portion of the audio data using numpy array indexing because soundfile data comes in integers
 
                         snippet_data = audio_file[start_frame:end_frame]
 
-                    # Storing the user input for the extension
-
                     extension = args.extension
 
-                    # Write the extracted audio data to a new file
-
                     output_filename = os.path.splitext(snippet)[0] + extension
 
                     # Creating the subdirectory for the categories
 
                     os.makedirs(
                         os.path.join(output_subdirectory, categories_dict[snippet]),
                         exist_ok=True,
                     )
 
-                    # Writing the new audio of 3 mins to the desired directory
-
                     export_segment = sf.write(
                         os.path.join(
                             output_subdirectory,
                             categories_dict[snippet],
                             site_name + output_filename,
                         ),
                         snippet_data,
                         samplerate,
                     )
 
         return export_segment, output_subdirectory
 
     def process_audio_files(directory, slice_duration, output_directory):
-        # Generating the subdirectory name
+        """
+            This function processes audio files in the given directory by slicing them
+            into smaller segments of a specified duration of seconds set by user and saves them into a specified
+            output directory.
+
+        Args:
+            directory (str): The directory containing the audio files to be processed.
+            slice_duration (float): The duration of each sliced segment in seconds.
+            output_directory (str): The directory path where sliced segments will be saved.
+
+        Steps:
+            1. Generate the subdirectory name for the output directory.
+            2. Create the output subdirectory.
+            3. Traverse the directory and process each audio file.
+        """
+
         subdir_name = generate_subdir_name()
 
-        # Creating the subdirectory
         output_subdirectory = os.path.join(output_directory, subdir_name)
         os.makedirs(output_subdirectory, exist_ok=True)
 
-        # Traversing the directories and files in the directory
-
         for root, dirs, files in os.walk(directory):
-            # Looping the files of that directory
-
             for file in files:
                 file_str = os.path.splitext(file)[0]
-                file_datetime = datetime.datetime.strptime(file_str, "%Y%m%dT%H%M%S")
-
-                audio, sample_rate = sf.read(os.path.join(root, file))
+                
+                try:
+                    file_datetime = datetime.datetime.strptime(file_str, "%Y%m%dT%H%M%S")
+                
+                except ValueError:
+                    logging.error(f"File {file} is not in the correct format. Skipping...")
+                    continue
 
-                # total samples in the audio file
+                try:
+                    audio, sample_rate = sf.read(os.path.join(root, file))
+                except Exception as e:
+                    logging.error(f"Error in the audio file {file}: {e}")
+                    continue
 
                 total_samples = len(audio)
 
-                # samples in each chunk
-
                 chunk_samples = int(slice_duration * sample_rate)
 
                 start = 0
 
                 for i in range(0, total_samples, chunk_samples):
                     chunk = audio[i : i + chunk_samples]
 
-                    # Getting the start time of the audio file from the actual recordings and adding the chunk duration
-
                     recording_time = (
                         file_datetime + datetime.timedelta(seconds=start)
                     ).strftime("%Y%m%dT%H%M%S")
 
                     filename = os.path.join(
-                        output_subdirectory, "{}.wav".format(recording_time)
+                        output_subdirectory, "{}.{}".format(recording_time, args.extension)
                     )
 
                     sf.write(filename, chunk, sample_rate)
 
                     start += slice_duration
 
     # fmt: off
     # Create an ArgumentParser object
     parser = argparse.ArgumentParser(
         description='A program that will help to extract recording from the actual long recordings.')
 
-    parser.add_argument('-r', '--root_directory', type=str, required=True, help='The root directory of the long recordings')  
-    parser.add_argument('-o', '--output_directory', type=str, help='The output directory to store the extracted audio segments')  
-    parser.add_argument('-c', '--csv_file_path', type=str, help='Path to the CSV file with the following requirements: Header should include "sample file" and "categories" columns. The "sample file" column should be in the format 20220608_170343, and the "categories" column should contain categories such as "Nocturnal", etc.') 
-    parser.add_argument('-d', '--duration', type=int, default=3, help='What duration of extracted segments you want?')  
+    parser.add_argument('-r', '--root_directory', type=str, required=True, help='The path to the folder containing the original recordings')  
+    parser.add_argument('-o', '--output_directory', type=str, help='The path to the folder of the extracted audio segments')  
+    parser.add_argument('-c', '--csv_file_path', type=str, help='The path to the CSV file. The header must include "sampleFile" and may include a "category" column. Recording named within the "sampleFile" column should be in the format "YYYYMMDD_HHMMSS"; if included, subgroups within "category" can be defined by the user, the recordings_times_generator.py (https://github.com/prayagnshah/Sound-Extraction/blob/main/src/README.md), or left blank"') 
+    parser.add_argument('-d', '--duration', type=int, default=3, help='The desired duration of the extracted segments')  
     parser.add_argument('-s', '--site_name', type=str,  help='The name of the site')
-    parser.add_argument('-span', '--span', action='store_true', help='Extract original files instead of spanning') 
+    parser.add_argument('-span', '--span', action='store_true', help='Extract original files instead of spanning; see README for more information') 
     parser.add_argument('-e', '--extension', type=str, choices=['.wav', '.flac'], default='.flac', help='The extension of the original audio files')
-    parser.add_argument('-slice', '--slice', type=int, help='In how many seconds you want to slice the audio files?') 
+    parser.add_argument('-slice', '--slice', type=int, help='Duration (in seconds) of the sliced audio files') 
     # Parse the command line arguments
 
     args = parser.parse_args()
 
     # fmt: on
 
     # Getting the root directory and output directory from the user
@@ -451,10 +454,9 @@
 
         filtered_recordings_dict = process_recordings(all_files, sample_recordings)
 
         export_segment, output_directory = extract_audio_segments(
             filtered_recordings_dict, output_directory, site_name, categories_dict
         )
 
-
 if __name__ == "__main__":
-    main()
+    main()
```

