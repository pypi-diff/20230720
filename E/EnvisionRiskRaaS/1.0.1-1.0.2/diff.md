# Comparing `tmp/envisionriskraas-1.0.1.tar.gz` & `tmp/envisionriskraas-1.0.2.tar.gz`

## Comparing `envisionriskraas-1.0.1.tar` & `envisionriskraas-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.1/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.1/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 envisionriskraas-1.0.1/README.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 envisionriskraas-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    86260 2020-02-02 00:00:00.000000 envisionriskraas-1.0.2/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 envisionriskraas-1.0.2/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 envisionriskraas-1.0.2/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 envisionriskraas-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 envisionriskraas-1.0.2/PKG-INFO
```

### Comparing `envisionriskraas-1.0.1/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.0.2/src/EnvisionRiskRaaS/RAAS.py`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.1/LICENSE.txt` & `envisionriskraas-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.0.1/README.md` & `envisionriskraas-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-#EnvisionRiskRaaS
+#EnvisionRiskRaaS\n
 Delve into the world of EnvisionRisk’s Python package, your portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our cutting-edge risk management services, retrieve relevant data, perform complex calculations, and generate actionable insights, all without leaving your Python programming environment. Embrace this smarter, efficient approach to handling market risk.
 
 Are you navigating the volatile waters of financial uncertainties, seeking to make strategic decisions? Allow EnvisionRisk’s Cloud Service to be your compass, providing a precise mechanism for quantifying market risks. Replace guesswork with certainty; our platform furnishes you with standardized metrics designed to enhance cost-efficiency and fortify your financial bulwark.
 
 Our REST API, a seamless blend of security and user-friendliness, stands as your reliable tool for everyday risk quantification. Transform data into actionable steps and unravel the potential concealed within the labyrinth of financial complexities.
 
 With an expansive coverage spanning more than 13,000 exchange-traded and over-the-counter instruments—and continuously growing—EnvisionRisk is primed to adapt to your ever-evolving needs.
 
 Join the EnvisionRisk community today. Convert your market insights into solid foresights, and consistently maintain a competitive edge in the ever-fluctuating financial market. Stay not just in the game, but ahead of it.
 
-##Authentication
+##Authentication\n
 EnvisionRisk employs robust authentication and authorization processes to safeguard systems and information. EnvisionRisk’s Market Risk-as-a-Service API operates on a token-based authentication system. To use the service you need to be a registered user. If you don’t already have credentials, you can sign up for a free trial account here:
 <a href='https://envisionrisk.shinyapps.io/user_management' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://camo.githubusercontent.com/e757b083ceb7645a42a28ce48d538a7c52808781191546a5cfe1bd6c37c7c677/68747470733a2f2f7777772e64726f70626f782e636f6d2f732f6330616f69363878686d70313132332f7369676e2d75702d627574746f6e2d706e672d33332e706e673f7261773d74727565' border='0' alt='Sign up' /></a>
 
-##Installation
+##Installation\n
 You can install the development version of EnvisionRiskRaaS like so:
 ```
-	pip install EnvisionRiskRaaS
+pip install EnvisionRiskRaaS
 ```
-##Example
+
+Example
+-------
+
 Although the following example may appear simple, it’s designed to illustrate how our service functions by requesting the simulated profit/loss (P/L) distribution for a single instrument — Apple (AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our service also allows you to request simulated P/L distribution for your custom portfolios. Through this, you gain invaluable insights into potential future outcomes, enabling you to make informed investment decisions.
 
 The Profit and Loss (P/L) distribution is a crucial component in the world of market risk management as it provides a quantitative way of understanding potential financial outcomes. Here’s why it plays an essential role:
 
 Risk Assessment: The P/L distribution represents the range of possible gains and losses that a portfolio might experience. It allows risk managers to visualize and quantify potential risks. For example, the tails of the distribution give insight into extreme events and potential for significant losses, enabling a comprehensive risk assessment.
 
 Risk Measures Calculation: Key risk measures, like Value at Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution. VaR estimates the potential loss a portfolio could face over a given period with a certain level of confidence, while ES provides the expected loss given that a loss exceeds the VaR threshold. These metrics help risk managers understand the risk landscape better and make informed decisions.
@@ -30,16 +33,18 @@
 Portfolio Optimization: By understanding the P/L distribution, managers can optimize the portfolio for desired outcomes. It allows them to adjust the portfolio composition to control the risk, striking a balance between risk and return.
 
 Regulatory Compliance: Regulators often require financial institutions to maintain capital reserves based on potential losses, which are derived from P/L distributions. Hence, understanding the P/L distribution is crucial to meet these regulatory requirements.
 
 Stress Testing: Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
 
 Therefore, P/L distribution serves as a key pillar of market risk management, providing insights into potential risks, informing decision-making, enabling portfolio optimization, and ensuring regulatory compliance.
-```
 
+
+
+```
 #### Get the delta vector (simulated price change) ####
 # The term '_raw' within the function name is indicative of a key feature: 
 # the simulated price changes are denominated in the same currency as 
 # the stock. This implies that the analysis maintains the original currency 
 # perspective of the stock, allowing for more accurate and relevant 
 # insights. It enhances ease of comprehension and direct applicability, 
 # bringing us closer to the context of the actual trading environment.
@@ -82,16 +87,20 @@
 plt.xlabel("Profit/Loss (in $)")
 plt.ylabel("Density")
 plt.yticks([])
 plt.text(0.5, -0.04, caption, ha='center', size=7)
 #plot
 plt.show()
 ```
-<img src="https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/man/figures/README-plot-1.png" height="400">
-##API documentation
+
+![Graph](https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/man/figures/README-plot-1.png "Graph")
+
+API documentation
+=================
+
 You can locate our extensive API documentation here. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
 
 For each API, you’ll find detailed descriptions, parameter information, example requests, and response formats to help you understand the API’s purpose and functionality. Whether you’re interested in user authentication, data retrieval, or performing specific actions, our documentation has you covered.
 
 In addition, you’ll find a section dedicated to ‘Common Use Cases’ where we illustrate how our APIs can be combined and utilized in various scenarios. This can be an invaluable resource for those seeking to maximize the potential of our services.
 
 Please note that our API documentation is constantly updated with new features and improvements to ensure you have the latest information at your fingertips.
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-#EnvisionRiskRaaS Delve into the world of EnvisionRiskâs Python package, your
-portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive
-tool allows you to tap into our cutting-edge risk management services, retrieve
-relevant data, perform complex calculations, and generate actionable insights,
-all without leaving your Python programming environment. Embrace this smarter,
-efficient approach to handling market risk. Are you navigating the volatile
-waters of financial uncertainties, seeking to make strategic decisions? Allow
-EnvisionRiskâs Cloud Service to be your compass, providing a precise
-mechanism for quantifying market risks. Replace guesswork with certainty; our
-platform furnishes you with standardized metrics designed to enhance cost-
-efficiency and fortify your financial bulwark. Our REST API, a seamless blend
-of security and user-friendliness, stands as your reliable tool for everyday
-risk quantification. Transform data into actionable steps and unravel the
-potential concealed within the labyrinth of financial complexities. With an
-expansive coverage spanning more than 13,000 exchange-traded and over-the-
-counter instrumentsâand continuously growingâEnvisionRisk is primed to
+#EnvisionRiskRaaS\n Delve into the world of EnvisionRiskâs Python package,
+your portal to our sophisticated Market Risk-as-a-Service (RaaS). This
+comprehensive tool allows you to tap into our cutting-edge risk management
+services, retrieve relevant data, perform complex calculations, and generate
+actionable insights, all without leaving your Python programming environment.
+Embrace this smarter, efficient approach to handling market risk. Are you
+navigating the volatile waters of financial uncertainties, seeking to make
+strategic decisions? Allow EnvisionRiskâs Cloud Service to be your compass,
+providing a precise mechanism for quantifying market risks. Replace guesswork
+with certainty; our platform furnishes you with standardized metrics designed
+to enhance cost-efficiency and fortify your financial bulwark. Our REST API, a
+seamless blend of security and user-friendliness, stands as your reliable tool
+for everyday risk quantification. Transform data into actionable steps and
+unravel the potential concealed within the labyrinth of financial complexities.
+With an expansive coverage spanning more than 13,000 exchange-traded and over-
+the-counter instrumentsâand continuously growingâEnvisionRisk is primed to
 adapt to your ever-evolving needs. Join the EnvisionRisk community today.
 Convert your market insights into solid foresights, and consistently maintain a
 competitive edge in the ever-fluctuating financial market. Stay not just in the
-game, but ahead of it. ##Authentication EnvisionRisk employs robust
+game, but ahead of it. ##Authentication\n EnvisionRisk employs robust
 authentication and authorization processes to safeguard systems and
 information. EnvisionRiskâs Market Risk-as-a-Service API operates on a token-
 based authentication system. To use the service you need to be a registered
 user. If you donât already have credentials, you can sign up for a free trial
-account here: [Sign_up] ##Installation You can install the development version
-of EnvisionRiskRaaS like so: ``` pip install EnvisionRiskRaaS ``` ##Example
-Although the following example may appear simple, itâs designed to illustrate
-how our service functions by requesting the simulated profit/loss (P/L)
-distribution for a single instrument â Apple (AAPL.US) as of 2023-06-28.
-Remember, this is just a starting point; our service also allows you to request
-simulated P/L distribution for your custom portfolios. Through this, you gain
-invaluable insights into potential future outcomes, enabling you to make
-informed investment decisions. The Profit and Loss (P/L) distribution is a
-crucial component in the world of market risk management as it provides a
+account here: [Sign_up] ##Installation\n You can install the development
+version of EnvisionRiskRaaS like so: ``` pip install EnvisionRiskRaaS ```
+Example ------- Although the following example may appear simple, itâs
+designed to illustrate how our service functions by requesting the simulated
+profit/loss (P/L) distribution for a single instrument â Apple (AAPL.US) as
+of 2023-06-28. Remember, this is just a starting point; our service also allows
+you to request simulated P/L distribution for your custom portfolios. Through
+this, you gain invaluable insights into potential future outcomes, enabling you
+to make informed investment decisions. The Profit and Loss (P/L) distribution
+is a crucial component in the world of market risk management as it provides a
 quantitative way of understanding potential financial outcomes. Hereâs why it
 plays an essential role: Risk Assessment: The P/L distribution represents the
 range of possible gains and losses that a portfolio might experience. It allows
 risk managers to visualize and quantify potential risks. For example, the tails
 of the distribution give insight into extreme events and potential for
 significant losses, enabling a comprehensive risk assessment. Risk Measures
 Calculation: Key risk measures, like Value at Risk (VaR) and Expected Shortfall
@@ -87,23 +87,24 @@
 plt.plot( xs, density(xs), color="#CA3542", alpha=0.5) plt.axvline(x =
 expected_shortfall_estimate, color = "#57575F", label = 'axvline - full
 height') #vertical line text, labels, remove tickers and insert caption
 plt.text(expected_shortfall_estimate, max(density(xs))/2, 'Expected-Shortfall
 (97.5%, 1 day)', ha='center', va='center',rotation='vertical',
 backgroundcolor='white') plt.xlabel("Profit/Loss (in $)") plt.ylabel("Density")
 plt.yticks([]) plt.text(0.5, -0.04, caption, ha='center', size=7) #plot
-plt.show() ``` [https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/
-man/figures/README-plot-1.png] ##API documentation You can locate our extensive
-API documentation here. This comprehensive guide is designed to walk you
-through our APIsâ functionalities, providing clear instructions on how to
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
+plt.show() ``` ![Graph](https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/
+master/man/figures/README-plot-1.png "Graph") API documentation
+================= You can locate our extensive API documentation here. This
+comprehensive guide is designed to walk you through our APIsâ
+functionalities, providing clear instructions on how to integrate and use them
+effectively. For each API, youâll find detailed descriptions, parameter
+information, example requests, and response formats to help you understand the
+APIâs purpose and functionality. Whether youâre interested in user
+authentication, data retrieval, or performing specific actions, our
+documentation has you covered. In addition, youâll find a section dedicated
+to âCommon Use Casesâ where we illustrate how our APIs can be combined and
+utilized in various scenarios. This can be an invaluable resource for those
+seeking to maximize the potential of our services. Please note that our API
+documentation is constantly updated with new features and improvements to
+ensure you have the latest information at your fingertips. Explore our API
+documentation today to get started with your integrations and to make the most
+out of our services!
```

### Comparing `envisionriskraas-1.0.1/pyproject.toml` & `envisionriskraas-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Jonas Hal", email="jonas.hal@envisionrisk.com" },
 ]
 description = "EnvisionRisk's Risk-as-a-service package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `envisionriskraas-1.0.1/PKG-INFO` & `envisionriskraas-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.0.1
+Version: 1.0.2
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
 
-#EnvisionRiskRaaS
+#EnvisionRiskRaaS\n
 Delve into the world of EnvisionRisk’s Python package, your portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our cutting-edge risk management services, retrieve relevant data, perform complex calculations, and generate actionable insights, all without leaving your Python programming environment. Embrace this smarter, efficient approach to handling market risk.
 
 Are you navigating the volatile waters of financial uncertainties, seeking to make strategic decisions? Allow EnvisionRisk’s Cloud Service to be your compass, providing a precise mechanism for quantifying market risks. Replace guesswork with certainty; our platform furnishes you with standardized metrics designed to enhance cost-efficiency and fortify your financial bulwark.
 
 Our REST API, a seamless blend of security and user-friendliness, stands as your reliable tool for everyday risk quantification. Transform data into actionable steps and unravel the potential concealed within the labyrinth of financial complexities.
 
 With an expansive coverage spanning more than 13,000 exchange-traded and over-the-counter instruments—and continuously growing—EnvisionRisk is primed to adapt to your ever-evolving needs.
 
 Join the EnvisionRisk community today. Convert your market insights into solid foresights, and consistently maintain a competitive edge in the ever-fluctuating financial market. Stay not just in the game, but ahead of it.
 
-##Authentication
+##Authentication\n
 EnvisionRisk employs robust authentication and authorization processes to safeguard systems and information. EnvisionRisk’s Market Risk-as-a-Service API operates on a token-based authentication system. To use the service you need to be a registered user. If you don’t already have credentials, you can sign up for a free trial account here:
 <a href='https://envisionrisk.shinyapps.io/user_management' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://camo.githubusercontent.com/e757b083ceb7645a42a28ce48d538a7c52808781191546a5cfe1bd6c37c7c677/68747470733a2f2f7777772e64726f70626f782e636f6d2f732f6330616f69363878686d70313132332f7369676e2d75702d627574746f6e2d706e672d33332e706e673f7261773d74727565' border='0' alt='Sign up' /></a>
 
-##Installation
+##Installation\n
 You can install the development version of EnvisionRiskRaaS like so:
 ```
-	pip install EnvisionRiskRaaS
+pip install EnvisionRiskRaaS
 ```
-##Example
+
+Example
+-------
+
 Although the following example may appear simple, it’s designed to illustrate how our service functions by requesting the simulated profit/loss (P/L) distribution for a single instrument — Apple (AAPL.US) as of 2023-06-28. Remember, this is just a starting point; our service also allows you to request simulated P/L distribution for your custom portfolios. Through this, you gain invaluable insights into potential future outcomes, enabling you to make informed investment decisions.
 
 The Profit and Loss (P/L) distribution is a crucial component in the world of market risk management as it provides a quantitative way of understanding potential financial outcomes. Here’s why it plays an essential role:
 
 Risk Assessment: The P/L distribution represents the range of possible gains and losses that a portfolio might experience. It allows risk managers to visualize and quantify potential risks. For example, the tails of the distribution give insight into extreme events and potential for significant losses, enabling a comprehensive risk assessment.
 
 Risk Measures Calculation: Key risk measures, like Value at Risk (VaR) and Expected Shortfall (ES), are derived from the P/L distribution. VaR estimates the potential loss a portfolio could face over a given period with a certain level of confidence, while ES provides the expected loss given that a loss exceeds the VaR threshold. These metrics help risk managers understand the risk landscape better and make informed decisions.
@@ -44,16 +47,18 @@
 Portfolio Optimization: By understanding the P/L distribution, managers can optimize the portfolio for desired outcomes. It allows them to adjust the portfolio composition to control the risk, striking a balance between risk and return.
 
 Regulatory Compliance: Regulators often require financial institutions to maintain capital reserves based on potential losses, which are derived from P/L distributions. Hence, understanding the P/L distribution is crucial to meet these regulatory requirements.
 
 Stress Testing: Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
 
 Therefore, P/L distribution serves as a key pillar of market risk management, providing insights into potential risks, informing decision-making, enabling portfolio optimization, and ensuring regulatory compliance.
-```
 
+
+
+```
 #### Get the delta vector (simulated price change) ####
 # The term '_raw' within the function name is indicative of a key feature: 
 # the simulated price changes are denominated in the same currency as 
 # the stock. This implies that the analysis maintains the original currency 
 # perspective of the stock, allowing for more accurate and relevant 
 # insights. It enhances ease of comprehension and direct applicability, 
 # bringing us closer to the context of the actual trading environment.
@@ -96,16 +101,20 @@
 plt.xlabel("Profit/Loss (in $)")
 plt.ylabel("Density")
 plt.yticks([])
 plt.text(0.5, -0.04, caption, ha='center', size=7)
 #plot
 plt.show()
 ```
-<img src="https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/man/figures/README-plot-1.png" height="400">
-##API documentation
+
+![Graph](https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/man/figures/README-plot-1.png "Graph")
+
+API documentation
+=================
+
 You can locate our extensive API documentation here. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
 
 For each API, you’ll find detailed descriptions, parameter information, example requests, and response formats to help you understand the API’s purpose and functionality. Whether you’re interested in user authentication, data retrieval, or performing specific actions, our documentation has you covered.
 
 In addition, you’ll find a section dedicated to ‘Common Use Cases’ where we illustrate how our APIs can be combined and utilized in various scenarios. This can be an invaluable resource for those seeking to maximize the potential of our services.
 
 Please note that our API documentation is constantly updated with new features and improvements to ensure you have the latest information at your fingertips.
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.0.2 Summary:
 EnvisionRisk's Risk-as-a-service package Project-URL: Homepage, https://
 www.envisionrisk.com/ Project-URL: GitHub profile, https://github.com/
 EnvisionRisk Author-email: Jonas Hal
 hal@envisionrisk.com> License-File: LICENSE.txt Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
-Description-Content-Type: text/markdown #EnvisionRiskRaaS Delve into the world
-of EnvisionRiskâs Python package, your portal to our sophisticated Market
-Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our
-cutting-edge risk management services, retrieve relevant data, perform complex
-calculations, and generate actionable insights, all without leaving your Python
-programming environment. Embrace this smarter, efficient approach to handling
-market risk. Are you navigating the volatile waters of financial uncertainties,
-seeking to make strategic decisions? Allow EnvisionRiskâs Cloud Service to be
-your compass, providing a precise mechanism for quantifying market risks.
-Replace guesswork with certainty; our platform furnishes you with standardized
-metrics designed to enhance cost-efficiency and fortify your financial bulwark.
-Our REST API, a seamless blend of security and user-friendliness, stands as
-your reliable tool for everyday risk quantification. Transform data into
-actionable steps and unravel the potential concealed within the labyrinth of
-financial complexities. With an expansive coverage spanning more than 13,000
-exchange-traded and over-the-counter instrumentsâand continuously
-growingâEnvisionRisk is primed to adapt to your ever-evolving needs. Join the
-EnvisionRisk community today. Convert your market insights into solid
-foresights, and consistently maintain a competitive edge in the ever-
+Description-Content-Type: text/markdown #EnvisionRiskRaaS\n Delve into the
+world of EnvisionRiskâs Python package, your portal to our sophisticated
+Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into
+our cutting-edge risk management services, retrieve relevant data, perform
+complex calculations, and generate actionable insights, all without leaving
+your Python programming environment. Embrace this smarter, efficient approach
+to handling market risk. Are you navigating the volatile waters of financial
+uncertainties, seeking to make strategic decisions? Allow EnvisionRiskâs
+Cloud Service to be your compass, providing a precise mechanism for quantifying
+market risks. Replace guesswork with certainty; our platform furnishes you with
+standardized metrics designed to enhance cost-efficiency and fortify your
+financial bulwark. Our REST API, a seamless blend of security and user-
+friendliness, stands as your reliable tool for everyday risk quantification.
+Transform data into actionable steps and unravel the potential concealed within
+the labyrinth of financial complexities. With an expansive coverage spanning
+more than 13,000 exchange-traded and over-the-counter instrumentsâand
+continuously growingâEnvisionRisk is primed to adapt to your ever-evolving
+needs. Join the EnvisionRisk community today. Convert your market insights into
+solid foresights, and consistently maintain a competitive edge in the ever-
 fluctuating financial market. Stay not just in the game, but ahead of it.
-##Authentication EnvisionRisk employs robust authentication and authorization
+##Authentication\n EnvisionRisk employs robust authentication and authorization
 processes to safeguard systems and information. EnvisionRiskâs Market Risk-
 as-a-Service API operates on a token-based authentication system. To use the
 service you need to be a registered user. If you donât already have
 credentials, you can sign up for a free trial account here: [Sign_up]
-##Installation You can install the development version of EnvisionRiskRaaS like
-so: ``` pip install EnvisionRiskRaaS ``` ##Example Although the following
-example may appear simple, itâs designed to illustrate how our service
-functions by requesting the simulated profit/loss (P/L) distribution for a
-single instrument â Apple (AAPL.US) as of 2023-06-28. Remember, this is just
-a starting point; our service also allows you to request simulated P/
+##Installation\n You can install the development version of EnvisionRiskRaaS
+like so: ``` pip install EnvisionRiskRaaS ``` Example ------- Although the
+following example may appear simple, itâs designed to illustrate how our
+service functions by requesting the simulated profit/loss (P/L) distribution
+for a single instrument â Apple (AAPL.US) as of 2023-06-28. Remember, this is
+just a starting point; our service also allows you to request simulated P/
 L distribution for your custom portfolios. Through this, you gain invaluable
 insights into potential future outcomes, enabling you to make informed
 investment decisions. The Profit and Loss (P/L) distribution is a crucial
 component in the world of market risk management as it provides a quantitative
 way of understanding potential financial outcomes. Hereâs why it plays an
 essential role: Risk Assessment: The P/L distribution represents the range of
 possible gains and losses that a portfolio might experience. It allows risk
@@ -95,23 +95,24 @@
 plt.plot( xs, density(xs), color="#CA3542", alpha=0.5) plt.axvline(x =
 expected_shortfall_estimate, color = "#57575F", label = 'axvline - full
 height') #vertical line text, labels, remove tickers and insert caption
 plt.text(expected_shortfall_estimate, max(density(xs))/2, 'Expected-Shortfall
 (97.5%, 1 day)', ha='center', va='center',rotation='vertical',
 backgroundcolor='white') plt.xlabel("Profit/Loss (in $)") plt.ylabel("Density")
 plt.yticks([]) plt.text(0.5, -0.04, caption, ha='center', size=7) #plot
-plt.show() ``` [https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/master/
-man/figures/README-plot-1.png] ##API documentation You can locate our extensive
-API documentation here. This comprehensive guide is designed to walk you
-through our APIsâ functionalities, providing clear instructions on how to
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
+plt.show() ``` ![Graph](https://github.com/EnvisionRisk/EnvisionRiskRaaS/blob/
+master/man/figures/README-plot-1.png "Graph") API documentation
+================= You can locate our extensive API documentation here. This
+comprehensive guide is designed to walk you through our APIsâ
+functionalities, providing clear instructions on how to integrate and use them
+effectively. For each API, youâll find detailed descriptions, parameter
+information, example requests, and response formats to help you understand the
+APIâs purpose and functionality. Whether youâre interested in user
+authentication, data retrieval, or performing specific actions, our
+documentation has you covered. In addition, youâll find a section dedicated
+to âCommon Use Casesâ where we illustrate how our APIs can be combined and
+utilized in various scenarios. This can be an invaluable resource for those
+seeking to maximize the potential of our services. Please note that our API
+documentation is constantly updated with new features and improvements to
+ensure you have the latest information at your fingertips. Explore our API
+documentation today to get started with your integrations and to make the most
+out of our services!
```

