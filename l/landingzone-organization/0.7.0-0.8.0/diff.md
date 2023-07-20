# Comparing `tmp/landingzone_organization-0.7.0.tar.gz` & `tmp/landingzone_organization-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingzone_organization-0.7.0.tar", max compression
+gzip compressed data, was "landingzone_organization-0.8.0.tar", max compression
```

## Comparing `landingzone_organization-0.7.0.tar` & `landingzone_organization-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0      981 2023-07-17 14:30:47.168590 landingzone_organization-0.7.0/README.md
--rw-r--r--   0        0        0      777 2023-07-17 14:30:47.924592 landingzone_organization-0.7.0/landingzone_organization/__init__.py
--rw-r--r--   0        0        0      532 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/account.py
--rw-r--r--   0        0        0       75 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/adapters/__init__.py
--rw-r--r--   0        0        0     3248 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/adapters/aws_organization.py
--rw-r--r--   0        0        0      509 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/commands/__init__.py
--rw-r--r--   0        0        0     1220 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/commands/account.py
--rw-r--r--   0        0        0      885 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/commands/export.py
--rw-r--r--   0        0        0      558 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/commands/organization.py
--rw-r--r--   0        0        0     2096 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/commands/profiles.py
--rw-r--r--   0        0        0      707 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/commands/workload.py
--rw-r--r--   0        0        0     1637 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/context.py
--rw-r--r--   0        0        0      744 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/cli/handler.py
--rw-r--r--   0        0        0      955 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/filtering.py
--rw-r--r--   0        0        0     1035 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/group.py
--rw-r--r--   0        0        0      929 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/groups.py
--rw-r--r--   0        0        0     3220 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/organization.py
--rw-r--r--   0        0        0      938 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/organization_unit.py
--rw-r--r--   0        0        0      917 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/profile.py
--rw-r--r--   0        0        0     1164 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/profiles.py
--rw-r--r--   0        0        0     1055 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/workload.py
--rw-r--r--   0        0        0     1828 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/workload_generator.py
--rw-r--r--   0        0        0     1559 2023-07-17 14:30:47.172590 landingzone_organization-0.7.0/landingzone_organization/workloads.py
--rw-r--r--   0        0        0     1386 2023-07-17 14:30:47.924592 landingzone_organization-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 landingzone_organization-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-20 19:13:05.191419 landingzone_organization-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0      981 2023-07-20 19:13:05.191419 landingzone_organization-0.8.0/README.md
+-rw-r--r--   0        0        0      797 2023-07-20 19:13:06.143424 landingzone_organization-0.8.0/landingzone_organization/__init__.py
+-rw-r--r--   0        0        0      561 2023-07-20 19:13:05.191419 landingzone_organization-0.8.0/landingzone_organization/account.py
+-rw-r--r--   0        0        0       75 2023-07-20 19:13:05.191419 landingzone_organization-0.8.0/landingzone_organization/adapters/__init__.py
+-rw-r--r--   0        0        0     3248 2023-07-20 19:13:05.191419 landingzone_organization-0.8.0/landingzone_organization/adapters/aws_organization.py
+-rw-r--r--   0        0        0      509 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1252 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/commands/account.py
+-rw-r--r--   0        0        0      901 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/commands/export.py
+-rw-r--r--   0        0        0      574 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/commands/organization.py
+-rw-r--r--   0        0        0     2112 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/commands/profiles.py
+-rw-r--r--   0        0        0      723 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/commands/workload.py
+-rw-r--r--   0        0        0     1637 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/context.py
+-rw-r--r--   0        0        0      744 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/cli/handler.py
+-rw-r--r--   0        0        0      955 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/filtering.py
+-rw-r--r--   0        0        0     1071 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/group.py
+-rw-r--r--   0        0        0      929 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/groups.py
+-rw-r--r--   0        0        0     3151 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/organization.py
+-rw-r--r--   0        0        0      938 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/organization_unit.py
+-rw-r--r--   0        0        0      917 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/profile.py
+-rw-r--r--   0        0        0     1186 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/profiles.py
+-rw-r--r--   0        0        0     1102 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/schemas/__init__.py
+-rw-r--r--   0        0        0      140 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/schemas/environment.yaml
+-rw-r--r--   0        0        0      190 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/schemas/workload.yaml
+-rw-r--r--   0        0        0     1296 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/workload.py
+-rw-r--r--   0        0        0     1828 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/workload_generator.py
+-rw-r--r--   0        0        0     2968 2023-07-20 19:13:05.195419 landingzone_organization-0.8.0/landingzone_organization/workloads.py
+-rw-r--r--   0        0        0     1405 2023-07-20 19:13:06.143424 landingzone_organization-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 landingzone_organization-0.8.0/PKG-INFO
```

### Comparing `landingzone_organization-0.7.0/README.md` & `landingzone_organization-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/__init__.py` & `landingzone_organization-0.8.0/landingzone_organization/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from landingzone_organization.workload import Workload
 from landingzone_organization.account import Account
 from landingzone_organization.groups import Groups
 from landingzone_organization.group import Group
 from landingzone_organization.profile import Profile
 from landingzone_organization.profiles import Profiles
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 __all__ = [
-    AWSOrganization,
-    Organization,
-    OrganizationUnit,
-    Workloads,
-    Workload,
-    Account,
-    Groups,
-    Group,
-    Profile,
-    Profiles,
+    "AWSOrganization",
+    "Organization",
+    "OrganizationUnit",
+    "Workloads",
+    "Workload",
+    "Account",
+    "Groups",
+    "Group",
+    "Profile",
+    "Profiles",
 ]
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/account.py` & `landingzone_organization-0.8.0/landingzone_organization/account.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
     @property
     def environment(self) -> Optional[str]:
         return resolve_account_environment(self.name)
 
     @property
     def weight(self) -> int:
-        return resolve_account_weight(self.environment)
+        return resolve_account_weight(self.environment) if self.environment else 100
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/adapters/aws_organization.py` & `landingzone_organization-0.8.0/landingzone_organization/adapters/aws_organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/cli/commands/account.py` & `landingzone_organization-0.8.0/landingzone_organization/cli/commands/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 @click.group()
 def cli():
     """Perform account operations"""
     pass
 
 
-@cli.command()
+@cli.command()  # type: ignore
 @click.argument("account-id")
 @click.pass_obj
 def view(ctx: Context, account_id: str):
     """List all workloads"""
     account = ctx.organization.by_account_id(account_id)
 
     if account:
         click.echo(f"Account ID  : {account.account_id}")
         click.echo(f"Name        : {account.name}")
         click.echo(f"Environment : {account.environment}")
     else:
         click.echo(f"The {account_id} is not known to this organization.")
 
 
-@cli.command()
+@cli.command()  # type: ignore
 @click.argument("output")
 @click.pass_obj
 def export(ctx: Context, output: str):
     """List all workloads"""
     perform_export(output, ctx.organization.accounts([]))
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/cli/commands/export.py` & `landingzone_organization-0.8.0/landingzone_organization/cli/commands/export.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 @click.group()
 def cli():
     """Perform profiles operations"""
     pass
 
 
-@cli.command()
+@cli.command()  # type: ignore
 @click.argument("config-path")
 @click.argument("ou-path")
 @click.pass_obj
 def workloads(ctx: Context, config_path: str, ou_path: str) -> None:
     """
     Export the workloads in the supplied path
     """
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/cli/commands/organization.py` & `landingzone_organization-0.8.0/landingzone_organization/cli/commands/organization.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @click.group()
 def cli():
     """Perform organization operations"""
     pass
 
 
-@cli.command()
+@cli.command()  # type: ignore
 @click.pass_obj
 def download(ctx: Context):
     """Download the organization structure"""
     click.echo(f"Download organization information")
     organization = AWSOrganization(ctx.session).parse()
 
     with open(ctx.data_file, "w") as fh:
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/cli/commands/profiles.py` & `landingzone_organization-0.8.0/landingzone_organization/cli/commands/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 @click.group()
 def cli():
     """Perform profiles operations"""
     pass
 
 
-@cli.command()
+@cli.command()  # type: ignore
 @click.argument("organization-name")
 @click.option("--sso-start-url", prompt="SSO start URL")
 @click.option("--sso-region", prompt="SSO region")
 @click.option("--role-session-name", prompt="SSO session name")
 @click.option("--sso-role-name", prompt="SSO role name")
 @click.pass_obj
 def generate(
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/cli/context.py` & `landingzone_organization-0.8.0/landingzone_organization/cli/context.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/cli/handler.py` & `landingzone_organization-0.8.0/landingzone_organization/cli/handler.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/filtering.py` & `landingzone_organization-0.8.0/landingzone_organization/filtering.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/group.py` & `landingzone_organization-0.8.0/landingzone_organization/group.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     _organization: Optional[Organization] = None
 
     @property
     def accounts(self) -> List[Account]:
         if not self._organization:
             return []
 
-        unit: Union[Organization, OrganizationUnit] = self._organization
+        champion: Union[Organization, OrganizationUnit] = self._organization
 
         for ou in self.organizational_unit:
-            unit = unit.by_name(ou)
+            challenger = champion.by_name(ou)
 
-            if not unit:
-                break
+            if challenger:
+                champion = challenger
 
-        return unit.accounts if unit else []
+        return champion.accounts  # type: ignore
 
     def organization(self, organization: Organization) -> None:
         self._organization = organization
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/groups.py` & `landingzone_organization-0.8.0/landingzone_organization/groups.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/organization.py` & `landingzone_organization-0.8.0/landingzone_organization/organization.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,56 +19,54 @@
     id: str
     unit: OrganizationUnit
 
     @property
     def accounts_recursive(self) -> List[Account]:
         return self.unit.accounts_recursive
 
-    def by_name(self, name: str) -> OrganizationUnit:
+    def by_name(self, name: str) -> Optional[OrganizationUnit]:
         return self.unit.by_name(name)
 
     def by_account_id(self, account_id: str) -> Optional[Account]:
         return next(filter(lambda account: account.account_id == account_id, self.accounts_recursive), None)  # type: ignore
 
     def __resolve_organization_unit(
         self, ou_names: List[str]
     ) -> Optional[OrganizationUnit]:
         unit = self.unit
 
         for ou_name in ou_names:
             unit = unit.by_name(ou_name)
 
             if not unit:
-                break
+                return None
 
         return unit
 
     def accounts(self, ou_names: List[str] = []) -> List[Account]:
         unit = self.__resolve_organization_unit(ou_names) or self.unit
         return unit.accounts_recursive
 
-    def workloads(self, ou_names: List[str]) -> Optional[Workloads]:
+    def workloads(self, ou_names: List[str]) -> Workloads:
         workloads = Workloads(workloads=[])
-        unit = self.unit
-
-        if len(ou_names) > 0:
-            unit = self.__resolve_organization_unit(ou_names)
+        unit = self.__resolve_organization_unit(ou_names)
 
         if unit:
             for account in unit.accounts_recursive:
                 if match_workload_pattern(account.name):
                     workloads.resolve_account(account)
 
         return workloads
 
     @property
     def platform_accounts(self) -> List[Account]:
-        workload_accounts = self.workloads(ou_names=[]).accounts
+        workloads = self.workloads(ou_names=[])
+
         workload_account_ids = list(
-            map(lambda account: account.account_id, workload_accounts)
+            map(lambda account: account.account_id, workloads.accounts)
         )
 
         def not_a_workload_account(account: Account):
             return account.account_id not in workload_account_ids
 
         return list(filter(not_a_workload_account, self.accounts_recursive))
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/organization_unit.py` & `landingzone_organization-0.8.0/landingzone_organization/organization_unit.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/profile.py` & `landingzone_organization-0.8.0/landingzone_organization/profile.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/profiles.py` & `landingzone_organization-0.8.0/landingzone_organization/profiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class Profiles:
     def __init__(self, config_file: str):
         self.__config_file = config_file
         self.__config = configparser.ConfigParser()
         self.__config.read(config_file)
-        self.__client_errors = {}
+        self.__client_errors: Dict[str, Exception] = {}
 
     @property
     def names(self) -> List[str]:
         def extract_profile_name(section: str) -> str:
             return section.split(" ")[-1]
 
         return list(map(extract_profile_name, self.__config.sections()))
```

### Comparing `landingzone_organization-0.7.0/landingzone_organization/workload_generator.py` & `landingzone_organization-0.8.0/landingzone_organization/workload_generator.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.7.0/landingzone_organization/workloads.py` & `landingzone_organization-0.8.0/landingzone_organization/workload.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 from __future__ import annotations
-from typing import List, Optional, Set
+from typing import List, Optional
 
 from landingzone_organization.account import Account
-from landingzone_organization.workload import Workload
-from landingzone_organization.filtering import resolve_workload_name
 
 
-class Workloads:
-    def __init__(self, workloads: List[Workload]) -> None:
-        self.__index = 0
-        self.__workloads = workloads
+class Workload:
+    def __init__(
+        self, name: str, display_name: Optional[str], accounts: List[Account]
+    ) -> None:
+        self.__name = name
+        self.__display_name = display_name
+        self.__accounts = accounts
 
-    def __len__(self) -> int:
-        return len(self.__workloads)
-
-    def __iter__(self):
-        for workload in self.__workloads:
-            yield workload
+    @property
+    def name(self) -> str:
+        return self.__name
 
     @property
-    def names(self) -> Set[str]:
-        return set(map(lambda workload: workload.name, self.__workloads))
+    def display_name(self) -> Optional[str]:
+        return self.__display_name
 
     @property
     def accounts(self) -> List[Account]:
-        accounts = []
-
-        for workload in self.__workloads:
-            accounts.extend(workload.accounts)
-
-        return accounts
+        return sorted(self.__accounts, key=lambda x: x.weight)
 
     @property
-    def environments(self) -> Set[str]:
-        environments = set()
-
-        for workload in self.__workloads:
-            environments.update(workload.environments)
-
-        return environments
-
-    def resolve_account(self, account: Account) -> None:
-        workload_name = resolve_workload_name(account.name)
-        workload = self.by_name(workload_name)
-
-        if not workload:
-            self.__workloads.append(Workload(name=workload_name, accounts=[account]))
-        else:
-            workload.append(account)
+    def environments(self) -> List[str]:
+        return list(map(lambda account: str(account.environment), self.accounts))
 
-    def by_name(self, name: str) -> Optional[Workload]:
-        return next(filter(lambda w: w.name == name, self.__workloads), None)  # type: ignore
+    def by_environment(self, name: str) -> Optional[Account]:
+        def match(account: Account):
+            return account.environment == name
+
+        return next(filter(match, self.accounts), None)  # type: ignore
+
+    def append(self, account: Account) -> None:
+        self.__accounts.append(account)
+
+    @staticmethod
+    def from_dict(data: dict, accounts: List[Account]) -> Workload:
+        return Workload(
+            name=data["Name"], display_name=data.get("DisplayName"), accounts=accounts
+        )
```

### Comparing `landingzone_organization-0.7.0/pyproject.toml` & `landingzone_organization-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "landingzone-organization"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 readme = "README.md"
 homepage = "https://binxio.github.io/landingzone-organization/"
 documentation = "https://binxio.github.io/landingzone-organization/3-user-documentation/"
 repository = "https://github.com/binxio/landingzone-organization"
 packages = [{include = "landingzone_organization"}]
@@ -20,29 +20,29 @@
 build_command = "pip install poetry && poetry build"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.26.83"
 click = "^8.1.3"
 jsonpickle = "^3.0.1"
+jsonschema = "^4.18.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.scripts]
+landingzone-organization = "landingzone_organization.cli:cli"
+
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 black = "^23.1.0"
 radon = "^5.1.0"
 xenon = "^0.9.0"
 mypy = "^1.4.1"
 aws-sam-cli = "^1.90.0"
-
-[tool.poetry.scripts]
-landingzone-organization = "landingzone_organization.cli:cli"
-
-[tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
+types-pyyaml = "^6.0.12.10"
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.coverage.run]
 branch = true
 source = ["aws_iam_login"]
```

### Comparing `landingzone_organization-0.7.0/PKG-INFO` & `landingzone_organization-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: landingzone-organization
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Home-page: https://binxio.github.io/landingzone-organization/
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.83,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jsonpickle (>=3.0.1,<4.0.0)
+Requires-Dist: jsonschema (>=4.18.3,<5.0.0)
 Project-URL: Documentation, https://binxio.github.io/landingzone-organization/3-user-documentation/
 Project-URL: Repository, https://github.com/binxio/landingzone-organization
 Description-Content-Type: text/markdown
 
 # landingzone-organization
 
 [![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://github.com/Nr18/pull-request-codecommit/graphs/commit-activity)
```

