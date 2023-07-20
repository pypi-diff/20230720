# Comparing `tmp/envisionriskraas-1.0.6.tar.gz` & `tmp/envisionriskraas-1.0.7.tar.gz`

## Comparing `envisionriskraas-1.0.6.tar` & `envisionriskraas-1.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.6/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.6/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.0.6/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 envisionriskraas-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.7/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.7/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.0.7/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 envisionriskraas-1.0.7/PKG-INFO
```

### Comparing `envisionriskraas-1.0.6/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.0.7/src/EnvisionRiskRaaS/RAAS.py`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.6/LICENSE.txt` & `envisionriskraas-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.6/README.md` & `envisionriskraas-1.0.7/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 With an expansive coverage spanning more than 13,000 exchange-traded and over-the-counter instruments—and continuously growing—EnvisionRisk is primed to adapt to your ever-evolving needs.
 
 Join the EnvisionRisk community today. Convert your market insights into solid foresights, and consistently maintain a competitive edge in the ever-fluctuating financial market. Stay not just in the game, but ahead of it.
 
 <h2>Authentication</h2>
 <hr>
 EnvisionRisk employs robust authentication and authorization processes to safeguard systems and information. EnvisionRisk’s Market Risk-as-a-Service API operates on a token-based authentication system. To use the service you need to be a registered user. If you don’t already have credentials, you can sign up for a free trial account here:
-
 <a href='https://envisionrisk.shinyapps.io/user_management' target='_blank'><img height='100' style='border:0px;height:100px;' src='https://camo.githubusercontent.com/e757b083ceb7645a42a28ce48d538a7c52808781191546a5cfe1bd6c37c7c677/68747470733a2f2f7777772e64726f70626f782e636f6d2f732f6330616f69363878686d70313132332f7369676e2d75702d627574746f6e2d706e672d33332e706e673f7261773d74727565' border='0' alt='Sign up' /></a>
 
 <h2>Installation</h2>
 <hr>
 You can install the development version of EnvisionRiskRaaS like so:
+
 ```
 pip install EnvisionRiskRaaS
 ```
 
 <h2>Example</h2>
 <hr>
 Although the following example may appear simple, it’s designed to illustrate how our service functions by requesting the simulated profit/loss (P/L) distribution for a single instrument — Apple (AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our service also allows you to request simulated P/L distribution for your custom portfolios. Through this, you gain invaluable insights into potential future outcomes, enabling you to make informed investment decisions.
```

### Comparing `envisionriskraas-1.0.6/pyproject.toml` & `envisionriskraas-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Jonas Hal", email="jonas.hal@envisionrisk.com" },
 ]
 description = "EnvisionRisk's Risk-as-a-service package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `envisionriskraas-1.0.6/PKG-INFO` & `envisionriskraas-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.0.6
+Version: 1.0.7
 Summary: EnvisionRisk's Risk-as-a-service package
 Project-URL: Homepage, https://www.envisionrisk.com/
 Project-URL: GitHub profile, https://github.com/EnvisionRisk
 Author-email: Jonas Hal <jonas.hal@envisionrisk.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,20 +23,20 @@
 With an expansive coverage spanning more than 13,000 exchange-traded and over-the-counter instruments—and continuously growing—EnvisionRisk is primed to adapt to your ever-evolving needs.
 
 Join the EnvisionRisk community today. Convert your market insights into solid foresights, and consistently maintain a competitive edge in the ever-fluctuating financial market. Stay not just in the game, but ahead of it.
 
 <h2>Authentication</h2>
 <hr>
 EnvisionRisk employs robust authentication and authorization processes to safeguard systems and information. EnvisionRisk’s Market Risk-as-a-Service API operates on a token-based authentication system. To use the service you need to be a registered user. If you don’t already have credentials, you can sign up for a free trial account here:
-
 <a href='https://envisionrisk.shinyapps.io/user_management' target='_blank'><img height='100' style='border:0px;height:100px;' src='https://camo.githubusercontent.com/e757b083ceb7645a42a28ce48d538a7c52808781191546a5cfe1bd6c37c7c677/68747470733a2f2f7777772e64726f70626f782e636f6d2f732f6330616f69363878686d70313132332f7369676e2d75702d627574746f6e2d706e672d33332e706e673f7261773d74727565' border='0' alt='Sign up' /></a>
 
 <h2>Installation</h2>
 <hr>
 You can install the development version of EnvisionRiskRaaS like so:
+
 ```
 pip install EnvisionRiskRaaS
 ```
 
 <h2>Example</h2>
 <hr>
 Although the following example may appear simple, it’s designed to illustrate how our service functions by requesting the simulated profit/loss (P/L) distribution for a single instrument — Apple (AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our service also allows you to request simulated P/L distribution for your custom portfolios. Through this, you gain invaluable insights into potential future outcomes, enabling you to make informed investment decisions.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.7 Summary:
 EnvisionRisk's Risk-as-a-service package Project-URL: Homepage, https://
 www.envisionrisk.com/ Project-URL: GitHub profile, https://github.com/
 EnvisionRisk Author-email: Jonas Hal
 hal@envisionrisk.com> License-File: LICENSE.txt Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

