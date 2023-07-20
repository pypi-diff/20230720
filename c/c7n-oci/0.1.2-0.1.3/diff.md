# Comparing `tmp/c7n_oci-0.1.2-py3-none-any.whl.zip` & `tmp/c7n_oci-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 23120 bytes, number of entries: 18
+Zip file size: 22014 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      189 b- defN 80-Jan-01 00:00 c7n_oci/actions/__init__.py
--rw-r--r--  2.0 unx     6233 b- defN 80-Jan-01 00:00 c7n_oci/actions/base.py
+-rw-r--r--  2.0 unx     6381 b- defN 80-Jan-01 00:00 c7n_oci/actions/base.py
 -rw-r--r--  2.0 unx      375 b- defN 80-Jan-01 00:00 c7n_oci/constants.py
 -rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 c7n_oci/entry.py
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 c7n_oci/filters/__init__.py
--rw-r--r--  2.0 unx     1019 b- defN 80-Jan-01 00:00 c7n_oci/provider.py
--rw-r--r--  2.0 unx     7939 b- defN 80-Jan-01 00:00 c7n_oci/query.py
+-rw-r--r--  2.0 unx      825 b- defN 80-Jan-01 00:00 c7n_oci/provider.py
+-rw-r--r--  2.0 unx     7917 b- defN 80-Jan-01 00:00 c7n_oci/query.py
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 c7n_oci/resources/__init__.py
--rw-r--r--  2.0 unx    11621 b- defN 80-Jan-01 00:00 c7n_oci/resources/compute.py
--rw-r--r--  2.0 unx     5178 b- defN 80-Jan-01 00:00 c7n_oci/resources/dns.py
--rw-r--r--  2.0 unx    33426 b- defN 80-Jan-01 00:00 c7n_oci/resources/identity.py
--rw-r--r--  2.0 unx     6637 b- defN 80-Jan-01 00:00 c7n_oci/resources/object_storage.py
+-rw-r--r--  2.0 unx     9672 b- defN 80-Jan-01 00:00 c7n_oci/resources/compute.py
+-rw-r--r--  2.0 unx     4642 b- defN 80-Jan-01 00:00 c7n_oci/resources/dns.py
+-rw-r--r--  2.0 unx    33036 b- defN 80-Jan-01 00:00 c7n_oci/resources/identity.py
+-rw-r--r--  2.0 unx     6454 b- defN 80-Jan-01 00:00 c7n_oci/resources/object_storage.py
 -rw-r--r--  2.0 unx      626 b- defN 80-Jan-01 00:00 c7n_oci/resources/resource_map.py
--rw-r--r--  2.0 unx    12586 b- defN 80-Jan-01 00:00 c7n_oci/resources/virtual_network.py
--rw-r--r--  2.0 unx     3677 b- defN 80-Jan-01 00:00 c7n_oci/session.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_oci-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4294 b- defN 16-Jan-01 00:00 c7n_oci-0.1.2.dist-info/METADATA
-?rw-------  2.0 unx     1436 b- defN 23-Jun-28 08:38 c7n_oci-0.1.2.dist-info/RECORD
-18 files, 95870 bytes uncompressed, 20788 bytes compressed:  78.3%
+-rw-r--r--  2.0 unx    12225 b- defN 80-Jan-01 00:00 c7n_oci/resources/virtual_network.py
+-rw-r--r--  2.0 unx     2406 b- defN 80-Jan-01 00:00 c7n_oci/session.py
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_oci-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4294 b- defN 16-Jan-01 00:00 c7n_oci-0.1.3.dist-info/METADATA
+?rw-------  2.0 unx     1434 b- defN 23-Jul-20 14:11 c7n_oci-0.1.3.dist-info/RECORD
+18 files, 91110 bytes uncompressed, 19682 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -39,17 +39,17 @@
 
 Filename: c7n_oci/resources/virtual_network.py
 Comment: 
 
 Filename: c7n_oci/session.py
 Comment: 
 
-Filename: c7n_oci-0.1.2.dist-info/WHEEL
+Filename: c7n_oci-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_oci-0.1.2.dist-info/METADATA
+Filename: c7n_oci-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: c7n_oci-0.1.2.dist-info/RECORD
+Filename: c7n_oci-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## c7n_oci/actions/base.py

```diff
@@ -1,11 +1,12 @@
 # Copyright The Cloud Custodian Authors.
 # SPDX-License-Identifier: Apache-2.0
 
 import abc
+import copy
 import logging
 from abc import ABC
 
 from c7n.actions import BaseAction
 from c7n.utils import type_schema
 
 log = logging.getLogger("custodian.oci.actions.base")
@@ -53,14 +54,19 @@
 
     # All the OCI actions that extends the OCIBaseAction should implement the below method to
     # have the logic for invoking the respective client
     @abc.abstractmethod
     def perform_action(self, resource):
         raise NotImplementedError("Base action class does not implement this behavior")
 
+    def extract_params(self, params):
+        op_params = copy.deepcopy(params)
+        del op_params["type"]
+        return op_params
+
     def update_params(self, resource, updated_resource_details):
         updated_params = {}
         for key, value in updated_resource_details.items():
             if key == "defined_tags":
                 # Get all existing resource tags
                 existing_tags = resource.get(key)
                 # Create new dict to keep track of the tags provided in the policy
```

## c7n_oci/provider.py

```diff
@@ -1,38 +1,33 @@
 # Copyright The Cloud Custodian Authors.
 # SPDX-License-Identifier: Apache-2.0
 
-from functools import partial
+import logging
+
+from c7n_oci.resources.resource_map import ResourceMap
 
 from c7n.provider import Provider, clouds
 from c7n.registry import PluginRegistry
-from c7n.utils import local_session
-from .session import Session
 
-from c7n_oci.resources.resource_map import ResourceMap
-
-import logging
+from .session import SessionFactory
 
 log = logging.getLogger("custodian.provider")
 
 
 @clouds.register("oci")
 class OCI(Provider):
     display_name = "Oracle Cloud Infrastructure"
     resource_prefix = "oci"
     resources = PluginRegistry("%s.resources" % resource_prefix)
     resource_map = ResourceMap
 
     def initialize(self, options):
-        session = local_session(self.get_session_factory(options))
-        session.initialize_session()
-        options["oci_config"] = session.get_oci_config()
         return options
 
     def initialize_policies(self, policy_collection, options):
         return policy_collection
 
     def get_session_factory(self, options):
-        return partial(Session)
+        return SessionFactory(profile=options['profile'])
 
 
 resources = OCI.resources
```

## c7n_oci/query.py

```diff
@@ -17,15 +17,15 @@
 
 
 class ResourceQuery:
     def __init__(self, session_factory):
         self.session_factory = session_factory
 
     def filter(self, resource_manager, client_name, operation, params):
-        session = local_session(self.session_factory)
+        session = resource_manager.get_session()
         client = session.client(client_name)
 
         return self._invoke_client_enum(client, operation, params)
 
     def _invoke_client_enum(self, client, operation, params):
         method = getattr(client, operation)
         response = oci.pagination.list_call_get_all_results(method, **params)
@@ -154,15 +154,15 @@
         if source_type in self.source_mapping:
             return self.source_mapping.get(source_type)(self)
         if source_type in sources:
             return sources[source_type](self)
         raise KeyError("Invalid Source %s" % source_type)
 
     def get_client(self):
-        return local_session(self.session_factory).client(
+        return self.get_session().client(
             f"{self.resource_type.service}.{self.resource_type.client}"
         )
 
     def _construct_list_func_ref(self):
         operation, return_type, extra_args = self.resource_type.enum_spec
         return getattr(self.get_client(), operation)
```

## c7n_oci/resources/compute.py

```diff
@@ -40,235 +40,260 @@
         extra_params = {"compartment_id", "instance_id"}
         resource_type = "OCI.Compute/Instance"
         id = "id"
         name = "display_name"
         search_resource_type = "instance"
 
 
-@Instance.filter_registry.register("monitoring")
-class InstanceMonitoring(Filter):
+@Instance.action_registry.register("remove-tag")
+class RemoveTagActionInstance(RemoveTagBaseAction):
     """
-    Instance Monitoring Filter
+    Remove Tag Action
 
     :example:
 
-    This filter returns the resources with the aggregated data that match the criteria specified in the request.
-    Compartment OCID required. For information on metric queries, see `Building Metric Queries
-    <https://docs.oracle.com/en-us/iaas/Content/Monitoring/Tasks/buildingqueries.htm>`_.
+        Remove the specified tags from the resource. Defined tag needs to be referred as
+        'namespace.tagName' as below in the policy file.
 
     .. code-block:: yaml
 
         policies:
-            - name: instance-with-low-cpu-utilization
-            description: |
-                Return the instances with the low CPU utilization
-            resource: oci.instance
-            filters:
-                - type: monitoring
-                  query: 'CpuUtilization[30d].mean() < 6'
+            - name: remove-tag
+              resource: oci.instance
+            actions:
+              - type: remove-tag
+                defined_tags: ['cloud_custodian.environment']
+                freeform_tags: ['organization', 'team']
 
     """  # noqa
 
-    schema = type_schema("monitoring", query={"type": "string"}, required=["query"])
-
-    def process(self, resources, event):
-        summarize_metrics = oci.monitoring.models.SummarizeMetricsDataDetails(
-            query=self.data.get("query"),
-            namespace="oci_computeagent",
-        )
-        monitoring_client = self.manager.get_session().get_monitoring_client()
-        comp_resources = {}
-        result = []
-        for resource in resources:
-            comp_id = resource.get("compartment_id")
-            if comp_id in comp_resources:
-                comp_resources.get(comp_id).append(resource)
-            else:
-                comp_resources[comp_id] = [resource]
-        # Query the MonitoringClient with the query against each compartment and perform
-        # the filtering
-        for compartment_id in comp_resources.keys():
-            metric_response = monitoring_client.summarize_metrics_data(
-                compartment_id=compartment_id,
-                summarize_metrics_data_details=summarize_metrics,
+    def perform_action(self, resource):
+        client = self.manager.get_client()
+        original_tag_count = self.tag_count(resource)
+        params_model = self.remove_tag(resource)
+        updated_tag_count = self.tag_count(params_model)
+        update_instance_details = oci.core.models.UpdateInstanceDetails(**params_model)
+        if self.tag_removed_from_resource(original_tag_count, updated_tag_count):
+            response = client.update_instance(
+                instance_id=resource.get("id"),
+                update_instance_details=update_instance_details,
             )
-            for metric_data in metric_response.data:
-                resource_id = metric_data.dimensions["resourceId"]
-                for resource in comp_resources.get(compartment_id):
-                    if resource.get("id") == resource_id:
-                        result.append(resource)
-        return result
+            log.debug(
+                f"Received status {response.status} for PUT:update_instance:remove-tag"
+                f" {response.request_id}"
+            )
+            return response
+        else:
+            log.debug(
+                "No tags matched. Skipping the remove-tag action on this resource - %s",
+                resource.get("display_name"),
+            )
+            return None
+
+
+@Instance.action_registry.register("start")
+class InstanceStart(OCIBaseAction):
+    """Starts a stopped compute instance.
 
+    :Example:
 
-@Instance.action_registry.register("instance-action")
-class InstanceAction(OCIBaseAction):
+    .. code-block:: yaml
+
+        policies:
+          - name: start-compute-instance
+            resource: oci.instance
+            actions:
+              - start
+
+    https://docs.oracle.com/en-us/iaas/Content/Compute/Tasks/restartinginstance.htm
     """
-        Instance action Action
 
-        :example:
+    schema = type_schema("start", rinherit=OCIBaseAction.schema)
 
-        Performs one of the following power actions on the specified instance:
+    def perform_action(self, resource):
+        client = self.manager.get_client()
+        response = client.instance_action(
+            instance_id=resource["id"],
+            action="START",
+        )
+        log.info(f"Received status {response.status} for POST:START {response.request_id}")
+        return response
 
-    - **START** - Powers on the instance.
 
-    - **STOP** - Powers off the instance.
+@Instance.action_registry.register("stop")
+class InstanceStop(OCIBaseAction):
+    """Stops a running compute instance.
 
-    - **RESET** - Powers off the instance and then powers it back on.
+    :Example:
 
-    - **SOFTSTOP** - Gracefully shuts down the instance by sending a shutdown command to the operating system. After waiting 15 minutes for the OS to shut down, the instance is powered off. If the applications that run on the instance take more than 15 minutes to shut down, they could be improperly stopped, resulting in data corruption. To avoid this, manually shut down the instance using the commands available in the OS before you softstop the instance.
+    .. code-block:: yaml
 
-    - **SOFTRESET** - Gracefully reboots the instance by sending a shutdown command to the operating system.After waiting 15 minutes for the OS to shut down, the instance is powered off and then powered back on.
+        policies:
+          - name: stop-compute-instance
+            resource: oci.instance
+            actions:
+              - stop
 
-    - **SENDDIAGNOSTICINTERRUPT** - For advanced users. **Caution: Sending a diagnostic interrupt to a live system can cause data corruption or system failure.** Sends a diagnostic interrupt that causes the instance's OS to crash and then reboot. Before you send a diagnostic interrupt, you must configure the instance to generate a crash dump file when it crashes. The crash dump captures information about the state of the OS at the time of the crash. After the OS restarts, you can analyze the crash dump to diagnose the issue. For more information, see [Sending a Diagnostic Interrupt](/iaas/Content/Compute/Tasks/sendingdiagnosticinterrupt.htm).
+          - name: force-stop-compute-instance
+            resource: oci.instance
+            actions:
+              - type: stop
+                force: true
 
-    - **DIAGNOSTICREBOOT** - Powers off the instance, rebuilds it, and then powers it back on. Before you send a diagnostic reboot, restart the instance's OS, confirm that the instance and networking settings are configured correctly, and try other [troubleshooting steps](/iaas/Content/Compute/References/troubleshooting-compute-instances.htm). Use diagnostic reboot as a final attempt to troubleshoot an unreachable instance. For virtual machine (VM) instances only. For more information, see [Performing a Diagnostic Reboot](/iaas/Content/Compute/Tasks/diagnostic-reboot.htm).
+    If 'force' option is passed, then a compute instance will be stopped immediately.
 
-    - **REBOOTMIGRATE** - Powers off the instance, moves it to new hardware, and then powers it back on. For more information, see [Infrastructure Maintenance](/iaas/Content/Compute/References/infrastructure-maintenance.htm).
+    https://docs.oracle.com/en-us/iaas/Content/Compute/Tasks/restartinginstance.htm
+    """
 
+    schema = type_schema("stop", force={"type": "boolean"})
 
-    For more information about managing instance lifecycle states, see
-    [Stopping and Starting an Instance](/iaas/Content/Compute/Tasks/restartinginstance.htm).
+    def perform_action(self, resource):
+        client = self.manager.get_client()
+        action = "STOP" if self.data.get("force") else "SOFTSTOP"
+        response = client.instance_action(instance_id=resource["id"], action=action)
+        log.info(f"Received status {response.status} for POST:{action} {response.request_id}")
+        response = None
+        return response
 
 
-        Please refer to the Oracle Cloud Infrastructure Python SDK documentation for parameter details to this action
-        https://docs.oracle.com/en-us/iaas/tools/python/latest/api/core/client/oci.core.ComputeClient.html#oci.core.ComputeClient.instance_action
+@Instance.action_registry.register("reboot")
+class InstanceReboot(OCIBaseAction):
+    """Restarts a compute instance.
 
-        .. code-block:: yaml
+    :Example:
 
-            policies:
-                - name: perform-instance-action-action
-                  resource: oci.instance
-                  actions:
-                    - type: instance-action
+    .. code-block:: yaml
 
-    """  # noqa
+        policies:
+          - name: reboot-compute-instance
+            resource: oci.instance
+            actions:
+              - reboot
 
-    schema = type_schema(
-        "instance-action", params={"type": "object"}, rinherit=OCIBaseAction.schema
-    )
+          - name: force-reboot-compute-instance
+            resource: oci.instance
+            actions:
+              - type: reboot
+                force: true
+
+    If 'force' option is passed, then a compute instance will be rebooted immediately.
+
+    https://docs.oracle.com/en-us/iaas/Content/Compute/Tasks/restartinginstance.htm
+    """
+
+    schema = type_schema("reboot", force={"type": "boolean"})
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["instance_id"] = resource.get("id")
-        if self.data.get("params") and self.data.get("params").get("action"):
-            params_dict["action"] = self.data.get("params").get("action")
-        else:
-            params_dict["action"] = resource.get("action")
-        if self.data.get("params").get("instance_power_action_details"):
-            instance_power_action_details_user = self.data.get("params").get(
-                "instance_power_action_details"
-            )
-            if instance_power_action_details_user.get("action_type"):
-                params_dict["action_type"] = instance_power_action_details_user.get("action_type")
-            params_model = self.update_params(resource, instance_power_action_details_user)
-            params_dict[
-                "instance_power_action_details"
-            ] = oci.core.models.InstancePowerActionDetails(**params_model)
-        response = client.instance_action(
-            instance_id=params_dict["instance_id"],
-            action=params_dict["action"],
-        )
-        log.info(
-            f"Received status {response.status} for POST:instance_action {response.request_id}"
-        )
+        action = "RESET" if self.data.get("force") else "SOFTRESET"
+        response = client.instance_action(instance_id=resource["id"], action=action)
+        log.info(f"Received status {response.status} for POST:{action} {response.request_id}")
         return response
 
 
-@Instance.action_registry.register("update-instance")
+@Instance.action_registry.register("update")
 class UpdateInstance(OCIBaseAction):
     """
-    Update instance Action
+    Update a compute instace
 
     :example:
 
-    Updates certain fields on the specified instance. Fields that are not provided in the request will not be updated. Avoid entering confidential information.
+    Updates certain fields on the specified instance. Fields that are not provided in the request will not be updated.
 
     Changes to metadata fields will be reflected in the instance metadata service (this may take up to a minute).
 
     The OCID of the instance remains the same.
 
-
-    Please refer to the Oracle Cloud Infrastructure Python SDK documentation for parameter details to this action
-    https://docs.oracle.com/en-us/iaas/tools/python/latest/api/core/client/oci.core.ComputeClient.html#oci.core.ComputeClient.update_instance
-
     .. code-block:: yaml
 
         policies:
-            - name: perform-update-instance-action
+            - name: update-compute-instance
               resource: oci.instance
               actions:
-                - type: update-instance
+                - type: update
+                  shape: VM.Standard.E3.Flex
 
+    https://docs.oracle.com/en-us/iaas/Content/Compute/Tasks/edit-instance.htm
     """  # noqa
 
     schema = type_schema(
-        "update-instance", params={"type": "object"}, rinherit=OCIBaseAction.schema
+        "update",
+        **{
+            "shape": {"type": "string"},
+            "shape_config": {
+                "type": "object",
+                "properties": {
+                    "memory_in_gbs": {"type": "number"},
+                    "ocpus": {"type": "number"},
+                    "nvmes": {"type": "integer"},
+                },
+            },
+            "freeform_tags": {"type": "object"},
+            "defined_tags": {"type": "object"},
+        },
     )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["instance_id"] = resource.get("id")
-        if self.data.get("params").get("update_instance_details"):
-            update_instance_details_user = self.data.get("params").get("update_instance_details")
-            params_model = self.update_params(resource, update_instance_details_user)
-            params_dict["update_instance_details"] = oci.core.models.UpdateInstanceDetails(
-                **params_model
-            )
+        update_instance_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_instance_details_user)
+        update_instance_details = oci.core.models.UpdateInstanceDetails(**params_model)
         response = client.update_instance(
-            instance_id=params_dict["instance_id"],
-            update_instance_details=params_dict["update_instance_details"],
+            instance_id=resource.get("id"), update_instance_details=update_instance_details
         )
         log.info(f"Received status {response.status} for PUT:update_instance {response.request_id}")
         return response
 
 
-@Instance.action_registry.register("remove-tag")
-class RemoveTagActionInstance(RemoveTagBaseAction):
+@Instance.filter_registry.register("metrics")
+class InstanceMetrics(Filter):
     """
-    Remove Tag Action
+    Instance Metrics Filter
 
     :example:
 
-        Remove the specified tags from the resource. Defined tag needs to be referred as 'namespace.tagName' as below in the policy file.
+    This filter returns the resources with the aggregated metrics data that match the criteria specified in the request.
+    Compartment OCID required. For information on metric queries, see `Building Metric Queries
+    <https://docs.oracle.com/en-us/iaas/Content/Monitoring/Tasks/buildingqueries.htm>`_.
 
     .. code-block:: yaml
 
         policies:
-            - name: remove-tag
-              resource: oci.instance
-            actions:
-              - type: remove-tag
-                defined_tags: ['cloud_custodian.environment']
-                freeform_tags: ['organization', 'team']
+            - name: instance-with-low-cpu-utilization
+            description: |
+                Return the instances with the low CPU utilization
+            resource: oci.instance
+            filters:
+                - type: metrics
+                  query: 'CpuUtilization[30d].mean() < 6'
 
     """  # noqa
 
-    def perform_action(self, resource):
-        client = self.manager.get_client()
-        params_dict = {}
-        params_dict["instance_id"] = resource.get("id")
-        original_tag_count = self.tag_count(resource)
-        params_model = self.remove_tag(resource)
-        updated_tag_count = self.tag_count(params_model)
-        params_dict["update_instance_details"] = oci.core.models.UpdateInstanceDetails(
-            **params_model
+    schema = type_schema("metrics", query={"type": "string"}, required=["query"])
+
+    def process(self, resources, event):
+        summarize_metrics = oci.monitoring.models.SummarizeMetricsDataDetails(
+            query=self.data.get("query"),
+            namespace="oci_computeagent",
         )
-        if self.tag_removed_from_resource(original_tag_count, updated_tag_count):
-            response = client.update_instance(
-                instance_id=params_dict["instance_id"],
-                update_instance_details=params_dict["update_instance_details"],
-            )
-            log.debug(
-                f"Received status {response.status} for PUT:update_instance:remove-tag"
-                f" {response.request_id}"
-            )
-            return response
-        else:
-            log.debug(
-                "No tags matched. Skipping the remove-tag action on this resource - %s",
-                resource.get("display_name"),
+        monitoring_client = self.manager.get_session().client("oci.monitoring.MonitoringClient")
+        comp_resources = {}
+        result = []
+        for resource in resources:
+            comp_id = resource.get("compartment_id")
+            if comp_id in comp_resources:
+                comp_resources.get(comp_id).append(resource)
+            else:
+                comp_resources[comp_id] = [resource]
+        # Query the MonitoringClient with the query against each compartment and perform
+        # the filtering
+        for compartment_id in comp_resources.keys():
+            metric_response = monitoring_client.summarize_metrics_data(
+                compartment_id=compartment_id,
+                summarize_metrics_data_details=summarize_metrics,
             )
-            return None
+            for metric_data in metric_response.data:
+                resource_id = metric_data.dimensions["resourceId"]
+                for resource in comp_resources.get(compartment_id):
+                    if resource.get("id") == resource_id:
+                        result.append(resource)
+        return result
```

## c7n_oci/resources/dns.py

```diff
@@ -40,16 +40,16 @@
         extra_params = {"compartment_id"}
         resource_type = "OCI.Dns/Zone"
         id = "id"
         name = "name"
         search_resource_type = "customerdnszone"
 
 
-@Zone.action_registry.register("update-zone")
-class UpdateZone(OCIBaseAction):
+@Zone.action_registry.register("update")
+class UpdateZoneAction(OCIBaseAction):
     """
         Update zone Action
 
         :example:
 
         Updates the zone with the specified information.
 
@@ -64,38 +64,34 @@
 
         .. code-block:: yaml
 
             policies:
                 - name: perform-update-zone-action
                   resource: oci.zone
                   actions:
-                    - type: update-zone
+                    - type: update
+                      defined_tags:
+                        Cloud_Custodian: True
+                      freeform_tags:
+                        Environment: development
 
     """  # noqa
 
-    schema = type_schema("update-zone", params={"type": "object"}, rinherit=OCIBaseAction.schema)
+    schema = type_schema(
+        "update", **{"freeform_tags": {"type": "object"}, "defined_tags": {"type": "object"}}
+    )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["zone_name_or_id"] = resource.get("id")
-        if self.data.get("params").get("update_zone_details"):
-            update_zone_details_user = self.data.get("params").get("update_zone_details")
-            params_model = self.update_params(resource, update_zone_details_user)
-            params_dict["update_zone_details"] = oci.dns.models.UpdateZoneDetails(**params_model)
-        if self.data.get("params") and self.data.get("params").get("scope"):
-            params_dict["scope"] = self.data.get("params").get("scope")
-        if self.data.get("params") and self.data.get("params").get("view_id"):
-            params_dict["view_id"] = self.data.get("params").get("view_id")
-        if self.data.get("params") and self.data.get("params").get("compartment_id"):
-            params_dict["compartment_id"] = self.data.get("params").get("compartment_id")
+        update_zone_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_zone_details_user)
+        update_zone_details = oci.dns.models.UpdateZoneDetails(**params_model)
         response = client.update_zone(
-            zone_name_or_id=params_dict["zone_name_or_id"],
-            update_zone_details=params_dict["update_zone_details"],
+            zone_name_or_id=resource.get("id"),
+            update_zone_details=update_zone_details,
         )
         log.info(f"Received status {response.status} for PUT:update_zone {response.request_id}")
         return response
 
 
 @Zone.action_registry.register("remove-tag")
 class RemoveTagActionZone(RemoveTagBaseAction):
```

## c7n_oci/resources/identity.py

```diff
@@ -40,16 +40,16 @@
         extra_params = {"compartment_id"}
         resource_type = "OCI.Identity/Compartment"
         id = "id"
         name = "name"
         search_resource_type = "compartment"
 
 
-@Compartment.action_registry.register("update-compartment")
-class UpdateCompartment(OCIBaseAction):
+@Compartment.action_registry.register("update")
+class UpdateCompartmentAction(OCIBaseAction):
     """
     Update compartment Action
 
     :example:
 
     Updates the specified compartment's description or name. You can't update the root compartment.
 
@@ -58,38 +58,33 @@
 
     .. code-block:: yaml
 
         policies:
             - name: perform-update-compartment-action
               resource: oci.compartment
               actions:
-                - type: update-compartment
+                - type: update
+                  defined_tags:
+                     Cloud_Custodian: True
+                  freeform_tags:
+                     Environment: development
 
     """  # noqa
 
     schema = type_schema(
-        "update-compartment", params={"type": "object"}, rinherit=OCIBaseAction.schema
+        "update", **{"freeform_tags": {"type": "object"}, "defined_tags": {"type": "object"}}
     )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["compartment_id"] = resource.get("id")
-        if self.data.get("params").get("update_compartment_details"):
-            update_compartment_details_user = self.data.get("params").get(
-                "update_compartment_details"
-            )
-            params_model = self.update_params(resource, update_compartment_details_user)
-            params_dict[
-                "update_compartment_details"
-            ] = oci.identity.models.UpdateCompartmentDetails(**params_model)
+        update_compartment_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_compartment_details_user)
+        update_compartment_details = oci.identity.models.UpdateCompartmentDetails(**params_model)
         response = client.update_compartment(
-            compartment_id=params_dict["compartment_id"],
-            update_compartment_details=params_dict["update_compartment_details"],
+            compartment_id=resource.get("id"), update_compartment_details=update_compartment_details
         )
         log.info(
             f"Received status {response.status} for PUT:update_compartment {response.request_id}"
         )
         return response
 
 
@@ -166,16 +161,16 @@
         extra_params = {"compartment_id"}
         resource_type = "OCI.Identity/Group"
         id = "id"
         name = "name"
         search_resource_type = "group"
 
 
-@Group.action_registry.register("update-group")
-class UpdateGroup(OCIBaseAction):
+@Group.action_registry.register("update")
+class UpdateGroupAction(OCIBaseAction):
     """
     Update group Action
 
     :example:
 
     Updates the specified group.
 
@@ -184,34 +179,33 @@
 
     .. code-block:: yaml
 
         policies:
             - name: perform-update-group-action
               resource: oci.group
               actions:
-                - type: update-group
+                - type: update
+                  defined_tags:
+                     Cloud_Custodian: True
+                  freeform_tags:
+                     Environment: development
 
     """  # noqa
 
-    schema = type_schema("update-group", params={"type": "object"}, rinherit=OCIBaseAction.schema)
+    schema = type_schema(
+        "update", **{"freeform_tags": {"type": "object"}, "defined_tags": {"type": "object"}}
+    )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["group_id"] = resource.get("id")
-        if self.data.get("params").get("update_group_details"):
-            update_group_details_user = self.data.get("params").get("update_group_details")
-            params_model = self.update_params(resource, update_group_details_user)
-            params_dict["update_group_details"] = oci.identity.models.UpdateGroupDetails(
-                **params_model
-            )
+        update_group_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_group_details_user)
+        update_group_details = oci.identity.models.UpdateGroupDetails(**params_model)
         response = client.update_group(
-            group_id=params_dict["group_id"],
-            update_group_details=params_dict["update_group_details"],
+            group_id=resource.get("id"), update_group_details=update_group_details
         )
         log.info(f"Received status {response.status} for PUT:update_group {response.request_id}")
         return response
 
 
 @Group.action_registry.register("remove-tag")
 class RemoveTagActionGroup(RemoveTagBaseAction):
@@ -284,16 +278,16 @@
         extra_params = {"compartment_id"}
         resource_type = "OCI.Identity/User"
         id = "id"
         name = "name"
         search_resource_type = "user"
 
 
-@User.action_registry.register("update-user")
-class UpdateUser(OCIBaseAction):
+@User.action_registry.register("update")
+class UpdateUserAction(OCIBaseAction):
     """
     Update user Action
 
     :example:
 
     Updates the description of the specified user.
 
@@ -302,34 +296,34 @@
 
     .. code-block:: yaml
 
         policies:
             - name: perform-update-user-action
               resource: oci.user
               actions:
-                - type: update-user
+                - type: update
+                  defined_tags:
+                     Cloud_Custodian: True
+                  freeform_tags:
+                     Environment: development
+
 
     """  # noqa
 
-    schema = type_schema("update-user", params={"type": "object"}, rinherit=OCIBaseAction.schema)
+    schema = type_schema(
+        "update", **{"freeform_tags": {"type": "object"}, "defined_tags": {"type": "object"}}
+    )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["user_id"] = resource.get("id")
-        if self.data.get("params").get("update_user_details"):
-            update_user_details_user = self.data.get("params").get("update_user_details")
-            params_model = self.update_params(resource, update_user_details_user)
-            params_dict["update_user_details"] = oci.identity.models.UpdateUserDetails(
-                **params_model
-            )
+        update_user_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_user_details_user)
+        update_user_details = oci.identity.models.UpdateUserDetails(**params_model)
         response = client.update_user(
-            user_id=params_dict["user_id"],
-            update_user_details=params_dict["update_user_details"],
+            user_id=resource.get("id"), update_user_details=update_user_details
         )
         log.info(f"Received status {response.status} for PUT:update_user {response.request_id}")
         return response
 
 
 @User.action_registry.register("remove-tag")
 class RemoveTagActionUser(RemoveTagBaseAction):
```

## c7n_oci/resources/object_storage.py

```diff
@@ -46,16 +46,16 @@
 
     def _get_extra_params(self):
         kw = {}
         kw[STORAGE_NAMESPACE] = self.get_client().get_namespace().data
         return kw
 
 
-@Bucket.action_registry.register("update-bucket")
-class UpdateBucket(OCIBaseAction):
+@Bucket.action_registry.register("update")
+class UpdateBucketAction(OCIBaseAction):
     """
         Update bucket Action
 
         :example:
 
         Performs a partial or full update of a bucket's user-defined metadata.
 
@@ -69,39 +69,42 @@
 
         .. code-block:: yaml
 
             policies:
                 - name: perform-update-bucket-action
                   resource: oci.bucket
                   actions:
-                    - type: update-bucket
+                    - type: update
+                      defined_tags:
+                         Cloud_Custodian: True
+                      freeform_tags:
+                         Environment: development
+                      public_access_type: "NoPublicAccess"
+
 
     """  # noqa
 
-    schema = type_schema("update-bucket", params={"type": "object"}, rinherit=OCIBaseAction.schema)
+    schema = type_schema(
+        "update",
+        **{
+            "freeform_tags": {"type": "object"},
+            "defined_tags": {"type": "object"},
+            "public_access_type": {"type": "string"},
+        },
+    )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["namespace_name"] = resource.get("namespace")
-        if self.data.get("params") and self.data.get("params").get("bucket_name"):
-            params_dict["bucket_name"] = self.data.get("params").get("bucket_name")
-        else:
-            params_dict["bucket_name"] = resource.get("name")
-        if self.data.get("params").get("update_bucket_details"):
-            update_bucket_details_user = self.data.get("params").get("update_bucket_details")
-            params_model = self.update_params(resource, update_bucket_details_user)
-            params_dict["update_bucket_details"] = oci.object_storage.models.UpdateBucketDetails(
-                **params_model
-            )
+        update_bucket_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_bucket_details_user)
+        update_bucket_details = oci.object_storage.models.UpdateBucketDetails(**params_model)
         response = client.update_bucket(
-            namespace_name=params_dict["namespace_name"],
-            bucket_name=params_dict["bucket_name"],
-            update_bucket_details=params_dict["update_bucket_details"],
+            namespace_name=resource.get("namespace"),
+            bucket_name=resource.get("name"),
+            update_bucket_details=update_bucket_details,
         )
         log.info(f"Received status {response.status} for POST:update_bucket {response.request_id}")
         return response
 
 
 @Bucket.action_registry.register("remove-tag")
 class RemoveTagActionBucket(RemoveTagBaseAction):
```

## c7n_oci/resources/virtual_network.py

```diff
@@ -40,16 +40,18 @@
         extra_params = {"compartment_id"}
         resource_type = "OCI.VirtualNetwork/Cross_connect"
         id = "id"
         name = "display_name"
         search_resource_type = "crossconnect"
 
 
-@Cross_connect.action_registry.register("update-cross-connect")
-class UpdateCrossConnect(OCIBaseAction):
+Cross_connect.action_registry.register("update")
+
+
+class UpdateCrossConnectAction(OCIBaseAction):
     """
     Update cross connect Action
 
     :example:
 
     Updates the specified cross-connect.
 
@@ -58,38 +60,34 @@
 
     .. code-block:: yaml
 
         policies:
             - name: perform-update-cross-connect-action
               resource: oci.cross_connect
               actions:
-                - type: update-cross-connect
+                - type: update
+                  defined_tags:
+                     Cloud_Custodian: True
+                  freeform_tags:
+                     Environment: development
 
     """  # noqa
 
     schema = type_schema(
-        "update-cross-connect", params={"type": "object"}, rinherit=OCIBaseAction.schema
+        "update", **{"freeform_tags": {"type": "object"}, "defined_tags": {"type": "object"}}
     )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["cross_connect_id"] = resource.get("id")
-        if self.data.get("params").get("update_cross_connect_details"):
-            update_cross_connect_details_user = self.data.get("params").get(
-                "update_cross_connect_details"
-            )
-            params_model = self.update_params(resource, update_cross_connect_details_user)
-            params_dict["update_cross_connect_details"] = oci.core.models.UpdateCrossConnectDetails(
-                **params_model
-            )
+        update_cross_connect_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_cross_connect_details_user)
+        update_cross_connect_details = oci.core.models.UpdateCrossConnectDetails(**params_model)
         response = client.update_cross_connect(
-            cross_connect_id=params_dict["cross_connect_id"],
-            update_cross_connect_details=params_dict["update_cross_connect_details"],
+            cross_connect_id=resource.get("id"),
+            update_cross_connect_details=update_cross_connect_details,
         )
         log.info(
             f"Received status {response.status} for PUT:update_cross_connect {response.request_id}"
         )
         return response
 
 
@@ -166,16 +164,16 @@
         extra_params = {"compartment_id"}
         resource_type = "OCI.VirtualNetwork/Vcn"
         id = "id"
         name = "display_name"
         search_resource_type = "vcn"
 
 
-@Vcn.action_registry.register("update-vcn")
-class UpdateVcn(OCIBaseAction):
+@Vcn.action_registry.register("update")
+class UpdateVcnAction(OCIBaseAction):
     """
     Update vcn Action
 
     :example:
 
     Updates the specified VCN.
 
@@ -185,32 +183,33 @@
 
     .. code-block:: yaml
 
         policies:
             - name: perform-update-vcn-action
               resource: oci.vcn
               actions:
-                - type: update-vcn
+                - type: update
+                  defined_tags:
+                     Cloud_Custodian: True
+                  freeform_tags:
+                     Environment: development
 
     """  # noqa
 
-    schema = type_schema("update-vcn", params={"type": "object"}, rinherit=OCIBaseAction.schema)
+    schema = type_schema(
+        "update", **{"freeform_tags": {"type": "object"}, "defined_tags": {"type": "object"}}
+    )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["vcn_id"] = resource.get("id")
-        if self.data.get("params").get("update_vcn_details"):
-            update_vcn_details_user = self.data.get("params").get("update_vcn_details")
-            params_model = self.update_params(resource, update_vcn_details_user)
-            params_dict["update_vcn_details"] = oci.core.models.UpdateVcnDetails(**params_model)
+        update_vcn_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_vcn_details_user)
+        update_vcn_details = oci.core.models.UpdateVcnDetails(**params_model)
         response = client.update_vcn(
-            vcn_id=params_dict["vcn_id"],
-            update_vcn_details=params_dict["update_vcn_details"],
+            vcn_id=resource.get("id"), update_vcn_details=update_vcn_details
         )
         log.info(f"Received status {response.status} for PUT:update_vcn {response.request_id}")
         return response
 
 
 @Vcn.action_registry.register("remove-tag")
 class RemoveTagActionVcn(RemoveTagBaseAction):
@@ -283,16 +282,16 @@
         extra_params = {"compartment_id"}
         resource_type = "OCI.VirtualNetwork/Subnet"
         id = "id"
         name = "display_name"
         search_resource_type = "subnet"
 
 
-@Subnet.action_registry.register("update-subnet")
-class UpdateSubnet(OCIBaseAction):
+@Subnet.action_registry.register("update")
+class UpdateSubnetAction(OCIBaseAction):
     """
     Update subnet Action
 
     :example:
 
     Updates the specified subnet.
 
@@ -302,34 +301,33 @@
 
     .. code-block:: yaml
 
         policies:
             - name: perform-update-subnet-action
               resource: oci.subnet
               actions:
-                - type: update-subnet
+                - type: update
+                  defined_tags:
+                     Cloud_Custodian: True
+                  freeform_tags:
+                     Environment: development
 
     """  # noqa
 
-    schema = type_schema("update-subnet", params={"type": "object"}, rinherit=OCIBaseAction.schema)
+    schema = type_schema(
+        "update", **{"freeform_tags": {"type": "object"}, "defined_tags": {"type": "object"}}
+    )
 
     def perform_action(self, resource):
         client = self.manager.get_client()
-        params_dict = {}
-        params_model = {}
-        params_dict["subnet_id"] = resource.get("id")
-        if self.data.get("params").get("update_subnet_details"):
-            update_subnet_details_user = self.data.get("params").get("update_subnet_details")
-            params_model = self.update_params(resource, update_subnet_details_user)
-            params_dict["update_subnet_details"] = oci.core.models.UpdateSubnetDetails(
-                **params_model
-            )
+        update_subnet_details_user = self.extract_params(self.data)
+        params_model = self.update_params(resource, update_subnet_details_user)
+        update_subnet_details = oci.core.models.UpdateSubnetDetails(**params_model)
         response = client.update_subnet(
-            subnet_id=params_dict["subnet_id"],
-            update_subnet_details=params_dict["update_subnet_details"],
+            subnet_id=resource.get("id"), update_subnet_details=update_subnet_details
         )
         log.info(f"Received status {response.status} for PUT:update_subnet {response.request_id}")
         return response
 
 
 @Subnet.action_registry.register("remove-tag")
 class RemoveTagActionSubnet(RemoveTagBaseAction):
```

## c7n_oci/session.py

```diff
@@ -2,102 +2,71 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import importlib
 import logging
 import os
 
 import oci
-
-from c7n_oci.constants import (
-    ENV_FINGERPRINT,
-    ENV_USER,
-    ENV_KEY_FILE,
-    ENV_REGION,
-    ENV_TENANCY,
-    DEFAULT_PROFILE,
-)
+from c7n_oci.constants import ENV_FINGERPRINT, ENV_USER, ENV_KEY_FILE, ENV_REGION, ENV_TENANCY
 
 log = logging.getLogger("custodian.oci.session")
 
 
-class Session:
-    def __init__(self, config_file_path=None, profile_name=DEFAULT_PROFILE):
-        self.config = None
-        self.authenticated = False
-        self.config_file_path = config_file_path
-        self.profile_name = profile_name
-
-    def initialize_session(self):
-        if self.authenticated:
-            return
-        if os.environ.get(ENV_FINGERPRINT) is not None:
-            self.config = {
+class SessionFactory:
+    def __init__(self, profile=None):
+        self.profile = profile
+        self.user_agent_name = "Oracle-CloudCustodian"
+        self._config = self._set_oci_config()
+        self._authenticate_user()
+
+    def _set_oci_config(self):
+        config = None
+        if self._check_environment_variables():
+            config = {
                 "fingerprint": os.environ.get(ENV_FINGERPRINT),
                 "key_file": os.environ.get(ENV_KEY_FILE),
                 "region": os.environ.get(ENV_REGION),
                 "tenancy": os.environ.get(ENV_TENANCY),
                 "user": os.environ.get(ENV_USER),
             }
-        elif self.profile_name is not None and self.config_file_path is None:
-            self.config = oci.config.from_file(profile_name=self.profile_name)
-        elif self.profile_name is None and self.config_file_path is not None:
-            self.config = oci.config.from_file(self.config_file_path)
-        elif self.profile_name and self.config_file_path:
-            self.config = oci.config.from_file(self.config_file_path, self.profile_name)
+        elif self.profile:
+            config = oci.config.from_file(profile_name=self.profile)
         else:
-            self.config = oci.config.from_file()
+            config = oci.config.from_file()
 
-        self.config["additional_user_agent"] = (
-            f'Oracle-CloudCustodian {self.config["additional_user_agent"]}'
-            if self.config.get("additional_user_agent")
-            else "Oracle-CloudCustodian"
+        config["additional_user_agent"] = (
+            f'{self.user_agent_name} {config["additional_user_agent"]}'
+            if config.get("additional_user_agent")
+            else self.user_agent_name
         )
+        return config
 
-        # The next statements are just to verify that the config is working
-        try:
-            identity_client = oci.identity.IdentityClient(self.config)
+    def _check_environment_variables(self):
+        return all(
+            os.environ.get(env)
+            for env in [ENV_FINGERPRINT, ENV_KEY_FILE, ENV_REGION, ENV_TENANCY, ENV_USER]
+        )
 
-            response = identity_client.get_user(self.config.get("user"))
-            self.authenticated = True
+    def _authenticate_user(self):
+        try:
+            identity_client = oci.identity.IdentityClient(self._config)
+            response = identity_client.get_user(self._config.get("user"))
             log.info(f"Successfully authenticated user [{response.data.name}]")
         except Exception as e:
-            log.error("Failed to authenticate.\nMessage: {}".format(e))
+            log.error("Failed to authenticate user.\nMessage: {}".format(e))
 
-    def get_oci_config(self):
-        return self.config
+    def __call__(self):
+        session = Session(self._config)
+        return session
 
-    def client(self, client):
-        self.initialize_session()
-        service_name, client_name = client.rsplit(".", 1)
-        svc_module = importlib.import_module(service_name)
-        klass = getattr(svc_module, client_name)
 
-        client_args = {"config": self.config}
-        client = klass(**client_args)
-        return client
-
-    def get_monitoring_client(self):
-        """Creates and returns the MonitoringClient which is used for the Cross-Service querying
-
-        Returns:
-              object: MonitoringClient object to make call to Monitoring service
-        """
-        self.initialize_session()
-        svc_module = importlib.import_module("oci.monitoring")
-        klass = getattr(svc_module, "MonitoringClient")
-        client_args = {"config": self.config}
-        client = klass(**client_args)
-        return client
+class Session:
+    def __init__(self, config):
+        self._config = config
 
-    def get_work_request_client(self):
-        """Creates WorkRequestClient which is used to check the status of the submitted
-           asynchronous job
-
-        Returns:
-            object: WorkRequestClient object to check the status of the submitted job
-        """
-        self.initialize_session()
-        svc_module = importlib.import_module("oci.work_requests")
-        klass = getattr(svc_module, "WorkRequestClient")
-        client_args = {"config": self.config}
-        client = klass(**client_args)
+    def client(self, client_string):
+        service_name, client_name = client_string.rsplit(".", 1)
+        service_module = importlib.import_module(service_name)
+        client_class = getattr(service_module, client_name)
+        client_args = {"config": self._config}
+        client = client_class(**client_args)
         return client
```

## Comparing `c7n_oci-0.1.2.dist-info/METADATA` & `c7n_oci-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: c7n-oci
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cloud Custodian - OCI Support
 Home-page: https://cloudcustodian.io
 License: Apache-2.0
 Author: Cloud Custodian Project
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: oci (==2.104.3) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: oci (==2.107.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: certifi (==2023.5.7) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: circuitbreaker (==1.4.0) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: cryptography (==39.0.2) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: cryptography (==41.0.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pyopenssl (==23.2.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: python-dateutil (==2.8.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pytz (==2023.3) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: cffi (==1.15.1) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: six (==1.16.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pycparser (==2.21) ; python_version >= "3.7" and python_version < "4.0"
 Project-URL: Documentation, https://cloudcustodian.io/docs/
```

## Comparing `c7n_oci-0.1.2.dist-info/RECORD` & `c7n_oci-0.1.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 c7n_oci/actions/__init__.py,sha256=okTU25TaP5qgoKW5577FLJzV5Yg5kl1ybia9bM9LYeE,189
-c7n_oci/actions/base.py,sha256=wjD5V_0MtETYRh2A1VJXxKjDBS3yUMJhbzLsibeqtd0,6233
+c7n_oci/actions/base.py,sha256=_lmCAsc6GUeD--fyu1yZ-ADjJSRrKAoswqM0pvu64ao,6381
 c7n_oci/constants.py,sha256=mhLF4-P4V_SAtpQ3l8dJIxYfu9izYrH_VbqSofVCb4E,375
 c7n_oci/entry.py,sha256=QGCvJIlRM649dLHIFnZjnOMYZXX8Xv45_O1vwkzFHPc,388
 c7n_oci/filters/__init__.py,sha256=R2mFrmBMYQznzGuzGQD6mqkcos4U9cix1uSQkh0m2lA,79
-c7n_oci/provider.py,sha256=2ugJBPGN7bOAc3L5HdMvDhYvlTsJb8r0f5wXkk-I-_8,1019
-c7n_oci/query.py,sha256=qu3Ahhy5J0g_XP5iQuDO48D2vABkkEjQdyhRfgrbn4Q,7939
+c7n_oci/provider.py,sha256=FXDkNuwfgMdwMjkV0aKO3yVIoKXaAcBbc5JFYSQxVRk,825
+c7n_oci/query.py,sha256=yhcnP2LGqsy_hprZ-VsxXpFDoSgiEpf4pCxkr1njQc0,7917
 c7n_oci/resources/__init__.py,sha256=R2mFrmBMYQznzGuzGQD6mqkcos4U9cix1uSQkh0m2lA,79
-c7n_oci/resources/compute.py,sha256=eDbyWaWsyVzCvh8S1K5lTl670lWZ7kjQcm_od6nuO30,11621
-c7n_oci/resources/dns.py,sha256=JjgkXEvXs77hohJ_Khjc_1tNBTNFowr6VXRAlk3Vc-A,5178
-c7n_oci/resources/identity.py,sha256=fRnzrbHBm5QNkj_R3KF_zH_rGBHU3vcrJB1ST8BwTCM,33426
-c7n_oci/resources/object_storage.py,sha256=h_5qz92-DLIT1ogRM_RoAvtNQuCl0SfgNNRS9667bAA,6637
+c7n_oci/resources/compute.py,sha256=4ksG680Ckx1XeZkxbK6R51LradmkWu43DfjEogaCKlo,9672
+c7n_oci/resources/dns.py,sha256=OZslm4rtkcUTMma3vKhtDfglBUR1HilqAuFc_mnDS-s,4642
+c7n_oci/resources/identity.py,sha256=Y62wDVs93SUhktTUnwptZ4RTrS4k1vU3vTfIUR39hWg,33036
+c7n_oci/resources/object_storage.py,sha256=-G2wTH2n60T7mLTYXasfCS9h9mSBwpleNBqKtzQTpNU,6454
 c7n_oci/resources/resource_map.py,sha256=YJqd5DI-vpT3arof70BHt5X_evZe69sm1Gl-9qGxMLc,626
-c7n_oci/resources/virtual_network.py,sha256=yH8BOUqX-dz7v-AderS0FJnOkXRVD52Jza2My1R0CeA,12586
-c7n_oci/session.py,sha256=_5qGqo6gM_c1PdiJEyfKqaNw50ff237jJIbMw4oMm6E,3677
-c7n_oci-0.1.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-c7n_oci-0.1.2.dist-info/RECORD,,
-c7n_oci-0.1.2.dist-info/METADATA,sha256=Axgjd9QIEfXRemKsO9OOwo7x04kAmOb-UtvUGZ7p6eI,4294
+c7n_oci/resources/virtual_network.py,sha256=YbQasuc3Dn8eOjhWG0bsR3ywU5D3kFgjc2kiHdNZEg8,12225
+c7n_oci/session.py,sha256=Sdddgkq4oUNa-IJ_5y5A-tegEW49Yyz8Pu5rRqjOjF4,2406
+c7n_oci-0.1.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+c7n_oci-0.1.3.dist-info/RECORD,,
+c7n_oci-0.1.3.dist-info/METADATA,sha256=jaIe15GZs4gxub3FvZsJb9rlV_KrnVOuw-UObAaNF4Y,4294
```

