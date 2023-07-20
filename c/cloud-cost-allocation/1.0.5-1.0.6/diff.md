# Comparing `tmp/cloud-cost-allocation-1.0.5.tar.gz` & `tmp/cloud-cost-allocation-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-cost-allocation-1.0.5.tar", last modified: Wed Jul  5 06:46:11 2023, max compression
+gzip compressed data, was "cloud-cost-allocation-1.0.6.tar", last modified: Thu Jul 20 15:50:30 2023, max compression
```

## Comparing `cloud-cost-allocation-1.0.5.tar` & `cloud-cost-allocation-1.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.897341 cloud-cost-allocation-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-07-05 06:46:11.897341 cloud-cost-allocation-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.889341 cloud-cost-allocation-1.0.5/cloud_cost_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23784 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/cloud_cost_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43878 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/cost_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/base_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/cloud_cost_allocation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-07-05 06:46:11.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-05 06:46:11.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 06:46:11.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 06:46:11.000000 cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/puml/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/cost-allocation-model.puml
--rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/cost-allocation-model.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/hierarchical-service-consumption-example.puml
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/hierarchical-service-consumption-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/hierarchical-service-cost-allocation-example.puml
--rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/puml/hierarchical-service-cost-allocation-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-05 06:46:11.897341 cloud-cost-allocation-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 06:46:11.893341 cloud-cost-allocation-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-05 06:45:59.000000 cloud-cost-allocation-1.0.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:30.749139 cloud-cost-allocation-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21187 2023-07-20 15:50:30.749139 cloud-cost-allocation-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:30.741139 cloud-cost-allocation-1.0.6/cloud_cost_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23784 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/cloud_cost_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43878 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/cost_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:30.745139 cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/base_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:30.745139 cloud-cost-allocation-1.0.6/cloud_cost_allocation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:30.745139 cloud-cost-allocation-1.0.6/cloud_cost_allocation/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/writer/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:30.741139 cloud-cost-allocation-1.0.6/cloud_cost_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21187 2023-07-20 15:50:30.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-20 15:50:30.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:50:30.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:50:30.000000 cloud-cost-allocation-1.0.6/cloud_cost_allocation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:30.749139 cloud-cost-allocation-1.0.6/puml/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/puml/cost-allocation-model.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/puml/cost-allocation-model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/puml/hierarchical-service-consumption-example.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/puml/hierarchical-service-consumption-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/puml/hierarchical-service-cost-allocation-example.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/puml/hierarchical-service-cost-allocation-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-20 15:50:30.749139 cloud-cost-allocation-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:50:30.749139 cloud-cost-allocation-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-20 15:50:18.000000 cloud-cost-allocation-1.0.6/tests/test.py
```

### Comparing `cloud-cost-allocation-1.0.5/LICENSE` & `cloud-cost-allocation-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/PKG-INFO` & `cloud-cost-allocation-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
@@ -60,16 +60,16 @@
 | *Product*             | A business product, which relies on one or multiple services. Products are somehow commercial packaging of services under the control of Product Managers.       |
 | *Product Dimension*   | An optional dimension for the cost report of a product, for example: a product feature, a product flavor, a market or a market segment.                          |
 | *Provider Service*    | The role of a service when it is consumed by another other service or product, a.k.a. a shared service.                                                          |
 | *Consumer Service*    | The role of a service when it consumes another service.                                                                                                          |
 | *Instance*            | A running instance or a deployment of a service. If we think of *Services* as *Classes* in object-oriented programming, then *Instances* would be the *Objects*. |
 | *Dimension*           | An optional dimension in the cost allocation, for example an environment like Test or Production, or a component in the architecture of the service.             |
 | *Meter*               | A meter that measures the functional activity or throughput of a service or of a product.                                                                        |
-| *Amortized Cost*      | The billing cost incremented with the amortized cost of the reservation purchases.                                                                               |
-| *On-demand Cost*      | The equivalent on-demand cost, i.e. as if no reservation purchase had been made.                                                                                 |
+| *Amortized Cost*      | The billing cost incremented with the amortized cost of the commitment-based purchases (reservations, saving plans).                                             |
+| *On-demand Cost*      | The equivalent on-demand cost, i.e. as if no commitment-based purchase had been made.                                                                            |
 | *Cost Item*           | A cost that is either coming from cloud provider billing or allocated by a provider service.                                                                     |
 | *Cost Allocation Key* | A numerical value to allocate a share of a cost. Cost share = cost * key / total keys.                                                                           |
 
 ## UML Class Diagram
 
 Keep calm and drink coffee.
 
@@ -114,17 +114,17 @@
     * Contrary to this, only the following costs are assigned to products from each service
         * The costs of cloud resources it uses directly and
         * Any costs from consumed services that did not report their costs to products
     * This ensures that there is no double counting of costs at product level
     * Assuming that all cloud resources are properly tagged and that services eventually allocate all their costs to products, then the costs of all cloud resources must be equal to the cost of all products
         * Similarly, the costs of a product that exclusively uses a single service would be equal to the total cost of that service
 8. On-demand costs and amortized costs are supported in parallel by the model
-    * Reporting the two is useful to investigate whether cost variations come from reservation management or something else
-    * Reporting the two is also useful for service owners and product managers alike to see the savings made thanks to the reservation purchases
-    * Reservation savings = On-demand costs - amortized costs
+    * Reporting the two is useful to investigate whether cost variations come from commitment management or something else
+    * Reporting the two is also useful for service owners and product managers alike to see the savings made thanks to the commitment-based purchases
+    * Commitment savings = On-demand costs - amortized costs
 9. Cycles in the cost allocation can be broken by providing a *service precedence list*
     * Example: A monitoring system *M* running on top of a container service *C* is also used by the container service itself
         * In this case, part of the costs of *M* should be assigned back to *C*
         * Since the costs of *C* are allocated to *M* (in part), this creates a loop
         * This cost allocation cycle *C* -> *M* -> *C* can be broken by specifying a precedence list *C,M*. In this case, *C* is allocated no cost from *M*
     * As another example, see `test5` 
     * The cost allocation could manage cycles in a more sophisticated way in the future
@@ -236,16 +236,21 @@
 # In case of list, first matching key is used
 Product = product
 
 [AzureEaAmortizedCost]
 
 # The service, instance, and dimensions to allocate Azure unused reservation cost
 UnusedReservationService = finops
-UnusedReservationInstance = reservation
-UnusedReservationComponent = unused
+UnusedReservationInstance = unused-commitment
+UnusedReservationComponent = reservation
+
+# The service, instance, and dimensions to allocate Azure unused savings plan cost
+UnusedSavingsPlanService = finops
+UnusedSavingsPlanInstance = unused-commitment
+UnusedSavingsPlanComponent = savings-plan
 
 [Cycles]
 
 # The precedence list for breaking cost allocation cycles
 # Here, the cycle a -> b -> d ->a will be broken to a -> b -> d (cost allocation d -> a is removed)
 ServicePrecedenceList = a,b,c
```

### Comparing `cloud-cost-allocation-1.0.5/README.md` & `cloud-cost-allocation-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 | *Product*             | A business product, which relies on one or multiple services. Products are somehow commercial packaging of services under the control of Product Managers.       |
 | *Product Dimension*   | An optional dimension for the cost report of a product, for example: a product feature, a product flavor, a market or a market segment.                          |
 | *Provider Service*    | The role of a service when it is consumed by another other service or product, a.k.a. a shared service.                                                          |
 | *Consumer Service*    | The role of a service when it consumes another service.                                                                                                          |
 | *Instance*            | A running instance or a deployment of a service. If we think of *Services* as *Classes* in object-oriented programming, then *Instances* would be the *Objects*. |
 | *Dimension*           | An optional dimension in the cost allocation, for example an environment like Test or Production, or a component in the architecture of the service.             |
 | *Meter*               | A meter that measures the functional activity or throughput of a service or of a product.                                                                        |
-| *Amortized Cost*      | The billing cost incremented with the amortized cost of the reservation purchases.                                                                               |
-| *On-demand Cost*      | The equivalent on-demand cost, i.e. as if no reservation purchase had been made.                                                                                 |
+| *Amortized Cost*      | The billing cost incremented with the amortized cost of the commitment-based purchases (reservations, saving plans).                                             |
+| *On-demand Cost*      | The equivalent on-demand cost, i.e. as if no commitment-based purchase had been made.                                                                            |
 | *Cost Item*           | A cost that is either coming from cloud provider billing or allocated by a provider service.                                                                     |
 | *Cost Allocation Key* | A numerical value to allocate a share of a cost. Cost share = cost * key / total keys.                                                                           |
 
 ## UML Class Diagram
 
 Keep calm and drink coffee.
 
@@ -86,17 +86,17 @@
     * Contrary to this, only the following costs are assigned to products from each service
         * The costs of cloud resources it uses directly and
         * Any costs from consumed services that did not report their costs to products
     * This ensures that there is no double counting of costs at product level
     * Assuming that all cloud resources are properly tagged and that services eventually allocate all their costs to products, then the costs of all cloud resources must be equal to the cost of all products
         * Similarly, the costs of a product that exclusively uses a single service would be equal to the total cost of that service
 8. On-demand costs and amortized costs are supported in parallel by the model
-    * Reporting the two is useful to investigate whether cost variations come from reservation management or something else
-    * Reporting the two is also useful for service owners and product managers alike to see the savings made thanks to the reservation purchases
-    * Reservation savings = On-demand costs - amortized costs
+    * Reporting the two is useful to investigate whether cost variations come from commitment management or something else
+    * Reporting the two is also useful for service owners and product managers alike to see the savings made thanks to the commitment-based purchases
+    * Commitment savings = On-demand costs - amortized costs
 9. Cycles in the cost allocation can be broken by providing a *service precedence list*
     * Example: A monitoring system *M* running on top of a container service *C* is also used by the container service itself
         * In this case, part of the costs of *M* should be assigned back to *C*
         * Since the costs of *C* are allocated to *M* (in part), this creates a loop
         * This cost allocation cycle *C* -> *M* -> *C* can be broken by specifying a precedence list *C,M*. In this case, *C* is allocated no cost from *M*
     * As another example, see `test5` 
     * The cost allocation could manage cycles in a more sophisticated way in the future
@@ -208,16 +208,21 @@
 # In case of list, first matching key is used
 Product = product
 
 [AzureEaAmortizedCost]
 
 # The service, instance, and dimensions to allocate Azure unused reservation cost
 UnusedReservationService = finops
-UnusedReservationInstance = reservation
-UnusedReservationComponent = unused
+UnusedReservationInstance = unused-commitment
+UnusedReservationComponent = reservation
+
+# The service, instance, and dimensions to allocate Azure unused savings plan cost
+UnusedSavingsPlanService = finops
+UnusedSavingsPlanInstance = unused-commitment
+UnusedSavingsPlanComponent = savings-plan
 
 [Cycles]
 
 # The precedence list for breaking cost allocation cycles
 # Here, the cycle a -> b -> d ->a will be broken to a -> b -> d (cost allocation d -> a is removed)
 ServicePrecedenceList = a,b,c
```

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/cloud_cost_allocator.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/cloud_cost_allocator.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/config.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/config.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/cost_items.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/cost_items.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/main.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/main.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,28 +35,31 @@
         if utils.is_float(cost_in_billing_currency):
             cloud_cost_item.amounts[0] = float(cost_in_billing_currency)
         else:
             error("CostInBillingCurrency cannot be parsed in line %s", line)
             return None
 
         # Compute and set on-demand cost (amount with index 1)
-        # https://docs.microsoft.com/en-us/azure/cost-management-billing/reservations/understand-reserved-instance-usage-ea
-        if line["ReservationId"]:
-            if line["ChargeType"] == "UnusedReservation":
-                cloud_cost_item.cloud_on_demand_cost = 0.0  # Unused reservations are not on-demand costs
+        # https://learn.microsoft.com/en-us/azure/cost-management-billing/reservations/understand-reserved-instance-usage-ea
+        # https://learn.microsoft.com/en-us/azure/cost-management-billing/savings-plan/utilization-cost-reports
+        pricing_model = line["PricingModel"]
+        charge_type = line["ChargeType"]
+        if pricing_model in ["Reservation", "SavingsPlan"]:
+            if charge_type in ["UnusedReservation", "UnusedSavingsPlan"]:
+                cloud_cost_item.cloud_on_demand_cost = 0.0  # Unused commitments are not on-demand costs
             else:
                 quantity = line["Quantity"]
                 unit_price = line["UnitPrice"]
                 if utils.is_float(quantity) and utils.is_float(unit_price):
                     cloud_cost_item.amounts[1] = float(quantity) * float(unit_price)
                 else:
                     error("Quantity or UnitPrice cannot be parsed in line %s", line)
-                    cloud_cost_item.amounts[1] = 0.0  # return None?
+                    cloud_cost_item.amounts[1] = 0.0  # Return None?
 
-        else:  # No reservation: on-demand cost is same as amortized cost
+        else:  # No unused commitment: on-demand cost is amortized cost
             cloud_cost_item.amounts[1] = cloud_cost_item.amounts[0]
 
         # Set currency
         cloud_cost_item.currency = line["BillingCurrencyCode"]
 
         # Process tags
         for tag in line["Tags"].split('","'):
@@ -65,29 +68,30 @@
                 if key_value_match:
                     key = key_value_match.group(1).strip().lower()
                     value = key_value_match.group(2).strip().lower()
                     cloud_cost_item.tags[key] = value
                 else:
                     error("Unexpected tag format in cost stream: '" + tag + "'")
 
-        # Process unused reservation
+        # Process unused commitment
         config = self.cost_item_factory.config
-        if line['ChargeType'] == 'UnusedReservation':
-            cloud_cost_item.service = config.config['AzureEaAmortizedCost']['UnusedReservationService']
-            if 'UnusedReservationInstance' in config.config['AzureEaAmortizedCost']:
-                cloud_cost_item.instance = config.config['AzureEaAmortizedCost']['UnusedReservationInstance']
+        if charge_type in ["UnusedReservation", "UnusedSavingsPlan"]:
+            cloud_cost_item.service = config.config['AzureEaAmortizedCost'][charge_type + 'Service']
+            unused_commitment_instance = charge_type + 'Instance'
+            if unused_commitment_instance in config.config['AzureEaAmortizedCost']:
+                cloud_cost_item.instance = config.config['AzureEaAmortizedCost'][unused_commitment_instance]
             else:
                 cloud_cost_item.instance = cloud_cost_item.service
             for dimension in config.dimensions:
-                unused_reservation_dimension = 'UnusedReservation' + dimension
-                if unused_reservation_dimension in config.config['AzureEaAmortizedCost']:
+                unused_commitment_dimension = charge_type + dimension
+                if unused_commitment_dimension in config.config['AzureEaAmortizedCost']:
                     cloud_cost_item.dimensions[dimension] =\
-                        config.config['AzureEaAmortizedCost'][unused_reservation_dimension]
+                        config.config['AzureEaAmortizedCost'][unused_commitment_dimension]
 
-        else:  # Not an unused reservation
+        else:  # Not an unused commitment
 
             # Fill cost item from tags
             self.fill_from_tags(cloud_cost_item)
 
             # Set default service
             if not cloud_cost_item.service:
                 cloud_cost_item.service = config.default_service
```

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/base_reader.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/base_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/csv_allocated_cost_reader.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/csv_allocated_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/utils/utils.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/base_writer.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/writer/base_writer.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation/writer/csv_allocated_cost_writer.py` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation/writer/csv_allocated_cost_writer.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/PKG-INFO` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
@@ -60,16 +60,16 @@
 | *Product*             | A business product, which relies on one or multiple services. Products are somehow commercial packaging of services under the control of Product Managers.       |
 | *Product Dimension*   | An optional dimension for the cost report of a product, for example: a product feature, a product flavor, a market or a market segment.                          |
 | *Provider Service*    | The role of a service when it is consumed by another other service or product, a.k.a. a shared service.                                                          |
 | *Consumer Service*    | The role of a service when it consumes another service.                                                                                                          |
 | *Instance*            | A running instance or a deployment of a service. If we think of *Services* as *Classes* in object-oriented programming, then *Instances* would be the *Objects*. |
 | *Dimension*           | An optional dimension in the cost allocation, for example an environment like Test or Production, or a component in the architecture of the service.             |
 | *Meter*               | A meter that measures the functional activity or throughput of a service or of a product.                                                                        |
-| *Amortized Cost*      | The billing cost incremented with the amortized cost of the reservation purchases.                                                                               |
-| *On-demand Cost*      | The equivalent on-demand cost, i.e. as if no reservation purchase had been made.                                                                                 |
+| *Amortized Cost*      | The billing cost incremented with the amortized cost of the commitment-based purchases (reservations, saving plans).                                             |
+| *On-demand Cost*      | The equivalent on-demand cost, i.e. as if no commitment-based purchase had been made.                                                                            |
 | *Cost Item*           | A cost that is either coming from cloud provider billing or allocated by a provider service.                                                                     |
 | *Cost Allocation Key* | A numerical value to allocate a share of a cost. Cost share = cost * key / total keys.                                                                           |
 
 ## UML Class Diagram
 
 Keep calm and drink coffee.
 
@@ -114,17 +114,17 @@
     * Contrary to this, only the following costs are assigned to products from each service
         * The costs of cloud resources it uses directly and
         * Any costs from consumed services that did not report their costs to products
     * This ensures that there is no double counting of costs at product level
     * Assuming that all cloud resources are properly tagged and that services eventually allocate all their costs to products, then the costs of all cloud resources must be equal to the cost of all products
         * Similarly, the costs of a product that exclusively uses a single service would be equal to the total cost of that service
 8. On-demand costs and amortized costs are supported in parallel by the model
-    * Reporting the two is useful to investigate whether cost variations come from reservation management or something else
-    * Reporting the two is also useful for service owners and product managers alike to see the savings made thanks to the reservation purchases
-    * Reservation savings = On-demand costs - amortized costs
+    * Reporting the two is useful to investigate whether cost variations come from commitment management or something else
+    * Reporting the two is also useful for service owners and product managers alike to see the savings made thanks to the commitment-based purchases
+    * Commitment savings = On-demand costs - amortized costs
 9. Cycles in the cost allocation can be broken by providing a *service precedence list*
     * Example: A monitoring system *M* running on top of a container service *C* is also used by the container service itself
         * In this case, part of the costs of *M* should be assigned back to *C*
         * Since the costs of *C* are allocated to *M* (in part), this creates a loop
         * This cost allocation cycle *C* -> *M* -> *C* can be broken by specifying a precedence list *C,M*. In this case, *C* is allocated no cost from *M*
     * As another example, see `test5` 
     * The cost allocation could manage cycles in a more sophisticated way in the future
@@ -236,16 +236,21 @@
 # In case of list, first matching key is used
 Product = product
 
 [AzureEaAmortizedCost]
 
 # The service, instance, and dimensions to allocate Azure unused reservation cost
 UnusedReservationService = finops
-UnusedReservationInstance = reservation
-UnusedReservationComponent = unused
+UnusedReservationInstance = unused-commitment
+UnusedReservationComponent = reservation
+
+# The service, instance, and dimensions to allocate Azure unused savings plan cost
+UnusedSavingsPlanService = finops
+UnusedSavingsPlanInstance = unused-commitment
+UnusedSavingsPlanComponent = savings-plan
 
 [Cycles]
 
 # The precedence list for breaking cost allocation cycles
 # Here, the cycle a -> b -> d ->a will be broken to a -> b -> d (cost allocation d -> a is removed)
 ServicePrecedenceList = a,b,c
```

### Comparing `cloud-cost-allocation-1.0.5/cloud_cost_allocation.egg-info/SOURCES.txt` & `cloud-cost-allocation-1.0.6/cloud_cost_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/puml/cost-allocation-model.puml` & `cloud-cost-allocation-1.0.6/puml/cost-allocation-model.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/puml/cost-allocation-model.svg` & `cloud-cost-allocation-1.0.6/puml/cost-allocation-model.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/puml/hierarchical-service-consumption-example.puml` & `cloud-cost-allocation-1.0.6/puml/hierarchical-service-consumption-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/puml/hierarchical-service-consumption-example.svg` & `cloud-cost-allocation-1.0.6/puml/hierarchical-service-consumption-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/puml/hierarchical-service-cost-allocation-example.puml` & `cloud-cost-allocation-1.0.6/puml/hierarchical-service-cost-allocation-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/puml/hierarchical-service-cost-allocation-example.svg` & `cloud-cost-allocation-1.0.6/puml/hierarchical-service-cost-allocation-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/setup.cfg` & `cloud-cost-allocation-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.5/setup.py` & `cloud-cost-allocation-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Import readme
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme_file:
     readme = readme_file.read()
 
 # Setup
 setup(
     name='cloud-cost-allocation',
-    version='1.0.5',
+    version='1.0.6',
     description='Python library for shared, hierarchical cost allocation based on user-defined usage metrics.',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=['cloud_cost_allocation',
               'cloud_cost_allocation.reader',
               'cloud_cost_allocation.utils',
               'cloud_cost_allocation.writer'],
```

### Comparing `cloud-cost-allocation-1.0.5/tests/test.py` & `cloud-cost-allocation-1.0.6/tests/test.py`

 * *Files identical despite different names*

