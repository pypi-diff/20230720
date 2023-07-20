# Comparing `tmp/port_pulumi-1.0.0.tar.gz` & `tmp/port_pulumi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-1.0.0.tar", last modified: Wed Jul 12 17:52:59 2023, max compression
+gzip compressed data, was "port_pulumi-1.1.0.tar", last modified: Thu Jul 20 12:37:50 2023, max compression
```

## Comparing `port_pulumi-1.0.0.tar` & `port_pulumi-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70602 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33763 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    34831 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    55056 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:52:59.706423 port_pulumi-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-12 17:52:59.000000 port_pulumi-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:50.054244 port_pulumi-1.1.0/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98686 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36131 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34831 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79853 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/setup.py
```

### Comparing `port_pulumi-1.0.0/PKG-INFO` & `port_pulumi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port_pulumi
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `port_pulumi-1.0.0/README.md` & `port_pulumi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.0.0/port_pulumi/__init__.py` & `port_pulumi-1.1.0/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.0.0/port_pulumi/_inputs.py` & `port_pulumi-1.1.0/port_pulumi/_inputs.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,25 +10,41 @@
 from . import _utilities
 
 __all__ = [
     'ActionApprovalEmailNotificationArgs',
     'ActionApprovalWebhookNotificationArgs',
     'ActionAzureMethodArgs',
     'ActionGithubMethodArgs',
+    'ActionGitlabMethodArgs',
     'ActionKafkaMethodArgs',
     'ActionUserPropertiesArgs',
     'ActionUserPropertiesArrayPropsArgs',
     'ActionUserPropertiesArrayPropsBooleanItemsArgs',
+    'ActionUserPropertiesArrayPropsDatasetArgs',
+    'ActionUserPropertiesArrayPropsDatasetRuleArgs',
+    'ActionUserPropertiesArrayPropsDatasetRuleValueArgs',
     'ActionUserPropertiesArrayPropsNumberItemsArgs',
     'ActionUserPropertiesArrayPropsObjectItemsArgs',
     'ActionUserPropertiesArrayPropsStringItemsArgs',
     'ActionUserPropertiesBooleanPropsArgs',
+    'ActionUserPropertiesBooleanPropsDatasetArgs',
+    'ActionUserPropertiesBooleanPropsDatasetRuleArgs',
+    'ActionUserPropertiesBooleanPropsDatasetRuleValueArgs',
     'ActionUserPropertiesNumberPropsArgs',
+    'ActionUserPropertiesNumberPropsDatasetArgs',
+    'ActionUserPropertiesNumberPropsDatasetRuleArgs',
+    'ActionUserPropertiesNumberPropsDatasetRuleValueArgs',
     'ActionUserPropertiesObjectPropsArgs',
+    'ActionUserPropertiesObjectPropsDatasetArgs',
+    'ActionUserPropertiesObjectPropsDatasetRuleArgs',
+    'ActionUserPropertiesObjectPropsDatasetRuleValueArgs',
     'ActionUserPropertiesStringPropsArgs',
+    'ActionUserPropertiesStringPropsDatasetArgs',
+    'ActionUserPropertiesStringPropsDatasetRuleArgs',
+    'ActionUserPropertiesStringPropsDatasetRuleValueArgs',
     'ActionWebhookMethodArgs',
     'BlueprintCalculationPropertiesArgs',
     'BlueprintKafkaChangelogDestinationArgs',
     'BlueprintMirrorPropertiesArgs',
     'BlueprintPropertiesArgs',
     'BlueprintPropertiesArrayPropsArgs',
     'BlueprintPropertiesArrayPropsBooleanItemsArgs',
@@ -168,14 +184,89 @@
 
     @report_workflow_status.setter
     def report_workflow_status(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "report_workflow_status", value)
 
 
 @pulumi.input_type
+class ActionGitlabMethodArgs:
+    def __init__(__self__, *,
+                 group_name: pulumi.Input[str],
+                 project_name: pulumi.Input[str],
+                 agent: Optional[pulumi.Input[bool]] = None,
+                 default_ref: Optional[pulumi.Input[str]] = None,
+                 omit_payload: Optional[pulumi.Input[bool]] = None,
+                 omit_user_inputs: Optional[pulumi.Input[bool]] = None):
+        pulumi.set(__self__, "group_name", group_name)
+        pulumi.set(__self__, "project_name", project_name)
+        if agent is not None:
+            pulumi.set(__self__, "agent", agent)
+        if default_ref is not None:
+            pulumi.set(__self__, "default_ref", default_ref)
+        if omit_payload is not None:
+            pulumi.set(__self__, "omit_payload", omit_payload)
+        if omit_user_inputs is not None:
+            pulumi.set(__self__, "omit_user_inputs", omit_user_inputs)
+
+    @property
+    @pulumi.getter(name="groupName")
+    def group_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "group_name")
+
+    @group_name.setter
+    def group_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "group_name", value)
+
+    @property
+    @pulumi.getter(name="projectName")
+    def project_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "project_name")
+
+    @project_name.setter
+    def project_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project_name", value)
+
+    @property
+    @pulumi.getter
+    def agent(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "agent")
+
+    @agent.setter
+    def agent(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "agent", value)
+
+    @property
+    @pulumi.getter(name="defaultRef")
+    def default_ref(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "default_ref")
+
+    @default_ref.setter
+    def default_ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_ref", value)
+
+    @property
+    @pulumi.getter(name="omitPayload")
+    def omit_payload(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "omit_payload")
+
+    @omit_payload.setter
+    def omit_payload(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "omit_payload", value)
+
+    @property
+    @pulumi.getter(name="omitUserInputs")
+    def omit_user_inputs(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "omit_user_inputs")
+
+    @omit_user_inputs.setter
+    def omit_user_inputs(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "omit_user_inputs", value)
+
+
+@pulumi.input_type
 class ActionKafkaMethodArgs:
     def __init__(__self__):
         pass
 
 
 @pulumi.input_type
 class ActionUserPropertiesArgs:
@@ -242,25 +333,34 @@
         pulumi.set(self, "string_props", value)
 
 
 @pulumi.input_type
 class ActionUserPropertiesArrayPropsArgs:
     def __init__(__self__, *,
                  boolean_items: Optional[pulumi.Input['ActionUserPropertiesArrayPropsBooleanItemsArgs']] = None,
+                 dataset: Optional[pulumi.Input['ActionUserPropertiesArrayPropsDatasetArgs']] = None,
+                 default_jq_query: Optional[pulumi.Input[str]] = None,
+                 depends_ons: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  max_items: Optional[pulumi.Input[int]] = None,
                  min_items: Optional[pulumi.Input[int]] = None,
                  number_items: Optional[pulumi.Input['ActionUserPropertiesArrayPropsNumberItemsArgs']] = None,
                  object_items: Optional[pulumi.Input['ActionUserPropertiesArrayPropsObjectItemsArgs']] = None,
                  required: Optional[pulumi.Input[bool]] = None,
                  string_items: Optional[pulumi.Input['ActionUserPropertiesArrayPropsStringItemsArgs']] = None,
                  title: Optional[pulumi.Input[str]] = None):
         if boolean_items is not None:
             pulumi.set(__self__, "boolean_items", boolean_items)
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if max_items is not None:
             pulumi.set(__self__, "max_items", max_items)
         if min_items is not None:
@@ -283,14 +383,41 @@
 
     @boolean_items.setter
     def boolean_items(self, value: Optional[pulumi.Input['ActionUserPropertiesArrayPropsBooleanItemsArgs']]):
         pulumi.set(self, "boolean_items", value)
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional[pulumi.Input['ActionUserPropertiesArrayPropsDatasetArgs']]:
+        return pulumi.get(self, "dataset")
+
+    @dataset.setter
+    def dataset(self, value: Optional[pulumi.Input['ActionUserPropertiesArrayPropsDatasetArgs']]):
+        pulumi.set(self, "dataset", value)
+
+    @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "default_jq_query")
+
+    @default_jq_query.setter
+    def default_jq_query(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_jq_query", value)
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "depends_ons")
+
+    @depends_ons.setter
+    def depends_ons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "depends_ons", value)
+
+    @property
+    @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -381,14 +508,108 @@
 
     @defaults.setter
     def defaults(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[bool]]]]):
         pulumi.set(self, "defaults", value)
 
 
 @pulumi.input_type
+class ActionUserPropertiesArrayPropsDatasetArgs:
+    def __init__(__self__, *,
+                 combinator: pulumi.Input[str],
+                 rules: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesArrayPropsDatasetRuleArgs']]]):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "combinator")
+
+    @combinator.setter
+    def combinator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "combinator", value)
+
+    @property
+    @pulumi.getter
+    def rules(self) -> pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesArrayPropsDatasetRuleArgs']]]:
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesArrayPropsDatasetRuleArgs']]]):
+        pulumi.set(self, "rules", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesArrayPropsDatasetRuleArgs:
+    def __init__(__self__, *,
+                 operator: pulumi.Input[str],
+                 value: pulumi.Input['ActionUserPropertiesArrayPropsDatasetRuleValueArgs'],
+                 blueprint: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input['ActionUserPropertiesArrayPropsDatasetRuleValueArgs']:
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input['ActionUserPropertiesArrayPropsDatasetRuleValueArgs']):
+        pulumi.set(self, "value", value)
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "blueprint")
+
+    @blueprint.setter
+    def blueprint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blueprint", value)
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "property")
+
+    @property.setter
+    def property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesArrayPropsDatasetRuleValueArgs:
+    def __init__(__self__, *,
+                 jq_query: pulumi.Input[str]):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "jq_query")
+
+    @jq_query.setter
+    def jq_query(self, value: pulumi.Input[str]):
+        pulumi.set(self, "jq_query", value)
+
+
+@pulumi.input_type
 class ActionUserPropertiesArrayPropsNumberItemsArgs:
     def __init__(__self__, *,
                  defaults: Optional[pulumi.Input[Sequence[pulumi.Input[float]]]] = None):
         if defaults is not None:
             pulumi.set(__self__, "defaults", defaults)
 
     @property
@@ -458,40 +679,76 @@
     def format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "format", value)
 
 
 @pulumi.input_type
 class ActionUserPropertiesBooleanPropsArgs:
     def __init__(__self__, *,
+                 dataset: Optional[pulumi.Input['ActionUserPropertiesBooleanPropsDatasetArgs']] = None,
                  default: Optional[pulumi.Input[bool]] = None,
+                 default_jq_query: Optional[pulumi.Input[str]] = None,
+                 depends_ons: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  required: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None):
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
         if default is not None:
             pulumi.set(__self__, "default", default)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if required is not None:
             pulumi.set(__self__, "required", required)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional[pulumi.Input['ActionUserPropertiesBooleanPropsDatasetArgs']]:
+        return pulumi.get(self, "dataset")
+
+    @dataset.setter
+    def dataset(self, value: Optional[pulumi.Input['ActionUserPropertiesBooleanPropsDatasetArgs']]):
+        pulumi.set(self, "dataset", value)
+
+    @property
+    @pulumi.getter
     def default(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "default")
 
     @default.setter
     def default(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "default", value)
 
     @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "default_jq_query")
+
+    @default_jq_query.setter
+    def default_jq_query(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_jq_query", value)
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "depends_ons")
+
+    @depends_ons.setter
+    def depends_ons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "depends_ons", value)
+
+    @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
@@ -521,28 +778,134 @@
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
 @pulumi.input_type
+class ActionUserPropertiesBooleanPropsDatasetArgs:
+    def __init__(__self__, *,
+                 combinator: pulumi.Input[str],
+                 rules: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesBooleanPropsDatasetRuleArgs']]]):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "combinator")
+
+    @combinator.setter
+    def combinator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "combinator", value)
+
+    @property
+    @pulumi.getter
+    def rules(self) -> pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesBooleanPropsDatasetRuleArgs']]]:
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesBooleanPropsDatasetRuleArgs']]]):
+        pulumi.set(self, "rules", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesBooleanPropsDatasetRuleArgs:
+    def __init__(__self__, *,
+                 operator: pulumi.Input[str],
+                 value: pulumi.Input['ActionUserPropertiesBooleanPropsDatasetRuleValueArgs'],
+                 blueprint: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input['ActionUserPropertiesBooleanPropsDatasetRuleValueArgs']:
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input['ActionUserPropertiesBooleanPropsDatasetRuleValueArgs']):
+        pulumi.set(self, "value", value)
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "blueprint")
+
+    @blueprint.setter
+    def blueprint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blueprint", value)
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "property")
+
+    @property.setter
+    def property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesBooleanPropsDatasetRuleValueArgs:
+    def __init__(__self__, *,
+                 jq_query: pulumi.Input[str]):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "jq_query")
+
+    @jq_query.setter
+    def jq_query(self, value: pulumi.Input[str]):
+        pulumi.set(self, "jq_query", value)
+
+
+@pulumi.input_type
 class ActionUserPropertiesNumberPropsArgs:
     def __init__(__self__, *,
+                 dataset: Optional[pulumi.Input['ActionUserPropertiesNumberPropsDatasetArgs']] = None,
                  default: Optional[pulumi.Input[float]] = None,
+                 default_jq_query: Optional[pulumi.Input[str]] = None,
+                 depends_ons: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 enum_jq_query: Optional[pulumi.Input[str]] = None,
                  enums: Optional[pulumi.Input[Sequence[pulumi.Input[float]]]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  maximum: Optional[pulumi.Input[float]] = None,
                  minimum: Optional[pulumi.Input[float]] = None,
                  required: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None):
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
         if default is not None:
             pulumi.set(__self__, "default", default)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if enum_jq_query is not None:
+            pulumi.set(__self__, "enum_jq_query", enum_jq_query)
         if enums is not None:
             pulumi.set(__self__, "enums", enums)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if maximum is not None:
             pulumi.set(__self__, "maximum", maximum)
         if minimum is not None:
@@ -550,31 +913,67 @@
         if required is not None:
             pulumi.set(__self__, "required", required)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional[pulumi.Input['ActionUserPropertiesNumberPropsDatasetArgs']]:
+        return pulumi.get(self, "dataset")
+
+    @dataset.setter
+    def dataset(self, value: Optional[pulumi.Input['ActionUserPropertiesNumberPropsDatasetArgs']]):
+        pulumi.set(self, "dataset", value)
+
+    @property
+    @pulumi.getter
     def default(self) -> Optional[pulumi.Input[float]]:
         return pulumi.get(self, "default")
 
     @default.setter
     def default(self, value: Optional[pulumi.Input[float]]):
         pulumi.set(self, "default", value)
 
     @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "default_jq_query")
+
+    @default_jq_query.setter
+    def default_jq_query(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_jq_query", value)
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "depends_ons")
+
+    @depends_ons.setter
+    def depends_ons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "depends_ons", value)
+
+    @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="enumJqQuery")
+    def enum_jq_query(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "enum_jq_query")
+
+    @enum_jq_query.setter
+    def enum_jq_query(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "enum_jq_query", value)
+
+    @property
     @pulumi.getter
     def enums(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[float]]]]:
         return pulumi.get(self, "enums")
 
     @enums.setter
     def enums(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[float]]]]):
         pulumi.set(self, "enums", value)
@@ -622,42 +1021,172 @@
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
 @pulumi.input_type
+class ActionUserPropertiesNumberPropsDatasetArgs:
+    def __init__(__self__, *,
+                 combinator: pulumi.Input[str],
+                 rules: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesNumberPropsDatasetRuleArgs']]]):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "combinator")
+
+    @combinator.setter
+    def combinator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "combinator", value)
+
+    @property
+    @pulumi.getter
+    def rules(self) -> pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesNumberPropsDatasetRuleArgs']]]:
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesNumberPropsDatasetRuleArgs']]]):
+        pulumi.set(self, "rules", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesNumberPropsDatasetRuleArgs:
+    def __init__(__self__, *,
+                 operator: pulumi.Input[str],
+                 value: pulumi.Input['ActionUserPropertiesNumberPropsDatasetRuleValueArgs'],
+                 blueprint: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input['ActionUserPropertiesNumberPropsDatasetRuleValueArgs']:
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input['ActionUserPropertiesNumberPropsDatasetRuleValueArgs']):
+        pulumi.set(self, "value", value)
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "blueprint")
+
+    @blueprint.setter
+    def blueprint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blueprint", value)
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "property")
+
+    @property.setter
+    def property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesNumberPropsDatasetRuleValueArgs:
+    def __init__(__self__, *,
+                 jq_query: pulumi.Input[str]):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "jq_query")
+
+    @jq_query.setter
+    def jq_query(self, value: pulumi.Input[str]):
+        pulumi.set(self, "jq_query", value)
+
+
+@pulumi.input_type
 class ActionUserPropertiesObjectPropsArgs:
     def __init__(__self__, *,
+                 dataset: Optional[pulumi.Input['ActionUserPropertiesObjectPropsDatasetArgs']] = None,
                  default: Optional[pulumi.Input[str]] = None,
+                 default_jq_query: Optional[pulumi.Input[str]] = None,
+                 depends_ons: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  required: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None):
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
         if default is not None:
             pulumi.set(__self__, "default", default)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if required is not None:
             pulumi.set(__self__, "required", required)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional[pulumi.Input['ActionUserPropertiesObjectPropsDatasetArgs']]:
+        return pulumi.get(self, "dataset")
+
+    @dataset.setter
+    def dataset(self, value: Optional[pulumi.Input['ActionUserPropertiesObjectPropsDatasetArgs']]):
+        pulumi.set(self, "dataset", value)
+
+    @property
+    @pulumi.getter
     def default(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "default")
 
     @default.setter
     def default(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default", value)
 
     @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "default_jq_query")
+
+    @default_jq_query.setter
+    def default_jq_query(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_jq_query", value)
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "depends_ons")
+
+    @depends_ons.setter
+    def depends_ons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "depends_ons", value)
+
+    @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
@@ -687,33 +1216,139 @@
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
 @pulumi.input_type
+class ActionUserPropertiesObjectPropsDatasetArgs:
+    def __init__(__self__, *,
+                 combinator: pulumi.Input[str],
+                 rules: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesObjectPropsDatasetRuleArgs']]]):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "combinator")
+
+    @combinator.setter
+    def combinator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "combinator", value)
+
+    @property
+    @pulumi.getter
+    def rules(self) -> pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesObjectPropsDatasetRuleArgs']]]:
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesObjectPropsDatasetRuleArgs']]]):
+        pulumi.set(self, "rules", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesObjectPropsDatasetRuleArgs:
+    def __init__(__self__, *,
+                 operator: pulumi.Input[str],
+                 value: pulumi.Input['ActionUserPropertiesObjectPropsDatasetRuleValueArgs'],
+                 blueprint: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input['ActionUserPropertiesObjectPropsDatasetRuleValueArgs']:
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input['ActionUserPropertiesObjectPropsDatasetRuleValueArgs']):
+        pulumi.set(self, "value", value)
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "blueprint")
+
+    @blueprint.setter
+    def blueprint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blueprint", value)
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "property")
+
+    @property.setter
+    def property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesObjectPropsDatasetRuleValueArgs:
+    def __init__(__self__, *,
+                 jq_query: pulumi.Input[str]):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "jq_query")
+
+    @jq_query.setter
+    def jq_query(self, value: pulumi.Input[str]):
+        pulumi.set(self, "jq_query", value)
+
+
+@pulumi.input_type
 class ActionUserPropertiesStringPropsArgs:
     def __init__(__self__, *,
                  blueprint: Optional[pulumi.Input[str]] = None,
+                 dataset: Optional[pulumi.Input['ActionUserPropertiesStringPropsDatasetArgs']] = None,
                  default: Optional[pulumi.Input[str]] = None,
+                 default_jq_query: Optional[pulumi.Input[str]] = None,
+                 depends_ons: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
+                 enum_jq_query: Optional[pulumi.Input[str]] = None,
                  enums: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  format: Optional[pulumi.Input[str]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  max_length: Optional[pulumi.Input[int]] = None,
                  min_length: Optional[pulumi.Input[int]] = None,
                  pattern: Optional[pulumi.Input[str]] = None,
                  required: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None):
         if blueprint is not None:
             pulumi.set(__self__, "blueprint", blueprint)
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
         if default is not None:
             pulumi.set(__self__, "default", default)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if enum_jq_query is not None:
+            pulumi.set(__self__, "enum_jq_query", enum_jq_query)
         if enums is not None:
             pulumi.set(__self__, "enums", enums)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if max_length is not None:
@@ -734,31 +1369,67 @@
 
     @blueprint.setter
     def blueprint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "blueprint", value)
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional[pulumi.Input['ActionUserPropertiesStringPropsDatasetArgs']]:
+        return pulumi.get(self, "dataset")
+
+    @dataset.setter
+    def dataset(self, value: Optional[pulumi.Input['ActionUserPropertiesStringPropsDatasetArgs']]):
+        pulumi.set(self, "dataset", value)
+
+    @property
+    @pulumi.getter
     def default(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "default")
 
     @default.setter
     def default(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default", value)
 
     @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "default_jq_query")
+
+    @default_jq_query.setter
+    def default_jq_query(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_jq_query", value)
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "depends_ons")
+
+    @depends_ons.setter
+    def depends_ons(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "depends_ons", value)
+
+    @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
+    @pulumi.getter(name="enumJqQuery")
+    def enum_jq_query(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "enum_jq_query")
+
+    @enum_jq_query.setter
+    def enum_jq_query(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "enum_jq_query", value)
+
+    @property
     @pulumi.getter
     def enums(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         return pulumi.get(self, "enums")
 
     @enums.setter
     def enums(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "enums", value)
@@ -824,14 +1495,108 @@
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
 @pulumi.input_type
+class ActionUserPropertiesStringPropsDatasetArgs:
+    def __init__(__self__, *,
+                 combinator: pulumi.Input[str],
+                 rules: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesStringPropsDatasetRuleArgs']]]):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "combinator")
+
+    @combinator.setter
+    def combinator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "combinator", value)
+
+    @property
+    @pulumi.getter
+    def rules(self) -> pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesStringPropsDatasetRuleArgs']]]:
+        return pulumi.get(self, "rules")
+
+    @rules.setter
+    def rules(self, value: pulumi.Input[Sequence[pulumi.Input['ActionUserPropertiesStringPropsDatasetRuleArgs']]]):
+        pulumi.set(self, "rules", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesStringPropsDatasetRuleArgs:
+    def __init__(__self__, *,
+                 operator: pulumi.Input[str],
+                 value: pulumi.Input['ActionUserPropertiesStringPropsDatasetRuleValueArgs'],
+                 blueprint: Optional[pulumi.Input[str]] = None,
+                 property: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: pulumi.Input[str]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input['ActionUserPropertiesStringPropsDatasetRuleValueArgs']:
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input['ActionUserPropertiesStringPropsDatasetRuleValueArgs']):
+        pulumi.set(self, "value", value)
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "blueprint")
+
+    @blueprint.setter
+    def blueprint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blueprint", value)
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "property")
+
+    @property.setter
+    def property(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "property", value)
+
+
+@pulumi.input_type
+class ActionUserPropertiesStringPropsDatasetRuleValueArgs:
+    def __init__(__self__, *,
+                 jq_query: pulumi.Input[str]):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "jq_query")
+
+    @jq_query.setter
+    def jq_query(self, value: pulumi.Input[str]):
+        pulumi.set(self, "jq_query", value)
+
+
+@pulumi.input_type
 class ActionWebhookMethodArgs:
     def __init__(__self__, *,
                  url: pulumi.Input[str],
                  agent: Optional[pulumi.Input[bool]] = None):
         pulumi.set(__self__, "url", url)
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
```

### Comparing `port_pulumi-1.0.0/port_pulumi/_utilities.py` & `port_pulumi-1.1.0/port_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.0.0/port_pulumi/action.py` & `port_pulumi-1.1.0/port_pulumi/action.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,14 +21,15 @@
                  title: pulumi.Input[str],
                  trigger: pulumi.Input[str],
                  approval_email_notification: Optional[pulumi.Input['ActionApprovalEmailNotificationArgs']] = None,
                  approval_webhook_notification: Optional[pulumi.Input['ActionApprovalWebhookNotificationArgs']] = None,
                  azure_method: Optional[pulumi.Input['ActionAzureMethodArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input['ActionGithubMethodArgs']] = None,
+                 gitlab_method: Optional[pulumi.Input['ActionGitlabMethodArgs']] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input['ActionKafkaMethodArgs']] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
                  user_properties: Optional[pulumi.Input['ActionUserPropertiesArgs']] = None,
                  webhook_method: Optional[pulumi.Input['ActionWebhookMethodArgs']] = None):
         """
         The set of arguments for constructing a Action resource.
@@ -37,14 +38,15 @@
         :param pulumi.Input[str] title: Title
         :param pulumi.Input[str] trigger: The trigger type of the action
         :param pulumi.Input['ActionApprovalEmailNotificationArgs'] approval_email_notification: The email notification of the approval
         :param pulumi.Input['ActionApprovalWebhookNotificationArgs'] approval_webhook_notification: The webhook notification of the approval
         :param pulumi.Input['ActionAzureMethodArgs'] azure_method: The invocation method of the action
         :param pulumi.Input[str] description: Description
         :param pulumi.Input['ActionGithubMethodArgs'] github_method: The invocation method of the action
+        :param pulumi.Input['ActionGitlabMethodArgs'] gitlab_method: The invocation method of the action
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input['ActionKafkaMethodArgs'] kafka_method: The invocation method of the action
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
         :param pulumi.Input['ActionUserPropertiesArgs'] user_properties: User properties
         :param pulumi.Input['ActionWebhookMethodArgs'] webhook_method: The invocation method of the action
         """
         pulumi.set(__self__, "blueprint", blueprint)
@@ -57,14 +59,16 @@
             pulumi.set(__self__, "approval_webhook_notification", approval_webhook_notification)
         if azure_method is not None:
             pulumi.set(__self__, "azure_method", azure_method)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if github_method is not None:
             pulumi.set(__self__, "github_method", github_method)
+        if gitlab_method is not None:
+            pulumi.set(__self__, "gitlab_method", gitlab_method)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if kafka_method is not None:
             pulumi.set(__self__, "kafka_method", kafka_method)
         if required_approval is not None:
             pulumi.set(__self__, "required_approval", required_approval)
         if user_properties is not None:
@@ -177,14 +181,26 @@
         return pulumi.get(self, "github_method")
 
     @github_method.setter
     def github_method(self, value: Optional[pulumi.Input['ActionGithubMethodArgs']]):
         pulumi.set(self, "github_method", value)
 
     @property
+    @pulumi.getter(name="gitlabMethod")
+    def gitlab_method(self) -> Optional[pulumi.Input['ActionGitlabMethodArgs']]:
+        """
+        The invocation method of the action
+        """
+        return pulumi.get(self, "gitlab_method")
+
+    @gitlab_method.setter
+    def gitlab_method(self, value: Optional[pulumi.Input['ActionGitlabMethodArgs']]):
+        pulumi.set(self, "gitlab_method", value)
+
+    @property
     @pulumi.getter
     def icon(self) -> Optional[pulumi.Input[str]]:
         """
         Icon
         """
         return pulumi.get(self, "icon")
 
@@ -246,14 +262,15 @@
     def __init__(__self__, *,
                  approval_email_notification: Optional[pulumi.Input['ActionApprovalEmailNotificationArgs']] = None,
                  approval_webhook_notification: Optional[pulumi.Input['ActionApprovalWebhookNotificationArgs']] = None,
                  azure_method: Optional[pulumi.Input['ActionAzureMethodArgs']] = None,
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input['ActionGithubMethodArgs']] = None,
+                 gitlab_method: Optional[pulumi.Input['ActionGitlabMethodArgs']] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input['ActionKafkaMethodArgs']] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  trigger: Optional[pulumi.Input[str]] = None,
                  user_properties: Optional[pulumi.Input['ActionUserPropertiesArgs']] = None,
@@ -262,14 +279,15 @@
         Input properties used for looking up and filtering Action resources.
         :param pulumi.Input['ActionApprovalEmailNotificationArgs'] approval_email_notification: The email notification of the approval
         :param pulumi.Input['ActionApprovalWebhookNotificationArgs'] approval_webhook_notification: The webhook notification of the approval
         :param pulumi.Input['ActionAzureMethodArgs'] azure_method: The invocation method of the action
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
         :param pulumi.Input['ActionGithubMethodArgs'] github_method: The invocation method of the action
+        :param pulumi.Input['ActionGitlabMethodArgs'] gitlab_method: The invocation method of the action
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
         :param pulumi.Input['ActionKafkaMethodArgs'] kafka_method: The invocation method of the action
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
         :param pulumi.Input[str] title: Title
         :param pulumi.Input[str] trigger: The trigger type of the action
         :param pulumi.Input['ActionUserPropertiesArgs'] user_properties: User properties
@@ -283,14 +301,16 @@
             pulumi.set(__self__, "azure_method", azure_method)
         if blueprint is not None:
             pulumi.set(__self__, "blueprint", blueprint)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if github_method is not None:
             pulumi.set(__self__, "github_method", github_method)
+        if gitlab_method is not None:
+            pulumi.set(__self__, "gitlab_method", gitlab_method)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if identifier is not None:
             pulumi.set(__self__, "identifier", identifier)
         if kafka_method is not None:
             pulumi.set(__self__, "kafka_method", kafka_method)
         if required_approval is not None:
@@ -373,14 +393,26 @@
         return pulumi.get(self, "github_method")
 
     @github_method.setter
     def github_method(self, value: Optional[pulumi.Input['ActionGithubMethodArgs']]):
         pulumi.set(self, "github_method", value)
 
     @property
+    @pulumi.getter(name="gitlabMethod")
+    def gitlab_method(self) -> Optional[pulumi.Input['ActionGitlabMethodArgs']]:
+        """
+        The invocation method of the action
+        """
+        return pulumi.get(self, "gitlab_method")
+
+    @gitlab_method.setter
+    def gitlab_method(self, value: Optional[pulumi.Input['ActionGitlabMethodArgs']]):
+        pulumi.set(self, "gitlab_method", value)
+
+    @property
     @pulumi.getter
     def icon(self) -> Optional[pulumi.Input[str]]:
         """
         Icon
         """
         return pulumi.get(self, "icon")
 
@@ -480,14 +512,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  approval_email_notification: Optional[pulumi.Input[pulumi.InputType['ActionApprovalEmailNotificationArgs']]] = None,
                  approval_webhook_notification: Optional[pulumi.Input[pulumi.InputType['ActionApprovalWebhookNotificationArgs']]] = None,
                  azure_method: Optional[pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']]] = None,
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
+                 gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  trigger: Optional[pulumi.Input[str]] = None,
                  user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
@@ -499,14 +532,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ActionApprovalEmailNotificationArgs']] approval_email_notification: The email notification of the approval
         :param pulumi.Input[pulumi.InputType['ActionApprovalWebhookNotificationArgs']] approval_webhook_notification: The webhook notification of the approval
         :param pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']] azure_method: The invocation method of the action
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
         :param pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']] github_method: The invocation method of the action
+        :param pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']] gitlab_method: The invocation method of the action
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
         :param pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']] kafka_method: The invocation method of the action
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
         :param pulumi.Input[str] title: Title
         :param pulumi.Input[str] trigger: The trigger type of the action
         :param pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']] user_properties: User properties
@@ -537,14 +571,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  approval_email_notification: Optional[pulumi.Input[pulumi.InputType['ActionApprovalEmailNotificationArgs']]] = None,
                  approval_webhook_notification: Optional[pulumi.Input[pulumi.InputType['ActionApprovalWebhookNotificationArgs']]] = None,
                  azure_method: Optional[pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']]] = None,
                  blueprint: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
+                 gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
                  icon: Optional[pulumi.Input[str]] = None,
                  identifier: Optional[pulumi.Input[str]] = None,
                  kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
                  required_approval: Optional[pulumi.Input[bool]] = None,
                  title: Optional[pulumi.Input[str]] = None,
                  trigger: Optional[pulumi.Input[str]] = None,
                  user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
@@ -562,14 +597,15 @@
             __props__.__dict__["approval_webhook_notification"] = approval_webhook_notification
             __props__.__dict__["azure_method"] = azure_method
             if blueprint is None and not opts.urn:
                 raise TypeError("Missing required property 'blueprint'")
             __props__.__dict__["blueprint"] = blueprint
             __props__.__dict__["description"] = description
             __props__.__dict__["github_method"] = github_method
+            __props__.__dict__["gitlab_method"] = gitlab_method
             __props__.__dict__["icon"] = icon
             if identifier is None and not opts.urn:
                 raise TypeError("Missing required property 'identifier'")
             __props__.__dict__["identifier"] = identifier
             __props__.__dict__["kafka_method"] = kafka_method
             __props__.__dict__["required_approval"] = required_approval
             if title is None and not opts.urn:
@@ -592,14 +628,15 @@
             opts: Optional[pulumi.ResourceOptions] = None,
             approval_email_notification: Optional[pulumi.Input[pulumi.InputType['ActionApprovalEmailNotificationArgs']]] = None,
             approval_webhook_notification: Optional[pulumi.Input[pulumi.InputType['ActionApprovalWebhookNotificationArgs']]] = None,
             azure_method: Optional[pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']]] = None,
             blueprint: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             github_method: Optional[pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']]] = None,
+            gitlab_method: Optional[pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']]] = None,
             icon: Optional[pulumi.Input[str]] = None,
             identifier: Optional[pulumi.Input[str]] = None,
             kafka_method: Optional[pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']]] = None,
             required_approval: Optional[pulumi.Input[bool]] = None,
             title: Optional[pulumi.Input[str]] = None,
             trigger: Optional[pulumi.Input[str]] = None,
             user_properties: Optional[pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']]] = None,
@@ -613,14 +650,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ActionApprovalEmailNotificationArgs']] approval_email_notification: The email notification of the approval
         :param pulumi.Input[pulumi.InputType['ActionApprovalWebhookNotificationArgs']] approval_webhook_notification: The webhook notification of the approval
         :param pulumi.Input[pulumi.InputType['ActionAzureMethodArgs']] azure_method: The invocation method of the action
         :param pulumi.Input[str] blueprint: The blueprint identifier the action relates to
         :param pulumi.Input[str] description: Description
         :param pulumi.Input[pulumi.InputType['ActionGithubMethodArgs']] github_method: The invocation method of the action
+        :param pulumi.Input[pulumi.InputType['ActionGitlabMethodArgs']] gitlab_method: The invocation method of the action
         :param pulumi.Input[str] icon: Icon
         :param pulumi.Input[str] identifier: Identifier
         :param pulumi.Input[pulumi.InputType['ActionKafkaMethodArgs']] kafka_method: The invocation method of the action
         :param pulumi.Input[bool] required_approval: Require approval before invoking the action
         :param pulumi.Input[str] title: Title
         :param pulumi.Input[str] trigger: The trigger type of the action
         :param pulumi.Input[pulumi.InputType['ActionUserPropertiesArgs']] user_properties: User properties
@@ -632,14 +670,15 @@
 
         __props__.__dict__["approval_email_notification"] = approval_email_notification
         __props__.__dict__["approval_webhook_notification"] = approval_webhook_notification
         __props__.__dict__["azure_method"] = azure_method
         __props__.__dict__["blueprint"] = blueprint
         __props__.__dict__["description"] = description
         __props__.__dict__["github_method"] = github_method
+        __props__.__dict__["gitlab_method"] = gitlab_method
         __props__.__dict__["icon"] = icon
         __props__.__dict__["identifier"] = identifier
         __props__.__dict__["kafka_method"] = kafka_method
         __props__.__dict__["required_approval"] = required_approval
         __props__.__dict__["title"] = title
         __props__.__dict__["trigger"] = trigger
         __props__.__dict__["user_properties"] = user_properties
@@ -691,14 +730,22 @@
     def github_method(self) -> pulumi.Output[Optional['outputs.ActionGithubMethod']]:
         """
         The invocation method of the action
         """
         return pulumi.get(self, "github_method")
 
     @property
+    @pulumi.getter(name="gitlabMethod")
+    def gitlab_method(self) -> pulumi.Output[Optional['outputs.ActionGitlabMethod']]:
+        """
+        The invocation method of the action
+        """
+        return pulumi.get(self, "gitlab_method")
+
+    @property
     @pulumi.getter
     def icon(self) -> pulumi.Output[Optional[str]]:
         """
         Icon
         """
         return pulumi.get(self, "icon")
```

### Comparing `port_pulumi-1.0.0/port_pulumi/blueprint.py` & `port_pulumi-1.1.0/port_pulumi/blueprint.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.0.0/port_pulumi/config/vars.py` & `port_pulumi-1.1.0/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.0.0/port_pulumi/entity.py` & `port_pulumi-1.1.0/port_pulumi/entity.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.0.0/port_pulumi/outputs.py` & `port_pulumi-1.1.0/port_pulumi/outputs.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,25 +11,41 @@
 from . import outputs
 
 __all__ = [
     'ActionApprovalEmailNotification',
     'ActionApprovalWebhookNotification',
     'ActionAzureMethod',
     'ActionGithubMethod',
+    'ActionGitlabMethod',
     'ActionKafkaMethod',
     'ActionUserProperties',
     'ActionUserPropertiesArrayProps',
     'ActionUserPropertiesArrayPropsBooleanItems',
+    'ActionUserPropertiesArrayPropsDataset',
+    'ActionUserPropertiesArrayPropsDatasetRule',
+    'ActionUserPropertiesArrayPropsDatasetRuleValue',
     'ActionUserPropertiesArrayPropsNumberItems',
     'ActionUserPropertiesArrayPropsObjectItems',
     'ActionUserPropertiesArrayPropsStringItems',
     'ActionUserPropertiesBooleanProps',
+    'ActionUserPropertiesBooleanPropsDataset',
+    'ActionUserPropertiesBooleanPropsDatasetRule',
+    'ActionUserPropertiesBooleanPropsDatasetRuleValue',
     'ActionUserPropertiesNumberProps',
+    'ActionUserPropertiesNumberPropsDataset',
+    'ActionUserPropertiesNumberPropsDatasetRule',
+    'ActionUserPropertiesNumberPropsDatasetRuleValue',
     'ActionUserPropertiesObjectProps',
+    'ActionUserPropertiesObjectPropsDataset',
+    'ActionUserPropertiesObjectPropsDatasetRule',
+    'ActionUserPropertiesObjectPropsDatasetRuleValue',
     'ActionUserPropertiesStringProps',
+    'ActionUserPropertiesStringPropsDataset',
+    'ActionUserPropertiesStringPropsDatasetRule',
+    'ActionUserPropertiesStringPropsDatasetRuleValue',
     'ActionWebhookMethod',
     'BlueprintCalculationProperties',
     'BlueprintKafkaChangelogDestination',
     'BlueprintMirrorProperties',
     'BlueprintProperties',
     'BlueprintPropertiesArrayProps',
     'BlueprintPropertiesArrayPropsBooleanItems',
@@ -154,14 +170,90 @@
     @property
     @pulumi.getter(name="reportWorkflowStatus")
     def report_workflow_status(self) -> Optional[bool]:
         return pulumi.get(self, "report_workflow_status")
 
 
 @pulumi.output_type
+class ActionGitlabMethod(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "groupName":
+            suggest = "group_name"
+        elif key == "projectName":
+            suggest = "project_name"
+        elif key == "defaultRef":
+            suggest = "default_ref"
+        elif key == "omitPayload":
+            suggest = "omit_payload"
+        elif key == "omitUserInputs":
+            suggest = "omit_user_inputs"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionGitlabMethod. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionGitlabMethod.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionGitlabMethod.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 group_name: str,
+                 project_name: str,
+                 agent: Optional[bool] = None,
+                 default_ref: Optional[str] = None,
+                 omit_payload: Optional[bool] = None,
+                 omit_user_inputs: Optional[bool] = None):
+        pulumi.set(__self__, "group_name", group_name)
+        pulumi.set(__self__, "project_name", project_name)
+        if agent is not None:
+            pulumi.set(__self__, "agent", agent)
+        if default_ref is not None:
+            pulumi.set(__self__, "default_ref", default_ref)
+        if omit_payload is not None:
+            pulumi.set(__self__, "omit_payload", omit_payload)
+        if omit_user_inputs is not None:
+            pulumi.set(__self__, "omit_user_inputs", omit_user_inputs)
+
+    @property
+    @pulumi.getter(name="groupName")
+    def group_name(self) -> str:
+        return pulumi.get(self, "group_name")
+
+    @property
+    @pulumi.getter(name="projectName")
+    def project_name(self) -> str:
+        return pulumi.get(self, "project_name")
+
+    @property
+    @pulumi.getter
+    def agent(self) -> Optional[bool]:
+        return pulumi.get(self, "agent")
+
+    @property
+    @pulumi.getter(name="defaultRef")
+    def default_ref(self) -> Optional[str]:
+        return pulumi.get(self, "default_ref")
+
+    @property
+    @pulumi.getter(name="omitPayload")
+    def omit_payload(self) -> Optional[bool]:
+        return pulumi.get(self, "omit_payload")
+
+    @property
+    @pulumi.getter(name="omitUserInputs")
+    def omit_user_inputs(self) -> Optional[bool]:
+        return pulumi.get(self, "omit_user_inputs")
+
+
+@pulumi.output_type
 class ActionKafkaMethod(dict):
     def __init__(__self__):
         pass
 
 
 @pulumi.output_type
 class ActionUserProperties(dict):
@@ -236,14 +328,18 @@
 @pulumi.output_type
 class ActionUserPropertiesArrayProps(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "booleanItems":
             suggest = "boolean_items"
+        elif key == "defaultJqQuery":
+            suggest = "default_jq_query"
+        elif key == "dependsOns":
+            suggest = "depends_ons"
         elif key == "maxItems":
             suggest = "max_items"
         elif key == "minItems":
             suggest = "min_items"
         elif key == "numberItems":
             suggest = "number_items"
         elif key == "objectItems":
@@ -260,25 +356,34 @@
 
     def get(self, key: str, default = None) -> Any:
         ActionUserPropertiesArrayProps.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  boolean_items: Optional['outputs.ActionUserPropertiesArrayPropsBooleanItems'] = None,
+                 dataset: Optional['outputs.ActionUserPropertiesArrayPropsDataset'] = None,
+                 default_jq_query: Optional[str] = None,
+                 depends_ons: Optional[Sequence[str]] = None,
                  description: Optional[str] = None,
                  icon: Optional[str] = None,
                  max_items: Optional[int] = None,
                  min_items: Optional[int] = None,
                  number_items: Optional['outputs.ActionUserPropertiesArrayPropsNumberItems'] = None,
                  object_items: Optional['outputs.ActionUserPropertiesArrayPropsObjectItems'] = None,
                  required: Optional[bool] = None,
                  string_items: Optional['outputs.ActionUserPropertiesArrayPropsStringItems'] = None,
                  title: Optional[str] = None):
         if boolean_items is not None:
             pulumi.set(__self__, "boolean_items", boolean_items)
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if max_items is not None:
             pulumi.set(__self__, "max_items", max_items)
         if min_items is not None:
@@ -297,14 +402,29 @@
     @property
     @pulumi.getter(name="booleanItems")
     def boolean_items(self) -> Optional['outputs.ActionUserPropertiesArrayPropsBooleanItems']:
         return pulumi.get(self, "boolean_items")
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional['outputs.ActionUserPropertiesArrayPropsDataset']:
+        return pulumi.get(self, "dataset")
+
+    @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[str]:
+        return pulumi.get(self, "default_jq_query")
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "depends_ons")
+
+    @property
+    @pulumi.getter
     def description(self) -> Optional[str]:
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def icon(self) -> Optional[str]:
         return pulumi.get(self, "icon")
@@ -355,14 +475,97 @@
     @property
     @pulumi.getter
     def defaults(self) -> Optional[Sequence[bool]]:
         return pulumi.get(self, "defaults")
 
 
 @pulumi.output_type
+class ActionUserPropertiesArrayPropsDataset(dict):
+    def __init__(__self__, *,
+                 combinator: str,
+                 rules: Sequence['outputs.ActionUserPropertiesArrayPropsDatasetRule']):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> str:
+        return pulumi.get(self, "combinator")
+
+    @property
+    @pulumi.getter
+    def rules(self) -> Sequence['outputs.ActionUserPropertiesArrayPropsDatasetRule']:
+        return pulumi.get(self, "rules")
+
+
+@pulumi.output_type
+class ActionUserPropertiesArrayPropsDatasetRule(dict):
+    def __init__(__self__, *,
+                 operator: str,
+                 value: 'outputs.ActionUserPropertiesArrayPropsDatasetRuleValue',
+                 blueprint: Optional[str] = None,
+                 property: Optional[str] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> str:
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def value(self) -> 'outputs.ActionUserPropertiesArrayPropsDatasetRuleValue':
+        return pulumi.get(self, "value")
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[str]:
+        return pulumi.get(self, "blueprint")
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[str]:
+        return pulumi.get(self, "property")
+
+
+@pulumi.output_type
+class ActionUserPropertiesArrayPropsDatasetRuleValue(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "jqQuery":
+            suggest = "jq_query"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesArrayPropsDatasetRuleValue. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionUserPropertiesArrayPropsDatasetRuleValue.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionUserPropertiesArrayPropsDatasetRuleValue.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 jq_query: str):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> str:
+        return pulumi.get(self, "jq_query")
+
+
+@pulumi.output_type
 class ActionUserPropertiesArrayPropsNumberItems(dict):
     def __init__(__self__, *,
                  defaults: Optional[Sequence[float]] = None):
         if defaults is not None:
             pulumi.set(__self__, "defaults", defaults)
 
     @property
@@ -411,37 +614,80 @@
     @pulumi.getter
     def format(self) -> Optional[str]:
         return pulumi.get(self, "format")
 
 
 @pulumi.output_type
 class ActionUserPropertiesBooleanProps(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "defaultJqQuery":
+            suggest = "default_jq_query"
+        elif key == "dependsOns":
+            suggest = "depends_ons"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesBooleanProps. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionUserPropertiesBooleanProps.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionUserPropertiesBooleanProps.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
+                 dataset: Optional['outputs.ActionUserPropertiesBooleanPropsDataset'] = None,
                  default: Optional[bool] = None,
+                 default_jq_query: Optional[str] = None,
+                 depends_ons: Optional[Sequence[str]] = None,
                  description: Optional[str] = None,
                  icon: Optional[str] = None,
                  required: Optional[bool] = None,
                  title: Optional[str] = None):
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
         if default is not None:
             pulumi.set(__self__, "default", default)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if required is not None:
             pulumi.set(__self__, "required", required)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional['outputs.ActionUserPropertiesBooleanPropsDataset']:
+        return pulumi.get(self, "dataset")
+
+    @property
+    @pulumi.getter
     def default(self) -> Optional[bool]:
         return pulumi.get(self, "default")
 
     @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[str]:
+        return pulumi.get(self, "default_jq_query")
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "depends_ons")
+
+    @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def icon(self) -> Optional[str]:
@@ -455,28 +701,144 @@
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
         return pulumi.get(self, "title")
 
 
 @pulumi.output_type
+class ActionUserPropertiesBooleanPropsDataset(dict):
+    def __init__(__self__, *,
+                 combinator: str,
+                 rules: Sequence['outputs.ActionUserPropertiesBooleanPropsDatasetRule']):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> str:
+        return pulumi.get(self, "combinator")
+
+    @property
+    @pulumi.getter
+    def rules(self) -> Sequence['outputs.ActionUserPropertiesBooleanPropsDatasetRule']:
+        return pulumi.get(self, "rules")
+
+
+@pulumi.output_type
+class ActionUserPropertiesBooleanPropsDatasetRule(dict):
+    def __init__(__self__, *,
+                 operator: str,
+                 value: 'outputs.ActionUserPropertiesBooleanPropsDatasetRuleValue',
+                 blueprint: Optional[str] = None,
+                 property: Optional[str] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> str:
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def value(self) -> 'outputs.ActionUserPropertiesBooleanPropsDatasetRuleValue':
+        return pulumi.get(self, "value")
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[str]:
+        return pulumi.get(self, "blueprint")
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[str]:
+        return pulumi.get(self, "property")
+
+
+@pulumi.output_type
+class ActionUserPropertiesBooleanPropsDatasetRuleValue(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "jqQuery":
+            suggest = "jq_query"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesBooleanPropsDatasetRuleValue. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionUserPropertiesBooleanPropsDatasetRuleValue.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionUserPropertiesBooleanPropsDatasetRuleValue.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 jq_query: str):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> str:
+        return pulumi.get(self, "jq_query")
+
+
+@pulumi.output_type
 class ActionUserPropertiesNumberProps(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "defaultJqQuery":
+            suggest = "default_jq_query"
+        elif key == "dependsOns":
+            suggest = "depends_ons"
+        elif key == "enumJqQuery":
+            suggest = "enum_jq_query"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesNumberProps. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionUserPropertiesNumberProps.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionUserPropertiesNumberProps.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
+                 dataset: Optional['outputs.ActionUserPropertiesNumberPropsDataset'] = None,
                  default: Optional[float] = None,
+                 default_jq_query: Optional[str] = None,
+                 depends_ons: Optional[Sequence[str]] = None,
                  description: Optional[str] = None,
+                 enum_jq_query: Optional[str] = None,
                  enums: Optional[Sequence[float]] = None,
                  icon: Optional[str] = None,
                  maximum: Optional[float] = None,
                  minimum: Optional[float] = None,
                  required: Optional[bool] = None,
                  title: Optional[str] = None):
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
         if default is not None:
             pulumi.set(__self__, "default", default)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if enum_jq_query is not None:
+            pulumi.set(__self__, "enum_jq_query", enum_jq_query)
         if enums is not None:
             pulumi.set(__self__, "enums", enums)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if maximum is not None:
             pulumi.set(__self__, "maximum", maximum)
         if minimum is not None:
@@ -484,23 +846,43 @@
         if required is not None:
             pulumi.set(__self__, "required", required)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional['outputs.ActionUserPropertiesNumberPropsDataset']:
+        return pulumi.get(self, "dataset")
+
+    @property
+    @pulumi.getter
     def default(self) -> Optional[float]:
         return pulumi.get(self, "default")
 
     @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[str]:
+        return pulumi.get(self, "default_jq_query")
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "depends_ons")
+
+    @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         return pulumi.get(self, "description")
 
     @property
+    @pulumi.getter(name="enumJqQuery")
+    def enum_jq_query(self) -> Optional[str]:
+        return pulumi.get(self, "enum_jq_query")
+
+    @property
     @pulumi.getter
     def enums(self) -> Optional[Sequence[float]]:
         return pulumi.get(self, "enums")
 
     @property
     @pulumi.getter
     def icon(self) -> Optional[str]:
@@ -524,38 +906,164 @@
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
         return pulumi.get(self, "title")
 
 
 @pulumi.output_type
+class ActionUserPropertiesNumberPropsDataset(dict):
+    def __init__(__self__, *,
+                 combinator: str,
+                 rules: Sequence['outputs.ActionUserPropertiesNumberPropsDatasetRule']):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> str:
+        return pulumi.get(self, "combinator")
+
+    @property
+    @pulumi.getter
+    def rules(self) -> Sequence['outputs.ActionUserPropertiesNumberPropsDatasetRule']:
+        return pulumi.get(self, "rules")
+
+
+@pulumi.output_type
+class ActionUserPropertiesNumberPropsDatasetRule(dict):
+    def __init__(__self__, *,
+                 operator: str,
+                 value: 'outputs.ActionUserPropertiesNumberPropsDatasetRuleValue',
+                 blueprint: Optional[str] = None,
+                 property: Optional[str] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> str:
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def value(self) -> 'outputs.ActionUserPropertiesNumberPropsDatasetRuleValue':
+        return pulumi.get(self, "value")
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[str]:
+        return pulumi.get(self, "blueprint")
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[str]:
+        return pulumi.get(self, "property")
+
+
+@pulumi.output_type
+class ActionUserPropertiesNumberPropsDatasetRuleValue(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "jqQuery":
+            suggest = "jq_query"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesNumberPropsDatasetRuleValue. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionUserPropertiesNumberPropsDatasetRuleValue.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionUserPropertiesNumberPropsDatasetRuleValue.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 jq_query: str):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> str:
+        return pulumi.get(self, "jq_query")
+
+
+@pulumi.output_type
 class ActionUserPropertiesObjectProps(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "defaultJqQuery":
+            suggest = "default_jq_query"
+        elif key == "dependsOns":
+            suggest = "depends_ons"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesObjectProps. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionUserPropertiesObjectProps.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionUserPropertiesObjectProps.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
+                 dataset: Optional['outputs.ActionUserPropertiesObjectPropsDataset'] = None,
                  default: Optional[str] = None,
+                 default_jq_query: Optional[str] = None,
+                 depends_ons: Optional[Sequence[str]] = None,
                  description: Optional[str] = None,
                  icon: Optional[str] = None,
                  required: Optional[bool] = None,
                  title: Optional[str] = None):
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
         if default is not None:
             pulumi.set(__self__, "default", default)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if required is not None:
             pulumi.set(__self__, "required", required)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional['outputs.ActionUserPropertiesObjectPropsDataset']:
+        return pulumi.get(self, "dataset")
+
+    @property
+    @pulumi.getter
     def default(self) -> Optional[str]:
         return pulumi.get(self, "default")
 
     @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[str]:
+        return pulumi.get(self, "default_jq_query")
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "depends_ons")
+
+    @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def icon(self) -> Optional[str]:
@@ -569,19 +1077,108 @@
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
         return pulumi.get(self, "title")
 
 
 @pulumi.output_type
+class ActionUserPropertiesObjectPropsDataset(dict):
+    def __init__(__self__, *,
+                 combinator: str,
+                 rules: Sequence['outputs.ActionUserPropertiesObjectPropsDatasetRule']):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> str:
+        return pulumi.get(self, "combinator")
+
+    @property
+    @pulumi.getter
+    def rules(self) -> Sequence['outputs.ActionUserPropertiesObjectPropsDatasetRule']:
+        return pulumi.get(self, "rules")
+
+
+@pulumi.output_type
+class ActionUserPropertiesObjectPropsDatasetRule(dict):
+    def __init__(__self__, *,
+                 operator: str,
+                 value: 'outputs.ActionUserPropertiesObjectPropsDatasetRuleValue',
+                 blueprint: Optional[str] = None,
+                 property: Optional[str] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> str:
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def value(self) -> 'outputs.ActionUserPropertiesObjectPropsDatasetRuleValue':
+        return pulumi.get(self, "value")
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[str]:
+        return pulumi.get(self, "blueprint")
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[str]:
+        return pulumi.get(self, "property")
+
+
+@pulumi.output_type
+class ActionUserPropertiesObjectPropsDatasetRuleValue(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "jqQuery":
+            suggest = "jq_query"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesObjectPropsDatasetRuleValue. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionUserPropertiesObjectPropsDatasetRuleValue.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionUserPropertiesObjectPropsDatasetRuleValue.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 jq_query: str):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> str:
+        return pulumi.get(self, "jq_query")
+
+
+@pulumi.output_type
 class ActionUserPropertiesStringProps(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "maxLength":
+        if key == "defaultJqQuery":
+            suggest = "default_jq_query"
+        elif key == "dependsOns":
+            suggest = "depends_ons"
+        elif key == "enumJqQuery":
+            suggest = "enum_jq_query"
+        elif key == "maxLength":
             suggest = "max_length"
         elif key == "minLength":
             suggest = "min_length"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesStringProps. Access the value via the '{suggest}' property getter instead.")
 
@@ -591,30 +1188,42 @@
 
     def get(self, key: str, default = None) -> Any:
         ActionUserPropertiesStringProps.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  blueprint: Optional[str] = None,
+                 dataset: Optional['outputs.ActionUserPropertiesStringPropsDataset'] = None,
                  default: Optional[str] = None,
+                 default_jq_query: Optional[str] = None,
+                 depends_ons: Optional[Sequence[str]] = None,
                  description: Optional[str] = None,
+                 enum_jq_query: Optional[str] = None,
                  enums: Optional[Sequence[str]] = None,
                  format: Optional[str] = None,
                  icon: Optional[str] = None,
                  max_length: Optional[int] = None,
                  min_length: Optional[int] = None,
                  pattern: Optional[str] = None,
                  required: Optional[bool] = None,
                  title: Optional[str] = None):
         if blueprint is not None:
             pulumi.set(__self__, "blueprint", blueprint)
+        if dataset is not None:
+            pulumi.set(__self__, "dataset", dataset)
         if default is not None:
             pulumi.set(__self__, "default", default)
+        if default_jq_query is not None:
+            pulumi.set(__self__, "default_jq_query", default_jq_query)
+        if depends_ons is not None:
+            pulumi.set(__self__, "depends_ons", depends_ons)
         if description is not None:
             pulumi.set(__self__, "description", description)
+        if enum_jq_query is not None:
+            pulumi.set(__self__, "enum_jq_query", enum_jq_query)
         if enums is not None:
             pulumi.set(__self__, "enums", enums)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if icon is not None:
             pulumi.set(__self__, "icon", icon)
         if max_length is not None:
@@ -631,23 +1240,43 @@
     @property
     @pulumi.getter
     def blueprint(self) -> Optional[str]:
         return pulumi.get(self, "blueprint")
 
     @property
     @pulumi.getter
+    def dataset(self) -> Optional['outputs.ActionUserPropertiesStringPropsDataset']:
+        return pulumi.get(self, "dataset")
+
+    @property
+    @pulumi.getter
     def default(self) -> Optional[str]:
         return pulumi.get(self, "default")
 
     @property
+    @pulumi.getter(name="defaultJqQuery")
+    def default_jq_query(self) -> Optional[str]:
+        return pulumi.get(self, "default_jq_query")
+
+    @property
+    @pulumi.getter(name="dependsOns")
+    def depends_ons(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "depends_ons")
+
+    @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         return pulumi.get(self, "description")
 
     @property
+    @pulumi.getter(name="enumJqQuery")
+    def enum_jq_query(self) -> Optional[str]:
+        return pulumi.get(self, "enum_jq_query")
+
+    @property
     @pulumi.getter
     def enums(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "enums")
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
@@ -681,14 +1310,97 @@
     @property
     @pulumi.getter
     def title(self) -> Optional[str]:
         return pulumi.get(self, "title")
 
 
 @pulumi.output_type
+class ActionUserPropertiesStringPropsDataset(dict):
+    def __init__(__self__, *,
+                 combinator: str,
+                 rules: Sequence['outputs.ActionUserPropertiesStringPropsDatasetRule']):
+        pulumi.set(__self__, "combinator", combinator)
+        pulumi.set(__self__, "rules", rules)
+
+    @property
+    @pulumi.getter
+    def combinator(self) -> str:
+        return pulumi.get(self, "combinator")
+
+    @property
+    @pulumi.getter
+    def rules(self) -> Sequence['outputs.ActionUserPropertiesStringPropsDatasetRule']:
+        return pulumi.get(self, "rules")
+
+
+@pulumi.output_type
+class ActionUserPropertiesStringPropsDatasetRule(dict):
+    def __init__(__self__, *,
+                 operator: str,
+                 value: 'outputs.ActionUserPropertiesStringPropsDatasetRuleValue',
+                 blueprint: Optional[str] = None,
+                 property: Optional[str] = None):
+        pulumi.set(__self__, "operator", operator)
+        pulumi.set(__self__, "value", value)
+        if blueprint is not None:
+            pulumi.set(__self__, "blueprint", blueprint)
+        if property is not None:
+            pulumi.set(__self__, "property", property)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> str:
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def value(self) -> 'outputs.ActionUserPropertiesStringPropsDatasetRuleValue':
+        return pulumi.get(self, "value")
+
+    @property
+    @pulumi.getter
+    def blueprint(self) -> Optional[str]:
+        return pulumi.get(self, "blueprint")
+
+    @property
+    @pulumi.getter
+    def property(self) -> Optional[str]:
+        return pulumi.get(self, "property")
+
+
+@pulumi.output_type
+class ActionUserPropertiesStringPropsDatasetRuleValue(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "jqQuery":
+            suggest = "jq_query"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ActionUserPropertiesStringPropsDatasetRuleValue. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ActionUserPropertiesStringPropsDatasetRuleValue.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ActionUserPropertiesStringPropsDatasetRuleValue.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 jq_query: str):
+        pulumi.set(__self__, "jq_query", jq_query)
+
+    @property
+    @pulumi.getter(name="jqQuery")
+    def jq_query(self) -> str:
+        return pulumi.get(self, "jq_query")
+
+
+@pulumi.output_type
 class ActionWebhookMethod(dict):
     def __init__(__self__, *,
                  url: str,
                  agent: Optional[bool] = None):
         pulumi.set(__self__, "url", url)
         if agent is not None:
             pulumi.set(__self__, "agent", agent)
```

### Comparing `port_pulumi-1.0.0/port_pulumi/provider.py` & `port_pulumi-1.1.0/port_pulumi/provider.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.0.0/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-1.1.0/port_pulumi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-pulumi
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `port_pulumi-1.0.0/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-1.1.0/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.0.0/setup.py` & `port_pulumi-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.0"
-PLUGIN_VERSION = "1.0.0"
+VERSION = "1.1.0"
+PLUGIN_VERSION = "1.1.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'port', PLUGIN_VERSION, '--server', 'github://api.github.com/port-labs/pulumi-port'])
         except OSError as error:
```

