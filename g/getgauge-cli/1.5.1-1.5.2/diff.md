# Comparing `tmp/getgauge-cli-1.5.1.tar.gz` & `tmp/getgauge-cli-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/getgauge-cli-1.5.1.tar", last modified: Fri Jun 23 15:01:08 2023, max compression
+gzip compressed data, was "getgauge-cli-1.5.2.tar", last modified: Thu Jul 20 15:08:47 2023, max compression
```

## Comparing `getgauge-cli-1.5.1.tar` & `getgauge-cli-1.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 15:01:00.000000 getgauge-cli-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-23 15:01:00.000000 getgauge-cli-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/getgauge_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:01:08.000000 getgauge-cli-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-23 15:01:07.000000 getgauge-cli-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:08:47.750997 getgauge-cli-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 15:08:33.000000 getgauge-cli-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-20 15:08:47.750997 getgauge-cli-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-20 15:08:33.000000 getgauge-cli-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:08:47.750997 getgauge-cli-1.5.2/getgauge_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-20 15:08:47.000000 getgauge-cli-1.5.2/getgauge_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-20 15:08:47.000000 getgauge-cli-1.5.2/getgauge_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:08:47.000000 getgauge-cli-1.5.2/getgauge_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 15:08:47.000000 getgauge-cli-1.5.2/getgauge_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:08:47.000000 getgauge-cli-1.5.2/getgauge_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:08:47.750997 getgauge-cli-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-20 15:08:46.000000 getgauge-cli-1.5.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `getgauge-cli-1.5.1/PKG-INFO` & `getgauge-cli-1.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,15 @@
 Metadata-Version: 2.1
 Name: getgauge-cli
-Version: 1.5.1
-Summary: UNKNOWN
+Version: 1.5.2
 Home-page: https://github.com/getgauge/gauge
 Author: getgauge
 Author-email: getgauge@googlegroups.com
 Maintainer: getgauge
 License: Apache-2.0
-Description: # PIP Installer for getgauge-cli tool
-        
-        This `setup.py` file is used for installed getgauge-cli tool.
-        the version number is manually bumped for now.
-        
-        Python package can be installed through multiple ways
-        
-        ## using setup.py
-        
-        - Navigate to the current directory `gauge\build\pip\`
-        - Run `python build.py --install` on command prompt (it will install the latest released version)
-        - To install a specific version set `GAUGE_VERSION` environment variable.
-        
-        ## using pip
-        
-        - pre-requisite: pip should be installed and available on machine
-        - run the command `pip install getgauge-cli`
-        
-        ## Check to ensure getgauge-cli is installed
-        
-        - Once the package has been setup. please exit the current terminal and relaunch terminal again
-        - run the command `gauge` , you should be able to see similar output
-        ```
-        Usage:
-          gauge <command> [flags] [args]
-        
-        Examples:
-          gauge run specs/
-          gauge run --parallel specs/
-        
-        Commands:
-          config      Change global configurations
-          daemon      Run as a daemon
-          docs        Generate documentation using specified plugin
-          format      Formats the specified spec files
-          help        Help about any command
-          init        Initialize project structure in the current directory
-          install     Download and install plugin(s)
-          list        List specifications, scenarios or tags for a gauge project
-          man         Generate man pages
-          run         Run specs
-          uninstall   Uninstalls a plugin
-          update      Updates a plugin
-          validate    Check for validation and parse errors
-          version     Print Gauge and plugin versions
-        
-        Flags:
-          -d, --dir string         Set the working directory for the current command, accepts a path relative to current directory (default ".")
-          -h, --help               Help for gauge
-          -l, --log-level string   Set level of logging to debug, info, warning, error or critical (default "info")
-          -m, --machine-readable   Prints output in JSON format
-          -v, --version            Print Gauge and plugin versions
-        
-        Use "gauge [command] --help" for more information about a command.
-        Complete manual is available at https://manpage.gauge.org/.
-        ```
-        
-        ## Using setup.py
-        - Install required dep by running `python/python3 -m pip install requirements.txt`.
-        - Check through and obtain a valid tag/build number from [releases](https://github.com/getgauge/gauge/releases)
-        - Run the command `python build.py --install` (set GAUGE_VERSION env to install specific version)
-        - This would install the version as specified along with latest release of Gauge-CLI Version
-        
-        - Run the command `python build.py --dist` to generate the PyPi distrubutable (set GAUGE_VERSION env to install specific version)
-        
-        ## Uninstalling Gauge CLI
-        
-        Gauge CLI uninstall should be done manually for now.
-        Run the following command on your prompt
-        ```
-        $ pip uninstall gauge-cli
-        ```
-        
 Platform: Windows
 Platform: Linux
 Platform: Unix
 Platform: Mac OS-X
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet
@@ -95,7 +21,80 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+
+# PIP Installer for getgauge-cli tool
+
+This `setup.py` file is used for installed getgauge-cli tool.
+the version number is manually bumped for now.
+
+Python package can be installed through multiple ways
+
+## using setup.py
+
+- Navigate to the current directory `gauge\build\pip\`
+- Run `python build.py --install` on command prompt (it will install the latest released version)
+- To install a specific version set `GAUGE_VERSION` environment variable.
+
+## using pip
+
+- pre-requisite: pip should be installed and available on machine
+- run the command `pip install getgauge-cli`
+
+## Check to ensure getgauge-cli is installed
+
+- Once the package has been setup. please exit the current terminal and relaunch terminal again
+- run the command `gauge` , you should be able to see similar output
+```
+Usage:
+  gauge <command> [flags] [args]
+
+Examples:
+  gauge run specs/
+  gauge run --parallel specs/
+
+Commands:
+  config      Change global configurations
+  daemon      Run as a daemon
+  docs        Generate documentation using specified plugin
+  format      Formats the specified spec files
+  help        Help about any command
+  init        Initialize project structure in the current directory
+  install     Download and install plugin(s)
+  list        List specifications, scenarios or tags for a gauge project
+  man         Generate man pages
+  run         Run specs
+  uninstall   Uninstalls a plugin
+  update      Updates a plugin
+  validate    Check for validation and parse errors
+  version     Print Gauge and plugin versions
+
+Flags:
+  -d, --dir string         Set the working directory for the current command, accepts a path relative to current directory (default ".")
+  -h, --help               Help for gauge
+  -l, --log-level string   Set level of logging to debug, info, warning, error or critical (default "info")
+  -m, --machine-readable   Prints output in JSON format
+  -v, --version            Print Gauge and plugin versions
+
+Use "gauge [command] --help" for more information about a command.
+Complete manual is available at https://manpage.gauge.org/.
+```
+
+## Using setup.py
+- Install required dep by running `python/python3 -m pip install requirements.txt`.
+- Check through and obtain a valid tag/build number from [releases](https://github.com/getgauge/gauge/releases)
+- Run the command `python build.py --install` (set GAUGE_VERSION env to install specific version)
+- This would install the version as specified along with latest release of Gauge-CLI Version
+
+- Run the command `python build.py --dist` to generate the PyPi distrubutable (set GAUGE_VERSION env to install specific version)
+
+## Uninstalling Gauge CLI
+
+Gauge CLI uninstall should be done manually for now.
+Run the following command on your prompt
+```
+$ pip uninstall gauge-cli
+```
```

### Comparing `getgauge-cli-1.5.1/README.md` & `getgauge-cli-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `getgauge-cli-1.5.1/getgauge_cli.egg-info/PKG-INFO` & `getgauge-cli-1.5.2/getgauge_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,15 @@
 Metadata-Version: 2.1
 Name: getgauge-cli
-Version: 1.5.1
-Summary: UNKNOWN
+Version: 1.5.2
 Home-page: https://github.com/getgauge/gauge
 Author: getgauge
 Author-email: getgauge@googlegroups.com
 Maintainer: getgauge
 License: Apache-2.0
-Description: # PIP Installer for getgauge-cli tool
-        
-        This `setup.py` file is used for installed getgauge-cli tool.
-        the version number is manually bumped for now.
-        
-        Python package can be installed through multiple ways
-        
-        ## using setup.py
-        
-        - Navigate to the current directory `gauge\build\pip\`
-        - Run `python build.py --install` on command prompt (it will install the latest released version)
-        - To install a specific version set `GAUGE_VERSION` environment variable.
-        
-        ## using pip
-        
-        - pre-requisite: pip should be installed and available on machine
-        - run the command `pip install getgauge-cli`
-        
-        ## Check to ensure getgauge-cli is installed
-        
-        - Once the package has been setup. please exit the current terminal and relaunch terminal again
-        - run the command `gauge` , you should be able to see similar output
-        ```
-        Usage:
-          gauge <command> [flags] [args]
-        
-        Examples:
-          gauge run specs/
-          gauge run --parallel specs/
-        
-        Commands:
-          config      Change global configurations
-          daemon      Run as a daemon
-          docs        Generate documentation using specified plugin
-          format      Formats the specified spec files
-          help        Help about any command
-          init        Initialize project structure in the current directory
-          install     Download and install plugin(s)
-          list        List specifications, scenarios or tags for a gauge project
-          man         Generate man pages
-          run         Run specs
-          uninstall   Uninstalls a plugin
-          update      Updates a plugin
-          validate    Check for validation and parse errors
-          version     Print Gauge and plugin versions
-        
-        Flags:
-          -d, --dir string         Set the working directory for the current command, accepts a path relative to current directory (default ".")
-          -h, --help               Help for gauge
-          -l, --log-level string   Set level of logging to debug, info, warning, error or critical (default "info")
-          -m, --machine-readable   Prints output in JSON format
-          -v, --version            Print Gauge and plugin versions
-        
-        Use "gauge [command] --help" for more information about a command.
-        Complete manual is available at https://manpage.gauge.org/.
-        ```
-        
-        ## Using setup.py
-        - Install required dep by running `python/python3 -m pip install requirements.txt`.
-        - Check through and obtain a valid tag/build number from [releases](https://github.com/getgauge/gauge/releases)
-        - Run the command `python build.py --install` (set GAUGE_VERSION env to install specific version)
-        - This would install the version as specified along with latest release of Gauge-CLI Version
-        
-        - Run the command `python build.py --dist` to generate the PyPi distrubutable (set GAUGE_VERSION env to install specific version)
-        
-        ## Uninstalling Gauge CLI
-        
-        Gauge CLI uninstall should be done manually for now.
-        Run the following command on your prompt
-        ```
-        $ pip uninstall gauge-cli
-        ```
-        
 Platform: Windows
 Platform: Linux
 Platform: Unix
 Platform: Mac OS-X
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet
@@ -95,7 +21,80 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+
+# PIP Installer for getgauge-cli tool
+
+This `setup.py` file is used for installed getgauge-cli tool.
+the version number is manually bumped for now.
+
+Python package can be installed through multiple ways
+
+## using setup.py
+
+- Navigate to the current directory `gauge\build\pip\`
+- Run `python build.py --install` on command prompt (it will install the latest released version)
+- To install a specific version set `GAUGE_VERSION` environment variable.
+
+## using pip
+
+- pre-requisite: pip should be installed and available on machine
+- run the command `pip install getgauge-cli`
+
+## Check to ensure getgauge-cli is installed
+
+- Once the package has been setup. please exit the current terminal and relaunch terminal again
+- run the command `gauge` , you should be able to see similar output
+```
+Usage:
+  gauge <command> [flags] [args]
+
+Examples:
+  gauge run specs/
+  gauge run --parallel specs/
+
+Commands:
+  config      Change global configurations
+  daemon      Run as a daemon
+  docs        Generate documentation using specified plugin
+  format      Formats the specified spec files
+  help        Help about any command
+  init        Initialize project structure in the current directory
+  install     Download and install plugin(s)
+  list        List specifications, scenarios or tags for a gauge project
+  man         Generate man pages
+  run         Run specs
+  uninstall   Uninstalls a plugin
+  update      Updates a plugin
+  validate    Check for validation and parse errors
+  version     Print Gauge and plugin versions
+
+Flags:
+  -d, --dir string         Set the working directory for the current command, accepts a path relative to current directory (default ".")
+  -h, --help               Help for gauge
+  -l, --log-level string   Set level of logging to debug, info, warning, error or critical (default "info")
+  -m, --machine-readable   Prints output in JSON format
+  -v, --version            Print Gauge and plugin versions
+
+Use "gauge [command] --help" for more information about a command.
+Complete manual is available at https://manpage.gauge.org/.
+```
+
+## Using setup.py
+- Install required dep by running `python/python3 -m pip install requirements.txt`.
+- Check through and obtain a valid tag/build number from [releases](https://github.com/getgauge/gauge/releases)
+- Run the command `python build.py --install` (set GAUGE_VERSION env to install specific version)
+- This would install the version as specified along with latest release of Gauge-CLI Version
+
+- Run the command `python build.py --dist` to generate the PyPi distrubutable (set GAUGE_VERSION env to install specific version)
+
+## Uninstalling Gauge CLI
+
+Gauge CLI uninstall should be done manually for now.
+Run the following command on your prompt
+```
+$ pip uninstall gauge-cli
+```
```

### Comparing `getgauge-cli-1.5.1/setup.py` & `getgauge-cli-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import platform
 import zipfile
 import os
 import sys
 
 
-_version = "1.5.1"
+_version = "1.5.2"
 _latest_version = ""
 
 
 class CustomInstallCommand(install):
     """Customized setuptools install command to download and setup."""
 
     _base_url = 'https://api.github.com/repos/getgauge/gauge/releases'
```

