# Comparing `tmp/nautobot_api_sandbox-0.1.1.tar.gz` & `tmp/nautobot_api_sandbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_api_sandbox-0.1.1.tar", max compression
+gzip compressed data, was "nautobot_api_sandbox-0.1.2.tar", max compression
```

## Comparing `nautobot_api_sandbox-0.1.1.tar` & `nautobot_api_sandbox-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1634 2023-07-20 16:23:55.677181 nautobot_api_sandbox-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/__init__.py
--rw-r--r--   0        0        0     4136 2023-07-20 16:19:50.697140 nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/nauto_demo_functions.py
--rw-r--r--   0        0        0     4583 2023-07-20 16:16:40.677109 nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
--rw-r--r--   0        0        0      606 2023-07-20 16:25:40.697200 nautobot_api_sandbox-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1634 2023-07-20 20:47:13.069848 nautobot_api_sandbox-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-17 21:52:11.544627 nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     2429 2023-07-20 20:46:46.869843 nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/click_ui.py
+-rw-r--r--   0        0        0     4439 2023-07-20 20:46:46.869843 nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/nauto_demo_functions.py
+-rw-r--r--   0        0        0     4600 2023-07-20 20:46:46.869843 nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/nautobot_api_sandbox_ui.py
+-rw-r--r--   0        0        0      656 2023-07-20 20:48:28.399861 nautobot_api_sandbox-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 nautobot_api_sandbox-0.1.2/PKG-INFO
```

### Comparing `nautobot_api_sandbox-0.1.1/README.md` & `nautobot_api_sandbox-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/nauto_demo_functions.py` & `nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/nauto_demo_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,28 +75,35 @@
                 raise
         return tenant
 
     def get_tenant(self, name):
         """Return the tenant with the specified name, or raise TenantNotFoundError if the tenant does not exist."""
         tenant = self.api.tenancy.tenants.get(name=name)
         if tenant is None:
-            raise TenantNotFoundError("Tenant with name '%s' not found.", name)
+            raise TenantNotFoundError("Tenant with name '%s' not found." % name)
         return tenant
 
+    def display_tenant(self, name):
+        """Display the ID and name of the tenant with the specified name."""
+        try:
+            tenant = self.get_tenant(name)
+            self.logger.info("Tenant ID: %s\nTenant Name: %s", tenant.id, tenant.name)
+        except TenantNotFoundError:
+            self.logger.error("Tenant '%s' not found. Please enter a valid tenant name.", name)
+
     def delete_tenant(self, name):
         """Delete the tenant with the specified name."""
-        tenant = self.get_tenant(name)
-        if tenant is not None:
-            try:
-                tenant.delete()
-                return True, "Tenant '%s' deleted successfully!" % name
-            except pynautobot.core.query.RequestError as request_error:
-                return False, "Failed to delete tenant '%s'. Error: %s" % (name, request_error)
-        else:
-            raise TenantNotFoundError("Tenant with name '%s' not found.", name)
+        try:
+            tenant = self.get_tenant(name)
+            tenant.delete()
+            return True, "Tenant '%s' deleted successfully!" % name
+        except TenantNotFoundError:
+            raise
+        except pynautobot.core.query.RequestError as request_error:
+            return False, "Failed to delete tenant '%s'. Error: %s" % (name, request_error)
 
     def get_tenants(self):
         """Return a list of all tenants."""
         return self.api.tenancy.tenants.all()
 
     def display_tenants(self):
         """Display the names of all tenants."""
```

### Comparing `nautobot_api_sandbox-0.1.1/nautobot_api_sandbox/nautobot_api_sandbox_ui.py` & `nautobot_api_sandbox-0.1.2/nautobot_api_sandbox/nautobot_api_sandbox_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,25 +39,25 @@
         try:
             nautobot_client = DemoNautobotClient(api_token=api_token)
             nautobot_client.api.dcim.sites.all()  # Make a simple request to check if the token is valid
             break
         except RequestError:
             logger.error("Invalid API token. Please try again.")
 
-    print(WELCOME_MSG)
+    logger.info(WELCOME_MSG)  # Use logger.info instead of print
 
     # Commands that need an argument
     commands_with_arg = ["show_devices", "create_tenant", "delete_tenant", "get_tenant"]
 
     while True:
         command_input = input("Enter a command: ").split()
         command = command_input[0].lower()  # Convert command to lowercase
         arg = " ".join(command_input[1:])  # Join all items after the command with a space
 
-        if command == "create_tenant" or command == "delete_tenant":
+        if command == "create_tenant" or command == "delete_tenant" or command == "get_tenant":
             tenant_name = arg  # Store the tenant name without modifying capitalization
         else:
             # Process the argument based on its length
             if len(arg) <= 5:
                 arg = arg.upper()  # Convert to uppercase if length is 5 or less
             else:
                 arg = arg.title()  # Convert to title case if more than one word
@@ -79,29 +79,29 @@
             if tenant is None:
                 logger.error("A tenant with the name '%s' already exists.", tenant_name)
             else:
                 logger.info("Tenant '%s' created successfully.", tenant_name)
         elif command == "delete_tenant":
             try:
                 success, message = nautobot_client.delete_tenant(arg)
-                if not success:
+                if success:
+                    logger.info(message)
+                else:
                     logger.error(message)
-            except TenantNotFoundError:
-                logger.error("Tenant '%s' not found. Please enter a valid tenant name.", arg)
+            except TenantNotFoundError as e:
+                logger.error(str(e))
         elif command == "show_tenants":
             nautobot_client.display_tenants()
         elif command == "get_tenant":
             try:
-                tenant = nautobot_client.get_tenant(arg)
-                if tenant is not None:
-                    logger.info("Tenant ID: %s\nTenant Name: %s", tenant.id, tenant.name)
+                nautobot_client.display_tenant(arg)  # Use the display_tenant method
             except TenantNotFoundError:
                 logger.error("Tenant '%s' not found. Please enter a valid tenant name.", arg)
         elif command == "help":
-            print(WELCOME_MSG)
+            logger.info(WELCOME_MSG)  # Use logger.info instead of print
         elif command == "exit":
             break
         else:
             logger.error("Unrecognized command. Type 'help' to see the list of available commands.")
 
 
 if __name__ == "__main__":
```

### Comparing `nautobot_api_sandbox-0.1.1/pyproject.toml` & `nautobot_api_sandbox-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "nautobot_api_sandbox"
-version = "0.1.1"
+version = "0.1.2"
 description = "This is just a simple program to test my programing knowledge and to learn more about API and Nautobot."
 authors = ["tPayne0647"]
 readme = "README.md"
 packages = [{include = "nautobot_api_sandbox"}]
 
 [tool.poetry.scripts]
 nautobot_api_sandbox = "nautobot_api_sandbox.nautobot_api_sandbox_ui:user_interface"
-
+nauto_click = "nautobot_api_sandbox.click_ui:main"
 [tool.poetry.dependencies]
 python = "^3.9"
 pynautobot = "1.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 pytest = "7.4.0"
```

### Comparing `nautobot_api_sandbox-0.1.1/PKG-INFO` & `nautobot_api_sandbox-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-api-sandbox
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is just a simple program to test my programing knowledge and to learn more about API and Nautobot.
 Author: tPayne0647
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

