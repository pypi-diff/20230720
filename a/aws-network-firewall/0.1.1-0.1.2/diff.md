# Comparing `tmp/aws_network_firewall-0.1.1.tar.gz` & `tmp/aws_network_firewall-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.1.1.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.1.2.tar", max compression
```

## Comparing `aws_network_firewall-0.1.1.tar` & `aws_network_firewall-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11335 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      787 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-07-20 19:43:16.679797 aws_network_firewall-0.1.1/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1133 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0     1191 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      579 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     2730 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/rule.py
--rw-r--r--   0        0        0     1962 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2002 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      509 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      320 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      353 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1638 2023-07-20 19:43:15.915801 aws_network_firewall-0.1.1/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1178 2023-07-20 19:43:16.679797 aws_network_firewall-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 aws_network_firewall-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-20 20:19:00.095717 aws_network_firewall-0.1.2/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1133 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0     1191 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      579 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     2730 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0     1962 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2002 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      509 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      353 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1638 2023-07-20 20:18:59.367708 aws_network_firewall-0.1.2/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1178 2023-07-20 20:19:00.095717 aws_network_firewall-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 aws_network_firewall-0.1.2/PKG-INFO
```

### Comparing `aws_network_firewall-0.1.1/LICENSE.txt` & `aws_network_firewall-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/README.md` & `aws_network_firewall-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AWS Network Firewall
 
 [![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://github.com/binxio/aws-network-firewall/graphs/commit-activity)
 [![GitHub release](https://img.shields.io/github/release/binxio/aws-network-firewall.svg)](https://github.com/binxio/aws-securityhub-suppression/releases/)
 [![Continuous Integration](https://github.com/binxio/aws-securityhub-suppression/actions/workflows/ci.yml/badge.svg)](https://github.com/binxio/aws-network-firewall/actions/workflows/ci.yml)
 
-This tool allows you to manage your Suppression's as Code.
+This tool allows you to manage your AWS Network Firewall rules as Code.
 
 **Useful links:**
 - [Documentation](https://binxio.github.io/aws-network-firewall/)
 - [Bug Tracker](https://github.com/binxio/aws-network-firewall/issues)
 - [PyPi](https://pypi.org/project/aws-network-firewall/)
```

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/account.py` & `aws_network_firewall-0.1.2/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.1.2/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.1.2/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/destination.py` & `aws_network_firewall-0.1.2/aws_network_firewall/destination.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.1.2/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/rule.py` & `aws_network_firewall-0.1.2/aws_network_firewall/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.1.2/aws_network_firewall/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/schemas/environment.yaml` & `aws_network_firewall-0.1.2/aws_network_firewall/schemas/environment.yaml`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.1.2/aws_network_firewall/suricata/rule.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.1.1/pyproject.toml` & `aws_network_firewall-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 radon = "^5.1.0"
 mypy = "^1.3.0"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
-types-pyyaml = "^6.0.12.10"
+types-pyyaml = "^6.0.12.11"
 
 [tool.semantic_release]
 version_variable = [
     "aws_network_firewall/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "main"
```

### Comparing `aws_network_firewall-0.1.1/PKG-INFO` & `aws_network_firewall-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,14 @@
 
 # AWS Network Firewall
 
 [![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://github.com/binxio/aws-network-firewall/graphs/commit-activity)
 [![GitHub release](https://img.shields.io/github/release/binxio/aws-network-firewall.svg)](https://github.com/binxio/aws-securityhub-suppression/releases/)
 [![Continuous Integration](https://github.com/binxio/aws-securityhub-suppression/actions/workflows/ci.yml/badge.svg)](https://github.com/binxio/aws-network-firewall/actions/workflows/ci.yml)
 
-This tool allows you to manage your Suppression's as Code.
+This tool allows you to manage your AWS Network Firewall rules as Code.
 
 **Useful links:**
 - [Documentation](https://binxio.github.io/aws-network-firewall/)
 - [Bug Tracker](https://github.com/binxio/aws-network-firewall/issues)
 - [PyPi](https://pypi.org/project/aws-network-firewall/)
```

