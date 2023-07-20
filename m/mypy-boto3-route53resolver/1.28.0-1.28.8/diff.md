# Comparing `tmp/mypy-boto3-route53resolver-1.28.0.tar.gz` & `tmp/mypy-boto3-route53resolver-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53resolver-1.28.0.tar", last modified: Thu Jul  6 21:00:29 2023, max compression
+gzip compressed data, was "mypy-boto3-route53resolver-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-route53resolver-1.28.0.tar` & `mypy-boto3-route53resolver-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.678415 mypy-boto3-route53resolver-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-07-06 21:00:29.678415 mypy-boto3-route53resolver-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23101 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.670415 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55274 2023-07-06 20:53:44.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55189 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-07-06 20:53:44.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-07-06 20:53:44.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-07-06 20:53:44.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-06 20:53:44.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57065 2023-07-06 20:53:49.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57024 2023-07-06 20:53:45.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:29.678415 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-07-06 21:00:29.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 21:00:29.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:29.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:29.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:29.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 21:00:29.000000 mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:29.678415 mypy-boto3-route53resolver-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 20:53:43.000000 mypy-boto3-route53resolver-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.004775 mypy-boto3-route53resolver-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-20 19:47:56.000775 mypy-boto3-route53resolver-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59202 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59111 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20774 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20756 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61212 2023-07-20 19:47:05.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61167 2023-07-20 19:47:04.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.004775 mypy-boto3-route53resolver-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/setup.py
```

### Comparing `mypy-boto3-route53resolver-1.28.0/LICENSE` & `mypy-boto3-route53resolver-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.0/PKG-INFO` & `mypy-boto3-route53resolver-1.28.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53resolver
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53Resolver 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.Route53Resolver 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,14 +287,15 @@
 from mypy_boto3_route53resolver.paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -320,14 +321,17 @@
 )
 list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator(
     "list_firewall_rule_groups"
 )
 list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator(
     "list_firewall_rules"
 )
+list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator(
+    "list_outpost_resolvers"
+)
 list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator(
     "list_resolver_configs"
 )
 list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator(
     "list_resolver_dnssec_configs"
 )
 list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = (
@@ -375,24 +379,26 @@
     IpAddressStatusType,
     ListFirewallConfigsPaginatorName,
     ListFirewallDomainListsPaginatorName,
     ListFirewallDomainsPaginatorName,
     ListFirewallRuleGroupAssociationsPaginatorName,
     ListFirewallRuleGroupsPaginatorName,
     ListFirewallRulesPaginatorName,
+    ListOutpostResolversPaginatorName,
     ListResolverConfigsPaginatorName,
     ListResolverDnssecConfigsPaginatorName,
     ListResolverEndpointIpAddressesPaginatorName,
     ListResolverEndpointsPaginatorName,
     ListResolverQueryLogConfigAssociationsPaginatorName,
     ListResolverQueryLogConfigsPaginatorName,
     ListResolverRuleAssociationsPaginatorName,
     ListResolverRulesPaginatorName,
     ListTagsForResourcePaginatorName,
     MutationProtectionStatusType,
+    OutpostResolverStatusType,
     ResolverAutodefinedReverseStatusType,
     ResolverDNSSECValidationStatusType,
     ResolverEndpointDirectionType,
     ResolverEndpointStatusType,
     ResolverEndpointTypeType,
     ResolverQueryLogConfigAssociationErrorType,
     ResolverQueryLogConfigAssociationStatusType,
@@ -422,108 +428,106 @@
 `mypy_boto3_route53resolver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53resolver.type_defs import (
     TagTypeDef,
     FirewallRuleGroupAssociationTypeDef,
+    ResponseMetadataTypeDef,
     IpAddressUpdateTypeDef,
     ResolverEndpointTypeDef,
     AssociateResolverQueryLogConfigRequestRequestTypeDef,
     ResolverQueryLogConfigAssociationTypeDef,
     AssociateResolverRuleRequestRequestTypeDef,
     ResolverRuleAssociationTypeDef,
     FirewallDomainListTypeDef,
     FirewallRuleGroupTypeDef,
     CreateFirewallRuleRequestRequestTypeDef,
     FirewallRuleTypeDef,
+    OutpostResolverTypeDef,
     IpAddressRequestTypeDef,
     ResolverQueryLogConfigTypeDef,
     TargetAddressTypeDef,
     DeleteFirewallDomainListRequestRequestTypeDef,
     DeleteFirewallRuleGroupRequestRequestTypeDef,
     DeleteFirewallRuleRequestRequestTypeDef,
+    DeleteOutpostResolverRequestRequestTypeDef,
     DeleteResolverEndpointRequestRequestTypeDef,
     DeleteResolverQueryLogConfigRequestRequestTypeDef,
     DeleteResolverRuleRequestRequestTypeDef,
     DisassociateFirewallRuleGroupRequestRequestTypeDef,
     DisassociateResolverQueryLogConfigRequestRequestTypeDef,
     DisassociateResolverRuleRequestRequestTypeDef,
     FilterTypeDef,
     FirewallConfigTypeDef,
     FirewallDomainListMetadataTypeDef,
     FirewallRuleGroupMetadataTypeDef,
     GetFirewallConfigRequestRequestTypeDef,
     GetFirewallDomainListRequestRequestTypeDef,
     GetFirewallRuleGroupAssociationRequestRequestTypeDef,
     GetFirewallRuleGroupPolicyRequestRequestTypeDef,
-    GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupRequestRequestTypeDef,
+    GetOutpostResolverRequestRequestTypeDef,
     GetResolverConfigRequestRequestTypeDef,
     ResolverConfigTypeDef,
     GetResolverDnssecConfigRequestRequestTypeDef,
     ResolverDnssecConfigTypeDef,
     GetResolverEndpointRequestRequestTypeDef,
     GetResolverQueryLogConfigAssociationRequestRequestTypeDef,
     GetResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigRequestRequestTypeDef,
     GetResolverRuleAssociationRequestRequestTypeDef,
     GetResolverRulePolicyRequestRequestTypeDef,
-    GetResolverRulePolicyResponseTypeDef,
     GetResolverRuleRequestRequestTypeDef,
     ImportFirewallDomainsRequestRequestTypeDef,
-    ImportFirewallDomainsResponseTypeDef,
     IpAddressResponseTypeDef,
-    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallConfigsRequestRequestTypeDef,
-    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
     ListFirewallDomainListsRequestRequestTypeDef,
-    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
     ListFirewallDomainsRequestRequestTypeDef,
-    ListFirewallDomainsResponseTypeDef,
-    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
     ListFirewallRuleGroupAssociationsRequestRequestTypeDef,
-    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
     ListFirewallRuleGroupsRequestRequestTypeDef,
-    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
     ListFirewallRulesRequestRequestTypeDef,
-    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListOutpostResolversRequestRequestTypeDef,
     ListResolverConfigsRequestRequestTypeDef,
-    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
     ListResolverEndpointIpAddressesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutFirewallRuleGroupPolicyRequestRequestTypeDef,
-    PutFirewallRuleGroupPolicyResponseTypeDef,
     PutResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    PutResolverQueryLogConfigPolicyResponseTypeDef,
     PutResolverRulePolicyRequestRequestTypeDef,
-    PutResolverRulePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
+    TargetAddressOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallConfigRequestRequestTypeDef,
     UpdateFirewallDomainsRequestRequestTypeDef,
-    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
     UpdateFirewallRuleRequestRequestTypeDef,
     UpdateIpAddressTypeDef,
+    UpdateOutpostResolverRequestRequestTypeDef,
     UpdateResolverConfigRequestRequestTypeDef,
     UpdateResolverDnssecConfigRequestRequestTypeDef,
     AssociateFirewallRuleGroupRequestRequestTypeDef,
     CreateFirewallDomainListRequestRequestTypeDef,
     CreateFirewallRuleGroupRequestRequestTypeDef,
+    CreateOutpostResolverRequestRequestTypeDef,
     CreateResolverQueryLogConfigRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateFirewallRuleGroupResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
+    GetFirewallRuleGroupPolicyResponseTypeDef,
+    GetResolverQueryLogConfigPolicyResponseTypeDef,
+    GetResolverRulePolicyResponseTypeDef,
+    ImportFirewallDomainsResponseTypeDef,
+    ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
+    PutFirewallRuleGroupPolicyResponseTypeDef,
+    PutResolverQueryLogConfigPolicyResponseTypeDef,
+    PutResolverRulePolicyResponseTypeDef,
+    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     AssociateResolverEndpointIpAddressRequestRequestTypeDef,
     DisassociateResolverEndpointIpAddressRequestRequestTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
@@ -544,46 +548,62 @@
     CreateFirewallRuleGroupResponseTypeDef,
     DeleteFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupResponseTypeDef,
     CreateFirewallRuleResponseTypeDef,
     DeleteFirewallRuleResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
     UpdateFirewallRuleResponseTypeDef,
+    CreateOutpostResolverResponseTypeDef,
+    DeleteOutpostResolverResponseTypeDef,
+    GetOutpostResolverResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
+    UpdateOutpostResolverResponseTypeDef,
     CreateResolverEndpointRequestRequestTypeDef,
     CreateResolverQueryLogConfigResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     CreateResolverRuleRequestRequestTypeDef,
     ResolverRuleConfigTypeDef,
-    ResolverRuleTypeDef,
-    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
     ListResolverDnssecConfigsRequestRequestTypeDef,
-    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
     ListResolverEndpointsRequestRequestTypeDef,
-    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
     ListResolverQueryLogConfigAssociationsRequestRequestTypeDef,
-    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
     ListResolverQueryLogConfigsRequestRequestTypeDef,
-    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
     ListResolverRuleAssociationsRequestRequestTypeDef,
-    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
     ListResolverRulesRequestRequestTypeDef,
     GetFirewallConfigResponseTypeDef,
     ListFirewallConfigsResponseTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
+    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
+    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
+    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
+    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    ListOutpostResolversRequestListOutpostResolversPaginateTypeDef,
+    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
+    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
+    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
+    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
+    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
+    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResolverRuleTypeDef,
     UpdateResolverEndpointRequestRequestTypeDef,
     UpdateResolverRuleRequestRequestTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     GetResolverRuleResponseTypeDef,
     ListResolverRulesResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
```

### Comparing `mypy-boto3-route53resolver-1.28.0/README.md` & `mypy-boto3-route53resolver-1.28.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -255,14 +255,15 @@
 from mypy_boto3_route53resolver.paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -288,14 +289,17 @@
 )
 list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator(
     "list_firewall_rule_groups"
 )
 list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator(
     "list_firewall_rules"
 )
+list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator(
+    "list_outpost_resolvers"
+)
 list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator(
     "list_resolver_configs"
 )
 list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator(
     "list_resolver_dnssec_configs"
 )
 list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = (
@@ -343,24 +347,26 @@
     IpAddressStatusType,
     ListFirewallConfigsPaginatorName,
     ListFirewallDomainListsPaginatorName,
     ListFirewallDomainsPaginatorName,
     ListFirewallRuleGroupAssociationsPaginatorName,
     ListFirewallRuleGroupsPaginatorName,
     ListFirewallRulesPaginatorName,
+    ListOutpostResolversPaginatorName,
     ListResolverConfigsPaginatorName,
     ListResolverDnssecConfigsPaginatorName,
     ListResolverEndpointIpAddressesPaginatorName,
     ListResolverEndpointsPaginatorName,
     ListResolverQueryLogConfigAssociationsPaginatorName,
     ListResolverQueryLogConfigsPaginatorName,
     ListResolverRuleAssociationsPaginatorName,
     ListResolverRulesPaginatorName,
     ListTagsForResourcePaginatorName,
     MutationProtectionStatusType,
+    OutpostResolverStatusType,
     ResolverAutodefinedReverseStatusType,
     ResolverDNSSECValidationStatusType,
     ResolverEndpointDirectionType,
     ResolverEndpointStatusType,
     ResolverEndpointTypeType,
     ResolverQueryLogConfigAssociationErrorType,
     ResolverQueryLogConfigAssociationStatusType,
@@ -390,108 +396,106 @@
 `mypy_boto3_route53resolver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53resolver.type_defs import (
     TagTypeDef,
     FirewallRuleGroupAssociationTypeDef,
+    ResponseMetadataTypeDef,
     IpAddressUpdateTypeDef,
     ResolverEndpointTypeDef,
     AssociateResolverQueryLogConfigRequestRequestTypeDef,
     ResolverQueryLogConfigAssociationTypeDef,
     AssociateResolverRuleRequestRequestTypeDef,
     ResolverRuleAssociationTypeDef,
     FirewallDomainListTypeDef,
     FirewallRuleGroupTypeDef,
     CreateFirewallRuleRequestRequestTypeDef,
     FirewallRuleTypeDef,
+    OutpostResolverTypeDef,
     IpAddressRequestTypeDef,
     ResolverQueryLogConfigTypeDef,
     TargetAddressTypeDef,
     DeleteFirewallDomainListRequestRequestTypeDef,
     DeleteFirewallRuleGroupRequestRequestTypeDef,
     DeleteFirewallRuleRequestRequestTypeDef,
+    DeleteOutpostResolverRequestRequestTypeDef,
     DeleteResolverEndpointRequestRequestTypeDef,
     DeleteResolverQueryLogConfigRequestRequestTypeDef,
     DeleteResolverRuleRequestRequestTypeDef,
     DisassociateFirewallRuleGroupRequestRequestTypeDef,
     DisassociateResolverQueryLogConfigRequestRequestTypeDef,
     DisassociateResolverRuleRequestRequestTypeDef,
     FilterTypeDef,
     FirewallConfigTypeDef,
     FirewallDomainListMetadataTypeDef,
     FirewallRuleGroupMetadataTypeDef,
     GetFirewallConfigRequestRequestTypeDef,
     GetFirewallDomainListRequestRequestTypeDef,
     GetFirewallRuleGroupAssociationRequestRequestTypeDef,
     GetFirewallRuleGroupPolicyRequestRequestTypeDef,
-    GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupRequestRequestTypeDef,
+    GetOutpostResolverRequestRequestTypeDef,
     GetResolverConfigRequestRequestTypeDef,
     ResolverConfigTypeDef,
     GetResolverDnssecConfigRequestRequestTypeDef,
     ResolverDnssecConfigTypeDef,
     GetResolverEndpointRequestRequestTypeDef,
     GetResolverQueryLogConfigAssociationRequestRequestTypeDef,
     GetResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigRequestRequestTypeDef,
     GetResolverRuleAssociationRequestRequestTypeDef,
     GetResolverRulePolicyRequestRequestTypeDef,
-    GetResolverRulePolicyResponseTypeDef,
     GetResolverRuleRequestRequestTypeDef,
     ImportFirewallDomainsRequestRequestTypeDef,
-    ImportFirewallDomainsResponseTypeDef,
     IpAddressResponseTypeDef,
-    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallConfigsRequestRequestTypeDef,
-    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
     ListFirewallDomainListsRequestRequestTypeDef,
-    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
     ListFirewallDomainsRequestRequestTypeDef,
-    ListFirewallDomainsResponseTypeDef,
-    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
     ListFirewallRuleGroupAssociationsRequestRequestTypeDef,
-    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
     ListFirewallRuleGroupsRequestRequestTypeDef,
-    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
     ListFirewallRulesRequestRequestTypeDef,
-    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListOutpostResolversRequestRequestTypeDef,
     ListResolverConfigsRequestRequestTypeDef,
-    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
     ListResolverEndpointIpAddressesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutFirewallRuleGroupPolicyRequestRequestTypeDef,
-    PutFirewallRuleGroupPolicyResponseTypeDef,
     PutResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    PutResolverQueryLogConfigPolicyResponseTypeDef,
     PutResolverRulePolicyRequestRequestTypeDef,
-    PutResolverRulePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
+    TargetAddressOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallConfigRequestRequestTypeDef,
     UpdateFirewallDomainsRequestRequestTypeDef,
-    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
     UpdateFirewallRuleRequestRequestTypeDef,
     UpdateIpAddressTypeDef,
+    UpdateOutpostResolverRequestRequestTypeDef,
     UpdateResolverConfigRequestRequestTypeDef,
     UpdateResolverDnssecConfigRequestRequestTypeDef,
     AssociateFirewallRuleGroupRequestRequestTypeDef,
     CreateFirewallDomainListRequestRequestTypeDef,
     CreateFirewallRuleGroupRequestRequestTypeDef,
+    CreateOutpostResolverRequestRequestTypeDef,
     CreateResolverQueryLogConfigRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateFirewallRuleGroupResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
+    GetFirewallRuleGroupPolicyResponseTypeDef,
+    GetResolverQueryLogConfigPolicyResponseTypeDef,
+    GetResolverRulePolicyResponseTypeDef,
+    ImportFirewallDomainsResponseTypeDef,
+    ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
+    PutFirewallRuleGroupPolicyResponseTypeDef,
+    PutResolverQueryLogConfigPolicyResponseTypeDef,
+    PutResolverRulePolicyResponseTypeDef,
+    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     AssociateResolverEndpointIpAddressRequestRequestTypeDef,
     DisassociateResolverEndpointIpAddressRequestRequestTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
@@ -512,46 +516,62 @@
     CreateFirewallRuleGroupResponseTypeDef,
     DeleteFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupResponseTypeDef,
     CreateFirewallRuleResponseTypeDef,
     DeleteFirewallRuleResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
     UpdateFirewallRuleResponseTypeDef,
+    CreateOutpostResolverResponseTypeDef,
+    DeleteOutpostResolverResponseTypeDef,
+    GetOutpostResolverResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
+    UpdateOutpostResolverResponseTypeDef,
     CreateResolverEndpointRequestRequestTypeDef,
     CreateResolverQueryLogConfigResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     CreateResolverRuleRequestRequestTypeDef,
     ResolverRuleConfigTypeDef,
-    ResolverRuleTypeDef,
-    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
     ListResolverDnssecConfigsRequestRequestTypeDef,
-    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
     ListResolverEndpointsRequestRequestTypeDef,
-    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
     ListResolverQueryLogConfigAssociationsRequestRequestTypeDef,
-    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
     ListResolverQueryLogConfigsRequestRequestTypeDef,
-    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
     ListResolverRuleAssociationsRequestRequestTypeDef,
-    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
     ListResolverRulesRequestRequestTypeDef,
     GetFirewallConfigResponseTypeDef,
     ListFirewallConfigsResponseTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
+    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
+    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
+    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
+    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    ListOutpostResolversRequestListOutpostResolversPaginateTypeDef,
+    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
+    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
+    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
+    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
+    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
+    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResolverRuleTypeDef,
     UpdateResolverEndpointRequestRequestTypeDef,
     UpdateResolverRuleRequestRequestTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     GetResolverRuleResponseTypeDef,
     ListResolverRulesResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/__init__.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         Client,
         ListFirewallConfigsPaginator,
         ListFirewallDomainListsPaginator,
         ListFirewallDomainsPaginator,
         ListFirewallRuleGroupAssociationsPaginator,
         ListFirewallRuleGroupsPaginator,
         ListFirewallRulesPaginator,
+        ListOutpostResolversPaginator,
         ListResolverConfigsPaginator,
         ListResolverDnssecConfigsPaginator,
         ListResolverEndpointIpAddressesPaginator,
         ListResolverEndpointsPaginator,
         ListResolverQueryLogConfigAssociationsPaginator,
         ListResolverQueryLogConfigsPaginator,
         ListResolverRuleAssociationsPaginator,
@@ -30,14 +31,15 @@
 
     list_firewall_configs_paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
     list_firewall_domain_lists_paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
     list_firewall_domains_paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
     list_firewall_rule_group_associations_paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
     list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
     list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
+    list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")
     list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
     list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
     list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
     list_resolver_endpoints_paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
     list_resolver_query_log_config_associations_paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
     list_resolver_query_log_configs_paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
     list_resolver_rule_associations_paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
@@ -49,14 +51,15 @@
 from .paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -71,14 +74,15 @@
     "Client",
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
     "ListFirewallRulesPaginator",
+    "ListOutpostResolversPaginator",
     "ListResolverConfigsPaginator",
     "ListResolverDnssecConfigsPaginator",
     "ListResolverEndpointIpAddressesPaginator",
     "ListResolverEndpointsPaginator",
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/__init__.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         Client,
         ListFirewallConfigsPaginator,
         ListFirewallDomainListsPaginator,
         ListFirewallDomainsPaginator,
         ListFirewallRuleGroupAssociationsPaginator,
         ListFirewallRuleGroupsPaginator,
         ListFirewallRulesPaginator,
+        ListOutpostResolversPaginator,
         ListResolverConfigsPaginator,
         ListResolverDnssecConfigsPaginator,
         ListResolverEndpointIpAddressesPaginator,
         ListResolverEndpointsPaginator,
         ListResolverQueryLogConfigAssociationsPaginator,
         ListResolverQueryLogConfigsPaginator,
         ListResolverRuleAssociationsPaginator,
@@ -30,14 +31,15 @@
 
     list_firewall_configs_paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
     list_firewall_domain_lists_paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
     list_firewall_domains_paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
     list_firewall_rule_group_associations_paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
     list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
     list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
+    list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")
     list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
     list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
     list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
     list_resolver_endpoints_paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
     list_resolver_query_log_config_associations_paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
     list_resolver_query_log_configs_paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
     list_resolver_rule_associations_paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
@@ -49,14 +51,15 @@
 from .paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -70,14 +73,15 @@
     "Client",
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
     "ListFirewallRulesPaginator",
+    "ListOutpostResolversPaginator",
     "ListResolverConfigsPaginator",
     "ListResolverDnssecConfigsPaginator",
     "ListResolverEndpointIpAddressesPaginator",
     "ListResolverEndpointsPaginator",
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/__main__.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Resolver 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.Route53Resolver 1.28.8\nVersion:         1.28.8\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/client.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -53,33 +54,36 @@
     AssociateFirewallRuleGroupResponseTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     AssociateResolverQueryLogConfigResponseTypeDef,
     AssociateResolverRuleResponseTypeDef,
     CreateFirewallDomainListResponseTypeDef,
     CreateFirewallRuleGroupResponseTypeDef,
     CreateFirewallRuleResponseTypeDef,
+    CreateOutpostResolverResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     CreateResolverQueryLogConfigResponseTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteFirewallDomainListResponseTypeDef,
     DeleteFirewallRuleGroupResponseTypeDef,
     DeleteFirewallRuleResponseTypeDef,
+    DeleteOutpostResolverResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
     DisassociateResolverQueryLogConfigResponseTypeDef,
     DisassociateResolverRuleResponseTypeDef,
     FilterTypeDef,
     GetFirewallConfigResponseTypeDef,
     GetFirewallDomainListResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
     GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupResponseTypeDef,
+    GetOutpostResolverResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     GetResolverEndpointResponseTypeDef,
     GetResolverQueryLogConfigAssociationResponseTypeDef,
     GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     GetResolverRuleAssociationResponseTypeDef,
@@ -90,14 +94,15 @@
     IpAddressUpdateTypeDef,
     ListFirewallConfigsResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
     ListResolverEndpointsResponseTypeDef,
     ListResolverQueryLogConfigAssociationsResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     ListResolverRuleAssociationsResponseTypeDef,
@@ -110,14 +115,15 @@
     TagTypeDef,
     TargetAddressTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     UpdateFirewallRuleResponseTypeDef,
     UpdateIpAddressTypeDef,
+    UpdateOutpostResolverResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     UpdateResolverEndpointResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -148,14 +154,15 @@
     InvalidRequestException: Type[BotocoreClientError]
     InvalidTagException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
 class Route53ResolverClient(BaseClient):
     """
@@ -278,24 +285,43 @@
         Creates an empty DNS Firewall rule group for filtering DNS network traffic in a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_firewall_rule_group)
         """
 
+    def create_outpost_resolver(
+        self,
+        *,
+        CreatorRequestId: str,
+        Name: str,
+        PreferredInstanceType: str,
+        OutpostArn: str,
+        InstanceCount: int = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateOutpostResolverResponseTypeDef:
+        """
+        Creates an Route 53 Resolver on an Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_outpost_resolver)
+        """
+
     def create_resolver_endpoint(
         self,
         *,
         CreatorRequestId: str,
         SecurityGroupIds: Sequence[str],
         Direction: ResolverEndpointDirectionType,
         IpAddresses: Sequence[IpAddressRequestTypeDef],
         Name: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ResolverEndpointType: ResolverEndpointTypeType = ...
+        ResolverEndpointType: ResolverEndpointTypeType = ...,
+        OutpostArn: str = ...,
+        PreferredInstanceType: str = ...
     ) -> CreateResolverEndpointResponseTypeDef:
         """
         Creates a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_resolver_endpoint)
         """
@@ -362,14 +388,22 @@
         """
         Deletes the specified firewall rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#delete_firewall_rule_group)
         """
 
+    def delete_outpost_resolver(self, *, Id: str) -> DeleteOutpostResolverResponseTypeDef:
+        """
+        Deletes a Resolver on the Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_outpost_resolver)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#delete_outpost_resolver)
+        """
+
     def delete_resolver_endpoint(
         self, *, ResolverEndpointId: str
     ) -> DeleteResolverEndpointResponseTypeDef:
         """
         Deletes a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_resolver_endpoint)
@@ -496,14 +530,23 @@
         Returns the Identity and Access Management (Amazon Web Services IAM) policy for
         sharing the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_rule_group_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_firewall_rule_group_policy)
         """
 
+    def get_outpost_resolver(self, *, Id: str) -> GetOutpostResolverResponseTypeDef:
+        """
+        Gets information about a specified Resolver on the Outpost, such as its instance
+        count and type, name, and the current status of the Resolver.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_outpost_resolver)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_outpost_resolver)
+        """
+
     def get_resolver_config(self, *, ResourceId: str) -> GetResolverConfigResponseTypeDef:
         """
         Retrieves the behavior configuration of Route 53 Resolver behavior for a single
         VPC from Amazon Virtual Private Cloud.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_resolver_config)
@@ -676,14 +719,25 @@
         Retrieves the firewall rules that you have defined for the specified firewall
         rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_firewall_rules)
         """
 
+    def list_outpost_resolvers(
+        self, *, OutpostArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListOutpostResolversResponseTypeDef:
+        """
+        Lists all the Resolvers on Outposts that were created using the current Amazon
+        Web Services account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_outpost_resolvers)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_outpost_resolvers)
+        """
+
     def list_resolver_configs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListResolverConfigsResponseTypeDef:
         """
         Retrieves the Resolver configurations that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_configs)
@@ -895,14 +949,30 @@
         """
         Changes the association of a  FirewallRuleGroup with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_firewall_rule_group_association)
         """
 
+    def update_outpost_resolver(
+        self,
+        *,
+        Id: str,
+        Name: str = ...,
+        InstanceCount: int = ...,
+        PreferredInstanceType: str = ...
+    ) -> UpdateOutpostResolverResponseTypeDef:
+        """
+        You can use `UpdateOutpostResolver` to update the instance count, type, or name
+        of a Resolver on an Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_outpost_resolver)
+        """
+
     def update_resolver_config(
         self, *, ResourceId: str, AutodefinedReverseFlag: AutodefinedReverseFlagType
     ) -> UpdateResolverConfigResponseTypeDef:
         """
         Updates the behavior configuration of Route 53 Resolver behavior for a single
         VPC from Amazon Virtual Private Cloud.
 
@@ -998,14 +1068,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_outpost_resolvers"]
+    ) -> ListOutpostResolversPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_resolver_configs"]
     ) -> ListResolverConfigsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/client.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -53,33 +54,36 @@
     AssociateFirewallRuleGroupResponseTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     AssociateResolverQueryLogConfigResponseTypeDef,
     AssociateResolverRuleResponseTypeDef,
     CreateFirewallDomainListResponseTypeDef,
     CreateFirewallRuleGroupResponseTypeDef,
     CreateFirewallRuleResponseTypeDef,
+    CreateOutpostResolverResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     CreateResolverQueryLogConfigResponseTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteFirewallDomainListResponseTypeDef,
     DeleteFirewallRuleGroupResponseTypeDef,
     DeleteFirewallRuleResponseTypeDef,
+    DeleteOutpostResolverResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
     DisassociateResolverQueryLogConfigResponseTypeDef,
     DisassociateResolverRuleResponseTypeDef,
     FilterTypeDef,
     GetFirewallConfigResponseTypeDef,
     GetFirewallDomainListResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
     GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupResponseTypeDef,
+    GetOutpostResolverResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     GetResolverEndpointResponseTypeDef,
     GetResolverQueryLogConfigAssociationResponseTypeDef,
     GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     GetResolverRuleAssociationResponseTypeDef,
@@ -90,14 +94,15 @@
     IpAddressUpdateTypeDef,
     ListFirewallConfigsResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
     ListResolverEndpointsResponseTypeDef,
     ListResolverQueryLogConfigAssociationsResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     ListResolverRuleAssociationsResponseTypeDef,
@@ -110,14 +115,15 @@
     TagTypeDef,
     TargetAddressTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     UpdateFirewallRuleResponseTypeDef,
     UpdateIpAddressTypeDef,
+    UpdateOutpostResolverResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     UpdateResolverEndpointResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -145,14 +151,15 @@
     InvalidRequestException: Type[BotocoreClientError]
     InvalidTagException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
+    ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnknownResourceException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 class Route53ResolverClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client)
@@ -264,24 +271,42 @@
         """
         Creates an empty DNS Firewall rule group for filtering DNS network traffic in a
         VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_firewall_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_firewall_rule_group)
         """
+    def create_outpost_resolver(
+        self,
+        *,
+        CreatorRequestId: str,
+        Name: str,
+        PreferredInstanceType: str,
+        OutpostArn: str,
+        InstanceCount: int = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> CreateOutpostResolverResponseTypeDef:
+        """
+        Creates an Route 53 Resolver on an Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_outpost_resolver)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_outpost_resolver)
+        """
     def create_resolver_endpoint(
         self,
         *,
         CreatorRequestId: str,
         SecurityGroupIds: Sequence[str],
         Direction: ResolverEndpointDirectionType,
         IpAddresses: Sequence[IpAddressRequestTypeDef],
         Name: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ResolverEndpointType: ResolverEndpointTypeType = ...
+        ResolverEndpointType: ResolverEndpointTypeType = ...,
+        OutpostArn: str = ...,
+        PreferredInstanceType: str = ...
     ) -> CreateResolverEndpointResponseTypeDef:
         """
         Creates a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.create_resolver_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#create_resolver_endpoint)
         """
@@ -342,14 +367,21 @@
     ) -> DeleteFirewallRuleGroupResponseTypeDef:
         """
         Deletes the specified firewall rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_firewall_rule_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#delete_firewall_rule_group)
         """
+    def delete_outpost_resolver(self, *, Id: str) -> DeleteOutpostResolverResponseTypeDef:
+        """
+        Deletes a Resolver on the Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_outpost_resolver)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#delete_outpost_resolver)
+        """
     def delete_resolver_endpoint(
         self, *, ResolverEndpointId: str
     ) -> DeleteResolverEndpointResponseTypeDef:
         """
         Deletes a Resolver endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.delete_resolver_endpoint)
@@ -463,14 +495,22 @@
         """
         Returns the Identity and Access Management (Amazon Web Services IAM) policy for
         sharing the specified rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_firewall_rule_group_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_firewall_rule_group_policy)
         """
+    def get_outpost_resolver(self, *, Id: str) -> GetOutpostResolverResponseTypeDef:
+        """
+        Gets information about a specified Resolver on the Outpost, such as its instance
+        count and type, name, and the current status of the Resolver.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_outpost_resolver)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_outpost_resolver)
+        """
     def get_resolver_config(self, *, ResourceId: str) -> GetResolverConfigResponseTypeDef:
         """
         Retrieves the behavior configuration of Route 53 Resolver behavior for a single
         VPC from Amazon Virtual Private Cloud.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_resolver_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_resolver_config)
@@ -627,14 +667,24 @@
         """
         Retrieves the firewall rules that you have defined for the specified firewall
         rule group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_firewall_rules)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_firewall_rules)
         """
+    def list_outpost_resolvers(
+        self, *, OutpostArn: str = ..., MaxResults: int = ..., NextToken: str = ...
+    ) -> ListOutpostResolversResponseTypeDef:
+        """
+        Lists all the Resolvers on Outposts that were created using the current Amazon
+        Web Services account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_outpost_resolvers)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#list_outpost_resolvers)
+        """
     def list_resolver_configs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListResolverConfigsResponseTypeDef:
         """
         Retrieves the Resolver configurations that you have defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.list_resolver_configs)
@@ -828,14 +878,29 @@
     ) -> UpdateFirewallRuleGroupAssociationResponseTypeDef:
         """
         Changes the association of a  FirewallRuleGroup with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_firewall_rule_group_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_firewall_rule_group_association)
         """
+    def update_outpost_resolver(
+        self,
+        *,
+        Id: str,
+        Name: str = ...,
+        InstanceCount: int = ...,
+        PreferredInstanceType: str = ...
+    ) -> UpdateOutpostResolverResponseTypeDef:
+        """
+        You can use `UpdateOutpostResolver` to update the instance count, type, or name
+        of a Resolver on an Outpost.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.update_outpost_resolver)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#update_outpost_resolver)
+        """
     def update_resolver_config(
         self, *, ResourceId: str, AutodefinedReverseFlag: AutodefinedReverseFlagType
     ) -> UpdateResolverConfigResponseTypeDef:
         """
         Updates the behavior configuration of Route 53 Resolver behavior for a single
         VPC from Amazon Virtual Private Cloud.
 
@@ -921,14 +986,22 @@
     ) -> ListFirewallRulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_paginator)
         """
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_outpost_resolvers"]
+    ) -> ListOutpostResolversPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_paginator)
+        """
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_resolver_configs"]
     ) -> ListResolverConfigsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/client/#get_paginator)
         """
     @overload
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/literals.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionType",
     "AutodefinedReverseFlagType",
     "BlockOverrideDnsTypeType",
     "BlockResponseType",
     "FirewallDomainImportOperationType",
     "FirewallDomainListStatusType",
@@ -33,24 +32,26 @@
     "IpAddressStatusType",
     "ListFirewallConfigsPaginatorName",
     "ListFirewallDomainListsPaginatorName",
     "ListFirewallDomainsPaginatorName",
     "ListFirewallRuleGroupAssociationsPaginatorName",
     "ListFirewallRuleGroupsPaginatorName",
     "ListFirewallRulesPaginatorName",
+    "ListOutpostResolversPaginatorName",
     "ListResolverConfigsPaginatorName",
     "ListResolverDnssecConfigsPaginatorName",
     "ListResolverEndpointIpAddressesPaginatorName",
     "ListResolverEndpointsPaginatorName",
     "ListResolverQueryLogConfigAssociationsPaginatorName",
     "ListResolverQueryLogConfigsPaginatorName",
     "ListResolverRuleAssociationsPaginatorName",
     "ListResolverRulesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "MutationProtectionStatusType",
+    "OutpostResolverStatusType",
     "ResolverAutodefinedReverseStatusType",
     "ResolverDNSSECValidationStatusType",
     "ResolverEndpointDirectionType",
     "ResolverEndpointStatusType",
     "ResolverEndpointTypeType",
     "ResolverQueryLogConfigAssociationErrorType",
     "ResolverQueryLogConfigAssociationStatusType",
@@ -64,15 +65,14 @@
     "Route53ResolverServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionType = Literal["ALERT", "ALLOW", "BLOCK"]
 AutodefinedReverseFlagType = Literal["DISABLE", "ENABLE", "USE_LOCAL_RESOURCE_SETTING"]
 BlockOverrideDnsTypeType = Literal["CNAME"]
 BlockResponseType = Literal["NODATA", "NXDOMAIN", "OVERRIDE"]
 FirewallDomainImportOperationType = Literal["REPLACE"]
 FirewallDomainListStatusType = Literal[
     "COMPLETE", "COMPLETE_IMPORT_FAILED", "DELETING", "IMPORTING", "UPDATING"
@@ -88,34 +88,45 @@
     "DELETE_FAILED_FAS_EXPIRED",
     "DELETING",
     "DETACHING",
     "FAILED_CREATION",
     "FAILED_RESOURCE_GONE",
     "REMAP_ATTACHING",
     "REMAP_DETACHING",
+    "UPDATE_FAILED",
     "UPDATING",
 ]
 ListFirewallConfigsPaginatorName = Literal["list_firewall_configs"]
 ListFirewallDomainListsPaginatorName = Literal["list_firewall_domain_lists"]
 ListFirewallDomainsPaginatorName = Literal["list_firewall_domains"]
 ListFirewallRuleGroupAssociationsPaginatorName = Literal["list_firewall_rule_group_associations"]
 ListFirewallRuleGroupsPaginatorName = Literal["list_firewall_rule_groups"]
 ListFirewallRulesPaginatorName = Literal["list_firewall_rules"]
+ListOutpostResolversPaginatorName = Literal["list_outpost_resolvers"]
 ListResolverConfigsPaginatorName = Literal["list_resolver_configs"]
 ListResolverDnssecConfigsPaginatorName = Literal["list_resolver_dnssec_configs"]
 ListResolverEndpointIpAddressesPaginatorName = Literal["list_resolver_endpoint_ip_addresses"]
 ListResolverEndpointsPaginatorName = Literal["list_resolver_endpoints"]
 ListResolverQueryLogConfigAssociationsPaginatorName = Literal[
     "list_resolver_query_log_config_associations"
 ]
 ListResolverQueryLogConfigsPaginatorName = Literal["list_resolver_query_log_configs"]
 ListResolverRuleAssociationsPaginatorName = Literal["list_resolver_rule_associations"]
 ListResolverRulesPaginatorName = Literal["list_resolver_rules"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MutationProtectionStatusType = Literal["DISABLED", "ENABLED"]
+OutpostResolverStatusType = Literal[
+    "ACTION_NEEDED",
+    "CREATING",
+    "DELETING",
+    "FAILED_CREATION",
+    "FAILED_DELETION",
+    "OPERATIONAL",
+    "UPDATING",
+]
 ResolverAutodefinedReverseStatusType = Literal[
     "DISABLED",
     "DISABLING",
     "ENABLED",
     "ENABLING",
     "UPDATING_TO_USE_LOCAL_RESOURCE_SETTING",
     "USE_LOCAL_RESOURCE_SETTING",
@@ -362,14 +373,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -516,14 +528,15 @@
 PaginatorName = Literal[
     "list_firewall_configs",
     "list_firewall_domain_lists",
     "list_firewall_domains",
     "list_firewall_rule_group_associations",
     "list_firewall_rule_groups",
     "list_firewall_rules",
+    "list_outpost_resolvers",
     "list_resolver_configs",
     "list_resolver_dnssec_configs",
     "list_resolver_endpoint_ip_addresses",
     "list_resolver_endpoints",
     "list_resolver_query_log_config_associations",
     "list_resolver_query_log_configs",
     "list_resolver_rule_associations",
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/literals.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActionType",
     "AutodefinedReverseFlagType",
     "BlockOverrideDnsTypeType",
     "BlockResponseType",
     "FirewallDomainImportOperationType",
     "FirewallDomainListStatusType",
@@ -32,24 +33,26 @@
     "IpAddressStatusType",
     "ListFirewallConfigsPaginatorName",
     "ListFirewallDomainListsPaginatorName",
     "ListFirewallDomainsPaginatorName",
     "ListFirewallRuleGroupAssociationsPaginatorName",
     "ListFirewallRuleGroupsPaginatorName",
     "ListFirewallRulesPaginatorName",
+    "ListOutpostResolversPaginatorName",
     "ListResolverConfigsPaginatorName",
     "ListResolverDnssecConfigsPaginatorName",
     "ListResolverEndpointIpAddressesPaginatorName",
     "ListResolverEndpointsPaginatorName",
     "ListResolverQueryLogConfigAssociationsPaginatorName",
     "ListResolverQueryLogConfigsPaginatorName",
     "ListResolverRuleAssociationsPaginatorName",
     "ListResolverRulesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "MutationProtectionStatusType",
+    "OutpostResolverStatusType",
     "ResolverAutodefinedReverseStatusType",
     "ResolverDNSSECValidationStatusType",
     "ResolverEndpointDirectionType",
     "ResolverEndpointStatusType",
     "ResolverEndpointTypeType",
     "ResolverQueryLogConfigAssociationErrorType",
     "ResolverQueryLogConfigAssociationStatusType",
@@ -63,14 +66,15 @@
     "Route53ResolverServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ActionType = Literal["ALERT", "ALLOW", "BLOCK"]
 AutodefinedReverseFlagType = Literal["DISABLE", "ENABLE", "USE_LOCAL_RESOURCE_SETTING"]
 BlockOverrideDnsTypeType = Literal["CNAME"]
 BlockResponseType = Literal["NODATA", "NXDOMAIN", "OVERRIDE"]
 FirewallDomainImportOperationType = Literal["REPLACE"]
 FirewallDomainListStatusType = Literal[
     "COMPLETE", "COMPLETE_IMPORT_FAILED", "DELETING", "IMPORTING", "UPDATING"
@@ -86,34 +90,45 @@
     "DELETE_FAILED_FAS_EXPIRED",
     "DELETING",
     "DETACHING",
     "FAILED_CREATION",
     "FAILED_RESOURCE_GONE",
     "REMAP_ATTACHING",
     "REMAP_DETACHING",
+    "UPDATE_FAILED",
     "UPDATING",
 ]
 ListFirewallConfigsPaginatorName = Literal["list_firewall_configs"]
 ListFirewallDomainListsPaginatorName = Literal["list_firewall_domain_lists"]
 ListFirewallDomainsPaginatorName = Literal["list_firewall_domains"]
 ListFirewallRuleGroupAssociationsPaginatorName = Literal["list_firewall_rule_group_associations"]
 ListFirewallRuleGroupsPaginatorName = Literal["list_firewall_rule_groups"]
 ListFirewallRulesPaginatorName = Literal["list_firewall_rules"]
+ListOutpostResolversPaginatorName = Literal["list_outpost_resolvers"]
 ListResolverConfigsPaginatorName = Literal["list_resolver_configs"]
 ListResolverDnssecConfigsPaginatorName = Literal["list_resolver_dnssec_configs"]
 ListResolverEndpointIpAddressesPaginatorName = Literal["list_resolver_endpoint_ip_addresses"]
 ListResolverEndpointsPaginatorName = Literal["list_resolver_endpoints"]
 ListResolverQueryLogConfigAssociationsPaginatorName = Literal[
     "list_resolver_query_log_config_associations"
 ]
 ListResolverQueryLogConfigsPaginatorName = Literal["list_resolver_query_log_configs"]
 ListResolverRuleAssociationsPaginatorName = Literal["list_resolver_rule_associations"]
 ListResolverRulesPaginatorName = Literal["list_resolver_rules"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MutationProtectionStatusType = Literal["DISABLED", "ENABLED"]
+OutpostResolverStatusType = Literal[
+    "ACTION_NEEDED",
+    "CREATING",
+    "DELETING",
+    "FAILED_CREATION",
+    "FAILED_DELETION",
+    "OPERATIONAL",
+    "UPDATING",
+]
 ResolverAutodefinedReverseStatusType = Literal[
     "DISABLED",
     "DISABLING",
     "ENABLED",
     "ENABLING",
     "UPDATING_TO_USE_LOCAL_RESOURCE_SETTING",
     "USE_LOCAL_RESOURCE_SETTING",
@@ -360,14 +375,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -514,14 +530,15 @@
 PaginatorName = Literal[
     "list_firewall_configs",
     "list_firewall_domain_lists",
     "list_firewall_domains",
     "list_firewall_rule_group_associations",
     "list_firewall_rule_groups",
     "list_firewall_rules",
+    "list_outpost_resolvers",
     "list_resolver_configs",
     "list_resolver_dnssec_configs",
     "list_resolver_endpoint_ip_addresses",
     "list_resolver_endpoints",
     "list_resolver_query_log_config_associations",
     "list_resolver_query_log_configs",
     "list_resolver_rule_associations",
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/paginator.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from mypy_boto3_route53resolver.paginator import (
         ListFirewallConfigsPaginator,
         ListFirewallDomainListsPaginator,
         ListFirewallDomainsPaginator,
         ListFirewallRuleGroupAssociationsPaginator,
         ListFirewallRuleGroupsPaginator,
         ListFirewallRulesPaginator,
+        ListOutpostResolversPaginator,
         ListResolverConfigsPaginator,
         ListResolverDnssecConfigsPaginator,
         ListResolverEndpointIpAddressesPaginator,
         ListResolverEndpointsPaginator,
         ListResolverQueryLogConfigAssociationsPaginator,
         ListResolverQueryLogConfigsPaginator,
         ListResolverRuleAssociationsPaginator,
@@ -32,14 +33,15 @@
 
     list_firewall_configs_paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
     list_firewall_domain_lists_paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
     list_firewall_domains_paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
     list_firewall_rule_group_associations_paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
     list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
     list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
+    list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")
     list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
     list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
     list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
     list_resolver_endpoints_paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
     list_resolver_query_log_config_associations_paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
     list_resolver_query_log_configs_paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
     list_resolver_rule_associations_paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
@@ -56,14 +58,15 @@
     FilterTypeDef,
     ListFirewallConfigsResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
     ListResolverEndpointsResponseTypeDef,
     ListResolverQueryLogConfigAssociationsResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     ListResolverRuleAssociationsResponseTypeDef,
@@ -75,14 +78,15 @@
 __all__ = (
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
     "ListFirewallRulesPaginator",
+    "ListOutpostResolversPaginator",
     "ListResolverConfigsPaginator",
     "ListResolverDnssecConfigsPaginator",
     "ListResolverEndpointIpAddressesPaginator",
     "ListResolverEndpointsPaginator",
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
@@ -104,45 +108,45 @@
 class ListFirewallConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallconfigspaginator)
         """
 
 
 class ListFirewallDomainListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainlistspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallDomainListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainlistspaginator)
         """
 
 
 class ListFirewallDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainspaginator)
     """
 
     def paginate(
-        self, *, FirewallDomainListId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FirewallDomainListId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainspaginator)
         """
 
 
@@ -155,30 +159,30 @@
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupassociationspaginator)
         """
 
 
 class ListFirewallRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupspaginator)
         """
 
 
@@ -190,30 +194,45 @@
 
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
 
+class ListOutpostResolversPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListOutpostResolvers)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listoutpostresolverspaginator)
+    """
+
+    def paginate(
+        self, *, OutpostArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListOutpostResolversResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListOutpostResolvers.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listoutpostresolverspaginator)
+        """
+
+
 class ListResolverConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverconfigspaginator)
         """
 
 
@@ -223,30 +242,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverDnssecConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
         """
 
 
 class ListResolverEndpointIpAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointipaddressespaginator)
     """
 
     def paginate(
-        self, *, ResolverEndpointId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResolverEndpointId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverEndpointIpAddressesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointipaddressespaginator)
         """
 
 
@@ -256,15 +275,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
         """
 
 
@@ -276,15 +295,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigassociationspaginator)
         """
 
 
@@ -296,15 +315,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverQueryLogConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigspaginator)
         """
 
 
@@ -314,15 +333,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverRuleAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
         """
 
 
@@ -332,28 +351,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/paginator.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from mypy_boto3_route53resolver.paginator import (
         ListFirewallConfigsPaginator,
         ListFirewallDomainListsPaginator,
         ListFirewallDomainsPaginator,
         ListFirewallRuleGroupAssociationsPaginator,
         ListFirewallRuleGroupsPaginator,
         ListFirewallRulesPaginator,
+        ListOutpostResolversPaginator,
         ListResolverConfigsPaginator,
         ListResolverDnssecConfigsPaginator,
         ListResolverEndpointIpAddressesPaginator,
         ListResolverEndpointsPaginator,
         ListResolverQueryLogConfigAssociationsPaginator,
         ListResolverQueryLogConfigsPaginator,
         ListResolverRuleAssociationsPaginator,
@@ -32,14 +33,15 @@
 
     list_firewall_configs_paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
     list_firewall_domain_lists_paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
     list_firewall_domains_paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
     list_firewall_rule_group_associations_paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
     list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
     list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
+    list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")
     list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
     list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
     list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
     list_resolver_endpoints_paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
     list_resolver_query_log_config_associations_paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
     list_resolver_query_log_configs_paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
     list_resolver_rule_associations_paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
@@ -56,14 +58,15 @@
     FilterTypeDef,
     ListFirewallConfigsResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
     ListResolverEndpointsResponseTypeDef,
     ListResolverQueryLogConfigAssociationsResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     ListResolverRuleAssociationsResponseTypeDef,
@@ -75,14 +78,15 @@
 __all__ = (
     "ListFirewallConfigsPaginator",
     "ListFirewallDomainListsPaginator",
     "ListFirewallDomainsPaginator",
     "ListFirewallRuleGroupAssociationsPaginator",
     "ListFirewallRuleGroupsPaginator",
     "ListFirewallRulesPaginator",
+    "ListOutpostResolversPaginator",
     "ListResolverConfigsPaginator",
     "ListResolverDnssecConfigsPaginator",
     "ListResolverEndpointIpAddressesPaginator",
     "ListResolverEndpointsPaginator",
     "ListResolverQueryLogConfigAssociationsPaginator",
     "ListResolverQueryLogConfigsPaginator",
     "ListResolverRuleAssociationsPaginator",
@@ -101,43 +105,43 @@
 class ListFirewallConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallconfigspaginator)
         """
 
 class ListFirewallDomainListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainlistspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallDomainListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainlistspaginator)
         """
 
 class ListFirewallDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainspaginator)
     """
 
     def paginate(
-        self, *, FirewallDomainListId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FirewallDomainListId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainspaginator)
         """
 
 class ListFirewallRuleGroupAssociationsPaginator(Paginator):
@@ -149,29 +153,29 @@
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupassociationspaginator)
         """
 
 class ListFirewallRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupspaginator)
         """
 
 class ListFirewallRulesPaginator(Paginator):
@@ -182,29 +186,43 @@
 
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
+class ListOutpostResolversPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListOutpostResolvers)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listoutpostresolverspaginator)
+    """
+
+    def paginate(
+        self, *, OutpostArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListOutpostResolversResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListOutpostResolvers.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listoutpostresolverspaginator)
+        """
+
 class ListResolverConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverconfigspaginator)
         """
 
 class ListResolverDnssecConfigsPaginator(Paginator):
@@ -213,29 +231,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverDnssecConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
         """
 
 class ListResolverEndpointIpAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointipaddressespaginator)
     """
 
     def paginate(
-        self, *, ResolverEndpointId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResolverEndpointId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverEndpointIpAddressesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointipaddressespaginator)
         """
 
 class ListResolverEndpointsPaginator(Paginator):
@@ -244,15 +262,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
         """
 
 class ListResolverQueryLogConfigAssociationsPaginator(Paginator):
@@ -263,15 +281,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigassociationspaginator)
         """
 
 class ListResolverQueryLogConfigsPaginator(Paginator):
@@ -282,15 +300,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverQueryLogConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigspaginator)
         """
 
 class ListResolverRuleAssociationsPaginator(Paginator):
@@ -299,15 +317,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverRuleAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
         """
 
 class ListResolverRulesPaginator(Paginator):
@@ -316,27 +334,27 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/type_defs.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     FirewallDomainListStatusType,
     FirewallDomainUpdateOperationType,
     FirewallFailOpenStatusType,
     FirewallRuleGroupAssociationStatusType,
     FirewallRuleGroupStatusType,
     IpAddressStatusType,
     MutationProtectionStatusType,
+    OutpostResolverStatusType,
     ResolverAutodefinedReverseStatusType,
     ResolverDNSSECValidationStatusType,
     ResolverEndpointDirectionType,
     ResolverEndpointStatusType,
     ResolverEndpointTypeType,
     ResolverQueryLogConfigAssociationErrorType,
     ResolverQueryLogConfigAssociationStatusType,
@@ -50,108 +51,106 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
     "FirewallRuleGroupAssociationTypeDef",
+    "ResponseMetadataTypeDef",
     "IpAddressUpdateTypeDef",
     "ResolverEndpointTypeDef",
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     "ResolverQueryLogConfigAssociationTypeDef",
     "AssociateResolverRuleRequestRequestTypeDef",
     "ResolverRuleAssociationTypeDef",
     "FirewallDomainListTypeDef",
     "FirewallRuleGroupTypeDef",
     "CreateFirewallRuleRequestRequestTypeDef",
     "FirewallRuleTypeDef",
+    "OutpostResolverTypeDef",
     "IpAddressRequestTypeDef",
     "ResolverQueryLogConfigTypeDef",
     "TargetAddressTypeDef",
     "DeleteFirewallDomainListRequestRequestTypeDef",
     "DeleteFirewallRuleGroupRequestRequestTypeDef",
     "DeleteFirewallRuleRequestRequestTypeDef",
+    "DeleteOutpostResolverRequestRequestTypeDef",
     "DeleteResolverEndpointRequestRequestTypeDef",
     "DeleteResolverQueryLogConfigRequestRequestTypeDef",
     "DeleteResolverRuleRequestRequestTypeDef",
     "DisassociateFirewallRuleGroupRequestRequestTypeDef",
     "DisassociateResolverQueryLogConfigRequestRequestTypeDef",
     "DisassociateResolverRuleRequestRequestTypeDef",
     "FilterTypeDef",
     "FirewallConfigTypeDef",
     "FirewallDomainListMetadataTypeDef",
     "FirewallRuleGroupMetadataTypeDef",
     "GetFirewallConfigRequestRequestTypeDef",
     "GetFirewallDomainListRequestRequestTypeDef",
     "GetFirewallRuleGroupAssociationRequestRequestTypeDef",
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
-    "GetFirewallRuleGroupPolicyResponseTypeDef",
     "GetFirewallRuleGroupRequestRequestTypeDef",
+    "GetOutpostResolverRequestRequestTypeDef",
     "GetResolverConfigRequestRequestTypeDef",
     "ResolverConfigTypeDef",
     "GetResolverDnssecConfigRequestRequestTypeDef",
     "ResolverDnssecConfigTypeDef",
     "GetResolverEndpointRequestRequestTypeDef",
     "GetResolverQueryLogConfigAssociationRequestRequestTypeDef",
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
-    "GetResolverQueryLogConfigPolicyResponseTypeDef",
     "GetResolverQueryLogConfigRequestRequestTypeDef",
     "GetResolverRuleAssociationRequestRequestTypeDef",
     "GetResolverRulePolicyRequestRequestTypeDef",
-    "GetResolverRulePolicyResponseTypeDef",
     "GetResolverRuleRequestRequestTypeDef",
     "ImportFirewallDomainsRequestRequestTypeDef",
-    "ImportFirewallDomainsResponseTypeDef",
     "IpAddressResponseTypeDef",
-    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListFirewallConfigsRequestRequestTypeDef",
-    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
     "ListFirewallDomainListsRequestRequestTypeDef",
-    "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
     "ListFirewallDomainsRequestRequestTypeDef",
-    "ListFirewallDomainsResponseTypeDef",
-    "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
-    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
     "ListFirewallRuleGroupsRequestRequestTypeDef",
-    "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
     "ListFirewallRulesRequestRequestTypeDef",
-    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    "ListOutpostResolversRequestRequestTypeDef",
     "ListResolverConfigsRequestRequestTypeDef",
-    "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
     "ListResolverEndpointIpAddressesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
-    "PutFirewallRuleGroupPolicyResponseTypeDef",
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
-    "PutResolverQueryLogConfigPolicyResponseTypeDef",
     "PutResolverRulePolicyRequestRequestTypeDef",
-    "PutResolverRulePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "TargetAddressOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallConfigRequestRequestTypeDef",
     "UpdateFirewallDomainsRequestRequestTypeDef",
-    "UpdateFirewallDomainsResponseTypeDef",
     "UpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     "UpdateFirewallRuleRequestRequestTypeDef",
     "UpdateIpAddressTypeDef",
+    "UpdateOutpostResolverRequestRequestTypeDef",
     "UpdateResolverConfigRequestRequestTypeDef",
     "UpdateResolverDnssecConfigRequestRequestTypeDef",
     "AssociateFirewallRuleGroupRequestRequestTypeDef",
     "CreateFirewallDomainListRequestRequestTypeDef",
     "CreateFirewallRuleGroupRequestRequestTypeDef",
+    "CreateOutpostResolverRequestRequestTypeDef",
     "CreateResolverQueryLogConfigRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateFirewallRuleGroupResponseTypeDef",
     "DisassociateFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupAssociationResponseTypeDef",
+    "GetFirewallRuleGroupPolicyResponseTypeDef",
+    "GetResolverQueryLogConfigPolicyResponseTypeDef",
+    "GetResolverRulePolicyResponseTypeDef",
+    "ImportFirewallDomainsResponseTypeDef",
+    "ListFirewallDomainsResponseTypeDef",
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
+    "PutFirewallRuleGroupPolicyResponseTypeDef",
+    "PutResolverQueryLogConfigPolicyResponseTypeDef",
+    "PutResolverRulePolicyResponseTypeDef",
+    "UpdateFirewallDomainsResponseTypeDef",
     "UpdateFirewallRuleGroupAssociationResponseTypeDef",
     "AssociateResolverEndpointIpAddressRequestRequestTypeDef",
     "DisassociateResolverEndpointIpAddressRequestRequestTypeDef",
     "AssociateResolverEndpointIpAddressResponseTypeDef",
     "CreateResolverEndpointResponseTypeDef",
     "DeleteResolverEndpointResponseTypeDef",
     "DisassociateResolverEndpointIpAddressResponseTypeDef",
@@ -172,46 +171,62 @@
     "CreateFirewallRuleGroupResponseTypeDef",
     "DeleteFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupResponseTypeDef",
     "CreateFirewallRuleResponseTypeDef",
     "DeleteFirewallRuleResponseTypeDef",
     "ListFirewallRulesResponseTypeDef",
     "UpdateFirewallRuleResponseTypeDef",
+    "CreateOutpostResolverResponseTypeDef",
+    "DeleteOutpostResolverResponseTypeDef",
+    "GetOutpostResolverResponseTypeDef",
+    "ListOutpostResolversResponseTypeDef",
+    "UpdateOutpostResolverResponseTypeDef",
     "CreateResolverEndpointRequestRequestTypeDef",
     "CreateResolverQueryLogConfigResponseTypeDef",
     "DeleteResolverQueryLogConfigResponseTypeDef",
     "GetResolverQueryLogConfigResponseTypeDef",
     "ListResolverQueryLogConfigsResponseTypeDef",
     "CreateResolverRuleRequestRequestTypeDef",
     "ResolverRuleConfigTypeDef",
-    "ResolverRuleTypeDef",
-    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
     "ListResolverDnssecConfigsRequestRequestTypeDef",
-    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
     "ListResolverEndpointsRequestRequestTypeDef",
-    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
     "ListResolverQueryLogConfigAssociationsRequestRequestTypeDef",
-    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
     "ListResolverQueryLogConfigsRequestRequestTypeDef",
-    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
     "ListResolverRuleAssociationsRequestRequestTypeDef",
-    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
     "ListResolverRulesRequestRequestTypeDef",
     "GetFirewallConfigResponseTypeDef",
     "ListFirewallConfigsResponseTypeDef",
     "UpdateFirewallConfigResponseTypeDef",
     "ListFirewallDomainListsResponseTypeDef",
     "ListFirewallRuleGroupsResponseTypeDef",
     "GetResolverConfigResponseTypeDef",
     "ListResolverConfigsResponseTypeDef",
     "UpdateResolverConfigResponseTypeDef",
     "GetResolverDnssecConfigResponseTypeDef",
     "ListResolverDnssecConfigsResponseTypeDef",
     "UpdateResolverDnssecConfigResponseTypeDef",
     "ListResolverEndpointIpAddressesResponseTypeDef",
+    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
+    "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
+    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
+    "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    "ListOutpostResolversRequestListOutpostResolversPaginateTypeDef",
+    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
+    "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
+    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
+    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
+    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
+    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResolverRuleTypeDef",
     "UpdateResolverEndpointRequestRequestTypeDef",
     "UpdateResolverRuleRequestRequestTypeDef",
     "CreateResolverRuleResponseTypeDef",
     "DeleteResolverRuleResponseTypeDef",
     "GetResolverRuleResponseTypeDef",
     "ListResolverRulesResponseTypeDef",
     "UpdateResolverRuleResponseTypeDef",
@@ -238,15 +253,25 @@
         "ManagedOwnerName": str,
         "Status": FirewallRuleGroupAssociationStatusType,
         "StatusMessage": str,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 IpAddressUpdateTypeDef = TypedDict(
     "IpAddressUpdateTypeDef",
     {
         "IpId": str,
         "SubnetId": str,
@@ -268,16 +293,17 @@
         "IpAddressCount": int,
         "HostVPCId": str,
         "Status": ResolverEndpointStatusType,
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
         "ResolverEndpointType": ResolverEndpointTypeType,
+        "OutpostArn": str,
+        "PreferredInstanceType": str,
     },
-    total=False,
 )
 
 AssociateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "ResolverQueryLogConfigId": str,
         "ResourceId": str,
@@ -291,15 +317,14 @@
         "ResolverQueryLogConfigId": str,
         "ResourceId": str,
         "Status": ResolverQueryLogConfigAssociationStatusType,
         "Error": ResolverQueryLogConfigAssociationErrorType,
         "ErrorMessage": str,
         "CreationTime": str,
     },
-    total=False,
 )
 
 _RequiredAssociateResolverRuleRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
         "VPCId": str,
@@ -327,15 +352,14 @@
         "Id": str,
         "ResolverRuleId": str,
         "Name": str,
         "VPCId": str,
         "Status": ResolverRuleAssociationStatusType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 FirewallDomainListTypeDef = TypedDict(
     "FirewallDomainListTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -344,15 +368,14 @@
         "Status": FirewallDomainListStatusType,
         "StatusMessage": str,
         "ManagedOwnerName": str,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 FirewallRuleGroupTypeDef = TypedDict(
     "FirewallRuleGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -362,15 +385,14 @@
         "StatusMessage": str,
         "OwnerId": str,
         "CreatorRequestId": str,
         "ShareStatus": ShareStatusType,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 _RequiredCreateFirewallRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "FirewallRuleGroupId": str,
@@ -411,15 +433,31 @@
         "BlockOverrideDomain": str,
         "BlockOverrideDnsType": Literal["CNAME"],
         "BlockOverrideTtl": int,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
+)
+
+OutpostResolverTypeDef = TypedDict(
+    "OutpostResolverTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": str,
+        "ModificationTime": str,
+        "CreatorRequestId": str,
+        "Id": str,
+        "InstanceCount": int,
+        "PreferredInstanceType": str,
+        "Name": str,
+        "Status": OutpostResolverStatusType,
+        "StatusMessage": str,
+        "OutpostArn": str,
+    },
 )
 
 _RequiredIpAddressRequestTypeDef = TypedDict(
     "_RequiredIpAddressRequestTypeDef",
     {
         "SubnetId": str,
     },
@@ -448,15 +486,14 @@
         "AssociationCount": int,
         "Arn": str,
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
         "CreationTime": str,
     },
-    total=False,
 )
 
 TargetAddressTypeDef = TypedDict(
     "TargetAddressTypeDef",
     {
         "Ip": str,
         "Port": int,
@@ -483,14 +520,21 @@
     "DeleteFirewallRuleRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
     },
 )
 
+DeleteOutpostResolverRequestRequestTypeDef = TypedDict(
+    "DeleteOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+
 DeleteResolverEndpointRequestRequestTypeDef = TypedDict(
     "DeleteResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 
@@ -544,40 +588,37 @@
     "FirewallConfigTypeDef",
     {
         "Id": str,
         "ResourceId": str,
         "OwnerId": str,
         "FirewallFailOpen": FirewallFailOpenStatusType,
     },
-    total=False,
 )
 
 FirewallDomainListMetadataTypeDef = TypedDict(
     "FirewallDomainListMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "CreatorRequestId": str,
         "ManagedOwnerName": str,
     },
-    total=False,
 )
 
 FirewallRuleGroupMetadataTypeDef = TypedDict(
     "FirewallRuleGroupMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "OwnerId": str,
         "CreatorRequestId": str,
         "ShareStatus": ShareStatusType,
     },
-    total=False,
 )
 
 GetFirewallConfigRequestRequestTypeDef = TypedDict(
     "GetFirewallConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -600,26 +641,25 @@
 GetFirewallRuleGroupPolicyRequestRequestTypeDef = TypedDict(
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
-    "GetFirewallRuleGroupPolicyResponseTypeDef",
+GetFirewallRuleGroupRequestRequestTypeDef = TypedDict(
+    "GetFirewallRuleGroupRequestRequestTypeDef",
     {
-        "FirewallRuleGroupPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FirewallRuleGroupId": str,
     },
 )
 
-GetFirewallRuleGroupRequestRequestTypeDef = TypedDict(
-    "GetFirewallRuleGroupRequestRequestTypeDef",
+GetOutpostResolverRequestRequestTypeDef = TypedDict(
+    "GetOutpostResolverRequestRequestTypeDef",
     {
-        "FirewallRuleGroupId": str,
+        "Id": str,
     },
 )
 
 GetResolverConfigRequestRequestTypeDef = TypedDict(
     "GetResolverConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
@@ -630,15 +670,14 @@
     "ResolverConfigTypeDef",
     {
         "Id": str,
         "ResourceId": str,
         "OwnerId": str,
         "AutodefinedReverse": ResolverAutodefinedReverseStatusType,
     },
-    total=False,
 )
 
 GetResolverDnssecConfigRequestRequestTypeDef = TypedDict(
     "GetResolverDnssecConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -648,15 +687,14 @@
     "ResolverDnssecConfigTypeDef",
     {
         "Id": str,
         "OwnerId": str,
         "ResourceId": str,
         "ValidationStatus": ResolverDNSSECValidationStatusType,
     },
-    total=False,
 )
 
 GetResolverEndpointRequestRequestTypeDef = TypedDict(
     "GetResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
@@ -672,22 +710,14 @@
 GetResolverQueryLogConfigPolicyRequestRequestTypeDef = TypedDict(
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
-    "GetResolverQueryLogConfigPolicyResponseTypeDef",
-    {
-        "ResolverQueryLogConfigPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "GetResolverQueryLogConfigRequestRequestTypeDef",
     {
         "ResolverQueryLogConfigId": str,
     },
 )
 
@@ -701,22 +731,14 @@
 GetResolverRulePolicyRequestRequestTypeDef = TypedDict(
     "GetResolverRulePolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetResolverRulePolicyResponseTypeDef = TypedDict(
-    "GetResolverRulePolicyResponseTypeDef",
-    {
-        "ResolverRulePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverRuleRequestRequestTypeDef = TypedDict(
     "GetResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
     },
 )
 
@@ -725,96 +747,56 @@
     {
         "FirewallDomainListId": str,
         "Operation": Literal["REPLACE"],
         "DomainFileUrl": str,
     },
 )
 
-ImportFirewallDomainsResponseTypeDef = TypedDict(
-    "ImportFirewallDomainsResponseTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Status": FirewallDomainListStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IpAddressResponseTypeDef = TypedDict(
     "IpAddressResponseTypeDef",
     {
         "IpId": str,
         "SubnetId": str,
         "Ip": str,
         "Ipv6": str,
         "Status": IpAddressStatusType,
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
-ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
-    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListFirewallConfigsRequestRequestTypeDef = TypedDict(
     "ListFirewallConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef = TypedDict(
-    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallDomainListsRequestRequestTypeDef = TypedDict(
     "ListFirewallDomainListsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
-    {
-        "FirewallDomainListId": str,
-    },
-)
-_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef(
-    _RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
-    _OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFirewallDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListFirewallDomainsRequestRequestTypeDef",
     {
         "FirewallDomainListId": str,
     },
 )
 _OptionalListFirewallDomainsRequestRequestTypeDef = TypedDict(
@@ -830,91 +812,36 @@
 class ListFirewallDomainsRequestRequestTypeDef(
     _RequiredListFirewallDomainsRequestRequestTypeDef,
     _OptionalListFirewallDomainsRequestRequestTypeDef,
 ):
     pass
 
 
-ListFirewallDomainsResponseTypeDef = TypedDict(
-    "ListFirewallDomainsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Domains": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
-        {
-            "FirewallRuleGroupId": str,
-            "VpcId": str,
-            "Priority": int,
-            "Status": FirewallRuleGroupAssociationStatusType,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListFirewallRuleGroupAssociationsRequestRequestTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "VpcId": str,
         "Priority": int,
         "Status": FirewallRuleGroupAssociationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef = TypedDict(
-    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListFirewallRuleGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
-    "_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
-    {
-        "FirewallRuleGroupId": str,
-    },
-)
-_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
-    "_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
-    {
-        "Priority": int,
-        "Action": ActionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
-    _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
-    _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFirewallRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListFirewallRulesRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
     },
 )
 _OptionalListFirewallRulesRequestRequestTypeDef = TypedDict(
@@ -931,53 +858,33 @@
 
 class ListFirewallRulesRequestRequestTypeDef(
     _RequiredListFirewallRulesRequestRequestTypeDef, _OptionalListFirewallRulesRequestRequestTypeDef
 ):
     pass
 
 
-ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
-    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+ListOutpostResolversRequestRequestTypeDef = TypedDict(
+    "ListOutpostResolversRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "OutpostArn": str,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 ListResolverConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
-    "_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
-    {
-        "ResolverEndpointId": str,
-    },
-)
-_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
-    "_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef(
-    _RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
-    _OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResolverEndpointIpAddressesRequestRequestTypeDef = TypedDict(
     "_RequiredListResolverEndpointIpAddressesRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 _OptionalListResolverEndpointIpAddressesRequestRequestTypeDef = TypedDict(
@@ -993,36 +900,14 @@
 class ListResolverEndpointIpAddressesRequestRequestTypeDef(
     _RequiredListResolverEndpointIpAddressesRequestRequestTypeDef,
     _OptionalListResolverEndpointIpAddressesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1038,80 +923,52 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 PutFirewallRuleGroupPolicyRequestRequestTypeDef = TypedDict(
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "FirewallRuleGroupPolicy": str,
     },
 )
 
-PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
-    "PutFirewallRuleGroupPolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResolverQueryLogConfigPolicyRequestRequestTypeDef = TypedDict(
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "ResolverQueryLogConfigPolicy": str,
     },
 )
 
-PutResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
-    "PutResolverQueryLogConfigPolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResolverRulePolicyRequestRequestTypeDef = TypedDict(
     "PutResolverRulePolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "ResolverRulePolicy": str,
     },
 )
 
-PutResolverRulePolicyResponseTypeDef = TypedDict(
-    "PutResolverRulePolicyResponseTypeDef",
+TargetAddressOutputTypeDef = TypedDict(
+    "TargetAddressOutputTypeDef",
     {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Ip": str,
+        "Port": int,
+        "Ipv6": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1132,25 +989,14 @@
     {
         "FirewallDomainListId": str,
         "Operation": FirewallDomainUpdateOperationType,
         "Domains": Sequence[str],
     },
 )
 
-UpdateFirewallDomainsResponseTypeDef = TypedDict(
-    "UpdateFirewallDomainsResponseTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Status": FirewallDomainListStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     {
         "FirewallRuleGroupAssociationId": str,
     },
 )
 _OptionalUpdateFirewallRuleGroupAssociationRequestRequestTypeDef = TypedDict(
@@ -1204,14 +1050,38 @@
     "UpdateIpAddressTypeDef",
     {
         "IpId": str,
         "Ipv6": str,
     },
 )
 
+_RequiredUpdateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalUpdateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOutpostResolverRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceCount": int,
+        "PreferredInstanceType": str,
+    },
+    total=False,
+)
+
+
+class UpdateOutpostResolverRequestRequestTypeDef(
+    _RequiredUpdateOutpostResolverRequestRequestTypeDef,
+    _OptionalUpdateOutpostResolverRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateResolverConfigRequestRequestTypeDef = TypedDict(
     "UpdateResolverConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
         "AutodefinedReverseFlag": AutodefinedReverseFlagType,
     },
 )
@@ -1293,14 +1163,40 @@
 class CreateFirewallRuleGroupRequestRequestTypeDef(
     _RequiredCreateFirewallRuleGroupRequestRequestTypeDef,
     _OptionalCreateFirewallRuleGroupRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOutpostResolverRequestRequestTypeDef",
+    {
+        "CreatorRequestId": str,
+        "Name": str,
+        "PreferredInstanceType": str,
+        "OutpostArn": str,
+    },
+)
+_OptionalCreateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOutpostResolverRequestRequestTypeDef",
+    {
+        "InstanceCount": int,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateOutpostResolverRequestRequestTypeDef(
+    _RequiredCreateOutpostResolverRequestRequestTypeDef,
+    _OptionalCreateOutpostResolverRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
     },
@@ -1317,69 +1213,139 @@
 class CreateResolverQueryLogConfigRequestRequestTypeDef(
     _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef,
     _OptionalCreateResolverQueryLogConfigRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 AssociateFirewallRuleGroupResponseTypeDef = TypedDict(
     "AssociateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFirewallRuleGroupResponseTypeDef = TypedDict(
     "DisassociateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallRuleGroupAssociationResponseTypeDef = TypedDict(
     "GetFirewallRuleGroupAssociationResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
+    "GetFirewallRuleGroupPolicyResponseTypeDef",
+    {
+        "FirewallRuleGroupPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
+    "GetResolverQueryLogConfigPolicyResponseTypeDef",
+    {
+        "ResolverQueryLogConfigPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResolverRulePolicyResponseTypeDef = TypedDict(
+    "GetResolverRulePolicyResponseTypeDef",
+    {
+        "ResolverRulePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportFirewallDomainsResponseTypeDef = TypedDict(
+    "ImportFirewallDomainsResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Status": FirewallDomainListStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallDomainsResponseTypeDef = TypedDict(
+    "ListFirewallDomainsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Domains": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRuleGroupAssociationsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRuleGroupAssociations": List[FirewallRuleGroupAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
+    "PutFirewallRuleGroupPolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
+    "PutResolverQueryLogConfigPolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResolverRulePolicyResponseTypeDef = TypedDict(
+    "PutResolverRulePolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDomainsResponseTypeDef = TypedDict(
+    "UpdateFirewallDomainsResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Status": FirewallDomainListStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallRuleGroupAssociationResponseTypeDef = TypedDict(
     "UpdateFirewallRuleGroupAssociationResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverEndpointIpAddressRequestRequestTypeDef = TypedDict(
     "AssociateResolverEndpointIpAddressRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
@@ -1395,215 +1361,256 @@
     },
 )
 
 AssociateResolverEndpointIpAddressResponseTypeDef = TypedDict(
     "AssociateResolverEndpointIpAddressResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResolverEndpointResponseTypeDef = TypedDict(
     "CreateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverEndpointResponseTypeDef = TypedDict(
     "DeleteResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverEndpointIpAddressResponseTypeDef = TypedDict(
     "DisassociateResolverEndpointIpAddressResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverEndpointResponseTypeDef = TypedDict(
     "GetResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverEndpointsResponseTypeDef = TypedDict(
     "ListResolverEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverEndpoints": List[ResolverEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverEndpointResponseTypeDef = TypedDict(
     "UpdateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "DisassociateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverQueryLogConfigAssociationResponseTypeDef = TypedDict(
     "GetResolverQueryLogConfigAssociationResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverQueryLogConfigAssociationsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigAssociations": List[ResolverQueryLogConfigAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverRuleResponseTypeDef = TypedDict(
     "AssociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverRuleResponseTypeDef = TypedDict(
     "DisassociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverRuleAssociationResponseTypeDef = TypedDict(
     "GetResolverRuleAssociationResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverRuleAssociationsResponseTypeDef = TypedDict(
     "ListResolverRuleAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverRuleAssociations": List[ResolverRuleAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallDomainListResponseTypeDef = TypedDict(
     "CreateFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallDomainListResponseTypeDef = TypedDict(
     "DeleteFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallDomainListResponseTypeDef = TypedDict(
     "GetFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallRuleGroupResponseTypeDef = TypedDict(
     "CreateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallRuleGroupResponseTypeDef = TypedDict(
     "DeleteFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallRuleGroupResponseTypeDef = TypedDict(
     "GetFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallRuleResponseTypeDef = TypedDict(
     "CreateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallRuleResponseTypeDef = TypedDict(
     "DeleteFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRulesResponseTypeDef = TypedDict(
     "ListFirewallRulesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRules": List[FirewallRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallRuleResponseTypeDef = TypedDict(
     "UpdateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOutpostResolverResponseTypeDef = TypedDict(
+    "CreateOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOutpostResolverResponseTypeDef = TypedDict(
+    "DeleteOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOutpostResolverResponseTypeDef = TypedDict(
+    "GetOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOutpostResolversResponseTypeDef = TypedDict(
+    "ListOutpostResolversResponseTypeDef",
+    {
+        "OutpostResolvers": List[OutpostResolverTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateOutpostResolverResponseTypeDef = TypedDict(
+    "UpdateOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverEndpointRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
@@ -1614,14 +1621,16 @@
 )
 _OptionalCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResolverEndpointRequestRequestTypeDef",
     {
         "Name": str,
         "Tags": Sequence[TagTypeDef],
         "ResolverEndpointType": ResolverEndpointTypeType,
+        "OutpostArn": str,
+        "PreferredInstanceType": str,
     },
     total=False,
 )
 
 
 class CreateResolverEndpointRequestRequestTypeDef(
     _RequiredCreateResolverEndpointRequestRequestTypeDef,
@@ -1630,42 +1639,42 @@
     pass
 
 
 CreateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "CreateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverQueryLogConfigResponseTypeDef = TypedDict(
     "DeleteResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverQueryLogConfigResponseTypeDef = TypedDict(
     "GetResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverQueryLogConfigsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigsResponseTypeDef",
     {
         "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigs": List[ResolverQueryLogConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResolverRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
@@ -1698,257 +1707,410 @@
         "Name": str,
         "TargetIps": Sequence[TargetAddressTypeDef],
         "ResolverEndpointId": str,
     },
     total=False,
 )
 
-ResolverRuleTypeDef = TypedDict(
-    "ResolverRuleTypeDef",
-    {
-        "Id": str,
-        "CreatorRequestId": str,
-        "Arn": str,
-        "DomainName": str,
-        "Status": ResolverRuleStatusType,
-        "StatusMessage": str,
-        "RuleType": RuleTypeOptionType,
-        "Name": str,
-        "TargetIps": List[TargetAddressTypeDef],
-        "ResolverEndpointId": str,
-        "OwnerId": str,
-        "ShareStatus": ShareStatusType,
-        "CreationTime": str,
-        "ModificationTime": str,
-    },
-    total=False,
-)
-
-ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef = TypedDict(
-    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverDnssecConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverDnssecConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef = TypedDict(
-    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverEndpointsRequestRequestTypeDef = TypedDict(
     "ListResolverEndpointsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef = TypedDict(
-    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverQueryLogConfigAssociationsRequestRequestTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef = TypedDict(
-    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverQueryLogConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverQueryLogConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef = TypedDict(
-    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverRuleAssociationsRequestRequestTypeDef = TypedDict(
     "ListResolverRuleAssociationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverRulesRequestListResolverRulesPaginateTypeDef = TypedDict(
-    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverRulesRequestRequestTypeDef = TypedDict(
     "ListResolverRulesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 GetFirewallConfigResponseTypeDef = TypedDict(
     "GetFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallConfigsResponseTypeDef = TypedDict(
     "ListFirewallConfigsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallConfigs": List[FirewallConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallConfigResponseTypeDef = TypedDict(
     "UpdateFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallDomainListsResponseTypeDef = TypedDict(
     "ListFirewallDomainListsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallDomainLists": List[FirewallDomainListMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRuleGroupsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRuleGroups": List[FirewallRuleGroupMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverConfigResponseTypeDef = TypedDict(
     "GetResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverConfigsResponseTypeDef = TypedDict(
     "ListResolverConfigsResponseTypeDef",
     {
         "NextToken": str,
         "ResolverConfigs": List[ResolverConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverConfigResponseTypeDef = TypedDict(
     "UpdateResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverDnssecConfigResponseTypeDef = TypedDict(
     "GetResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverDnssecConfigsResponseTypeDef = TypedDict(
     "ListResolverDnssecConfigsResponseTypeDef",
     {
         "NextToken": str,
         "ResolverDnssecConfigs": List[ResolverDnssecConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverDnssecConfigResponseTypeDef = TypedDict(
     "UpdateResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverEndpointIpAddressesResponseTypeDef = TypedDict(
     "ListResolverEndpointIpAddressesResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IpAddresses": List[IpAddressResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
+    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef = TypedDict(
+    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    {
+        "FirewallDomainListId": str,
+    },
+)
+_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef(
+    _RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    _OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+):
+    pass
+
+
+ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
+        {
+            "FirewallRuleGroupId": str,
+            "VpcId": str,
+            "Priority": int,
+            "Status": FirewallRuleGroupAssociationStatusType,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef = TypedDict(
+    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
+    "_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    {
+        "FirewallRuleGroupId": str,
+    },
+)
+_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
+    "_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    {
+        "Priority": int,
+        "Action": ActionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
+    _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+):
+    pass
+
+
+ListOutpostResolversRequestListOutpostResolversPaginateTypeDef = TypedDict(
+    "ListOutpostResolversRequestListOutpostResolversPaginateTypeDef",
+    {
+        "OutpostArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
+    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef = TypedDict(
+    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
+    "_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    {
+        "ResolverEndpointId": str,
+    },
+)
+_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
+    "_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef(
+    _RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    _OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+):
+    pass
+
+
+ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef = TypedDict(
+    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef = TypedDict(
+    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef = TypedDict(
+    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef = TypedDict(
+    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverRulesRequestListResolverRulesPaginateTypeDef = TypedDict(
+    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResolverRuleTypeDef = TypedDict(
+    "ResolverRuleTypeDef",
+    {
+        "Id": str,
+        "CreatorRequestId": str,
+        "Arn": str,
+        "DomainName": str,
+        "Status": ResolverRuleStatusType,
+        "StatusMessage": str,
+        "RuleType": RuleTypeOptionType,
+        "Name": str,
+        "TargetIps": List[TargetAddressOutputTypeDef],
+        "ResolverEndpointId": str,
+        "OwnerId": str,
+        "ShareStatus": ShareStatusType,
+        "CreationTime": str,
+        "ModificationTime": str,
     },
 )
 
 _RequiredUpdateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
@@ -1980,44 +2142,44 @@
     },
 )
 
 CreateResolverRuleResponseTypeDef = TypedDict(
     "CreateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverRuleResponseTypeDef = TypedDict(
     "DeleteResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverRuleResponseTypeDef = TypedDict(
     "GetResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverRulesResponseTypeDef = TypedDict(
     "ListResolverRulesResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverRules": List[ResolverRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverRuleResponseTypeDef = TypedDict(
     "UpdateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver/type_defs.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     FirewallDomainListStatusType,
     FirewallDomainUpdateOperationType,
     FirewallFailOpenStatusType,
     FirewallRuleGroupAssociationStatusType,
     FirewallRuleGroupStatusType,
     IpAddressStatusType,
     MutationProtectionStatusType,
+    OutpostResolverStatusType,
     ResolverAutodefinedReverseStatusType,
     ResolverDNSSECValidationStatusType,
     ResolverEndpointDirectionType,
     ResolverEndpointStatusType,
     ResolverEndpointTypeType,
     ResolverQueryLogConfigAssociationErrorType,
     ResolverQueryLogConfigAssociationStatusType,
@@ -49,108 +50,106 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
     "FirewallRuleGroupAssociationTypeDef",
+    "ResponseMetadataTypeDef",
     "IpAddressUpdateTypeDef",
     "ResolverEndpointTypeDef",
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     "ResolverQueryLogConfigAssociationTypeDef",
     "AssociateResolverRuleRequestRequestTypeDef",
     "ResolverRuleAssociationTypeDef",
     "FirewallDomainListTypeDef",
     "FirewallRuleGroupTypeDef",
     "CreateFirewallRuleRequestRequestTypeDef",
     "FirewallRuleTypeDef",
+    "OutpostResolverTypeDef",
     "IpAddressRequestTypeDef",
     "ResolverQueryLogConfigTypeDef",
     "TargetAddressTypeDef",
     "DeleteFirewallDomainListRequestRequestTypeDef",
     "DeleteFirewallRuleGroupRequestRequestTypeDef",
     "DeleteFirewallRuleRequestRequestTypeDef",
+    "DeleteOutpostResolverRequestRequestTypeDef",
     "DeleteResolverEndpointRequestRequestTypeDef",
     "DeleteResolverQueryLogConfigRequestRequestTypeDef",
     "DeleteResolverRuleRequestRequestTypeDef",
     "DisassociateFirewallRuleGroupRequestRequestTypeDef",
     "DisassociateResolverQueryLogConfigRequestRequestTypeDef",
     "DisassociateResolverRuleRequestRequestTypeDef",
     "FilterTypeDef",
     "FirewallConfigTypeDef",
     "FirewallDomainListMetadataTypeDef",
     "FirewallRuleGroupMetadataTypeDef",
     "GetFirewallConfigRequestRequestTypeDef",
     "GetFirewallDomainListRequestRequestTypeDef",
     "GetFirewallRuleGroupAssociationRequestRequestTypeDef",
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
-    "GetFirewallRuleGroupPolicyResponseTypeDef",
     "GetFirewallRuleGroupRequestRequestTypeDef",
+    "GetOutpostResolverRequestRequestTypeDef",
     "GetResolverConfigRequestRequestTypeDef",
     "ResolverConfigTypeDef",
     "GetResolverDnssecConfigRequestRequestTypeDef",
     "ResolverDnssecConfigTypeDef",
     "GetResolverEndpointRequestRequestTypeDef",
     "GetResolverQueryLogConfigAssociationRequestRequestTypeDef",
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
-    "GetResolverQueryLogConfigPolicyResponseTypeDef",
     "GetResolverQueryLogConfigRequestRequestTypeDef",
     "GetResolverRuleAssociationRequestRequestTypeDef",
     "GetResolverRulePolicyRequestRequestTypeDef",
-    "GetResolverRulePolicyResponseTypeDef",
     "GetResolverRuleRequestRequestTypeDef",
     "ImportFirewallDomainsRequestRequestTypeDef",
-    "ImportFirewallDomainsResponseTypeDef",
     "IpAddressResponseTypeDef",
-    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListFirewallConfigsRequestRequestTypeDef",
-    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
     "ListFirewallDomainListsRequestRequestTypeDef",
-    "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
     "ListFirewallDomainsRequestRequestTypeDef",
-    "ListFirewallDomainsResponseTypeDef",
-    "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
-    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
     "ListFirewallRuleGroupsRequestRequestTypeDef",
-    "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
     "ListFirewallRulesRequestRequestTypeDef",
-    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    "ListOutpostResolversRequestRequestTypeDef",
     "ListResolverConfigsRequestRequestTypeDef",
-    "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
     "ListResolverEndpointIpAddressesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "TagOutputTypeDef",
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
-    "PutFirewallRuleGroupPolicyResponseTypeDef",
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
-    "PutResolverQueryLogConfigPolicyResponseTypeDef",
     "PutResolverRulePolicyRequestRequestTypeDef",
-    "PutResolverRulePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "TargetAddressOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallConfigRequestRequestTypeDef",
     "UpdateFirewallDomainsRequestRequestTypeDef",
-    "UpdateFirewallDomainsResponseTypeDef",
     "UpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     "UpdateFirewallRuleRequestRequestTypeDef",
     "UpdateIpAddressTypeDef",
+    "UpdateOutpostResolverRequestRequestTypeDef",
     "UpdateResolverConfigRequestRequestTypeDef",
     "UpdateResolverDnssecConfigRequestRequestTypeDef",
     "AssociateFirewallRuleGroupRequestRequestTypeDef",
     "CreateFirewallDomainListRequestRequestTypeDef",
     "CreateFirewallRuleGroupRequestRequestTypeDef",
+    "CreateOutpostResolverRequestRequestTypeDef",
     "CreateResolverQueryLogConfigRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateFirewallRuleGroupResponseTypeDef",
     "DisassociateFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupAssociationResponseTypeDef",
+    "GetFirewallRuleGroupPolicyResponseTypeDef",
+    "GetResolverQueryLogConfigPolicyResponseTypeDef",
+    "GetResolverRulePolicyResponseTypeDef",
+    "ImportFirewallDomainsResponseTypeDef",
+    "ListFirewallDomainsResponseTypeDef",
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
+    "PutFirewallRuleGroupPolicyResponseTypeDef",
+    "PutResolverQueryLogConfigPolicyResponseTypeDef",
+    "PutResolverRulePolicyResponseTypeDef",
+    "UpdateFirewallDomainsResponseTypeDef",
     "UpdateFirewallRuleGroupAssociationResponseTypeDef",
     "AssociateResolverEndpointIpAddressRequestRequestTypeDef",
     "DisassociateResolverEndpointIpAddressRequestRequestTypeDef",
     "AssociateResolverEndpointIpAddressResponseTypeDef",
     "CreateResolverEndpointResponseTypeDef",
     "DeleteResolverEndpointResponseTypeDef",
     "DisassociateResolverEndpointIpAddressResponseTypeDef",
@@ -171,46 +170,62 @@
     "CreateFirewallRuleGroupResponseTypeDef",
     "DeleteFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupResponseTypeDef",
     "CreateFirewallRuleResponseTypeDef",
     "DeleteFirewallRuleResponseTypeDef",
     "ListFirewallRulesResponseTypeDef",
     "UpdateFirewallRuleResponseTypeDef",
+    "CreateOutpostResolverResponseTypeDef",
+    "DeleteOutpostResolverResponseTypeDef",
+    "GetOutpostResolverResponseTypeDef",
+    "ListOutpostResolversResponseTypeDef",
+    "UpdateOutpostResolverResponseTypeDef",
     "CreateResolverEndpointRequestRequestTypeDef",
     "CreateResolverQueryLogConfigResponseTypeDef",
     "DeleteResolverQueryLogConfigResponseTypeDef",
     "GetResolverQueryLogConfigResponseTypeDef",
     "ListResolverQueryLogConfigsResponseTypeDef",
     "CreateResolverRuleRequestRequestTypeDef",
     "ResolverRuleConfigTypeDef",
-    "ResolverRuleTypeDef",
-    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
     "ListResolverDnssecConfigsRequestRequestTypeDef",
-    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
     "ListResolverEndpointsRequestRequestTypeDef",
-    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
     "ListResolverQueryLogConfigAssociationsRequestRequestTypeDef",
-    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
     "ListResolverQueryLogConfigsRequestRequestTypeDef",
-    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
     "ListResolverRuleAssociationsRequestRequestTypeDef",
-    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
     "ListResolverRulesRequestRequestTypeDef",
     "GetFirewallConfigResponseTypeDef",
     "ListFirewallConfigsResponseTypeDef",
     "UpdateFirewallConfigResponseTypeDef",
     "ListFirewallDomainListsResponseTypeDef",
     "ListFirewallRuleGroupsResponseTypeDef",
     "GetResolverConfigResponseTypeDef",
     "ListResolverConfigsResponseTypeDef",
     "UpdateResolverConfigResponseTypeDef",
     "GetResolverDnssecConfigResponseTypeDef",
     "ListResolverDnssecConfigsResponseTypeDef",
     "UpdateResolverDnssecConfigResponseTypeDef",
     "ListResolverEndpointIpAddressesResponseTypeDef",
+    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
+    "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
+    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
+    "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    "ListOutpostResolversRequestListOutpostResolversPaginateTypeDef",
+    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
+    "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
+    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
+    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
+    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
+    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ResolverRuleTypeDef",
     "UpdateResolverEndpointRequestRequestTypeDef",
     "UpdateResolverRuleRequestRequestTypeDef",
     "CreateResolverRuleResponseTypeDef",
     "DeleteResolverRuleResponseTypeDef",
     "GetResolverRuleResponseTypeDef",
     "ListResolverRulesResponseTypeDef",
     "UpdateResolverRuleResponseTypeDef",
@@ -237,15 +252,25 @@
         "ManagedOwnerName": str,
         "Status": FirewallRuleGroupAssociationStatusType,
         "StatusMessage": str,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 IpAddressUpdateTypeDef = TypedDict(
     "IpAddressUpdateTypeDef",
     {
         "IpId": str,
         "SubnetId": str,
@@ -267,16 +292,17 @@
         "IpAddressCount": int,
         "HostVPCId": str,
         "Status": ResolverEndpointStatusType,
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
         "ResolverEndpointType": ResolverEndpointTypeType,
+        "OutpostArn": str,
+        "PreferredInstanceType": str,
     },
-    total=False,
 )
 
 AssociateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "ResolverQueryLogConfigId": str,
         "ResourceId": str,
@@ -290,15 +316,14 @@
         "ResolverQueryLogConfigId": str,
         "ResourceId": str,
         "Status": ResolverQueryLogConfigAssociationStatusType,
         "Error": ResolverQueryLogConfigAssociationErrorType,
         "ErrorMessage": str,
         "CreationTime": str,
     },
-    total=False,
 )
 
 _RequiredAssociateResolverRuleRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
         "VPCId": str,
@@ -324,15 +349,14 @@
         "Id": str,
         "ResolverRuleId": str,
         "Name": str,
         "VPCId": str,
         "Status": ResolverRuleAssociationStatusType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 FirewallDomainListTypeDef = TypedDict(
     "FirewallDomainListTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -341,15 +365,14 @@
         "Status": FirewallDomainListStatusType,
         "StatusMessage": str,
         "ManagedOwnerName": str,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 FirewallRuleGroupTypeDef = TypedDict(
     "FirewallRuleGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -359,15 +382,14 @@
         "StatusMessage": str,
         "OwnerId": str,
         "CreatorRequestId": str,
         "ShareStatus": ShareStatusType,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 _RequiredCreateFirewallRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "FirewallRuleGroupId": str,
@@ -406,15 +428,31 @@
         "BlockOverrideDomain": str,
         "BlockOverrideDnsType": Literal["CNAME"],
         "BlockOverrideTtl": int,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
+)
+
+OutpostResolverTypeDef = TypedDict(
+    "OutpostResolverTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": str,
+        "ModificationTime": str,
+        "CreatorRequestId": str,
+        "Id": str,
+        "InstanceCount": int,
+        "PreferredInstanceType": str,
+        "Name": str,
+        "Status": OutpostResolverStatusType,
+        "StatusMessage": str,
+        "OutpostArn": str,
+    },
 )
 
 _RequiredIpAddressRequestTypeDef = TypedDict(
     "_RequiredIpAddressRequestTypeDef",
     {
         "SubnetId": str,
     },
@@ -441,15 +479,14 @@
         "AssociationCount": int,
         "Arn": str,
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
         "CreationTime": str,
     },
-    total=False,
 )
 
 TargetAddressTypeDef = TypedDict(
     "TargetAddressTypeDef",
     {
         "Ip": str,
         "Port": int,
@@ -476,14 +513,21 @@
     "DeleteFirewallRuleRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
     },
 )
 
+DeleteOutpostResolverRequestRequestTypeDef = TypedDict(
+    "DeleteOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+
 DeleteResolverEndpointRequestRequestTypeDef = TypedDict(
     "DeleteResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 
@@ -537,40 +581,37 @@
     "FirewallConfigTypeDef",
     {
         "Id": str,
         "ResourceId": str,
         "OwnerId": str,
         "FirewallFailOpen": FirewallFailOpenStatusType,
     },
-    total=False,
 )
 
 FirewallDomainListMetadataTypeDef = TypedDict(
     "FirewallDomainListMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "CreatorRequestId": str,
         "ManagedOwnerName": str,
     },
-    total=False,
 )
 
 FirewallRuleGroupMetadataTypeDef = TypedDict(
     "FirewallRuleGroupMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "OwnerId": str,
         "CreatorRequestId": str,
         "ShareStatus": ShareStatusType,
     },
-    total=False,
 )
 
 GetFirewallConfigRequestRequestTypeDef = TypedDict(
     "GetFirewallConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -593,26 +634,25 @@
 GetFirewallRuleGroupPolicyRequestRequestTypeDef = TypedDict(
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
-    "GetFirewallRuleGroupPolicyResponseTypeDef",
+GetFirewallRuleGroupRequestRequestTypeDef = TypedDict(
+    "GetFirewallRuleGroupRequestRequestTypeDef",
     {
-        "FirewallRuleGroupPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FirewallRuleGroupId": str,
     },
 )
 
-GetFirewallRuleGroupRequestRequestTypeDef = TypedDict(
-    "GetFirewallRuleGroupRequestRequestTypeDef",
+GetOutpostResolverRequestRequestTypeDef = TypedDict(
+    "GetOutpostResolverRequestRequestTypeDef",
     {
-        "FirewallRuleGroupId": str,
+        "Id": str,
     },
 )
 
 GetResolverConfigRequestRequestTypeDef = TypedDict(
     "GetResolverConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
@@ -623,15 +663,14 @@
     "ResolverConfigTypeDef",
     {
         "Id": str,
         "ResourceId": str,
         "OwnerId": str,
         "AutodefinedReverse": ResolverAutodefinedReverseStatusType,
     },
-    total=False,
 )
 
 GetResolverDnssecConfigRequestRequestTypeDef = TypedDict(
     "GetResolverDnssecConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -641,15 +680,14 @@
     "ResolverDnssecConfigTypeDef",
     {
         "Id": str,
         "OwnerId": str,
         "ResourceId": str,
         "ValidationStatus": ResolverDNSSECValidationStatusType,
     },
-    total=False,
 )
 
 GetResolverEndpointRequestRequestTypeDef = TypedDict(
     "GetResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
@@ -665,22 +703,14 @@
 GetResolverQueryLogConfigPolicyRequestRequestTypeDef = TypedDict(
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
-    "GetResolverQueryLogConfigPolicyResponseTypeDef",
-    {
-        "ResolverQueryLogConfigPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "GetResolverQueryLogConfigRequestRequestTypeDef",
     {
         "ResolverQueryLogConfigId": str,
     },
 )
 
@@ -694,22 +724,14 @@
 GetResolverRulePolicyRequestRequestTypeDef = TypedDict(
     "GetResolverRulePolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetResolverRulePolicyResponseTypeDef = TypedDict(
-    "GetResolverRulePolicyResponseTypeDef",
-    {
-        "ResolverRulePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverRuleRequestRequestTypeDef = TypedDict(
     "GetResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
     },
 )
 
@@ -718,94 +740,56 @@
     {
         "FirewallDomainListId": str,
         "Operation": Literal["REPLACE"],
         "DomainFileUrl": str,
     },
 )
 
-ImportFirewallDomainsResponseTypeDef = TypedDict(
-    "ImportFirewallDomainsResponseTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Status": FirewallDomainListStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IpAddressResponseTypeDef = TypedDict(
     "IpAddressResponseTypeDef",
     {
         "IpId": str,
         "SubnetId": str,
         "Ip": str,
         "Ipv6": str,
         "Status": IpAddressStatusType,
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
-ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
-    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListFirewallConfigsRequestRequestTypeDef = TypedDict(
     "ListFirewallConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef = TypedDict(
-    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallDomainListsRequestRequestTypeDef = TypedDict(
     "ListFirewallDomainListsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
-    {
-        "FirewallDomainListId": str,
-    },
-)
-_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef(
-    _RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
-    _OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFirewallDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListFirewallDomainsRequestRequestTypeDef",
     {
         "FirewallDomainListId": str,
     },
 )
 _OptionalListFirewallDomainsRequestRequestTypeDef = TypedDict(
@@ -819,89 +803,36 @@
 
 class ListFirewallDomainsRequestRequestTypeDef(
     _RequiredListFirewallDomainsRequestRequestTypeDef,
     _OptionalListFirewallDomainsRequestRequestTypeDef,
 ):
     pass
 
-ListFirewallDomainsResponseTypeDef = TypedDict(
-    "ListFirewallDomainsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Domains": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
-        {
-            "FirewallRuleGroupId": str,
-            "VpcId": str,
-            "Priority": int,
-            "Status": FirewallRuleGroupAssociationStatusType,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListFirewallRuleGroupAssociationsRequestRequestTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "VpcId": str,
         "Priority": int,
         "Status": FirewallRuleGroupAssociationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef = TypedDict(
-    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListFirewallRuleGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
-    "_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
-    {
-        "FirewallRuleGroupId": str,
-    },
-)
-_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
-    "_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
-    {
-        "Priority": int,
-        "Action": ActionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
-    _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
-    _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFirewallRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListFirewallRulesRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
     },
 )
 _OptionalListFirewallRulesRequestRequestTypeDef = TypedDict(
@@ -916,51 +847,33 @@
 )
 
 class ListFirewallRulesRequestRequestTypeDef(
     _RequiredListFirewallRulesRequestRequestTypeDef, _OptionalListFirewallRulesRequestRequestTypeDef
 ):
     pass
 
-ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
-    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+ListOutpostResolversRequestRequestTypeDef = TypedDict(
+    "ListOutpostResolversRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "OutpostArn": str,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 ListResolverConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
-    "_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
-    {
-        "ResolverEndpointId": str,
-    },
-)
-_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
-    "_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef(
-    _RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
-    _OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResolverEndpointIpAddressesRequestRequestTypeDef = TypedDict(
     "_RequiredListResolverEndpointIpAddressesRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 _OptionalListResolverEndpointIpAddressesRequestRequestTypeDef = TypedDict(
@@ -974,34 +887,14 @@
 
 class ListResolverEndpointIpAddressesRequestRequestTypeDef(
     _RequiredListResolverEndpointIpAddressesRequestRequestTypeDef,
     _OptionalListResolverEndpointIpAddressesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1015,80 +908,52 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 PutFirewallRuleGroupPolicyRequestRequestTypeDef = TypedDict(
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "FirewallRuleGroupPolicy": str,
     },
 )
 
-PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
-    "PutFirewallRuleGroupPolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResolverQueryLogConfigPolicyRequestRequestTypeDef = TypedDict(
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "ResolverQueryLogConfigPolicy": str,
     },
 )
 
-PutResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
-    "PutResolverQueryLogConfigPolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResolverRulePolicyRequestRequestTypeDef = TypedDict(
     "PutResolverRulePolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "ResolverRulePolicy": str,
     },
 )
 
-PutResolverRulePolicyResponseTypeDef = TypedDict(
-    "PutResolverRulePolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TargetAddressOutputTypeDef = TypedDict(
+    "TargetAddressOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Ip": str,
+        "Port": int,
+        "Ipv6": str,
     },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1109,25 +974,14 @@
     {
         "FirewallDomainListId": str,
         "Operation": FirewallDomainUpdateOperationType,
         "Domains": Sequence[str],
     },
 )
 
-UpdateFirewallDomainsResponseTypeDef = TypedDict(
-    "UpdateFirewallDomainsResponseTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Status": FirewallDomainListStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     {
         "FirewallRuleGroupAssociationId": str,
     },
 )
 _OptionalUpdateFirewallRuleGroupAssociationRequestRequestTypeDef = TypedDict(
@@ -1177,14 +1031,36 @@
     "UpdateIpAddressTypeDef",
     {
         "IpId": str,
         "Ipv6": str,
     },
 )
 
+_RequiredUpdateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateOutpostResolverRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalUpdateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateOutpostResolverRequestRequestTypeDef",
+    {
+        "Name": str,
+        "InstanceCount": int,
+        "PreferredInstanceType": str,
+    },
+    total=False,
+)
+
+class UpdateOutpostResolverRequestRequestTypeDef(
+    _RequiredUpdateOutpostResolverRequestRequestTypeDef,
+    _OptionalUpdateOutpostResolverRequestRequestTypeDef,
+):
+    pass
+
 UpdateResolverConfigRequestRequestTypeDef = TypedDict(
     "UpdateResolverConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
         "AutodefinedReverseFlag": AutodefinedReverseFlagType,
     },
 )
@@ -1260,14 +1136,38 @@
 
 class CreateFirewallRuleGroupRequestRequestTypeDef(
     _RequiredCreateFirewallRuleGroupRequestRequestTypeDef,
     _OptionalCreateFirewallRuleGroupRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateOutpostResolverRequestRequestTypeDef",
+    {
+        "CreatorRequestId": str,
+        "Name": str,
+        "PreferredInstanceType": str,
+        "OutpostArn": str,
+    },
+)
+_OptionalCreateOutpostResolverRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateOutpostResolverRequestRequestTypeDef",
+    {
+        "InstanceCount": int,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateOutpostResolverRequestRequestTypeDef(
+    _RequiredCreateOutpostResolverRequestRequestTypeDef,
+    _OptionalCreateOutpostResolverRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
     },
@@ -1282,69 +1182,139 @@
 
 class CreateResolverQueryLogConfigRequestRequestTypeDef(
     _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef,
     _OptionalCreateResolverQueryLogConfigRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 AssociateFirewallRuleGroupResponseTypeDef = TypedDict(
     "AssociateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFirewallRuleGroupResponseTypeDef = TypedDict(
     "DisassociateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallRuleGroupAssociationResponseTypeDef = TypedDict(
     "GetFirewallRuleGroupAssociationResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
+    "GetFirewallRuleGroupPolicyResponseTypeDef",
+    {
+        "FirewallRuleGroupPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
+    "GetResolverQueryLogConfigPolicyResponseTypeDef",
+    {
+        "ResolverQueryLogConfigPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResolverRulePolicyResponseTypeDef = TypedDict(
+    "GetResolverRulePolicyResponseTypeDef",
+    {
+        "ResolverRulePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportFirewallDomainsResponseTypeDef = TypedDict(
+    "ImportFirewallDomainsResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Status": FirewallDomainListStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallDomainsResponseTypeDef = TypedDict(
+    "ListFirewallDomainsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Domains": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRuleGroupAssociationsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRuleGroupAssociations": List[FirewallRuleGroupAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
+    "PutFirewallRuleGroupPolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
+    "PutResolverQueryLogConfigPolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResolverRulePolicyResponseTypeDef = TypedDict(
+    "PutResolverRulePolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDomainsResponseTypeDef = TypedDict(
+    "UpdateFirewallDomainsResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Status": FirewallDomainListStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallRuleGroupAssociationResponseTypeDef = TypedDict(
     "UpdateFirewallRuleGroupAssociationResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverEndpointIpAddressRequestRequestTypeDef = TypedDict(
     "AssociateResolverEndpointIpAddressRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
@@ -1360,215 +1330,256 @@
     },
 )
 
 AssociateResolverEndpointIpAddressResponseTypeDef = TypedDict(
     "AssociateResolverEndpointIpAddressResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResolverEndpointResponseTypeDef = TypedDict(
     "CreateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverEndpointResponseTypeDef = TypedDict(
     "DeleteResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverEndpointIpAddressResponseTypeDef = TypedDict(
     "DisassociateResolverEndpointIpAddressResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverEndpointResponseTypeDef = TypedDict(
     "GetResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverEndpointsResponseTypeDef = TypedDict(
     "ListResolverEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverEndpoints": List[ResolverEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverEndpointResponseTypeDef = TypedDict(
     "UpdateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "DisassociateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverQueryLogConfigAssociationResponseTypeDef = TypedDict(
     "GetResolverQueryLogConfigAssociationResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverQueryLogConfigAssociationsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigAssociations": List[ResolverQueryLogConfigAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverRuleResponseTypeDef = TypedDict(
     "AssociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverRuleResponseTypeDef = TypedDict(
     "DisassociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverRuleAssociationResponseTypeDef = TypedDict(
     "GetResolverRuleAssociationResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverRuleAssociationsResponseTypeDef = TypedDict(
     "ListResolverRuleAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverRuleAssociations": List[ResolverRuleAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallDomainListResponseTypeDef = TypedDict(
     "CreateFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallDomainListResponseTypeDef = TypedDict(
     "DeleteFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallDomainListResponseTypeDef = TypedDict(
     "GetFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallRuleGroupResponseTypeDef = TypedDict(
     "CreateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallRuleGroupResponseTypeDef = TypedDict(
     "DeleteFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallRuleGroupResponseTypeDef = TypedDict(
     "GetFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallRuleResponseTypeDef = TypedDict(
     "CreateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallRuleResponseTypeDef = TypedDict(
     "DeleteFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRulesResponseTypeDef = TypedDict(
     "ListFirewallRulesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRules": List[FirewallRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallRuleResponseTypeDef = TypedDict(
     "UpdateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOutpostResolverResponseTypeDef = TypedDict(
+    "CreateOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteOutpostResolverResponseTypeDef = TypedDict(
+    "DeleteOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOutpostResolverResponseTypeDef = TypedDict(
+    "GetOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOutpostResolversResponseTypeDef = TypedDict(
+    "ListOutpostResolversResponseTypeDef",
+    {
+        "OutpostResolvers": List[OutpostResolverTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateOutpostResolverResponseTypeDef = TypedDict(
+    "UpdateOutpostResolverResponseTypeDef",
+    {
+        "OutpostResolver": OutpostResolverTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverEndpointRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
@@ -1579,56 +1590,58 @@
 )
 _OptionalCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_OptionalCreateResolverEndpointRequestRequestTypeDef",
     {
         "Name": str,
         "Tags": Sequence[TagTypeDef],
         "ResolverEndpointType": ResolverEndpointTypeType,
+        "OutpostArn": str,
+        "PreferredInstanceType": str,
     },
     total=False,
 )
 
 class CreateResolverEndpointRequestRequestTypeDef(
     _RequiredCreateResolverEndpointRequestRequestTypeDef,
     _OptionalCreateResolverEndpointRequestRequestTypeDef,
 ):
     pass
 
 CreateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "CreateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverQueryLogConfigResponseTypeDef = TypedDict(
     "DeleteResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverQueryLogConfigResponseTypeDef = TypedDict(
     "GetResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverQueryLogConfigsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigsResponseTypeDef",
     {
         "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigs": List[ResolverQueryLogConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResolverRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
@@ -1659,257 +1672,402 @@
         "Name": str,
         "TargetIps": Sequence[TargetAddressTypeDef],
         "ResolverEndpointId": str,
     },
     total=False,
 )
 
-ResolverRuleTypeDef = TypedDict(
-    "ResolverRuleTypeDef",
-    {
-        "Id": str,
-        "CreatorRequestId": str,
-        "Arn": str,
-        "DomainName": str,
-        "Status": ResolverRuleStatusType,
-        "StatusMessage": str,
-        "RuleType": RuleTypeOptionType,
-        "Name": str,
-        "TargetIps": List[TargetAddressTypeDef],
-        "ResolverEndpointId": str,
-        "OwnerId": str,
-        "ShareStatus": ShareStatusType,
-        "CreationTime": str,
-        "ModificationTime": str,
-    },
-    total=False,
-)
-
-ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef = TypedDict(
-    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverDnssecConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverDnssecConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef = TypedDict(
-    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverEndpointsRequestRequestTypeDef = TypedDict(
     "ListResolverEndpointsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef = TypedDict(
-    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverQueryLogConfigAssociationsRequestRequestTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef = TypedDict(
-    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverQueryLogConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverQueryLogConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef = TypedDict(
-    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverRuleAssociationsRequestRequestTypeDef = TypedDict(
     "ListResolverRuleAssociationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverRulesRequestListResolverRulesPaginateTypeDef = TypedDict(
-    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverRulesRequestRequestTypeDef = TypedDict(
     "ListResolverRulesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 GetFirewallConfigResponseTypeDef = TypedDict(
     "GetFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallConfigsResponseTypeDef = TypedDict(
     "ListFirewallConfigsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallConfigs": List[FirewallConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallConfigResponseTypeDef = TypedDict(
     "UpdateFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallDomainListsResponseTypeDef = TypedDict(
     "ListFirewallDomainListsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallDomainLists": List[FirewallDomainListMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRuleGroupsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRuleGroups": List[FirewallRuleGroupMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverConfigResponseTypeDef = TypedDict(
     "GetResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverConfigsResponseTypeDef = TypedDict(
     "ListResolverConfigsResponseTypeDef",
     {
         "NextToken": str,
         "ResolverConfigs": List[ResolverConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverConfigResponseTypeDef = TypedDict(
     "UpdateResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverDnssecConfigResponseTypeDef = TypedDict(
     "GetResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverDnssecConfigsResponseTypeDef = TypedDict(
     "ListResolverDnssecConfigsResponseTypeDef",
     {
         "NextToken": str,
         "ResolverDnssecConfigs": List[ResolverDnssecConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverDnssecConfigResponseTypeDef = TypedDict(
     "UpdateResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverEndpointIpAddressesResponseTypeDef = TypedDict(
     "ListResolverEndpointIpAddressesResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IpAddresses": List[IpAddressResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
+    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef = TypedDict(
+    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    {
+        "FirewallDomainListId": str,
+    },
+)
+_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef(
+    _RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    _OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+):
+    pass
+
+ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
+        {
+            "FirewallRuleGroupId": str,
+            "VpcId": str,
+            "Priority": int,
+            "Status": FirewallRuleGroupAssociationStatusType,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef = TypedDict(
+    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
+    "_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    {
+        "FirewallRuleGroupId": str,
+    },
+)
+_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
+    "_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    {
+        "Priority": int,
+        "Action": ActionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
+    _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+):
+    pass
+
+ListOutpostResolversRequestListOutpostResolversPaginateTypeDef = TypedDict(
+    "ListOutpostResolversRequestListOutpostResolversPaginateTypeDef",
+    {
+        "OutpostArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
+    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef = TypedDict(
+    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
+    "_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    {
+        "ResolverEndpointId": str,
+    },
+)
+_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
+    "_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef(
+    _RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    _OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+):
+    pass
+
+ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef = TypedDict(
+    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef = TypedDict(
+    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef = TypedDict(
+    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef = TypedDict(
+    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverRulesRequestListResolverRulesPaginateTypeDef = TypedDict(
+    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResolverRuleTypeDef = TypedDict(
+    "ResolverRuleTypeDef",
+    {
+        "Id": str,
+        "CreatorRequestId": str,
+        "Arn": str,
+        "DomainName": str,
+        "Status": ResolverRuleStatusType,
+        "StatusMessage": str,
+        "RuleType": RuleTypeOptionType,
+        "Name": str,
+        "TargetIps": List[TargetAddressOutputTypeDef],
+        "ResolverEndpointId": str,
+        "OwnerId": str,
+        "ShareStatus": ShareStatusType,
+        "CreationTime": str,
+        "ModificationTime": str,
     },
 )
 
 _RequiredUpdateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
@@ -1939,44 +2097,44 @@
     },
 )
 
 CreateResolverRuleResponseTypeDef = TypedDict(
     "CreateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverRuleResponseTypeDef = TypedDict(
     "DeleteResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverRuleResponseTypeDef = TypedDict(
     "GetResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverRulesResponseTypeDef = TypedDict(
     "ListResolverRulesResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverRules": List[ResolverRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverRuleResponseTypeDef = TypedDict(
     "UpdateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/PKG-INFO` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53resolver
-Version: 1.28.0
-Summary: Type annotations for boto3.Route53Resolver 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.8
+Summary: Type annotations for boto3.Route53Resolver 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -287,14 +287,15 @@
 from mypy_boto3_route53resolver.paginator import (
     ListFirewallConfigsPaginator,
     ListFirewallDomainListsPaginator,
     ListFirewallDomainsPaginator,
     ListFirewallRuleGroupAssociationsPaginator,
     ListFirewallRuleGroupsPaginator,
     ListFirewallRulesPaginator,
+    ListOutpostResolversPaginator,
     ListResolverConfigsPaginator,
     ListResolverDnssecConfigsPaginator,
     ListResolverEndpointIpAddressesPaginator,
     ListResolverEndpointsPaginator,
     ListResolverQueryLogConfigAssociationsPaginator,
     ListResolverQueryLogConfigsPaginator,
     ListResolverRuleAssociationsPaginator,
@@ -320,14 +321,17 @@
 )
 list_firewall_rule_groups_paginator: ListFirewallRuleGroupsPaginator = client.get_paginator(
     "list_firewall_rule_groups"
 )
 list_firewall_rules_paginator: ListFirewallRulesPaginator = client.get_paginator(
     "list_firewall_rules"
 )
+list_outpost_resolvers_paginator: ListOutpostResolversPaginator = client.get_paginator(
+    "list_outpost_resolvers"
+)
 list_resolver_configs_paginator: ListResolverConfigsPaginator = client.get_paginator(
     "list_resolver_configs"
 )
 list_resolver_dnssec_configs_paginator: ListResolverDnssecConfigsPaginator = client.get_paginator(
     "list_resolver_dnssec_configs"
 )
 list_resolver_endpoint_ip_addresses_paginator: ListResolverEndpointIpAddressesPaginator = (
@@ -375,24 +379,26 @@
     IpAddressStatusType,
     ListFirewallConfigsPaginatorName,
     ListFirewallDomainListsPaginatorName,
     ListFirewallDomainsPaginatorName,
     ListFirewallRuleGroupAssociationsPaginatorName,
     ListFirewallRuleGroupsPaginatorName,
     ListFirewallRulesPaginatorName,
+    ListOutpostResolversPaginatorName,
     ListResolverConfigsPaginatorName,
     ListResolverDnssecConfigsPaginatorName,
     ListResolverEndpointIpAddressesPaginatorName,
     ListResolverEndpointsPaginatorName,
     ListResolverQueryLogConfigAssociationsPaginatorName,
     ListResolverQueryLogConfigsPaginatorName,
     ListResolverRuleAssociationsPaginatorName,
     ListResolverRulesPaginatorName,
     ListTagsForResourcePaginatorName,
     MutationProtectionStatusType,
+    OutpostResolverStatusType,
     ResolverAutodefinedReverseStatusType,
     ResolverDNSSECValidationStatusType,
     ResolverEndpointDirectionType,
     ResolverEndpointStatusType,
     ResolverEndpointTypeType,
     ResolverQueryLogConfigAssociationErrorType,
     ResolverQueryLogConfigAssociationStatusType,
@@ -422,108 +428,106 @@
 `mypy_boto3_route53resolver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53resolver.type_defs import (
     TagTypeDef,
     FirewallRuleGroupAssociationTypeDef,
+    ResponseMetadataTypeDef,
     IpAddressUpdateTypeDef,
     ResolverEndpointTypeDef,
     AssociateResolverQueryLogConfigRequestRequestTypeDef,
     ResolverQueryLogConfigAssociationTypeDef,
     AssociateResolverRuleRequestRequestTypeDef,
     ResolverRuleAssociationTypeDef,
     FirewallDomainListTypeDef,
     FirewallRuleGroupTypeDef,
     CreateFirewallRuleRequestRequestTypeDef,
     FirewallRuleTypeDef,
+    OutpostResolverTypeDef,
     IpAddressRequestTypeDef,
     ResolverQueryLogConfigTypeDef,
     TargetAddressTypeDef,
     DeleteFirewallDomainListRequestRequestTypeDef,
     DeleteFirewallRuleGroupRequestRequestTypeDef,
     DeleteFirewallRuleRequestRequestTypeDef,
+    DeleteOutpostResolverRequestRequestTypeDef,
     DeleteResolverEndpointRequestRequestTypeDef,
     DeleteResolverQueryLogConfigRequestRequestTypeDef,
     DeleteResolverRuleRequestRequestTypeDef,
     DisassociateFirewallRuleGroupRequestRequestTypeDef,
     DisassociateResolverQueryLogConfigRequestRequestTypeDef,
     DisassociateResolverRuleRequestRequestTypeDef,
     FilterTypeDef,
     FirewallConfigTypeDef,
     FirewallDomainListMetadataTypeDef,
     FirewallRuleGroupMetadataTypeDef,
     GetFirewallConfigRequestRequestTypeDef,
     GetFirewallDomainListRequestRequestTypeDef,
     GetFirewallRuleGroupAssociationRequestRequestTypeDef,
     GetFirewallRuleGroupPolicyRequestRequestTypeDef,
-    GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupRequestRequestTypeDef,
+    GetOutpostResolverRequestRequestTypeDef,
     GetResolverConfigRequestRequestTypeDef,
     ResolverConfigTypeDef,
     GetResolverDnssecConfigRequestRequestTypeDef,
     ResolverDnssecConfigTypeDef,
     GetResolverEndpointRequestRequestTypeDef,
     GetResolverQueryLogConfigAssociationRequestRequestTypeDef,
     GetResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigRequestRequestTypeDef,
     GetResolverRuleAssociationRequestRequestTypeDef,
     GetResolverRulePolicyRequestRequestTypeDef,
-    GetResolverRulePolicyResponseTypeDef,
     GetResolverRuleRequestRequestTypeDef,
     ImportFirewallDomainsRequestRequestTypeDef,
-    ImportFirewallDomainsResponseTypeDef,
     IpAddressResponseTypeDef,
-    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallConfigsRequestRequestTypeDef,
-    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
     ListFirewallDomainListsRequestRequestTypeDef,
-    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
     ListFirewallDomainsRequestRequestTypeDef,
-    ListFirewallDomainsResponseTypeDef,
-    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
     ListFirewallRuleGroupAssociationsRequestRequestTypeDef,
-    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
     ListFirewallRuleGroupsRequestRequestTypeDef,
-    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
     ListFirewallRulesRequestRequestTypeDef,
-    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListOutpostResolversRequestRequestTypeDef,
     ListResolverConfigsRequestRequestTypeDef,
-    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
     ListResolverEndpointIpAddressesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    TagOutputTypeDef,
     PutFirewallRuleGroupPolicyRequestRequestTypeDef,
-    PutFirewallRuleGroupPolicyResponseTypeDef,
     PutResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    PutResolverQueryLogConfigPolicyResponseTypeDef,
     PutResolverRulePolicyRequestRequestTypeDef,
-    PutResolverRulePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
+    TargetAddressOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallConfigRequestRequestTypeDef,
     UpdateFirewallDomainsRequestRequestTypeDef,
-    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
     UpdateFirewallRuleRequestRequestTypeDef,
     UpdateIpAddressTypeDef,
+    UpdateOutpostResolverRequestRequestTypeDef,
     UpdateResolverConfigRequestRequestTypeDef,
     UpdateResolverDnssecConfigRequestRequestTypeDef,
     AssociateFirewallRuleGroupRequestRequestTypeDef,
     CreateFirewallDomainListRequestRequestTypeDef,
     CreateFirewallRuleGroupRequestRequestTypeDef,
+    CreateOutpostResolverRequestRequestTypeDef,
     CreateResolverQueryLogConfigRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateFirewallRuleGroupResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
+    GetFirewallRuleGroupPolicyResponseTypeDef,
+    GetResolverQueryLogConfigPolicyResponseTypeDef,
+    GetResolverRulePolicyResponseTypeDef,
+    ImportFirewallDomainsResponseTypeDef,
+    ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
+    PutFirewallRuleGroupPolicyResponseTypeDef,
+    PutResolverQueryLogConfigPolicyResponseTypeDef,
+    PutResolverRulePolicyResponseTypeDef,
+    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     AssociateResolverEndpointIpAddressRequestRequestTypeDef,
     DisassociateResolverEndpointIpAddressRequestRequestTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
@@ -544,46 +548,62 @@
     CreateFirewallRuleGroupResponseTypeDef,
     DeleteFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupResponseTypeDef,
     CreateFirewallRuleResponseTypeDef,
     DeleteFirewallRuleResponseTypeDef,
     ListFirewallRulesResponseTypeDef,
     UpdateFirewallRuleResponseTypeDef,
+    CreateOutpostResolverResponseTypeDef,
+    DeleteOutpostResolverResponseTypeDef,
+    GetOutpostResolverResponseTypeDef,
+    ListOutpostResolversResponseTypeDef,
+    UpdateOutpostResolverResponseTypeDef,
     CreateResolverEndpointRequestRequestTypeDef,
     CreateResolverQueryLogConfigResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     CreateResolverRuleRequestRequestTypeDef,
     ResolverRuleConfigTypeDef,
-    ResolverRuleTypeDef,
-    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
     ListResolverDnssecConfigsRequestRequestTypeDef,
-    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
     ListResolverEndpointsRequestRequestTypeDef,
-    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
     ListResolverQueryLogConfigAssociationsRequestRequestTypeDef,
-    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
     ListResolverQueryLogConfigsRequestRequestTypeDef,
-    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
     ListResolverRuleAssociationsRequestRequestTypeDef,
-    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
     ListResolverRulesRequestRequestTypeDef,
     GetFirewallConfigResponseTypeDef,
     ListFirewallConfigsResponseTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
+    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
+    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
+    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
+    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    ListOutpostResolversRequestListOutpostResolversPaginateTypeDef,
+    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
+    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
+    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
+    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
+    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
+    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ResolverRuleTypeDef,
     UpdateResolverEndpointRequestRequestTypeDef,
     UpdateResolverRuleRequestRequestTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     GetResolverRuleResponseTypeDef,
     ListResolverRulesResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
```

### Comparing `mypy-boto3-route53resolver-1.28.0/mypy_boto3_route53resolver.egg-info/SOURCES.txt` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.0/setup.py` & `mypy-boto3-route53resolver-1.28.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53resolver",
-    version="1.28.0",
+    version="1.28.8",
     packages=["mypy_boto3_route53resolver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53Resolver 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Route53Resolver 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

