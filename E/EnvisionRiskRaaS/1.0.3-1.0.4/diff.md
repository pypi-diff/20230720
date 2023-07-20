# Comparing `tmp/envisionriskraas-1.0.3.tar.gz` & `tmp/envisionriskraas-1.0.4.tar.gz`

## Comparing `envisionriskraas-1.0.3.tar` & `envisionriskraas-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.3/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.3/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 envisionriskraas-1.0.3/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     9436 2020-02-02 00:00:00.000000 envisionriskraas-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 envisionriskraas-1.0.4/PKG-INFO
```

### Comparing `envisionriskraas-1.0.3/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.0.4/src/EnvisionRiskRaaS/RAAS.py`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.3/LICENSE.txt` & `envisionriskraas-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.3/README.md` & `envisionriskraas-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 You can install the development version of EnvisionRiskRaaS like so:
 ```
 pip install EnvisionRiskRaaS
 ```
 
 Example
 -------
-
+<hr>
 Although the following example may appear simple, it’s designed to illustrate how our service functions by requesting the simulated profit/loss (P/L) distribution for a single instrument — Apple (AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our service also allows you to request simulated P/L distribution for your custom portfolios. Through this, you gain invaluable insights into potential future outcomes, enabling you to make informed investment decisions.
 
 The Profit and Loss (P/L) distribution is a crucial component in the world of market risk management as it provides a quantitative way of understanding potential financial outcomes. Here’s why it plays an essential role:
 
-Risk Assessment: The P/L distribution represents the range of possible gains and losses that a portfolio might experience. It allows risk managers to visualize and quantify potential risks. For example, the tails of the distribution give insight into extreme events and potential for significant losses, enabling a comprehensive risk assessment.
+- <b>Risk Assessment:</b> The P/L distribution represents the range of possible gains and losses that a portfolio might experience. It allows risk managers to visualize and quantify potential risks. For example, the tails of the distribution give insight into extreme events and potential for significant losses, enabling a comprehensive risk assessment.
 
-Risk Measures Calculation: Key risk measures, like Value at Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution. VaR estimates the potential loss a portfolio could face over a given period with a certain level of confidence, while ES provides the expected loss given that a loss exceeds the VaR threshold. These metrics help risk managers understand the risk landscape better and make informed decisions.
+- <b>Risk Measures Calculation:</b> Key risk measures, like Value at Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution. VaR estimates the potential loss a portfolio could face over a given period with a certain level of confidence, while ES provides the expected loss given that a loss exceeds the VaR threshold. These metrics help risk managers understand the risk landscape better and make informed decisions.
 
-Portfolio Optimization: By understanding the P/L distribution, managers can optimize the portfolio for desired outcomes. It allows them to adjust the portfolio composition to control the risk, striking a balance between risk and return.
+- <b>Portfolio Optimization:</b> By understanding the P/L distribution, managers can optimize the portfolio for desired outcomes. It allows them to adjust the portfolio composition to control the risk, striking a balance between risk and return.
 
-Regulatory Compliance: Regulators often require financial institutions to maintain capital reserves based on potential losses, which are derived from P/L distributions. Hence, understanding the P/L distribution is crucial to meet these regulatory requirements.
+- <b>Regulatory Compliance:</b> Regulators often require financial institutions to maintain capital reserves based on potential losses, which are derived from P/L distributions. Hence, understanding the P/L distribution is crucial to meet these regulatory requirements.
 
-Stress Testing: Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
+- <b>Stress Testing:</b> Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
 
 Therefore, P/L distribution serves as a key pillar of market risk management, providing insights into potential risks, informing decision-making, enabling portfolio optimization, and ensuring regulatory compliance.
 
 ```
 #### Get the delta vector (simulated price change) ####
 # The term '_raw' within the function name is indicative of a key feature: 
 # the simulated price changes are denominated in the same currency as 
@@ -91,18 +91,17 @@
 plt.ylabel("Density")
 plt.yticks([])
 plt.text(0.5, -0.04, caption, ha='center', size=7)
 #plot
 plt.show()
 ```
 
-<img height='36' style='border:0px;height:36px;' src='https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/man/figures/README-plot-1.png ' border='0' />
-<a href="https://www.w3schools.com">
-<img src="w3html.gif" alt="W3Schools.com" width="100" height="132">
-</a>
+<img height='36' style='border:0px;height:36px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
+.. image:: https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png
+
 
 API documentation
 -----------------
 You can locate our extensive API documentation here. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
 
 For each API, you’ll find detailed descriptions, parameter information, example requests, and response formats to help you understand the API’s purpose and functionality. Whether you’re interested in user authentication, data retrieval, or performing specific actions, our documentation has you covered.
```

#### html2text {}

```diff
@@ -20,42 +20,43 @@
 fluctuating financial market. Stay not just in the game, but ahead of it.
 Authentication -------------- EnvisionRisk employs robust authentication and
 authorization processes to safeguard systems and information. EnvisionRiskâs
 Market Risk-as-a-Service API operates on a token-based authentication system.
 To use the service you need to be a registered user. If you donât already
 have credentials, you can sign up for a free trial account here: [Sign_up]
 Installation ------------ You can install the development version of
-EnvisionRiskRaaS like so: ``` pip install EnvisionRiskRaaS ``` Example ------
-- Although the following example may appear simple, itâs designed to
-illustrate how our service functions by requesting the simulated profit/loss
-(P/L) distribution for a single instrument â Apple (AAPL.US) as of 2023-06-
-28. Remember, this is just a starting point; our service also allows you to
-request simulated P/L distribution for your custom portfolios. Through this,
-you gain invaluable insights into potential future outcomes, enabling you to
-make informed investment decisions. The Profit and Loss (P/L) distribution is a
+EnvisionRiskRaaS like so: ``` pip install EnvisionRiskRaaS ``` Example -------
+===============================================================================
+Although the following example may appear simple, itâs designed to illustrate
+how our service functions by requesting the simulated profit/loss (P/L)
+distribution for a single instrument â Apple (AAPL.US) as of 2023-06-28.
+Remember, this is just a starting point; our service also allows you to request
+simulated P/L distribution for your custom portfolios. Through this, you gain
+invaluable insights into potential future outcomes, enabling you to make
+informed investment decisions. The Profit and Loss (P/L) distribution is a
 crucial component in the world of market risk management as it provides a
 quantitative way of understanding potential financial outcomes. Hereâs why it
-plays an essential role: Risk Assessment: The P/L distribution represents the
+plays an essential role: - Risk Assessment: The P/L distribution represents the
 range of possible gains and losses that a portfolio might experience. It allows
 risk managers to visualize and quantify potential risks. For example, the tails
 of the distribution give insight into extreme events and potential for
-significant losses, enabling a comprehensive risk assessment. Risk Measures
+significant losses, enabling a comprehensive risk assessment. - Risk Measures
 Calculation: Key risk measures, like Value at Risk (VaR) and Expected Shortfall
 (ES), are derived from the P/L distribution. VaR estimates the potential loss a
 portfolio could face over a given period with a certain level of confidence,
 while ES provides the expected loss given that a loss exceeds the VaR
 threshold. These metrics help risk managers understand the risk landscape
-better and make informed decisions. Portfolio Optimization: By understanding
+better and make informed decisions. - Portfolio Optimization: By understanding
 the P/L distribution, managers can optimize the portfolio for desired outcomes.
 It allows them to adjust the portfolio composition to control the risk,
-striking a balance between risk and return. Regulatory Compliance: Regulators
+striking a balance between risk and return. - Regulatory Compliance: Regulators
 often require financial institutions to maintain capital reserves based on
 potential losses, which are derived from P/L distributions. Hence,
 understanding the P/L distribution is crucial to meet these regulatory
-requirements. Stress Testing: Stress testing involves applying extreme but
+requirements. - Stress Testing: Stress testing involves applying extreme but
 plausible hypothetical scenarios to the P/L distribution to assess the
 portfolioâs resilience. This helps managers prepare for unexpected market
 events and ensure that the portfolio can withstand adverse conditions.
 Therefore, P/L distribution serves as a key pillar of market risk management,
 providing insights into potential risks, informing decision-making, enabling
 portfolio optimization, and ensuring regulatory compliance. ``` #### Get the
 delta vector (simulated price change) #### # The term '_raw' within the
@@ -88,23 +89,25 @@
 plt.plot( xs, density(xs), color="#CA3542", alpha=0.5) plt.axvline(x =
 expected_shortfall_estimate, color = "#57575F", label = 'axvline - full
 height') #vertical line text, labels, remove tickers and insert caption
 plt.text(expected_shortfall_estimate, max(density(xs))/2, 'Expected-Shortfall
 (97.5%, 1 day)', ha='center', va='center',rotation='vertical',
 backgroundcolor='white') plt.xlabel("Profit/Loss (in $)") plt.ylabel("Density")
 plt.yticks([]) plt.text(0.5, -0.04, caption, ha='center', size=7) #plot
-plt.show() ``` [https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/
-man/figures/README-plot-1.png ] [W3Schools.com] API documentation -------------
----- You can locate our extensive API documentation here. This comprehensive
-guide is designed to walk you through our APIsâ functionalities, providing
-clear instructions on how to integrate and use them effectively. For each API,
-youâll find detailed descriptions, parameter information, example requests,
-and response formats to help you understand the APIâs purpose and
-functionality. Whether youâre interested in user authentication, data
-retrieval, or performing specific actions, our documentation has you covered.
-In addition, youâll find a section dedicated to âCommon Use Casesâ where
-we illustrate how our APIs can be combined and utilized in various scenarios.
-This can be an invaluable resource for those seeking to maximize the potential
-of our services. Please note that our API documentation is constantly updated
-with new features and improvements to ensure you have the latest information at
-your fingertips. Explore our API documentation today to get started with your
-integrations and to make the most out of our services!
+plt.show() ``` [https://raw.githubusercontent.com/EnvisionRisk/
+EnvisionRiskRaaS/master/man/figures/README-plot-1.png] .. image:: https://
+raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/
+README-plot-1.png API documentation ----------------- You can locate our
+extensive API documentation here. This comprehensive guide is designed to walk
+you through our APIsâ functionalities, providing clear instructions on how to
+integrate and use them effectively. For each API, youâll find detailed
+descriptions, parameter information, example requests, and response formats to
+help you understand the APIâs purpose and functionality. Whether youâre
+interested in user authentication, data retrieval, or performing specific
+actions, our documentation has you covered. In addition, youâll find a
+section dedicated to âCommon Use Casesâ where we illustrate how our APIs
+can be combined and utilized in various scenarios. This can be an invaluable
+resource for those seeking to maximize the potential of our services. Please
+note that our API documentation is constantly updated with new features and
+improvements to ensure you have the latest information at your fingertips.
+Explore our API documentation today to get started with your integrations and
+to make the most out of our services!
```

### Comparing `envisionriskraas-1.0.3/pyproject.toml` & `envisionriskraas-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Jonas Hal", email="jonas.hal@envisionrisk.com" },
 ]
 description = "EnvisionRisk's Risk-as-a-service package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `envisionriskraas-1.0.3/PKG-INFO` & `envisionriskraas-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.0.3
+Version: 1.0.4
 Summary: EnvisionRisk's Risk-as-a-service package
 Project-URL: Homepage, https://www.envisionrisk.com/
 Project-URL: GitHub profile, https://github.com/EnvisionRisk
 Author-email: Jonas Hal <jonas.hal@envisionrisk.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,28 +35,28 @@
 You can install the development version of EnvisionRiskRaaS like so:
 ```
 pip install EnvisionRiskRaaS
 ```
 
 Example
 -------
-
+<hr>
 Although the following example may appear simple, it’s designed to illustrate how our service functions by requesting the simulated profit/loss (P/L) distribution for a single instrument — Apple (AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our service also allows you to request simulated P/L distribution for your custom portfolios. Through this, you gain invaluable insights into potential future outcomes, enabling you to make informed investment decisions.
 
 The Profit and Loss (P/L) distribution is a crucial component in the world of market risk management as it provides a quantitative way of understanding potential financial outcomes. Here’s why it plays an essential role:
 
-Risk Assessment: The P/L distribution represents the range of possible gains and losses that a portfolio might experience. It allows risk managers to visualize and quantify potential risks. For example, the tails of the distribution give insight into extreme events and potential for significant losses, enabling a comprehensive risk assessment.
+- <b>Risk Assessment:</b> The P/L distribution represents the range of possible gains and losses that a portfolio might experience. It allows risk managers to visualize and quantify potential risks. For example, the tails of the distribution give insight into extreme events and potential for significant losses, enabling a comprehensive risk assessment.
 
-Risk Measures Calculation: Key risk measures, like Value at Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution. VaR estimates the potential loss a portfolio could face over a given period with a certain level of confidence, while ES provides the expected loss given that a loss exceeds the VaR threshold. These metrics help risk managers understand the risk landscape better and make informed decisions.
+- <b>Risk Measures Calculation:</b> Key risk measures, like Value at Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution. VaR estimates the potential loss a portfolio could face over a given period with a certain level of confidence, while ES provides the expected loss given that a loss exceeds the VaR threshold. These metrics help risk managers understand the risk landscape better and make informed decisions.
 
-Portfolio Optimization: By understanding the P/L distribution, managers can optimize the portfolio for desired outcomes. It allows them to adjust the portfolio composition to control the risk, striking a balance between risk and return.
+- <b>Portfolio Optimization:</b> By understanding the P/L distribution, managers can optimize the portfolio for desired outcomes. It allows them to adjust the portfolio composition to control the risk, striking a balance between risk and return.
 
-Regulatory Compliance: Regulators often require financial institutions to maintain capital reserves based on potential losses, which are derived from P/L distributions. Hence, understanding the P/L distribution is crucial to meet these regulatory requirements.
+- <b>Regulatory Compliance:</b> Regulators often require financial institutions to maintain capital reserves based on potential losses, which are derived from P/L distributions. Hence, understanding the P/L distribution is crucial to meet these regulatory requirements.
 
-Stress Testing: Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
+- <b>Stress Testing:</b> Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
 
 Therefore, P/L distribution serves as a key pillar of market risk management, providing insights into potential risks, informing decision-making, enabling portfolio optimization, and ensuring regulatory compliance.
 
 ```
 #### Get the delta vector (simulated price change) ####
 # The term '_raw' within the function name is indicative of a key feature: 
 # the simulated price changes are denominated in the same currency as 
@@ -105,18 +105,17 @@
 plt.ylabel("Density")
 plt.yticks([])
 plt.text(0.5, -0.04, caption, ha='center', size=7)
 #plot
 plt.show()
 ```
 
-<img height='36' style='border:0px;height:36px;' src='https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/man/figures/README-plot-1.png ' border='0' />
-<a href="https://www.w3schools.com">
-<img src="w3html.gif" alt="W3Schools.com" width="100" height="132">
-</a>
+<img height='36' style='border:0px;height:36px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
+.. image:: https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png
+
 
 API documentation
 -----------------
 You can locate our extensive API documentation here. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
 
 For each API, you’ll find detailed descriptions, parameter information, example requests, and response formats to help you understand the API’s purpose and functionality. Whether you’re interested in user authentication, data retrieval, or performing specific actions, our documentation has you covered.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.3 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.4 Summary:
 EnvisionRisk's Risk-as-a-service package Project-URL: Homepage, https://
 www.envisionrisk.com/ Project-URL: GitHub profile, https://github.com/
 EnvisionRisk Author-email: Jonas Hal
 hal@envisionrisk.com> License-File: LICENSE.txt Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Description-Content-Type: text/markdown EnvisionRiskRaaS =================
@@ -28,43 +28,45 @@
 game, but ahead of it. Authentication -------------- EnvisionRisk employs
 robust authentication and authorization processes to safeguard systems and
 information. EnvisionRiskâs Market Risk-as-a-Service API operates on a token-
 based authentication system. To use the service you need to be a registered
 user. If you donât already have credentials, you can sign up for a free trial
 account here: [Sign_up] Installation ------------ You can install the
 development version of EnvisionRiskRaaS like so: ``` pip install
-EnvisionRiskRaaS ``` Example ------- Although the following example may appear
-simple, itâs designed to illustrate how our service functions by requesting
-the simulated profit/loss (P/L) distribution for a single instrument â Apple
-(AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our
-service also allows you to request simulated P/L distribution for your custom
-portfolios. Through this, you gain invaluable insights into potential future
-outcomes, enabling you to make informed investment decisions. The Profit and
-Loss (P/L) distribution is a crucial component in the world of market risk
-management as it provides a quantitative way of understanding potential
-financial outcomes. Hereâs why it plays an essential role: Risk Assessment:
-The P/L distribution represents the range of possible gains and losses that a
-portfolio might experience. It allows risk managers to visualize and quantify
-potential risks. For example, the tails of the distribution give insight into
-extreme events and potential for significant losses, enabling a comprehensive
-risk assessment. Risk Measures Calculation: Key risk measures, like Value at
-Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution.
-VaR estimates the potential loss a portfolio could face over a given period
-with a certain level of confidence, while ES provides the expected loss given
-that a loss exceeds the VaR threshold. These metrics help risk managers
-understand the risk landscape better and make informed decisions. Portfolio
-Optimization: By understanding the P/L distribution, managers can optimize the
-portfolio for desired outcomes. It allows them to adjust the portfolio
-composition to control the risk, striking a balance between risk and return.
-Regulatory Compliance: Regulators often require financial institutions to
-maintain capital reserves based on potential losses, which are derived from P/
-L distributions. Hence, understanding the P/L distribution is crucial to meet
-these regulatory requirements. Stress Testing: Stress testing involves applying
-extreme but plausible hypothetical scenarios to the P/L distribution to assess
-the portfolioâs resilience. This helps managers prepare for unexpected market
+EnvisionRiskRaaS ``` Example -------
+===============================================================================
+Although the following example may appear simple, itâs designed to illustrate
+how our service functions by requesting the simulated profit/loss (P/L)
+distribution for a single instrument â Apple (AAPL.US) as of 2023-06-28.
+Remember, this is just a starting point; our service also allows you to request
+simulated P/L distribution for your custom portfolios. Through this, you gain
+invaluable insights into potential future outcomes, enabling you to make
+informed investment decisions. The Profit and Loss (P/L) distribution is a
+crucial component in the world of market risk management as it provides a
+quantitative way of understanding potential financial outcomes. Hereâs why it
+plays an essential role: - Risk Assessment: The P/L distribution represents the
+range of possible gains and losses that a portfolio might experience. It allows
+risk managers to visualize and quantify potential risks. For example, the tails
+of the distribution give insight into extreme events and potential for
+significant losses, enabling a comprehensive risk assessment. - Risk Measures
+Calculation: Key risk measures, like Value at Risk (VaR) and Expected Shortfall
+(ES), are derived from the P/L distribution. VaR estimates the potential loss a
+portfolio could face over a given period with a certain level of confidence,
+while ES provides the expected loss given that a loss exceeds the VaR
+threshold. These metrics help risk managers understand the risk landscape
+better and make informed decisions. - Portfolio Optimization: By understanding
+the P/L distribution, managers can optimize the portfolio for desired outcomes.
+It allows them to adjust the portfolio composition to control the risk,
+striking a balance between risk and return. - Regulatory Compliance: Regulators
+often require financial institutions to maintain capital reserves based on
+potential losses, which are derived from P/L distributions. Hence,
+understanding the P/L distribution is crucial to meet these regulatory
+requirements. - Stress Testing: Stress testing involves applying extreme but
+plausible hypothetical scenarios to the P/L distribution to assess the
+portfolioâs resilience. This helps managers prepare for unexpected market
 events and ensure that the portfolio can withstand adverse conditions.
 Therefore, P/L distribution serves as a key pillar of market risk management,
 providing insights into potential risks, informing decision-making, enabling
 portfolio optimization, and ensuring regulatory compliance. ``` #### Get the
 delta vector (simulated price change) #### # The term '_raw' within the
 function name is indicative of a key feature: # the simulated price changes are
 denominated in the same currency as # the stock. This implies that the analysis
@@ -95,23 +97,25 @@
 plt.plot( xs, density(xs), color="#CA3542", alpha=0.5) plt.axvline(x =
 expected_shortfall_estimate, color = "#57575F", label = 'axvline - full
 height') #vertical line text, labels, remove tickers and insert caption
 plt.text(expected_shortfall_estimate, max(density(xs))/2, 'Expected-Shortfall
 (97.5%, 1 day)', ha='center', va='center',rotation='vertical',
 backgroundcolor='white') plt.xlabel("Profit/Loss (in $)") plt.ylabel("Density")
 plt.yticks([]) plt.text(0.5, -0.04, caption, ha='center', size=7) #plot
-plt.show() ``` [https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/
-man/figures/README-plot-1.png ] [W3Schools.com] API documentation -------------
----- You can locate our extensive API documentation here. This comprehensive
-guide is designed to walk you through our APIsâ functionalities, providing
-clear instructions on how to integrate and use them effectively. For each API,
-youâll find detailed descriptions, parameter information, example requests,
-and response formats to help you understand the APIâs purpose and
-functionality. Whether youâre interested in user authentication, data
-retrieval, or performing specific actions, our documentation has you covered.
-In addition, youâll find a section dedicated to âCommon Use Casesâ where
-we illustrate how our APIs can be combined and utilized in various scenarios.
-This can be an invaluable resource for those seeking to maximize the potential
-of our services. Please note that our API documentation is constantly updated
-with new features and improvements to ensure you have the latest information at
-your fingertips. Explore our API documentation today to get started with your
-integrations and to make the most out of our services!
+plt.show() ``` [https://raw.githubusercontent.com/EnvisionRisk/
+EnvisionRiskRaaS/master/man/figures/README-plot-1.png] .. image:: https://
+raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/
+README-plot-1.png API documentation ----------------- You can locate our
+extensive API documentation here. This comprehensive guide is designed to walk
+you through our APIsâ functionalities, providing clear instructions on how to
+integrate and use them effectively. For each API, youâll find detailed
+descriptions, parameter information, example requests, and response formats to
+help you understand the APIâs purpose and functionality. Whether youâre
+interested in user authentication, data retrieval, or performing specific
+actions, our documentation has you covered. In addition, youâll find a
+section dedicated to âCommon Use Casesâ where we illustrate how our APIs
+can be combined and utilized in various scenarios. This can be an invaluable
+resource for those seeking to maximize the potential of our services. Please
+note that our API documentation is constantly updated with new features and
+improvements to ensure you have the latest information at your fingertips.
+Explore our API documentation today to get started with your integrations and
+to make the most out of our services!
```

