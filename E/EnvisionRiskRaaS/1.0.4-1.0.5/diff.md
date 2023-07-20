# Comparing `tmp/envisionriskraas-1.0.4.tar.gz` & `tmp/envisionriskraas-1.0.5.tar.gz`

## Comparing `envisionriskraas-1.0.4.tar` & `envisionriskraas-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.5/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.5/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 envisionriskraas-1.0.5/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     9406 2020-02-02 00:00:00.000000 envisionriskraas-1.0.5/PKG-INFO
```

### Comparing `envisionriskraas-1.0.4/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.0.5/src/EnvisionRiskRaaS/RAAS.py`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.4/LICENSE.txt` & `envisionriskraas-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.4/README.md` & `envisionriskraas-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 EnvisionRiskRaaS
-=================
+================= <hr>
 Delve into the world of EnvisionRisk’s Python package, your portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our cutting-edge risk management services, retrieve relevant data, perform complex calculations, and generate actionable insights, all without leaving your Python programming environment. Embrace this smarter, efficient approach to handling market risk.
 
 Are you navigating the volatile waters of financial uncertainties, seeking to make strategic decisions? Allow EnvisionRisk’s Cloud Service to be your compass, providing a precise mechanism for quantifying market risks. Replace guesswork with certainty; our platform furnishes you with standardized metrics designed to enhance cost-efficiency and fortify your financial bulwark.
 
 Our REST API, a seamless blend of security and user-friendliness, stands as your reliable tool for everyday risk quantification. Transform data into actionable steps and unravel the potential concealed within the labyrinth of financial complexities.
 
 With an expansive coverage spanning more than 13,000 exchange-traded and over-the-counter instruments—and continuously growing—EnvisionRisk is primed to adapt to your ever-evolving needs.
 
 Join the EnvisionRisk community today. Convert your market insights into solid foresights, and consistently maintain a competitive edge in the ever-fluctuating financial market. Stay not just in the game, but ahead of it.
 
 Authentication
---------------
+-------------- <hr>
 EnvisionRisk employs robust authentication and authorization processes to safeguard systems and information. EnvisionRisk’s Market Risk-as-a-Service API operates on a token-based authentication system. To use the service you need to be a registered user. If you don’t already have credentials, you can sign up for a free trial account here:
 
 <a href='https://envisionrisk.shinyapps.io/user_management' target='_blank'><img height='100' style='border:0px;height:100px;' src='https://camo.githubusercontent.com/e757b083ceb7645a42a28ce48d538a7c52808781191546a5cfe1bd6c37c7c677/68747470733a2f2f7777772e64726f70626f782e636f6d2f732f6330616f69363878686d70313132332f7369676e2d75702d627574746f6e2d706e672d33332e706e673f7261773d74727565' border='0' alt='Sign up' /></a>
 
 Installation
-------------
+------------ <hr>
 You can install the development version of EnvisionRiskRaaS like so:
 ```
 pip install EnvisionRiskRaaS
 ```
 
 Example
--------
-<hr>
+------- <hr>
 Although the following example may appear simple, it’s designed to illustrate how our service functions by requesting the simulated profit/loss (P/L) distribution for a single instrument — Apple (AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our service also allows you to request simulated P/L distribution for your custom portfolios. Through this, you gain invaluable insights into potential future outcomes, enabling you to make informed investment decisions.
 
 The Profit and Loss (P/L) distribution is a crucial component in the world of market risk management as it provides a quantitative way of understanding potential financial outcomes. Here’s why it plays an essential role:
 
 - <b>Risk Assessment:</b> The P/L distribution represents the range of possible gains and losses that a portfolio might experience. It allows risk managers to visualize and quantify potential risks. For example, the tails of the distribution give insight into extreme events and potential for significant losses, enabling a comprehensive risk assessment.
 
 - <b>Risk Measures Calculation:</b> Key risk measures, like Value at Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution. VaR estimates the potential loss a portfolio could face over a given period with a certain level of confidence, while ES provides the expected loss given that a loss exceeds the VaR threshold. These metrics help risk managers understand the risk landscape better and make informed decisions.
@@ -91,20 +90,18 @@
 plt.ylabel("Density")
 plt.yticks([])
 plt.text(0.5, -0.04, caption, ha='center', size=7)
 #plot
 plt.show()
 ```
 
-<img height='36' style='border:0px;height:36px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
-.. image:: https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png
-
+<img height='400' style='border:0px;height:400px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
 
 API documentation
------------------
+----------------- <hr>
 You can locate our extensive API documentation here. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
 
 For each API, you’ll find detailed descriptions, parameter information, example requests, and response formats to help you understand the API’s purpose and functionality. Whether you’re interested in user authentication, data retrieval, or performing specific actions, our documentation has you covered.
 
 In addition, you’ll find a section dedicated to ‘Common Use Cases’ where we illustrate how our APIs can be combined and utilized in various scenarios. This can be an invaluable resource for those seeking to maximize the potential of our services.
 
 Please note that our API documentation is constantly updated with new features and improvements to ensure you have the latest information at your fingertips.
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
-EnvisionRiskRaaS ================= Delve into the world of EnvisionRiskâs
-Python package, your portal to our sophisticated Market Risk-as-a-Service
-(RaaS). This comprehensive tool allows you to tap into our cutting-edge risk
-management services, retrieve relevant data, perform complex calculations, and
-generate actionable insights, all without leaving your Python programming
-environment. Embrace this smarter, efficient approach to handling market risk.
-Are you navigating the volatile waters of financial uncertainties, seeking to
-make strategic decisions? Allow EnvisionRiskâs Cloud Service to be your
-compass, providing a precise mechanism for quantifying market risks. Replace
-guesswork with certainty; our platform furnishes you with standardized metrics
-designed to enhance cost-efficiency and fortify your financial bulwark. Our
-REST API, a seamless blend of security and user-friendliness, stands as your
-reliable tool for everyday risk quantification. Transform data into actionable
-steps and unravel the potential concealed within the labyrinth of financial
-complexities. With an expansive coverage spanning more than 13,000 exchange-
-traded and over-the-counter instrumentsâand continuously
-growingâEnvisionRisk is primed to adapt to your ever-evolving needs. Join the
-EnvisionRisk community today. Convert your market insights into solid
-foresights, and consistently maintain a competitive edge in the ever-
-fluctuating financial market. Stay not just in the game, but ahead of it.
-Authentication -------------- EnvisionRisk employs robust authentication and
-authorization processes to safeguard systems and information. EnvisionRiskâs
-Market Risk-as-a-Service API operates on a token-based authentication system.
-To use the service you need to be a registered user. If you donât already
-have credentials, you can sign up for a free trial account here: [Sign_up]
-Installation ------------ You can install the development version of
-EnvisionRiskRaaS like so: ``` pip install EnvisionRiskRaaS ``` Example -------
+EnvisionRiskRaaS =================
+===============================================================================
+Delve into the world of EnvisionRiskâs Python package, your portal to our
+sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows
+you to tap into our cutting-edge risk management services, retrieve relevant
+data, perform complex calculations, and generate actionable insights, all
+without leaving your Python programming environment. Embrace this smarter,
+efficient approach to handling market risk. Are you navigating the volatile
+waters of financial uncertainties, seeking to make strategic decisions? Allow
+EnvisionRiskâs Cloud Service to be your compass, providing a precise
+mechanism for quantifying market risks. Replace guesswork with certainty; our
+platform furnishes you with standardized metrics designed to enhance cost-
+efficiency and fortify your financial bulwark. Our REST API, a seamless blend
+of security and user-friendliness, stands as your reliable tool for everyday
+risk quantification. Transform data into actionable steps and unravel the
+potential concealed within the labyrinth of financial complexities. With an
+expansive coverage spanning more than 13,000 exchange-traded and over-the-
+counter instrumentsâand continuously growingâEnvisionRisk is primed to
+adapt to your ever-evolving needs. Join the EnvisionRisk community today.
+Convert your market insights into solid foresights, and consistently maintain a
+competitive edge in the ever-fluctuating financial market. Stay not just in the
+game, but ahead of it. Authentication --------------
+===============================================================================
+EnvisionRisk employs robust authentication and authorization processes to
+safeguard systems and information. EnvisionRiskâs Market Risk-as-a-Service
+API operates on a token-based authentication system. To use the service you
+need to be a registered user. If you donât already have credentials, you can
+sign up for a free trial account here: [Sign_up] Installation ------------
+===============================================================================
+You can install the development version of EnvisionRiskRaaS like so: ``` pip
+install EnvisionRiskRaaS ``` Example -------
 ===============================================================================
 Although the following example may appear simple, itâs designed to illustrate
 how our service functions by requesting the simulated profit/loss (P/L)
 distribution for a single instrument â Apple (AAPL.US) as of 2023-06-28.
 Remember, this is just a starting point; our service also allows you to request
 simulated P/L distribution for your custom portfolios. Through this, you gain
 invaluable insights into potential future outcomes, enabling you to make
@@ -90,24 +94,24 @@
 expected_shortfall_estimate, color = "#57575F", label = 'axvline - full
 height') #vertical line text, labels, remove tickers and insert caption
 plt.text(expected_shortfall_estimate, max(density(xs))/2, 'Expected-Shortfall
 (97.5%, 1 day)', ha='center', va='center',rotation='vertical',
 backgroundcolor='white') plt.xlabel("Profit/Loss (in $)") plt.ylabel("Density")
 plt.yticks([]) plt.text(0.5, -0.04, caption, ha='center', size=7) #plot
 plt.show() ``` [https://raw.githubusercontent.com/EnvisionRisk/
-EnvisionRiskRaaS/master/man/figures/README-plot-1.png] .. image:: https://
-raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/
-README-plot-1.png API documentation ----------------- You can locate our
-extensive API documentation here. This comprehensive guide is designed to walk
-you through our APIsâ functionalities, providing clear instructions on how to
-integrate and use them effectively. For each API, youâll find detailed
-descriptions, parameter information, example requests, and response formats to
-help you understand the APIâs purpose and functionality. Whether youâre
-interested in user authentication, data retrieval, or performing specific
-actions, our documentation has you covered. In addition, youâll find a
-section dedicated to âCommon Use Casesâ where we illustrate how our APIs
-can be combined and utilized in various scenarios. This can be an invaluable
-resource for those seeking to maximize the potential of our services. Please
-note that our API documentation is constantly updated with new features and
-improvements to ensure you have the latest information at your fingertips.
-Explore our API documentation today to get started with your integrations and
-to make the most out of our services!
+EnvisionRiskRaaS/master/man/figures/README-plot-1.png] API documentation ------
+-----------
+===============================================================================
+You can locate our extensive API documentation here. This comprehensive guide
+is designed to walk you through our APIsâ functionalities, providing clear
+instructions on how to integrate and use them effectively. For each API,
+youâll find detailed descriptions, parameter information, example requests,
+and response formats to help you understand the APIâs purpose and
+functionality. Whether youâre interested in user authentication, data
+retrieval, or performing specific actions, our documentation has you covered.
+In addition, youâll find a section dedicated to âCommon Use Casesâ where
+we illustrate how our APIs can be combined and utilized in various scenarios.
+This can be an invaluable resource for those seeking to maximize the potential
+of our services. Please note that our API documentation is constantly updated
+with new features and improvements to ensure you have the latest information at
+your fingertips. Explore our API documentation today to get started with your
+integrations and to make the most out of our services!
```

### Comparing `envisionriskraas-1.0.4/pyproject.toml` & `envisionriskraas-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Jonas Hal", email="jonas.hal@envisionrisk.com" },
 ]
 description = "EnvisionRisk's Risk-as-a-service package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `envisionriskraas-1.0.4/PKG-INFO` & `envisionriskraas-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.0.4
+Version: 1.0.5
 Summary: EnvisionRisk's Risk-as-a-service package
 Project-URL: Homepage, https://www.envisionrisk.com/
 Project-URL: GitHub profile, https://github.com/EnvisionRisk
 Author-email: Jonas Hal <jonas.hal@envisionrisk.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 EnvisionRiskRaaS
-=================
+================= <hr>
 Delve into the world of EnvisionRisk’s Python package, your portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our cutting-edge risk management services, retrieve relevant data, perform complex calculations, and generate actionable insights, all without leaving your Python programming environment. Embrace this smarter, efficient approach to handling market risk.
 
 Are you navigating the volatile waters of financial uncertainties, seeking to make strategic decisions? Allow EnvisionRisk’s Cloud Service to be your compass, providing a precise mechanism for quantifying market risks. Replace guesswork with certainty; our platform furnishes you with standardized metrics designed to enhance cost-efficiency and fortify your financial bulwark.
 
 Our REST API, a seamless blend of security and user-friendliness, stands as your reliable tool for everyday risk quantification. Transform data into actionable steps and unravel the potential concealed within the labyrinth of financial complexities.
 
 With an expansive coverage spanning more than 13,000 exchange-traded and over-the-counter instruments—and continuously growing—EnvisionRisk is primed to adapt to your ever-evolving needs.
 
 Join the EnvisionRisk community today. Convert your market insights into solid foresights, and consistently maintain a competitive edge in the ever-fluctuating financial market. Stay not just in the game, but ahead of it.
 
 Authentication
---------------
+-------------- <hr>
 EnvisionRisk employs robust authentication and authorization processes to safeguard systems and information. EnvisionRisk’s Market Risk-as-a-Service API operates on a token-based authentication system. To use the service you need to be a registered user. If you don’t already have credentials, you can sign up for a free trial account here:
 
 <a href='https://envisionrisk.shinyapps.io/user_management' target='_blank'><img height='100' style='border:0px;height:100px;' src='https://camo.githubusercontent.com/e757b083ceb7645a42a28ce48d538a7c52808781191546a5cfe1bd6c37c7c677/68747470733a2f2f7777772e64726f70626f782e636f6d2f732f6330616f69363878686d70313132332f7369676e2d75702d627574746f6e2d706e672d33332e706e673f7261773d74727565' border='0' alt='Sign up' /></a>
 
 Installation
-------------
+------------ <hr>
 You can install the development version of EnvisionRiskRaaS like so:
 ```
 pip install EnvisionRiskRaaS
 ```
 
 Example
--------
-<hr>
+------- <hr>
 Although the following example may appear simple, it’s designed to illustrate how our service functions by requesting the simulated profit/loss (P/L) distribution for a single instrument — Apple (AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our service also allows you to request simulated P/L distribution for your custom portfolios. Through this, you gain invaluable insights into potential future outcomes, enabling you to make informed investment decisions.
 
 The Profit and Loss (P/L) distribution is a crucial component in the world of market risk management as it provides a quantitative way of understanding potential financial outcomes. Here’s why it plays an essential role:
 
 - <b>Risk Assessment:</b> The P/L distribution represents the range of possible gains and losses that a portfolio might experience. It allows risk managers to visualize and quantify potential risks. For example, the tails of the distribution give insight into extreme events and potential for significant losses, enabling a comprehensive risk assessment.
 
 - <b>Risk Measures Calculation:</b> Key risk measures, like Value at Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution. VaR estimates the potential loss a portfolio could face over a given period with a certain level of confidence, while ES provides the expected loss given that a loss exceeds the VaR threshold. These metrics help risk managers understand the risk landscape better and make informed decisions.
@@ -105,20 +104,18 @@
 plt.ylabel("Density")
 plt.yticks([])
 plt.text(0.5, -0.04, caption, ha='center', size=7)
 #plot
 plt.show()
 ```
 
-<img height='36' style='border:0px;height:36px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
-.. image:: https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png
-
+<img height='400' style='border:0px;height:400px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
 
 API documentation
------------------
+----------------- <hr>
 You can locate our extensive API documentation here. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
 
 For each API, you’ll find detailed descriptions, parameter information, example requests, and response formats to help you understand the API’s purpose and functionality. Whether you’re interested in user authentication, data retrieval, or performing specific actions, our documentation has you covered.
 
 In addition, you’ll find a section dedicated to ‘Common Use Cases’ where we illustrate how our APIs can be combined and utilized in various scenarios. This can be an invaluable resource for those seeking to maximize the potential of our services.
 
 Please note that our API documentation is constantly updated with new features and improvements to ensure you have the latest information at your fingertips.
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.4 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.5 Summary:
 EnvisionRisk's Risk-as-a-service package Project-URL: Homepage, https://
 www.envisionrisk.com/ Project-URL: GitHub profile, https://github.com/
 EnvisionRisk Author-email: Jonas Hal
 hal@envisionrisk.com> License-File: LICENSE.txt Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Description-Content-Type: text/markdown EnvisionRiskRaaS =================
+===============================================================================
 Delve into the world of EnvisionRiskâs Python package, your portal to our
 sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows
 you to tap into our cutting-edge risk management services, retrieve relevant
 data, perform complex calculations, and generate actionable insights, all
 without leaving your Python programming environment. Embrace this smarter,
 efficient approach to handling market risk. Are you navigating the volatile
 waters of financial uncertainties, seeking to make strategic decisions? Allow
@@ -21,22 +22,24 @@
 risk quantification. Transform data into actionable steps and unravel the
 potential concealed within the labyrinth of financial complexities. With an
 expansive coverage spanning more than 13,000 exchange-traded and over-the-
 counter instrumentsâand continuously growingâEnvisionRisk is primed to
 adapt to your ever-evolving needs. Join the EnvisionRisk community today.
 Convert your market insights into solid foresights, and consistently maintain a
 competitive edge in the ever-fluctuating financial market. Stay not just in the
-game, but ahead of it. Authentication -------------- EnvisionRisk employs
-robust authentication and authorization processes to safeguard systems and
-information. EnvisionRiskâs Market Risk-as-a-Service API operates on a token-
-based authentication system. To use the service you need to be a registered
-user. If you donât already have credentials, you can sign up for a free trial
-account here: [Sign_up] Installation ------------ You can install the
-development version of EnvisionRiskRaaS like so: ``` pip install
-EnvisionRiskRaaS ``` Example -------
+game, but ahead of it. Authentication --------------
+===============================================================================
+EnvisionRisk employs robust authentication and authorization processes to
+safeguard systems and information. EnvisionRiskâs Market Risk-as-a-Service
+API operates on a token-based authentication system. To use the service you
+need to be a registered user. If you donât already have credentials, you can
+sign up for a free trial account here: [Sign_up] Installation ------------
+===============================================================================
+You can install the development version of EnvisionRiskRaaS like so: ``` pip
+install EnvisionRiskRaaS ``` Example -------
 ===============================================================================
 Although the following example may appear simple, itâs designed to illustrate
 how our service functions by requesting the simulated profit/loss (P/L)
 distribution for a single instrument â Apple (AAPL.US) as of 2023-06-28.
 Remember, this is just a starting point; our service also allows you to request
 simulated P/L distribution for your custom portfolios. Through this, you gain
 invaluable insights into potential future outcomes, enabling you to make
@@ -98,24 +101,24 @@
 expected_shortfall_estimate, color = "#57575F", label = 'axvline - full
 height') #vertical line text, labels, remove tickers and insert caption
 plt.text(expected_shortfall_estimate, max(density(xs))/2, 'Expected-Shortfall
 (97.5%, 1 day)', ha='center', va='center',rotation='vertical',
 backgroundcolor='white') plt.xlabel("Profit/Loss (in $)") plt.ylabel("Density")
 plt.yticks([]) plt.text(0.5, -0.04, caption, ha='center', size=7) #plot
 plt.show() ``` [https://raw.githubusercontent.com/EnvisionRisk/
-EnvisionRiskRaaS/master/man/figures/README-plot-1.png] .. image:: https://
-raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/
-README-plot-1.png API documentation ----------------- You can locate our
-extensive API documentation here. This comprehensive guide is designed to walk
-you through our APIsâ functionalities, providing clear instructions on how to
-integrate and use them effectively. For each API, youâll find detailed
-descriptions, parameter information, example requests, and response formats to
-help you understand the APIâs purpose and functionality. Whether youâre
-interested in user authentication, data retrieval, or performing specific
-actions, our documentation has you covered. In addition, youâll find a
-section dedicated to âCommon Use Casesâ where we illustrate how our APIs
-can be combined and utilized in various scenarios. This can be an invaluable
-resource for those seeking to maximize the potential of our services. Please
-note that our API documentation is constantly updated with new features and
-improvements to ensure you have the latest information at your fingertips.
-Explore our API documentation today to get started with your integrations and
-to make the most out of our services!
+EnvisionRiskRaaS/master/man/figures/README-plot-1.png] API documentation ------
+-----------
+===============================================================================
+You can locate our extensive API documentation here. This comprehensive guide
+is designed to walk you through our APIsâ functionalities, providing clear
+instructions on how to integrate and use them effectively. For each API,
+youâll find detailed descriptions, parameter information, example requests,
+and response formats to help you understand the APIâs purpose and
+functionality. Whether youâre interested in user authentication, data
+retrieval, or performing specific actions, our documentation has you covered.
+In addition, youâll find a section dedicated to âCommon Use Casesâ where
+we illustrate how our APIs can be combined and utilized in various scenarios.
+This can be an invaluable resource for those seeking to maximize the potential
+of our services. Please note that our API documentation is constantly updated
+with new features and improvements to ensure you have the latest information at
+your fingertips. Explore our API documentation today to get started with your
+integrations and to make the most out of our services!
```

