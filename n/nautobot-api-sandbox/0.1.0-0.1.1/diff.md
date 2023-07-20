# Comparing `tmp/nautobot_api_sandbox-0.1.0.tar.gz` & `tmp/nautobot_api_sandbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_api_sandbox-0.1.0.tar", max compression
+gzip compressed data, was "nautobot_api_sandbox-0.1.1.tar", max compression
```

## Comparing `nautobot_api_sandbox-0.1.0.tar` & `nautobot_api_sandbox-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1443 2023-07-20 00:44:25.039568 nautobot_api_sandbox-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-18 01:52:28.578529 nautobot_api_sandbox-0.1.0/nautobot_api_sandbox/__init__.py
--rw-r--r--   0        0        0     3947 2023-07-20 00:44:08.069568 nautobot_api_sandbox-0.1.0/nautobot_api_sandbox/nauto_demo_functions.py
--rw-r--r--   0        0        0     4490 2023-07-20 00:44:08.069568 nautobot_api_sandbox-0.1.0/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
--rw-r--r--   0        0        0      606 2023-07-20 00:44:08.069568 nautobot_api_sandbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1634 2023-07-20 16:23:55.677181 nautobot_api_sandbox-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/__init__.py
+-rw-r--r--   0        0        0     4136 2023-07-20 16:19:50.697140 nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/nauto_demo_functions.py
+-rw-r--r--   0        0        0     4583 2023-07-20 16:16:40.677109 nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
+-rw-r--r--   0        0        0      606 2023-07-20 16:25:40.697200 nautobot_api_sandbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.1/PKG-INFO
```

### Comparing `nautobot_api_sandbox-0.1.0/nautobot_api_sandbox/nauto_demo_functions.py` & `nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/nauto_demo_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,19 @@
             raise TenantNotFoundError("Tenant with name '%s' not found.", name)
         return tenant
 
     def delete_tenant(self, name):
         """Delete the tenant with the specified name."""
         tenant = self.get_tenant(name)
         if tenant is not None:
-            tenant.delete()
-            self.logger.info("Tenant '%s' deleted successfully!", name)
+            try:
+                tenant.delete()
+                return True, "Tenant '%s' deleted successfully!" % name
+            except pynautobot.core.query.RequestError as request_error:
+                return False, "Failed to delete tenant '%s'. Error: %s" % (name, request_error)
         else:
             raise TenantNotFoundError("Tenant with name '%s' not found.", name)
 
     def get_tenants(self):
         """Return a list of all tenants."""
         return self.api.tenancy.tenants.all()
```

### Comparing `nautobot_api_sandbox-0.1.0/nautobot_api_sandbox/nautobot_api_sandbox_ui.py` & `nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/nautobot_api_sandbox_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,17 @@
             tenant = nautobot_client.create_tenant(tenant_name)
             if tenant is None:
                 logger.error("A tenant with the name '%s' already exists.", tenant_name)
             else:
                 logger.info("Tenant '%s' created successfully.", tenant_name)
         elif command == "delete_tenant":
             try:
-                nautobot_client.delete_tenant(arg)
+                success, message = nautobot_client.delete_tenant(arg)
+                if not success:
+                    logger.error(message)
             except TenantNotFoundError:
                 logger.error("Tenant '%s' not found. Please enter a valid tenant name.", arg)
         elif command == "show_tenants":
             nautobot_client.display_tenants()
         elif command == "get_tenant":
             try:
                 tenant = nautobot_client.get_tenant(arg)
```

### Comparing `nautobot_api_sandbox-0.1.0/pyproject.toml` & `nautobot_api_sandbox-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot_api_sandbox"
-version = "0.1.0"
+version = "0.1.1"
 description = "This is just a simple program to test my programing knowledge and to learn more about API and Nautobot."
 authors = ["tPayne0647"]
 readme = "README.md"
 packages = [{include = "nautobot_api_sandbox"}]
 
 [tool.poetry.scripts]
 nautobot_api_sandbox = "nautobot_api_sandbox.nautobot_api_sandbox_ui:user_interface"
```

### Comparing `nautobot_api_sandbox-0.1.0/PKG-INFO` & `nautobot_api_sandbox-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,50 @@
-Metadata-Version: 2.1
-Name: nautobot-api-sandbox
-Version: 0.1.0
-Summary: This is just a simple program to test my programing knowledge and to learn more about API and Nautobot.
-Author: tPayne0647
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pynautobot (==1.5.0)
-Description-Content-Type: text/markdown
-
 # Nautobot API Sandbox
 
-This is a simple program to test my programming knowledge and learn more about API and Nautobot.
+This is a simple program to test my programming knowledge and learn more about API, Nautobot, and developing in general.
+
+https://demo.nautobot.com/
+
+## Getting Started
 
-## Prerequisites
+1. Install package: `pip install nautobot_api_sandbox`
+2. Run package: `nautobot_api_sandbox`
+3. Enter Demo token: `aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa`
+
+   This will start the Nautobot API Sandbox command-line interface.
+   Follow the instructions in the application to interact with the Nautobot API.
+   NOTE: You don't need to add '()' or "" quotes. Simply type the command + the name (e.g., create_tenant tpayne, show_devices atl01).
+
+
+## Development Prerequisites
 
 Before getting started, make sure you have the following installed on your machine:
 
 - Python 3.9 or later
 - Poetry
-
-## Getting Started
+## Development
 
 1. Clone the repository: `git clone git@github.com:tPayne0647/nautobot-api-sandbox.git`
 2. Navigate to the project directory: `cd nautobot-api-sandbox`
 3. Install the project dependencies using Poetry: `poetry install`
+4. Install the development dependencies: `poetry install --dev`
 4. Activate the virtual environment created by Poetry: `poetry shell`
 5. Run the program: `nautobot_api_sandbox`
 
-Demo token: aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
-
-   This will start the Nautobot API Sandbox command-line interface.
-   Follow the instructions in the application to interact with the Nautobot API.
-   NOTE: You don't need to add '()' or "" quotes. Simply type the command + the name (e.g., create_tenant tpayne, show_devices atl01).
-
-## Development
-
-If you're contributing to the project or want to run tests, make sure to install the development dependencies as well: `poetry install --dev`
 To run the tests: `poetry run pytest`
 
-Any help or tips would be awesome!
+Any help or tips would be greatly appreciated!!
 
 ## Currently Working On / Want to Add
 
-- Exception handling? Need to learn more about how these work exactly...
-- Valid unittest?
-- Integrate click?
-- Make sure using logging correctly
-- Poetry integration
-- publish application?
+- [ ] Exception handling?
+- [ ] Valid unittest? Need more tests...
+- [ ] Integrate click? really want to rework UI
+- [ ] Make sure using logging correctly
+- [x] Fix delete_tenant RequestError 409
+- [x] Update readme instructions
+- [x] Poetry integration
+- [x] Publish package
 
-This is a work in progress!!!
 
+This is a work in progress!!!
```

