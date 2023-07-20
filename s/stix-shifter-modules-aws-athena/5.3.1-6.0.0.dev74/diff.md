# Comparing `tmp/stix_shifter_modules_aws_athena-5.3.1-py2.py3-none-any.whl.zip` & `tmp/stix_shifter_modules_aws_athena-6.0.0.dev74-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,39 +1,40 @@
-Zip file size: 79942 bytes, number of entries: 37
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/__init__.py
--rw-rw-r--  2.0 unx     1374 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/entry_point.py
--rw-rw-r--  2.0 unx   252493 b- defN 23-Jun-15 14:07 stix_shifter_modules/aws_athena/configuration/config.json
--rw-rw-r--  2.0 unx      229 b- defN 23-Jun-15 14:07 stix_shifter_modules/aws_athena/configuration/dialects.json
--rw-rw-r--  2.0 unx     4766 b- defN 23-Jun-15 14:07 stix_shifter_modules/aws_athena/configuration/lang_en.json
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/__init__.py
--rw-rw-r--  2.0 unx    22646 b- defN 23-Jun-15 14:07 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
--rw-rw-r--  2.0 unx    24044 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
--rw-rw-r--  2.0 unx     1024 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
--rw-rw-r--  2.0 unx     1522 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/results_translator.py
--rw-rw-r--  2.0 unx     1075 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/transformers.py
--rw-rw-r--  2.0 unx     4765 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
--rw-rw-r--  2.0 unx     1894 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx      139 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
--rw-rw-r--  2.0 unx     2439 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
--rw-rw-r--  2.0 unx    18300 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx      591 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
--rw-rw-r--  2.0 unx    94369 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/to_stix_map.json
--rw-rw-r--  2.0 unx      891 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx     1894 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    18297 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    93792 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
--rw-rw-r--  2.0 unx      891 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
--rw-rw-r--  2.0 unx     4173 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
--rw-rw-r--  2.0 unx     1207 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
--rw-rw-r--  2.0 unx     1959 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
--rw-rw-r--  2.0 unx     1370 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
--rw-rw-r--  2.0 unx     7443 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
--rw-rw-r--  2.0 unx    14478 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
--rw-rw-r--  2.0 unx     3175 b- defN 23-Jun-15 14:04 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
--rw-rw-r--  2.0 unx    12786 b- defN 23-Jun-15 14:07 stix_shifter_modules_aws_athena-5.3.1.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     8040 b- defN 23-Jun-15 14:07 stix_shifter_modules_aws_athena-5.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-15 14:07 stix_shifter_modules_aws_athena-5.3.1.dist-info/NOTICE
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-15 14:07 stix_shifter_modules_aws_athena-5.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       21 b- defN 23-Jun-15 14:07 stix_shifter_modules_aws_athena-5.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4540 b- defN 23-Jun-15 14:07 stix_shifter_modules_aws_athena-5.3.1.dist-info/RECORD
-37 files, 608155 bytes uncompressed, 72124 bytes compressed:  88.1%
+Zip file size: 81137 bytes, number of entries: 38
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/__init__.py
+-rw-rw-r--  2.0 unx     1374 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/entry_point.py
+-rw-rw-r--  2.0 unx   239955 b- defN 23-Jul-20 18:39 stix_shifter_modules/aws_athena/configuration/config.json
+-rw-rw-r--  2.0 unx      229 b- defN 23-Jul-20 18:39 stix_shifter_modules/aws_athena/configuration/dialects.json
+-rw-rw-r--  2.0 unx     4766 b- defN 23-Jul-20 18:39 stix_shifter_modules/aws_athena/configuration/lang_en.json
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/__init__.py
+-rw-rw-r--  2.0 unx    27024 b- defN 23-Jul-20 18:39 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
+-rw-rw-r--  2.0 unx    24044 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
+-rw-rw-r--  2.0 unx     1024 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
+-rw-rw-r--  2.0 unx     1075 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/transformers.py
+-rw-rw-r--  2.0 unx     4765 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
+-rw-rw-r--  2.0 unx     1894 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    10146 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
+-rw-rw-r--  2.0 unx      139 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
+-rw-rw-r--  2.0 unx     2439 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
+-rw-rw-r--  2.0 unx    18300 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    75601 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
+-rw-rw-r--  2.0 unx      591 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx     2350 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
+-rw-rw-r--  2.0 unx     1894 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    18297 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    93792 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
+-rw-rw-r--  2.0 unx      891 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
+-rw-rw-r--  2.0 unx     4173 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
+-rw-rw-r--  2.0 unx     1207 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
+-rw-rw-r--  2.0 unx     1959 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
+-rw-rw-r--  2.0 unx     1370 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
+-rw-rw-r--  2.0 unx     7443 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
+-rw-rw-r--  2.0 unx    15539 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
+-rw-rw-r--  2.0 unx     3175 b- defN 23-Jul-20 18:36 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
+-rw-rw-r--  2.0 unx    12786 b- defN 23-Jul-20 18:39 stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     8046 b- defN 23-Jul-20 18:39 stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-20 18:39 stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/NOTICE
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-20 18:39 stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jul-20 18:39 stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4727 b- defN 23-Jul-20 18:39 stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/RECORD
+38 files, 593378 bytes uncompressed, 72985 bytes compressed:  87.7%
```

## zipnote {}

```diff
@@ -21,44 +21,47 @@
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/query_translator.py
 Comment: 
 
-Filename: stix_shifter_modules/aws_athena/stix_translation/results_translator.py
-Comment: 
-
 Filename: stix_shifter_modules/aws_athena/stix_translation/transformers.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
 Comment: 
 
+Filename: stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
+Comment: 
+
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
 Comment: 
 
-Filename: stix_shifter_modules/aws_athena/stix_translation/json/operators.json
+Filename: stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
 Comment: 
 
-Filename: stix_shifter_modules/aws_athena/stix_translation/json/to_stix_map.json
+Filename: stix_shifter_modules/aws_athena/stix_translation/json/operators.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
 Comment: 
 
+Filename: stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
+Comment: 
+
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
@@ -87,26 +90,26 @@
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.1.dist-info/LICENSE.md
+Filename: stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/LICENSE.md
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.1.dist-info/METADATA
+Filename: stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/METADATA
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.1.dist-info/NOTICE
+Filename: stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/NOTICE
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.1.dist-info/WHEEL
+Filename: stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/WHEEL
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.1.dist-info/top_level.txt
+Filename: stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/top_level.txt
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-5.3.1.dist-info/RECORD
+Filename: stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stix_shifter_modules/aws_athena/configuration/config.json

### Pretty-printed

 * *Similarity: 0.9999782781139315%*

 * *Differences: {"'connection'": "{'options': {'mapping': {'default': {'vpcflow_from_stix_map': {'ipv4-addr': "*

 * *                 "{'fields': {'value': ['srcaddr', 'dstaddr'], 'x_aws_interface_id': "*

 * *                 "['interface_id']}}, 'ipv6-addr': {'fields': {'value': ['srcaddr', 'dstaddr'], "*

 * *                 "'x_aws_interface_id': ['interface_id']}}, 'network-traffic': {'fields': "*

 * *                 "{'src_port': ['srcport'], 'dst_port': ['dstport'], 'src_ref.value': ['srcaddr'], "*

 * *                 "'dst_ref.value': ['d […]*

```diff
@@ -318,14 +318,397 @@
                                 ],
                                 "start": [
                                     "event_firstseen"
                                 ]
                             }
                         }
                     },
+                    "guardduty_to_stix_map": {
+                        "accountid": {
+                            "key": "x-aws-details.account_id",
+                            "object": "aws_details"
+                        },
+                        "description": {
+                            "key": "x-ibm-finding.description",
+                            "object": "ibm_finding"
+                        },
+                        "dnsrequest_resource_instancedetails_networkinterfaces_0_privateipaddress": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "dns_private_ip1"
+                            },
+                            {
+                                "key": "domain-name.resolves_to_refs",
+                                "object": "private_dns_name",
+                                "references": [
+                                    "dns_private_ip1"
+                                ]
+                            },
+                            {
+                                "key": "x-ibm-finding.src_ip_ref",
+                                "object": "ibm_finding",
+                                "references": "dns_private_ip1"
+                            },
+                            {
+                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                "key": "ipv4-addr.x_aws_interface_id",
+                                "object": "dns_private_ip1"
+                            },
+                            {
+                                "key": "ipv4-addr.x_aws_ip_type",
+                                "object": "dns_private_ip1",
+                                "value": "private"
+                            }
+                        ],
+                        "portprobe_resource_instancedetails_networkinterfaces_0_privateipaddress": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "pp_private_ip1"
+                            },
+                            {
+                                "key": "domain-name.resolves_to_refs",
+                                "object": "private_dns_name",
+                                "references": [
+                                    "pp_private_ip1"
+                                ]
+                            },
+                            {
+                                "key": "x-ibm-finding.src_ip_ref",
+                                "object": "ibm_finding",
+                                "references": "pp_private_ip1"
+                            },
+                            {
+                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                "key": "ipv4-addr.x_aws_interface_id",
+                                "object": "pp_private_ip1"
+                            },
+                            {
+                                "key": "ipv4-addr.x_aws_ip_type",
+                                "object": "pp_private_ip1",
+                                "value": "private"
+                            }
+                        ],
+                        "region": {
+                            "key": "x-aws-details.region",
+                            "object": "aws_details"
+                        },
+                        "resource_accesskeydetails_accesskeyid": {
+                            "key": "x-aws-api.access_key_id",
+                            "object": "api_details"
+                        },
+                        "resource_accesskeydetails_principalid": {
+                            "key": "user-account.user_id",
+                            "object": "api_user"
+                        },
+                        "resource_accesskeydetails_username": {
+                            "key": "user-account.account_login",
+                            "object": "api_user"
+                        },
+                        "resource_instancedetails_availabilityzone": {
+                            "key": "x-aws-instance.availability_zone",
+                            "object": "instance"
+                        },
+                        "resource_instancedetails_imageid": {
+                            "key": "x-aws-instance.image_id",
+                            "object": "instance"
+                        },
+                        "resource_instancedetails_instanceid": {
+                            "key": "x-aws-instance.instance_id",
+                            "object": "instance"
+                        },
+                        "resource_instancedetails_networkinterfaces_0_ipv6addresses_0": [
+                            {
+                                "key": "ipv6-addr.value",
+                                "object": "nc_ipv6_ip"
+                            },
+                            {
+                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                "key": "ipv6-addr.x_aws_interface_id",
+                                "object": "nc_ipv6_ip"
+                            }
+                        ],
+                        "resource_instancedetails_networkinterfaces_0_privatednsname": [
+                            {
+                                "key": "domain-name.value",
+                                "object": "private_dns_name"
+                            }
+                        ],
+                        "resource_instancedetails_networkinterfaces_0_privateipaddress": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "nc_private_ip1"
+                            },
+                            {
+                                "key": "network-traffic.src_ref",
+                                "object": "nc_nt",
+                                "references": "nc_private_ip1"
+                            },
+                            {
+                                "key": "domain-name.resolves_to_refs",
+                                "object": "private_dns_name",
+                                "references": [
+                                    "nc_private_ip1"
+                                ]
+                            },
+                            {
+                                "key": "x-ibm-finding.src_ip_ref",
+                                "object": "ibm_finding",
+                                "references": "nc_private_ip1"
+                            },
+                            {
+                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                "key": "ipv4-addr.x_aws_interface_id",
+                                "object": "nc_private_ip1"
+                            },
+                            {
+                                "key": "ipv4-addr.x_aws_ip_type",
+                                "object": "nc_private_ip1",
+                                "value": "private"
+                            }
+                        ],
+                        "resource_instancedetails_networkinterfaces_0_publicdnsname": [
+                            {
+                                "key": "domain-name.value",
+                                "object": "nc_public_name"
+                            }
+                        ],
+                        "resource_instancedetails_networkinterfaces_0_publicip": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "nc_public_ip"
+                            },
+                            {
+                                "key": "domain-name.resolves_to_refs",
+                                "object": "nc_public_name",
+                                "references": [
+                                    "nc_public_ip"
+                                ]
+                            },
+                            {
+                                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
+                                "key": "ipv4-addr.x_aws_interface_id",
+                                "object": "nc_public_ip"
+                            },
+                            {
+                                "key": "ipv4-addr.x_aws_ip_type",
+                                "object": "nc_public_ip",
+                                "value": "public"
+                            }
+                        ],
+                        "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupid": {
+                            "key": "x-aws-vpc.security_group_id",
+                            "object": "vpc"
+                        },
+                        "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupname": {
+                            "key": "x-aws-vpc.security_group_name",
+                            "object": "vpc"
+                        },
+                        "resource_instancedetails_networkinterfaces_0_subnetid": {
+                            "key": "x-aws-vpc.subnet_id",
+                            "object": "vpc"
+                        },
+                        "resource_instancedetails_networkinterfaces_0_vpcid": {
+                            "key": "x-aws-vpc.vpc_id",
+                            "object": "vpc"
+                        },
+                        "resource_instancedetails_networkinterfaces_1_privatednsname": [
+                            {
+                                "key": "domain-name.value",
+                                "object": "nc_private_name2"
+                            }
+                        ],
+                        "resource_instancedetails_networkinterfaces_1_privateipaddress": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "nc_private_ip2"
+                            },
+                            {
+                                "key": "domain-name.resolves_to_refs",
+                                "object": "nc_private_name2",
+                                "references": [
+                                    "nc_private_ip2"
+                                ]
+                            },
+                            {
+                                "ds_key": "resource_instancedetails_networkinterfaces_1_networkinterfaceid",
+                                "key": "ipv4-addr.x_aws_interface_id",
+                                "object": "nc_private_ip2"
+                            },
+                            {
+                                "key": "ipv4-addr.x_aws_ip_type",
+                                "object": "nc_private_ip2",
+                                "value": "private"
+                            }
+                        ],
+                        "resource_instancedetails_platform": [
+                            {
+                                "key": "software.name",
+                                "object": "software"
+                            },
+                            {
+                                "key": "x-ibm-finding.src_os_ref",
+                                "object": "ibm_finding",
+                                "references": "software"
+                            }
+                        ],
+                        "service_action_awsapicallaction_api": {
+                            "key": "x-aws-api.api",
+                            "object": "api_details"
+                        },
+                        "service_action_awsapicallaction_remoteipdetails_ipaddressv4": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "api_remote_ip"
+                            },
+                            {
+                                "key": "x-ibm-finding.dst_ip_ref",
+                                "object": "ibm_finding",
+                                "references": "api_remote_ip"
+                            },
+                            {
+                                "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
+                                "key": "x-ibm-finding.dst_geolocation",
+                                "object": "ibm_finding"
+                            },
+                            {
+                                "ds_key": "service_action_awsapicallaction_remoteipdetails_city_cityname",
+                                "key": "ipv4-addr.x_aws_remote_city_name",
+                                "object": "api_remote_ip"
+                            },
+                            {
+                                "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
+                                "key": "ipv4-addr.x_aws_remote_country_name",
+                                "object": "api_remote_ip"
+                            }
+                        ],
+                        "service_action_awsapicallaction_servicename": {
+                            "key": "x-aws-api.service_name",
+                            "object": "api_details"
+                        },
+                        "service_action_dnsrequestaction_domain": [
+                            {
+                                "key": "domain-name.value",
+                                "object": "dns_domain_name"
+                            }
+                        ],
+                        "service_action_networkconnectionaction_localportdetails_port": [
+                            {
+                                "key": "network-traffic.src_port",
+                                "object": "nc_nt",
+                                "transformer": "ToInteger"
+                            }
+                        ],
+                        "service_action_networkconnectionaction_protocol": [
+                            {
+                                "key": "network-traffic.protocols",
+                                "object": "nc_nt",
+                                "transformer": "ToLowercaseArray"
+                            }
+                        ],
+                        "service_action_networkconnectionaction_remoteipdetails_ipaddressv4": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "nc_remote_ip"
+                            },
+                            {
+                                "key": "network-traffic.dst_ref",
+                                "object": "nc_nt",
+                                "references": "nc_remote_ip"
+                            },
+                            {
+                                "key": "x-ibm-finding.dst_ip_ref",
+                                "object": "ibm_finding",
+                                "references": "nc_remote_ip"
+                            },
+                            {
+                                "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
+                                "key": "x-ibm-finding.dst_geolocation",
+                                "object": "ibm_finding"
+                            },
+                            {
+                                "ds_key": "service_action_networkconnectionaction_remoteipdetails_city_cityname",
+                                "key": "ipv4-addr.x_aws_remote_city_name",
+                                "object": "nc_remote_ip"
+                            },
+                            {
+                                "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
+                                "key": "ipv4-addr.x_aws_remote_country_name",
+                                "object": "nc_remote_ip"
+                            }
+                        ],
+                        "service_action_networkconnectionaction_remoteportdetails_port": [
+                            {
+                                "key": "network-traffic.dst_port",
+                                "object": "nc_nt",
+                                "transformer": "ToInteger"
+                            }
+                        ],
+                        "service_action_portprobeaction_portprobedetails_0_localportdetails_port": [
+                            {
+                                "key": "x-ibm-finding.probe_port",
+                                "object": "ibm_finding"
+                            }
+                        ],
+                        "service_action_portprobeaction_portprobedetails_0_remoteipdetails_ipaddressv4": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "pp_remote_ip"
+                            },
+                            {
+                                "key": "x-ibm-finding.dst_ip_ref",
+                                "object": "ibm_finding",
+                                "references": "pp_remote_ip"
+                            },
+                            {
+                                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
+                                "key": "x-ibm-finding.dst_geolocation",
+                                "object": "ibm_finding"
+                            },
+                            {
+                                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_city_cityname",
+                                "key": "ipv4-addr.x_aws_remote_city_name",
+                                "object": "pp_remote_ip"
+                            },
+                            {
+                                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
+                                "key": "ipv4-addr.x_aws_remote_country_name",
+                                "object": "pp_remote_ip"
+                            }
+                        ],
+                        "service_eventfirstseen": [
+                            {
+                                "key": "first_observed"
+                            },
+                            {
+                                "key": "x-ibm-finding.start",
+                                "object": "ibm_finding"
+                            }
+                        ],
+                        "service_eventlastseen": [
+                            {
+                                "key": "last_observed"
+                            },
+                            {
+                                "key": "x-ibm-finding.end",
+                                "object": "ibm_finding"
+                            }
+                        ],
+                        "severity": {
+                            "key": "x-ibm-finding.severity",
+                            "object": "ibm_finding"
+                        },
+                        "title": {
+                            "key": "x-ibm-finding.name",
+                            "object": "ibm_finding"
+                        },
+                        "type": {
+                            "key": "x-ibm-finding.finding_type",
+                            "object": "ibm_finding"
+                        }
+                    },
                     "hash_algorithm_map": {
                         "0": "Unknown",
                         "1": "MD5",
                         "2": "SHA-1",
                         "3": "SHA-256",
                         "4": "SHA-512",
                         "5": "CTPH",
@@ -1290,3176 +1673,2672 @@
                                 ],
                                 "uid": [
                                     "resources.uid"
                                 ]
                             }
                         }
                     },
-                    "operators": {
-                        "ComparisonComparators.Equal": "=",
-                        "ComparisonComparators.GreaterThan": ">",
-                        "ComparisonComparators.GreaterThanOrEqual": ">=",
-                        "ComparisonComparators.In": "IN",
-                        "ComparisonComparators.LessThan": "<",
-                        "ComparisonComparators.LessThanOrEqual": "<=",
-                        "ComparisonComparators.Like": "LIKE",
-                        "ComparisonComparators.Matches": "REGEXP_LIKE",
-                        "ComparisonComparators.NotEqual": "!=",
-                        "ComparisonExpressionOperators.And": "AND",
-                        "ComparisonExpressionOperators.Or": "OR",
-                        "ObservationOperators.And": "INTERSECT",
-                        "ObservationOperators.Or": "UNION"
-                    },
-                    "to_stix_map": {
-                        "guardduty": {
-                            "accountid": {
-                                "key": "x-aws-details.account_id",
-                                "object": "aws_details"
+                    "ocsf_to_stix_map": {
+                        "_time": [
+                            {
+                                "key": "first_observed",
+                                "transformer": "EpochToTimestamp"
                             },
-                            "description": {
-                                "key": "x-ibm-finding.description",
-                                "object": "ibm_finding"
+                            {
+                                "key": "last_observed",
+                                "transformer": "EpochToTimestamp"
                             },
-                            "dnsrequest_resource_instancedetails_networkinterfaces_0_privateipaddress": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "dns_private_ip1"
-                                },
-                                {
-                                    "key": "domain-name.resolves_to_refs",
-                                    "object": "private_dns_name",
-                                    "references": [
-                                        "dns_private_ip1"
-                                    ]
-                                },
-                                {
-                                    "key": "x-ibm-finding.src_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "dns_private_ip1"
-                                },
-                                {
-                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                    "key": "ipv4-addr.x_aws_interface_id",
-                                    "object": "dns_private_ip1"
+                            {
+                                "key": "x-ibm-finding.time_observed",
+                                "object": "ibm_finding",
+                                "transformer": "EpochToTimestamp"
+                            }
+                        ],
+                        "activity": {
+                            "key": "x-oca-event.action",
+                            "object": "x_oca_event"
+                        },
+                        "activity_id": {
+                            "key": "x-oca-event.code",
+                            "object": "x_oca_event",
+                            "transformer": "ToString"
+                        },
+                        "activity_name": {
+                            "key": "x-oca-event.action",
+                            "object": "x_oca_event"
+                        },
+                        "api": {
+                            "operation": {
+                                "key": "x-ocsf-cloud.operation",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "request": {
+                                "flags": {
+                                    "key": "x-ocsf-cloud.request_flags",
+                                    "object": "ocsf_cloud_api",
+                                    "transformer": "ToLowercaseArray"
                                 },
-                                {
-                                    "key": "ipv4-addr.x_aws_ip_type",
-                                    "object": "dns_private_ip1",
-                                    "value": "private"
+                                "uid": {
+                                    "key": "x-ocsf-cloud.request_uid",
+                                    "object": "ocsf_cloud_api"
                                 }
-                            ],
-                            "portprobe_resource_instancedetails_networkinterfaces_0_privateipaddress": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "pp_private_ip1"
+                            },
+                            "response": {
+                                "code": {
+                                    "key": "x-ocsf-cloud.response_code",
+                                    "object": "ocsf_cloud_api",
+                                    "transformer": "ToInteger"
                                 },
-                                {
-                                    "key": "domain-name.resolves_to_refs",
-                                    "object": "private_dns_name",
-                                    "references": [
-                                        "pp_private_ip1"
-                                    ]
+                                "error": {
+                                    "key": "x-ocsf-cloud.response_error",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                {
-                                    "key": "x-ibm-finding.src_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "pp_private_ip1"
+                                "error_message": {
+                                    "key": "x-ocsf-cloud.response_error_message",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                {
-                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                    "key": "ipv4-addr.x_aws_interface_id",
-                                    "object": "pp_private_ip1"
+                                "flags": {
+                                    "key": "x-ocsf-cloud.response_flags",
+                                    "object": "ocsf_cloud_api",
+                                    "transformer": "ToLowercaseArray"
                                 },
-                                {
-                                    "key": "ipv4-addr.x_aws_ip_type",
-                                    "object": "pp_private_ip1",
-                                    "value": "private"
+                                "message": {
+                                    "key": "x-ocsf-cloud.response_message",
+                                    "object": "ocsf_cloud_api"
                                 }
-                            ],
-                            "region": {
-                                "key": "x-aws-details.region",
-                                "object": "aws_details"
                             },
-                            "resource_accesskeydetails_accesskeyid": {
-                                "key": "x-aws-api.access_key_id",
-                                "object": "api_details"
-                            },
-                            "resource_accesskeydetails_principalid": {
-                                "key": "user-account.user_id",
-                                "object": "api_user"
-                            },
-                            "resource_accesskeydetails_username": {
-                                "key": "user-account.account_login",
-                                "object": "api_user"
-                            },
-                            "resource_instancedetails_availabilityzone": {
-                                "key": "x-aws-instance.availability_zone",
-                                "object": "instance"
-                            },
-                            "resource_instancedetails_imageid": {
-                                "key": "x-aws-instance.image_id",
-                                "object": "instance"
-                            },
-                            "resource_instancedetails_instanceid": {
-                                "key": "x-aws-instance.instance_id",
-                                "object": "instance"
-                            },
-                            "resource_instancedetails_networkinterfaces_0_ipv6addresses_0": [
-                                {
-                                    "key": "ipv6-addr.value",
-                                    "object": "nc_ipv6_ip"
-                                },
-                                {
-                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                    "key": "ipv6-addr.x_aws_interface_id",
-                                    "object": "nc_ipv6_ip"
-                                }
-                            ],
-                            "resource_instancedetails_networkinterfaces_0_privatednsname": [
-                                {
-                                    "key": "domain-name.value",
-                                    "object": "private_dns_name"
-                                }
-                            ],
-                            "resource_instancedetails_networkinterfaces_0_privateipaddress": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "nc_private_ip1"
-                                },
-                                {
-                                    "key": "network-traffic.src_ref",
-                                    "object": "nc_nt",
-                                    "references": "nc_private_ip1"
-                                },
-                                {
-                                    "key": "domain-name.resolves_to_refs",
-                                    "object": "private_dns_name",
-                                    "references": [
-                                        "nc_private_ip1"
-                                    ]
+                            "service": {
+                                "labels": {
+                                    "key": "x-ocsf-cloud.service_labels",
+                                    "object": "ocsf_cloud_api",
+                                    "transformer": "ToLowercaseArray"
                                 },
-                                {
-                                    "key": "x-ibm-finding.src_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "nc_private_ip1"
+                                "name": {
+                                    "key": "x-ocsf-cloud.service_name",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                {
-                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                    "key": "ipv4-addr.x_aws_interface_id",
-                                    "object": "nc_private_ip1"
+                                "uid": {
+                                    "key": "x-ocsf-cloud.service_uid",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                {
-                                    "key": "ipv4-addr.x_aws_ip_type",
-                                    "object": "nc_private_ip1",
-                                    "value": "private"
-                                }
-                            ],
-                            "resource_instancedetails_networkinterfaces_0_publicdnsname": [
-                                {
-                                    "key": "domain-name.value",
-                                    "object": "nc_public_name"
+                                "version": {
+                                    "key": "x-ocsf-cloud.service_uid",
+                                    "object": "ocsf_cloud_api"
                                 }
-                            ],
-                            "resource_instancedetails_networkinterfaces_0_publicip": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "nc_public_ip"
-                                },
-                                {
-                                    "key": "domain-name.resolves_to_refs",
-                                    "object": "nc_public_name",
-                                    "references": [
-                                        "nc_public_ip"
-                                    ]
-                                },
-                                {
-                                    "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                                    "key": "ipv4-addr.x_aws_interface_id",
-                                    "object": "nc_public_ip"
+                            },
+                            "version": {
+                                "key": "x-ocsf-cloud.api_version",
+                                "object": "ocsf_cloud_api"
+                            }
+                        },
+                        "attacks": {
+                            "tactics": {
+                                "name": {
+                                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_name",
+                                    "object": "ttp-tagging"
                                 },
-                                {
-                                    "key": "ipv4-addr.x_aws_ip_type",
-                                    "object": "nc_public_ip",
-                                    "value": "public"
+                                "uid": {
+                                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_id",
+                                    "object": "ttp-tagging"
                                 }
-                            ],
-                            "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupid": {
-                                "key": "x-aws-vpc.security_group_id",
-                                "object": "vpc"
-                            },
-                            "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupname": {
-                                "key": "x-aws-vpc.security_group_name",
-                                "object": "vpc"
-                            },
-                            "resource_instancedetails_networkinterfaces_0_subnetid": {
-                                "key": "x-aws-vpc.subnet_id",
-                                "object": "vpc"
-                            },
-                            "resource_instancedetails_networkinterfaces_0_vpcid": {
-                                "key": "x-aws-vpc.vpc_id",
-                                "object": "vpc"
                             },
-                            "resource_instancedetails_networkinterfaces_1_privatednsname": [
-                                {
-                                    "key": "domain-name.value",
-                                    "object": "nc_private_name2"
+                            "technique": {
+                                "name": [
+                                    {
+                                        "key": "x-ibm-ttp-tagging.name",
+                                        "object": "ttp-tagging"
+                                    },
+                                    {
+                                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_name",
+                                        "object": "ttp-tagging"
+                                    },
+                                    {
+                                        "key": "x-ibm-finding.ttp_tagging_refs",
+                                        "object": "ibm_finding",
+                                        "references": [
+                                            "ttp-tagging"
+                                        ]
+                                    }
+                                ],
+                                "uid": {
+                                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_id",
+                                    "object": "ttp-tagging"
                                 }
-                            ],
-                            "resource_instancedetails_networkinterfaces_1_privateipaddress": [
+                            },
+                            "version": {
+                                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.versoin",
+                                "object": "ttp-tagging"
+                            }
+                        },
+                        "category_name": {
+                            "key": "x-oca-event.category",
+                            "object": "x_oca_event"
+                        },
+                        "category_uid": {
+                            "key": "x-oca-event.code",
+                            "object": "x_oca_event",
+                            "transformer": "ToString"
+                        },
+                        "class_name": {
+                            "key": "x-oca-event.module",
+                            "object": "x_oca_event"
+                        },
+                        "class_uid": {
+                            "key": "x-oca-event.extensions.x-cloud-api.class_uid",
+                            "object": "x_oca_event",
+                            "transformer": "ToInteger"
+                        },
+                        "cloud": {
+                            "account_type": {
+                                "key": "x-ocsf-cloud.account_type",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "account_type_id": {
+                                "key": "x-ocsf-cloud.account_type_id",
+                                "object": "ocsf_cloud_api",
+                                "transformer": "ToInteger"
+                            },
+                            "account_uid": {
+                                "key": "x-ocsf-cloud.account_uid",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "org_uid": {
+                                "key": "x-ocsf-cloud.org_uid",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "project_uid": {
+                                "key": "x-ocsf-cloud.project_uid",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "provider": {
+                                "key": "x-ocsf-cloud.provider",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "region": {
+                                "key": "x-ocsf-cloud.region",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "resource_uid": {
+                                "key": "x-ocsf-cloud.resource_uid",
+                                "object": "ocsf_cloud_api"
+                            },
+                            "zone": {
+                                "key": "x-ocsf-cloud.zone",
+                                "object": "ocsf_cloud_api"
+                            }
+                        },
+                        "compliance": {
+                            "requirements": {
+                                "key": "x-ocsf-compliance.requirements",
+                                "object": "compliance"
+                            },
+                            "status": {
+                                "key": "x-ocsf-compliance.status",
+                                "object": "compliance"
+                            },
+                            "status_detail": {
+                                "key": "x-ocsf-compliance.status_detail",
+                                "object": "compliance"
+                            }
+                        },
+                        "confidence": {
+                            "key": "x-oca-event.confidence",
+                            "object": "x-oca-event"
+                        },
+                        "connection_info": {
+                            "boundary": {
+                                "key": "network-traffic.extensions.x-network-ext.boundary",
+                                "object": "nt"
+                            },
+                            "boundary_id": {
+                                "key": "network-traffic.extensions.x-network-ext.boundary_id",
+                                "object": "nt"
+                            },
+                            "direction": {
+                                "key": "network-traffic.extensions.x-network-ext.direction",
+                                "object": "nt"
+                            },
+                            "direction_id": {
+                                "key": "network-traffic.extensions.x-network-ext.direction_id",
+                                "object": "nt"
+                            },
+                            "protocol_name": {
+                                "key": "network-traffic.extensions.x-network-ext.protocol_name",
+                                "object": "nt"
+                            },
+                            "protocol_num": {
+                                "group": true,
+                                "key": "network-traffic.protocols",
+                                "object": "nt",
+                                "transformer": "ProtocolNumToName"
+                            },
+                            "protocol_ver": {
+                                "group": true,
+                                "key": "network-traffic.protocols",
+                                "object": "nt",
+                                "transformer": "ToLowercaseArray"
+                            },
+                            "protocol_ver_id": {
+                                "key": "network-traffic.extensions.x-network-ext.protocol_ver_id",
+                                "object": "nt"
+                            },
+                            "tcp_flags": {
+                                "key": "network-traffic.extensions.tcp-ext.src_flags_hex",
+                                "object": "nt"
+                            }
+                        },
+                        "count": [
+                            {
+                                "key": "number_observed",
+                                "transformer": "ToInteger"
+                            },
+                            {
+                                "key": "x-ibm-finding.event_count",
+                                "object": "ibm_finding",
+                                "transformer": "ToInteger"
+                            }
+                        ],
+                        "data": {
+                            "key": "x-oca-event.extensions.x-ocsf-data.data",
+                            "object": "x-oca-event"
+                        },
+                        "dst_endpoint": {
+                            "instance_uid": {
+                                "key": "x-oca-asset.extensions.x-dst-endpoint.instance_uid",
+                                "object": "asset"
+                            },
+                            "interface_uid": {
+                                "key": "x-oca-asset.extensions.x-dst-endpoint.interface_uid",
+                                "object": "asset"
+                            },
+                            "intermediate_ips": [
                                 {
                                     "key": "ipv4-addr.value",
-                                    "object": "nc_private_ip2"
+                                    "object": "dst_ipv4",
+                                    "transformer": "FilterIPv4List",
+                                    "unwrap": true
                                 },
                                 {
-                                    "key": "domain-name.resolves_to_refs",
-                                    "object": "nc_private_name2",
-                                    "references": [
-                                        "nc_private_ip2"
-                                    ]
-                                },
-                                {
-                                    "ds_key": "resource_instancedetails_networkinterfaces_1_networkinterfaceid",
-                                    "key": "ipv4-addr.x_aws_interface_id",
-                                    "object": "nc_private_ip2"
-                                },
-                                {
-                                    "key": "ipv4-addr.x_aws_ip_type",
-                                    "object": "nc_private_ip2",
-                                    "value": "private"
-                                }
-                            ],
-                            "resource_instancedetails_platform": [
-                                {
-                                    "key": "software.name",
-                                    "object": "software"
+                                    "key": "ipv6-addr.value",
+                                    "object": "dst_ipv6",
+                                    "transformer": "FilterIPv6List",
+                                    "unwrap": true
                                 },
                                 {
-                                    "key": "x-ibm-finding.src_os_ref",
-                                    "object": "ibm_finding",
-                                    "references": "software"
+                                    "key": "x-oca-asset.ip_refs",
+                                    "object": "asset",
+                                    "references": [
+                                        "dst_ipv4",
+                                        "dst_ipv6"
+                                    ],
+                                    "unwrap": true
                                 }
                             ],
-                            "service_action_awsapicallaction_api": {
-                                "key": "x-aws-api.api",
-                                "object": "api_details"
-                            },
-                            "service_action_awsapicallaction_remoteipdetails_ipaddressv4": [
+                            "ip": [
                                 {
                                     "key": "ipv4-addr.value",
-                                    "object": "api_remote_ip"
-                                },
-                                {
-                                    "key": "x-ibm-finding.dst_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "api_remote_ip"
-                                },
-                                {
-                                    "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
-                                    "key": "x-ibm-finding.dst_geolocation",
-                                    "object": "ibm_finding"
+                                    "object": "dst_ip",
+                                    "transformer": "CheckIPv4"
                                 },
                                 {
-                                    "ds_key": "service_action_awsapicallaction_remoteipdetails_city_cityname",
-                                    "key": "ipv4-addr.x_aws_remote_city_name",
-                                    "object": "api_remote_ip"
-                                },
-                                {
-                                    "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
-                                    "key": "ipv4-addr.x_aws_remote_country_name",
-                                    "object": "api_remote_ip"
-                                }
-                            ],
-                            "service_action_awsapicallaction_servicename": {
-                                "key": "x-aws-api.service_name",
-                                "object": "api_details"
-                            },
-                            "service_action_dnsrequestaction_domain": [
-                                {
-                                    "key": "domain-name.value",
-                                    "object": "dns_domain_name"
-                                }
-                            ],
-                            "service_action_networkconnectionaction_localportdetails_port": [
-                                {
-                                    "key": "network-traffic.src_port",
-                                    "object": "nc_nt",
-                                    "transformer": "ToInteger"
-                                }
-                            ],
-                            "service_action_networkconnectionaction_protocol": [
-                                {
-                                    "key": "network-traffic.protocols",
-                                    "object": "nc_nt",
-                                    "transformer": "ToLowercaseArray"
-                                }
-                            ],
-                            "service_action_networkconnectionaction_remoteipdetails_ipaddressv4": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "nc_remote_ip"
+                                    "key": "ipv6-addr.value",
+                                    "object": "dst_ip",
+                                    "transformer": "CheckIPv6"
                                 },
                                 {
                                     "key": "network-traffic.dst_ref",
-                                    "object": "nc_nt",
-                                    "references": "nc_remote_ip"
+                                    "object": "nt",
+                                    "references": "dst_ip"
                                 },
                                 {
                                     "key": "x-ibm-finding.dst_ip_ref",
                                     "object": "ibm_finding",
-                                    "references": "nc_remote_ip"
-                                },
-                                {
-                                    "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
-                                    "key": "x-ibm-finding.dst_geolocation",
-                                    "object": "ibm_finding"
+                                    "references": "dst_ip"
                                 },
                                 {
-                                    "ds_key": "service_action_networkconnectionaction_remoteipdetails_city_cityname",
-                                    "key": "ipv4-addr.x_aws_remote_city_name",
-                                    "object": "nc_remote_ip"
+                                    "group": true,
+                                    "key": "x-oca-asset.ip_refs",
+                                    "object": "host",
+                                    "references": [
+                                        "dst_ip"
+                                    ]
                                 },
                                 {
-                                    "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
-                                    "key": "ipv4-addr.x_aws_remote_country_name",
-                                    "object": "nc_remote_ip"
-                                }
-                            ],
-                            "service_action_networkconnectionaction_remoteportdetails_port": [
-                                {
-                                    "key": "network-traffic.dst_port",
-                                    "object": "nc_nt",
-                                    "transformer": "ToInteger"
+                                    "key": "x-oca-event.network_ref",
+                                    "object": "event",
+                                    "references": "nt"
                                 }
                             ],
-                            "service_action_portprobeaction_portprobedetails_0_localportdetails_port": [
-                                {
-                                    "key": "x-ibm-finding.probe_port",
+                            "name": {
+                                "key": "x-oca-asset.name",
+                                "object": "asset"
+                            },
+                            "port": {
+                                "key": "network-traffic.dst_port",
+                                "object": "nt",
+                                "transformer": "ToInteger"
+                            },
+                            "subnet_uid": {
+                                "key": "x-oca-asset.extensions.x-dst-endpoint.subnet_uid",
+                                "object": "asset"
+                            },
+                            "svc_name": {
+                                "key": "x-oca-asset.extensions.x-dst-endpoint.svc_name",
+                                "object": "asset"
+                            },
+                            "vpc_uid": {
+                                "key": "x-oca-asset.extensions.x-dst-endpoint.vpc_uid",
+                                "object": "asset"
+                            }
+                        },
+                        "duration": {
+                            "key": "x-oca-event.duration",
+                            "object": "x_oca_event",
+                            "transformer": "ToInteger"
+                        },
+                        "end_time": [
+                            {
+                                "key": "x-ibm-finding.end",
+                                "object": "ibm_finding",
+                                "transformer": "EpochToTimestamp"
+                            },
+                            {
+                                "key": "last_observed",
+                                "transformer": "EpochToTimestamp"
+                            }
+                        ],
+                        "enrichments": {
+                            "data": {
+                                "key": "x-ocsf-enrichments.data",
+                                "object": "enrichments"
+                            },
+                            "name": {
+                                "key": "x-ocsf-enrichments.name",
+                                "object": "enrichments"
+                            },
+                            "provider": {
+                                "key": "x-ocsf-enrichments.provider",
+                                "object": "enrichments"
+                            },
+                            "type": {
+                                "key": "x-ocsf-enrichments.type",
+                                "object": "enrichments"
+                            },
+                            "value": {
+                                "key": "x-ocsf-enrichments.value",
+                                "object": "enrichments"
+                            }
+                        },
+                        "finding": {
+                            "created_time": {
+                                "key": "x-ibm-finding.start",
+                                "object": "ibm_finding"
+                            },
+                            "desc": {
+                                "key": "x-ibm-finding.description",
+                                "object": "ibm_finding"
+                            },
+                            "first_seen_time": {
+                                "key": "x-ibm-finding.time_observed",
+                                "object": "ibm_finding"
+                            },
+                            "last_seen_time": {
+                                "key": "x-ibm-finding.extensions.x-ocsf-findings.last_seen_time",
+                                "object": "ibm_finding"
+                            },
+                            "modified_time": {
+                                "key": "x-ibm-finding.extensions.x-ocsf-findings.modified_time",
+                                "object": "ibm_finding"
+                            },
+                            "product_uid": {
+                                "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
+                                "object": "ibm_finding"
+                            },
+                            "related_events": {
+                                "product_uid": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
                                     "object": "ibm_finding"
-                                }
-                            ],
-                            "service_action_portprobeaction_portprobedetails_0_remoteipdetails_ipaddressv4": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "pp_remote_ip"
                                 },
-                                {
-                                    "key": "x-ibm-finding.dst_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "pp_remote_ip"
-                                },
-                                {
-                                    "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
-                                    "key": "x-ibm-finding.dst_geolocation",
+                                "type": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.type",
                                     "object": "ibm_finding"
                                 },
-                                {
-                                    "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_city_cityname",
-                                    "key": "ipv4-addr.x_aws_remote_city_name",
-                                    "object": "pp_remote_ip"
-                                },
-                                {
-                                    "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
-                                    "key": "ipv4-addr.x_aws_remote_country_name",
-                                    "object": "pp_remote_ip"
-                                }
-                            ],
-                            "service_eventfirstseen": [
-                                {
-                                    "key": "first_observed"
+                                "type_uid": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.type_uid",
+                                    "object": "ibm_finding"
                                 },
-                                {
-                                    "key": "x-ibm-finding.start",
+                                "uid": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.uid",
                                     "object": "ibm_finding"
                                 }
-                            ],
-                            "service_eventlastseen": [
-                                {
-                                    "key": "last_observed"
+                            },
+                            "remediation": {
+                                "desc": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_desc",
+                                    "object": "ibm_finding"
                                 },
-                                {
-                                    "key": "x-ibm-finding.end",
+                                "kb_articles": {
+                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_kb_articles",
                                     "object": "ibm_finding"
                                 }
-                            ],
-                            "severity": {
-                                "key": "x-ibm-finding.severity",
+                            },
+                            "src_url": {
+                                "key": "x-ibm-finding.extensions.x-ocsf-findings.src_url",
+                                "object": "ibm_finding"
+                            },
+                            "supporting_data": {
+                                "key": "x-ibm-finding.extensions.x-ocsf-findings.upporting_data",
                                 "object": "ibm_finding"
                             },
                             "title": {
                                 "key": "x-ibm-finding.name",
                                 "object": "ibm_finding"
                             },
-                            "type": {
-                                "key": "x-ibm-finding.finding_type",
+                            "types": {
+                                "key": "x-ibm-finding.types",
+                                "object": "ibm_finding"
+                            },
+                            "uid": {
+                                "key": "x-ibm-finding.alert_id",
                                 "object": "ibm_finding"
                             }
                         },
-                        "ocsf": {
-                            "_time": [
-                                {
-                                    "key": "first_observed",
-                                    "transformer": "EpochToTimestamp"
-                                },
-                                {
-                                    "key": "last_observed",
-                                    "transformer": "EpochToTimestamp"
+                        "http_request": {
+                            "args": {
+                                "key": "x-ocsf-http-request.value",
+                                "object": "http_request"
+                            },
+                            "http_headers": {
+                                "name": {
+                                    "key": "x-ocsf-http-request.http_headers_name",
+                                    "object": "ocsf_cloud_api"
                                 },
-                                {
-                                    "key": "x-ibm-finding.time_observed",
-                                    "object": "ibm_finding",
-                                    "transformer": "EpochToTimestamp"
+                                "value": {
+                                    "key": "x-ocsf-http-request.http_headers_value",
+                                    "object": "http_request"
                                 }
-                            ],
-                            "activity": {
-                                "key": "x-oca-event.action",
-                                "object": "x_oca_event"
-                            },
-                            "activity_id": {
-                                "key": "x-oca-event.code",
-                                "object": "x_oca_event",
-                                "transformer": "ToString"
-                            },
-                            "activity_name": {
-                                "key": "x-oca-event.action",
-                                "object": "x_oca_event"
-                            },
-                            "api": {
-                                "operation": {
-                                    "key": "x-ocsf-cloud.operation",
-                                    "object": "ocsf_cloud_api"
+                            },
+                            "http_method": {
+                                "key": "x-ocsf-http-request.http_method",
+                                "object": "http_request"
+                            },
+                            "prefix": {
+                                "key": "x-ocsf-http-request.prefix",
+                                "object": "http_request"
+                            },
+                            "referrer": {
+                                "key": "x-ocsf-http-request.referrer",
+                                "object": "http_request"
+                            },
+                            "uid": {
+                                "key": "x-ocsf-http-request.uid",
+                                "object": "http_request"
+                            },
+                            "url": {
+                                "key": "url.value",
+                                "object": "url"
+                            },
+                            "user_agent": {
+                                "key": "x-ocsf-http-request.user_agent",
+                                "object": "http_request"
+                            },
+                            "version": {
+                                "key": "x-ocsf-http-request.version",
+                                "object": "http_request"
+                            },
+                            "x_forwarded_for": {
+                                "key": "x-ocsf-http-request.x_forwarded_for",
+                                "object": "http_request"
+                            }
+                        },
+                        "identity": {
+                            "authorizations": {
+                                "decision": {
+                                    "key": "x-ocsf-identity.authorizations.decision",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "request": {
-                                    "flags": {
-                                        "key": "x-ocsf-cloud.request_flags",
-                                        "object": "ocsf_cloud_api",
-                                        "transformer": "ToLowercaseArray"
+                                "policy": {
+                                    "desc": {
+                                        "key": "x-ocsf-identity.authorizations.policy_desc",
+                                        "object": "x-ocsf-identity"
                                     },
-                                    "uid": {
-                                        "key": "x-ocsf-cloud.request_uid",
-                                        "object": "ocsf_cloud_api"
-                                    }
-                                },
-                                "response": {
-                                    "code": {
-                                        "key": "x-ocsf-cloud.response_code",
-                                        "object": "ocsf_cloud_api",
-                                        "transformer": "ToInteger"
-                                    },
-                                    "error": {
-                                        "key": "x-ocsf-cloud.response_error",
-                                        "object": "ocsf_cloud_api"
-                                    },
-                                    "error_message": {
-                                        "key": "x-ocsf-cloud.response_error_message",
-                                        "object": "ocsf_cloud_api"
-                                    },
-                                    "flags": {
-                                        "key": "x-ocsf-cloud.response_flags",
-                                        "object": "ocsf_cloud_api",
-                                        "transformer": "ToLowercaseArray"
-                                    },
-                                    "message": {
-                                        "key": "x-ocsf-cloud.response_message",
-                                        "object": "ocsf_cloud_api"
-                                    }
-                                },
-                                "service": {
-                                    "labels": {
-                                        "key": "x-ocsf-cloud.service_labels",
-                                        "object": "ocsf_cloud_api",
-                                        "transformer": "ToLowercaseArray"
+                                    "group": {
+                                        "desc": {
+                                            "key": "x-ocsf-identity.authorizations.policy_group_desc",
+                                            "object": "x-ocsf-identity"
+                                        },
+                                        "name": {
+                                            "key": "x-ocsf-identity.authorizations.policy_group_namee",
+                                            "object": "x-ocsf-identity"
+                                        },
+                                        "privileges": {
+                                            "key": "x-ocsf-identity.authorizations.policy_group_privileges",
+                                            "object": "x-ocsf-identity"
+                                        },
+                                        "type": {
+                                            "key": "x-ocsf-identity.authorizations.policy_group_type",
+                                            "object": "x-ocsf-identity"
+                                        },
+                                        "uid": {
+                                            "key": "x-ocsf-identity.authorizations.policy_group_uid",
+                                            "object": "x-ocsf-identity"
+                                        }
                                     },
                                     "name": {
-                                        "key": "x-ocsf-cloud.service_name",
-                                        "object": "ocsf_cloud_api"
+                                        "key": "x-ocsf-identity.authorizations.name",
+                                        "object": "x-ocsf-identity"
                                     },
                                     "uid": {
-                                        "key": "x-ocsf-cloud.service_uid",
-                                        "object": "ocsf_cloud_api"
+                                        "key": "x-ocsf-identity.authorizations.uid",
+                                        "object": "x-ocsf-identity"
                                     },
                                     "version": {
-                                        "key": "x-ocsf-cloud.service_uid",
-                                        "object": "ocsf_cloud_api"
+                                        "key": "x-ocsf-identity.authorizations.version",
+                                        "object": "x-ocsf-identity"
                                     }
-                                },
-                                "version": {
-                                    "key": "x-ocsf-cloud.api_version",
-                                    "object": "ocsf_cloud_api"
                                 }
                             },
-                            "attacks": {
-                                "tactics": {
-                                    "name": {
-                                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_name",
-                                        "object": "ttp-tagging"
-                                    },
-                                    "uid": {
-                                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_id",
-                                        "object": "ttp-tagging"
-                                    }
-                                },
-                                "technique": {
-                                    "name": [
-                                        {
-                                            "key": "x-ibm-ttp-tagging.name",
-                                            "object": "ttp-tagging"
-                                        },
-                                        {
-                                            "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_name",
-                                            "object": "ttp-tagging"
-                                        },
-                                        {
-                                            "key": "x-ibm-finding.ttp_tagging_refs",
-                                            "object": "ibm_finding",
-                                            "references": [
-                                                "ttp-tagging"
-                                            ]
-                                        }
-                                    ],
-                                    "uid": {
-                                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_id",
-                                        "object": "ttp-tagging"
-                                    }
+                            "idp": {
+                                "name": {
+                                    "key": "x-ocsf-identity.idp.name",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "version": {
-                                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.versoin",
-                                    "object": "ttp-tagging"
+                                "uid": {
+                                    "key": "x-ocsf-identity.idp.uid",
+                                    "object": "x-ocsf-identity"
                                 }
                             },
-                            "category_name": {
-                                "key": "x-oca-event.category",
-                                "object": "x_oca_event"
-                            },
-                            "category_uid": {
-                                "key": "x-oca-event.code",
-                                "object": "x_oca_event",
-                                "transformer": "ToString"
-                            },
-                            "class_name": {
-                                "key": "x-oca-event.module",
-                                "object": "x_oca_event"
-                            },
-                            "class_uid": {
-                                "key": "x-oca-event.extensions.x-cloud-api.class_uid",
-                                "object": "x_oca_event",
-                                "transformer": "ToInteger"
+                            "invoked_by": {
+                                "key": "x-ocsf-identity.invoked_by",
+                                "object": "x-ocsf-identity"
                             },
-                            "cloud": {
-                                "account_type": {
-                                    "key": "x-ocsf-cloud.account_type",
-                                    "object": "ocsf_cloud_api"
-                                },
-                                "account_type_id": {
-                                    "key": "x-ocsf-cloud.account_type_id",
-                                    "object": "ocsf_cloud_api",
-                                    "transformer": "ToInteger"
-                                },
-                                "account_uid": {
-                                    "key": "x-ocsf-cloud.account_uid",
-                                    "object": "ocsf_cloud_api"
-                                },
-                                "org_uid": {
-                                    "key": "x-ocsf-cloud.org_uid",
-                                    "object": "ocsf_cloud_api"
+                            "message": {
+                                "key": "x-ocsf-identity.message",
+                                "object": "x-ocsf-identity"
+                            },
+                            "session": {
+                                "created_time": {
+                                    "key": "x-ocsf-identity.session.created_time",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "project_uid": {
-                                    "key": "x-ocsf-cloud.project_uid",
-                                    "object": "ocsf_cloud_api"
+                                "credential_uid": {
+                                    "key": "x-ocsf-identity.session.credential_uid",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "provider": {
-                                    "key": "x-ocsf-cloud.provider",
-                                    "object": "ocsf_cloud_api"
+                                "expiration_time": {
+                                    "key": "x-ocsf-identity.session.expiration_time",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "region": {
-                                    "key": "x-ocsf-cloud.region",
-                                    "object": "ocsf_cloud_api"
+                                "issuer": {
+                                    "key": "x-ocsf-identity.session.issuer",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "resource_uid": {
-                                    "key": "x-ocsf-cloud.resource_uid",
-                                    "object": "ocsf_cloud_api"
+                                "mfa": {
+                                    "key": "x-ocsf-identity.session.mfa",
+                                    "object": "x-ocsf-identity"
                                 },
-                                "zone": {
-                                    "key": "x-ocsf-cloud.zone",
-                                    "object": "ocsf_cloud_api"
-                                }
-                            },
-                            "compliance": {
-                                "requirements": {
-                                    "key": "x-ocsf-compliance.requirements",
-                                    "object": "compliance"
-                                },
-                                "status": {
-                                    "key": "x-ocsf-compliance.status",
-                                    "object": "compliance"
-                                },
-                                "status_detail": {
-                                    "key": "x-ocsf-compliance.status_detail",
-                                    "object": "compliance"
+                                "uid": {
+                                    "key": "x-ocsf-identity.session.uid",
+                                    "object": "x-ocsf-identity"
                                 }
                             },
-                            "confidence": {
-                                "key": "x-oca-event.confidence",
-                                "object": "x-oca-event"
-                            },
-                            "connection_info": {
-                                "boundary": {
-                                    "key": "network-traffic.extensions.x-network-ext.boundary",
-                                    "object": "nt"
-                                },
-                                "boundary_id": {
-                                    "key": "network-traffic.extensions.x-network-ext.boundary_id",
-                                    "object": "nt"
-                                },
-                                "direction": {
-                                    "key": "network-traffic.extensions.x-network-ext.direction",
-                                    "object": "nt"
-                                },
-                                "direction_id": {
-                                    "key": "network-traffic.extensions.x-network-ext.direction_id",
-                                    "object": "nt"
-                                },
-                                "protocol_name": {
-                                    "key": "network-traffic.extensions.x-network-ext.protocol_name",
-                                    "object": "nt"
-                                },
-                                "protocol_num": {
-                                    "group": true,
-                                    "key": "network-traffic.protocols",
-                                    "object": "nt",
-                                    "transformer": "ProtocolNumToName"
-                                },
-                                "protocol_ver": {
-                                    "group": true,
-                                    "key": "network-traffic.protocols",
-                                    "object": "nt",
-                                    "transformer": "ToLowercaseArray"
+                            "user": {
+                                "account_type": {
+                                    "key": "user-account.account_type",
+                                    "object": "user"
                                 },
-                                "protocol_ver_id": {
-                                    "key": "network-traffic.extensions.x-network-ext.protocol_ver_id",
-                                    "object": "nt"
-                                },
-                                "tcp_flags": {
-                                    "key": "network-traffic.extensions.tcp-ext.src_flags_hex",
-                                    "object": "nt"
-                                }
-                            },
-                            "count": [
-                                {
-                                    "key": "number_observed",
+                                "account_type_id": {
+                                    "key": "user-account.extensions.aws-account-ext.account_type_id",
+                                    "object": "user",
                                     "transformer": "ToInteger"
                                 },
-                                {
-                                    "key": "x-ibm-finding.event_count",
-                                    "object": "ibm_finding",
-                                    "transformer": "ToInteger"
-                                }
-                            ],
-                            "data": {
-                                "key": "x-oca-event.extensions.x-ocsf-data.data",
-                                "object": "x-oca-event"
-                            },
-                            "dst_endpoint": {
-                                "instance_uid": {
-                                    "key": "x-oca-asset.extensions.x-dst-endpoint.instance_uid",
-                                    "object": "asset"
-                                },
-                                "interface_uid": {
-                                    "key": "x-oca-asset.extensions.x-dst-endpoint.interface_uid",
-                                    "object": "asset"
+                                "account_uid": {
+                                    "key": "user-account.user_id",
+                                    "object": "user"
                                 },
-                                "intermediate_ips": [
-                                    {
-                                        "key": "ipv4-addr.value",
-                                        "object": "dst_ipv4",
-                                        "transformer": "FilterIPv4List",
-                                        "unwrap": true
-                                    },
-                                    {
-                                        "key": "ipv6-addr.value",
-                                        "object": "dst_ipv6",
-                                        "transformer": "FilterIPv6List",
-                                        "unwrap": true
-                                    },
-                                    {
-                                        "key": "x-oca-asset.ip_refs",
-                                        "object": "asset",
-                                        "references": [
-                                            "dst_ipv4",
-                                            "dst_ipv6"
-                                        ],
-                                        "unwrap": true
-                                    }
-                                ],
-                                "ip": [
-                                    {
-                                        "key": "ipv4-addr.value",
-                                        "object": "dst_ip",
-                                        "transformer": "CheckIPv4"
-                                    },
-                                    {
-                                        "key": "ipv6-addr.value",
-                                        "object": "dst_ip",
-                                        "transformer": "CheckIPv6"
+                                "credential_uid": {
+                                    "key": "user-account.extensions.aws-account-ext.credential_uid",
+                                    "object": "user"
+                                },
+                                "domain": {
+                                    "key": "user-account.extensions.aws-account-ext.domain",
+                                    "object": "user"
+                                },
+                                "email_addr": {
+                                    "key": "email-addr.value",
+                                    "object": "email_addr"
+                                },
+                                "groups": {
+                                    "desc": {
+                                        "key": "user-account.extensions.aws-account-ext.group_desc",
+                                        "object": "user"
                                     },
-                                    {
-                                        "key": "network-traffic.dst_ref",
-                                        "object": "nt",
-                                        "references": "dst_ip"
+                                    "name": {
+                                        "key": "user-account.extensions.aws-account-ext.group_name",
+                                        "object": "user"
                                     },
-                                    {
-                                        "key": "x-ibm-finding.dst_ip_ref",
-                                        "object": "ibm_finding",
-                                        "references": "dst_ip"
+                                    "privileges": {
+                                        "key": "user-account.extensions.aws-account-ext.group_privileges",
+                                        "object": "user"
                                     },
-                                    {
-                                        "group": true,
-                                        "key": "x-oca-asset.ip_refs",
-                                        "object": "host",
-                                        "references": [
-                                            "dst_ip"
-                                        ]
+                                    "type": {
+                                        "key": "user-account.extensions.aws-account-ext.group_type",
+                                        "object": "user"
                                     },
-                                    {
-                                        "key": "x-oca-event.network_ref",
-                                        "object": "event",
-                                        "references": "nt"
+                                    "uid": {
+                                        "key": "user-account.extensions.aws-account-ext.group_uid",
+                                        "object": "user"
                                     }
-                                ],
-                                "name": {
-                                    "key": "x-oca-asset.name",
-                                    "object": "asset"
                                 },
-                                "port": {
-                                    "key": "network-traffic.dst_port",
-                                    "object": "nt",
-                                    "transformer": "ToInteger"
+                                "name": {
+                                    "key": "user-account.display_name",
+                                    "object": "user"
                                 },
-                                "subnet_uid": {
-                                    "key": "x-oca-asset.extensions.x-dst-endpoint.subnet_uid",
-                                    "object": "asset"
-                                },
-                                "svc_name": {
-                                    "key": "x-oca-asset.extensions.x-dst-endpoint.svc_name",
-                                    "object": "asset"
-                                },
-                                "vpc_uid": {
-                                    "key": "x-oca-asset.extensions.x-dst-endpoint.vpc_uid",
-                                    "object": "asset"
-                                }
-                            },
-                            "duration": {
-                                "key": "x-oca-event.duration",
-                                "object": "x_oca_event",
-                                "transformer": "ToInteger"
-                            },
-                            "end_time": [
-                                {
-                                    "key": "x-ibm-finding.end",
-                                    "object": "ibm_finding",
-                                    "transformer": "EpochToTimestamp"
+                                "org_uid": {
+                                    "key": "user-account.extensions.aws-account-ext.org_uid",
+                                    "object": "user"
                                 },
-                                {
-                                    "key": "last_observed",
-                                    "transformer": "EpochToTimestamp"
-                                }
-                            ],
-                            "enrichments": {
-                                "data": {
-                                    "key": "x-ocsf-enrichments.data",
-                                    "object": "enrichments"
+                                "session_uid": {
+                                    "key": "user-account.extensions.aws-account-ext.session_uid",
+                                    "object": "user"
+                                },
+                                "session_uuid": {
+                                    "key": "user-account.extensions.aws-account-ext.session_uuid",
+                                    "object": "user"
                                 },
-                                "name": {
-                                    "key": "x-ocsf-enrichments.name",
-                                    "object": "enrichments"
+                                "type": {
+                                    "key": "user-account.extensions.aws-account-ext.type",
+                                    "object": "user"
                                 },
-                                "provider": {
-                                    "key": "x-ocsf-enrichments.provider",
-                                    "object": "enrichments"
+                                "type_id": {
+                                    "key": "user-account.extensions.aws-account-ext.type_id",
+                                    "object": "user",
+                                    "transformer": "ToInteger"
                                 },
-                                "type": {
-                                    "key": "x-ocsf-enrichments.type",
-                                    "object": "enrichments"
+                                "uid": {
+                                    "key": "user-account.extensions.aws-account-ext.uid",
+                                    "object": "user"
                                 },
-                                "value": {
-                                    "key": "x-ocsf-enrichments.value",
-                                    "object": "enrichments"
+                                "uuid": {
+                                    "key": "user-account.extensions.aws-account-ext.uuid",
+                                    "object": "user"
                                 }
+                            }
+                        },
+                        "malware": {
+                            "classification_ids": {
+                                "key": "x-ocsf-malware.classification_ids",
+                                "object": "malware"
+                            },
+                            "classifications": {
+                                "key": "x-ocsf-malware.classifications",
+                                "object": "malware"
                             },
-                            "finding": {
+                            "cves": {
                                 "created_time": {
-                                    "key": "x-ibm-finding.start",
-                                    "object": "ibm_finding"
+                                    "key": "x-ocsf-malware.created_time",
+                                    "object": "malware"
                                 },
-                                "desc": {
-                                    "key": "x-ibm-finding.description",
-                                    "object": "ibm_finding"
+                                "cvss": {
+                                    "base_score": {
+                                        "key": "x-ocsf-malware.base_score",
+                                        "object": "malware"
+                                    },
+                                    "depth": {
+                                        "key": "x-ocsf-malware.depth",
+                                        "object": "malware"
+                                    },
+                                    "metrics": {
+                                        "name": {
+                                            "key": "x-ocsf-malware.name",
+                                            "object": "malware"
+                                        },
+                                        "value": {
+                                            "key": "x-ocsf-malware.value",
+                                            "object": "malware"
+                                        }
+                                    },
+                                    "overall_score": {
+                                        "key": "x-ocsf-malware.overall_score",
+                                        "object": "malware"
+                                    },
+                                    "severity": {
+                                        "key": "x-ocsf-malware.severity",
+                                        "object": "malware"
+                                    },
+                                    "vector_string": {
+                                        "key": "x-ocsf-malware.vector_string",
+                                        "object": "malware"
+                                    },
+                                    "version": {
+                                        "key": "x-ocsf-malware.version",
+                                        "object": "malware"
+                                    }
                                 },
-                                "first_seen_time": {
-                                    "key": "x-ibm-finding.time_observed",
-                                    "object": "ibm_finding"
+                                "cwe_uid": {
+                                    "key": "x-ocsf-malware.cwe_uid",
+                                    "object": "malware"
                                 },
-                                "last_seen_time": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.last_seen_time",
-                                    "object": "ibm_finding"
+                                "cwe_url": {
+                                    "key": "x-ocsf-malware.cwe_url",
+                                    "object": "malware"
                                 },
                                 "modified_time": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.modified_time",
-                                    "object": "ibm_finding"
-                                },
-                                "product_uid": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
-                                    "object": "ibm_finding"
+                                    "key": "x-ocsf-malware.modified_time",
+                                    "object": "malware"
                                 },
-                                "related_events": {
-                                    "product_uid": {
-                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
-                                        "object": "ibm_finding"
+                                "product": {
+                                    "feature": {
+                                        "name": {
+                                            "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                                            "object": "malware-software"
+                                        },
+                                        "uid": {
+                                            "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                                            "object": "malware-software"
+                                        },
+                                        "version": {
+                                            "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                                            "object": "malware-software"
+                                        }
                                     },
-                                    "type": {
-                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.type",
-                                        "object": "ibm_finding"
+                                    "lang": {
+                                        "key": "software.languages",
+                                        "object": "malware-software"
                                     },
-                                    "type_uid": {
-                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.type_uid",
-                                        "object": "ibm_finding"
+                                    "name": {
+                                        "key": "software.name",
+                                        "object": "malware-software"
+                                    },
+                                    "path": {
+                                        "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                                        "object": "malware-software"
                                     },
                                     "uid": {
-                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.uid",
-                                        "object": "ibm_finding"
-                                    }
-                                },
-                                "remediation": {
-                                    "desc": {
-                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_desc",
-                                        "object": "ibm_finding"
+                                        "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                                        "object": "malware-software"
+                                    },
+                                    "vendor_name": {
+                                        "key": "software.vendor",
+                                        "object": "malware-software"
                                     },
-                                    "kb_articles": {
-                                        "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_kb_articles",
-                                        "object": "ibm_finding"
+                                    "version": {
+                                        "key": "software.version",
+                                        "object": "malware-software"
                                     }
                                 },
-                                "src_url": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.src_url",
-                                    "object": "ibm_finding"
-                                },
-                                "supporting_data": {
-                                    "key": "x-ibm-finding.extensions.x-ocsf-findings.upporting_data",
-                                    "object": "ibm_finding"
-                                },
-                                "title": {
-                                    "key": "x-ibm-finding.name",
-                                    "object": "ibm_finding"
-                                },
-                                "types": {
-                                    "key": "x-ibm-finding.types",
-                                    "object": "ibm_finding"
+                                "type": {
+                                    "key": "x-ocsf-malware.type",
+                                    "object": "malware"
                                 },
                                 "uid": {
-                                    "key": "x-ibm-finding.alert_id",
-                                    "object": "ibm_finding"
+                                    "key": "x-ocsf-malware.uid",
+                                    "object": "malware"
                                 }
                             },
-                            "http_request": {
-                                "args": {
-                                    "key": "x-ocsf-http-request.value",
-                                    "object": "http_request"
-                                },
-                                "http_headers": {
+                            "name": {
+                                "key": "x-ocsf-malware.name",
+                                "object": "malware"
+                            },
+                            "path": {
+                                "key": "x-ocsf-malware.path",
+                                "object": "malware"
+                            },
+                            "provider": {
+                                "key": "x-ocsf-malware.provider",
+                                "object": "malware"
+                            },
+                            "uid": {
+                                "key": "x-ocsf-malware.uid",
+                                "object": "malware"
+                            }
+                        },
+                        "message": {
+                            "key": "x-ocsf-cloud.message",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "metadata": {
+                            "correlation_uid": {
+                                "key": "x-ocsf-metadata.correlation_uid",
+                                "object": "metadata"
+                            },
+                            "labels": {
+                                "key": "x-ocsf-metadata.labels",
+                                "object": "metadata"
+                            },
+                            "logged_time": {
+                                "key": "x-ocsf-metadata.logged_time",
+                                "object": "metadata"
+                            },
+                            "modified_time": {
+                                "key": "x-ocsf-metadata.modified_time",
+                                "object": "metadata"
+                            },
+                            "processed_time": {
+                                "key": "x-ocsf-metadata.processed_time",
+                                "object": "metadata"
+                            },
+                            "product": {
+                                "feature": {
                                     "name": {
-                                        "key": "x-ocsf-http-request.http_headers_name",
-                                        "object": "ocsf_cloud_api"
+                                        "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                                        "object": "metadata-software"
+                                    },
+                                    "uid": {
+                                        "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                                        "object": "metadata-software"
                                     },
-                                    "value": {
-                                        "key": "x-ocsf-http-request.http_headers_value",
-                                        "object": "http_request"
+                                    "version": {
+                                        "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                                        "object": "metadata-software"
                                     }
                                 },
-                                "http_method": {
-                                    "key": "x-ocsf-http-request.http_method",
-                                    "object": "http_request"
+                                "lang": {
+                                    "key": "software.languages",
+                                    "object": "metadata-software"
                                 },
-                                "prefix": {
-                                    "key": "x-ocsf-http-request.prefix",
-                                    "object": "http_request"
+                                "name": {
+                                    "key": "software.name",
+                                    "object": "metadata-software"
                                 },
-                                "referrer": {
-                                    "key": "x-ocsf-http-request.referrer",
-                                    "object": "http_request"
+                                "path": {
+                                    "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                                    "object": "metadata-software"
                                 },
                                 "uid": {
-                                    "key": "x-ocsf-http-request.uid",
-                                    "object": "http_request"
-                                },
-                                "url": {
-                                    "key": "url.value",
-                                    "object": "url"
+                                    "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                                    "object": "metadata-software"
                                 },
-                                "user_agent": {
-                                    "key": "x-ocsf-http-request.user_agent",
-                                    "object": "http_request"
+                                "vendor_name": {
+                                    "key": "software.vendor",
+                                    "object": "metadata-software"
                                 },
                                 "version": {
-                                    "key": "x-ocsf-http-request.version",
-                                    "object": "http_request"
+                                    "key": "software.version",
+                                    "object": "metadata-software"
+                                }
+                            },
+                            "sequence": {
+                                "key": "x-ocsf-metadata.sequence",
+                                "object": "metadata",
+                                "transformer": "ToInteger"
+                            },
+                            "uid": {
+                                "key": "x-ocsf-metadata.uid",
+                                "object": "metadata"
+                            },
+                            "version": {
+                                "key": "x-ocsf-metadata.version",
+                                "object": "metadata"
+                            }
+                        },
+                        "observables": {
+                            "name": [
+                                {
+                                    "key": "x-ibm-observables.name",
+                                    "object": "observables"
                                 },
-                                "x_forwarded_for": {
-                                    "key": "x-ocsf-http-request.x_forwarded_for",
-                                    "object": "http_request"
+                                {
+                                    "key": "x-ibm-finding.ioc_refs",
+                                    "object": "ibm_finding",
+                                    "references": [
+                                        "observables"
+                                    ]
                                 }
+                            ],
+                            "type": {
+                                "key": "x-ibm-observables.finding_type",
+                                "object": "observables"
                             },
-                            "identity": {
-                                "authorizations": {
-                                    "decision": {
-                                        "key": "x-ocsf-identity.authorizations.decision",
-                                        "object": "x-ocsf-identity"
+                            "type_id": {
+                                "key": "x-ibm-observables.alert_id",
+                                "object": "observables",
+                                "transformer": "ToInteger"
+                            },
+                            "value": {
+                                "key": "x-ibm-observables.description",
+                                "object": "observables"
+                            }
+                        },
+                        "process": {
+                            "cmd_line": {
+                                "key": "process.command_line",
+                                "object": "process"
+                            },
+                            "created_time": {
+                                "key": "process.created",
+                                "object": "process"
+                            },
+                            "file": {
+                                "accessed_time": {
+                                    "key": "file.accessed",
+                                    "object": "file"
+                                },
+                                "accessor": {
+                                    "account_type": {
+                                        "key": "user-account.account_type",
+                                        "object": "accessor-user-account"
+                                    },
+                                    "account_type_id": {
+                                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                        "object": "accessor-user-account"
+                                    },
+                                    "account_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                        "object": "accessor-user-account"
                                     },
-                                    "policy": {
+                                    "credential_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                        "object": "accessor-user-account"
+                                    },
+                                    "domain": {
+                                        "key": "user-account.extensions.x-accessor-ext.domain",
+                                        "object": "accessor-user-account"
+                                    },
+                                    "email_addr": {
+                                        "key": "email-addr.value",
+                                        "object": "email-addr"
+                                    },
+                                    "groups": {
                                         "desc": {
-                                            "key": "x-ocsf-identity.authorizations.policy_desc",
-                                            "object": "x-ocsf-identity"
-                                        },
-                                        "group": {
-                                            "desc": {
-                                                "key": "x-ocsf-identity.authorizations.policy_group_desc",
-                                                "object": "x-ocsf-identity"
-                                            },
-                                            "name": {
-                                                "key": "x-ocsf-identity.authorizations.policy_group_namee",
-                                                "object": "x-ocsf-identity"
-                                            },
-                                            "privileges": {
-                                                "key": "x-ocsf-identity.authorizations.policy_group_privileges",
-                                                "object": "x-ocsf-identity"
-                                            },
-                                            "type": {
-                                                "key": "x-ocsf-identity.authorizations.policy_group_type",
-                                                "object": "x-ocsf-identity"
-                                            },
-                                            "uid": {
-                                                "key": "x-ocsf-identity.authorizations.policy_group_uid",
-                                                "object": "x-ocsf-identity"
-                                            }
+                                            "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                            "object": "accessor-user-account"
                                         },
                                         "name": {
-                                            "key": "x-ocsf-identity.authorizations.name",
-                                            "object": "x-ocsf-identity"
+                                            "key": "user-account.extensions.x-accessor-ext.group_name",
+                                            "object": "accessor-user-account"
                                         },
-                                        "uid": {
-                                            "key": "x-ocsf-identity.authorizations.uid",
-                                            "object": "x-ocsf-identity"
+                                        "privileges": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                            "object": "accessor-user-account"
                                         },
-                                        "version": {
-                                            "key": "x-ocsf-identity.authorizations.version",
-                                            "object": "x-ocsf-identity"
+                                        "type": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_type",
+                                            "object": "accessor-user-account"
+                                        },
+                                        "uid": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                            "object": "accessor-user-account"
                                         }
-                                    }
-                                },
-                                "idp": {
+                                    },
                                     "name": {
-                                        "key": "x-ocsf-identity.idp.name",
-                                        "object": "x-ocsf-identity"
+                                        "key": "user-account.display_name",
+                                        "object": "accessor-user-account"
                                     },
-                                    "uid": {
-                                        "key": "x-ocsf-identity.idp.uid",
-                                        "object": "x-ocsf-identity"
-                                    }
-                                },
-                                "invoked_by": {
-                                    "key": "x-ocsf-identity.invoked_by",
-                                    "object": "x-ocsf-identity"
-                                },
-                                "message": {
-                                    "key": "x-ocsf-identity.message",
-                                    "object": "x-ocsf-identity"
-                                },
-                                "session": {
-                                    "created_time": {
-                                        "key": "x-ocsf-identity.session.created_time",
-                                        "object": "x-ocsf-identity"
+                                    "org_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                        "object": "accessor-user-account"
                                     },
-                                    "credential_uid": {
-                                        "key": "x-ocsf-identity.session.credential_uid",
-                                        "object": "x-ocsf-identity"
+                                    "session_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                        "object": "accessor-user-account"
                                     },
-                                    "expiration_time": {
-                                        "key": "x-ocsf-identity.session.expiration_time",
-                                        "object": "x-ocsf-identity"
+                                    "session_uuid": {
+                                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                        "object": "accessor-user-account"
                                     },
-                                    "issuer": {
-                                        "key": "x-ocsf-identity.session.issuer",
-                                        "object": "x-ocsf-identity"
+                                    "type": {
+                                        "key": "user-account.extensions.x-accessor-ext.type",
+                                        "object": "accessor-user-account"
                                     },
-                                    "mfa": {
-                                        "key": "x-ocsf-identity.session.mfa",
-                                        "object": "x-ocsf-identity"
+                                    "type_id": {
+                                        "key": "user-account.extensions.x-accessor-ext.type_id",
+                                        "object": "accessor-user-account"
                                     },
                                     "uid": {
-                                        "key": "x-ocsf-identity.session.uid",
-                                        "object": "x-ocsf-identity"
+                                        "key": "user-account.user_id",
+                                        "object": "accessor-user-account"
+                                    },
+                                    "uuid": {
+                                        "key": "user-account.extensions.x-accessor-ext.uuid",
+                                        "object": "accessor-user-account"
                                     }
                                 },
-                                "user": {
+                                "attributes": {
+                                    "key": "file.extensions.x-ocsf-file-ext.attributes",
+                                    "object": "file"
+                                },
+                                "company_name": {
+                                    "key": "file.extensions.x-ocsf-file-ext.company_name",
+                                    "object": "file"
+                                },
+                                "confidentiality": {
+                                    "key": "file.extensions.x-ocsf-file-ext.confidentiality",
+                                    "object": "file"
+                                },
+                                "confidentiality_id": {
+                                    "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
+                                    "object": "file"
+                                },
+                                "created_time": {
+                                    "key": "file.created",
+                                    "object": "file"
+                                },
+                                "creator": {
                                     "account_type": {
                                         "key": "user-account.account_type",
-                                        "object": "user"
+                                        "object": "creator-user-account"
                                     },
                                     "account_type_id": {
-                                        "key": "user-account.extensions.aws-account-ext.account_type_id",
-                                        "object": "user",
-                                        "transformer": "ToInteger"
+                                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                        "object": "creator-user-account"
                                     },
                                     "account_uid": {
-                                        "key": "user-account.user_id",
-                                        "object": "user"
+                                        "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                        "object": "creator-user-account"
                                     },
                                     "credential_uid": {
-                                        "key": "user-account.extensions.aws-account-ext.credential_uid",
-                                        "object": "user"
+                                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                        "object": "creator-user-account"
                                     },
                                     "domain": {
-                                        "key": "user-account.extensions.aws-account-ext.domain",
-                                        "object": "user"
+                                        "key": "user-account.extensions.x-accessor-ext.domain",
+                                        "object": "creator-user-account"
                                     },
                                     "email_addr": {
                                         "key": "email-addr.value",
-                                        "object": "email_addr"
+                                        "object": "creator-email-addr"
                                     },
                                     "groups": {
                                         "desc": {
-                                            "key": "user-account.extensions.aws-account-ext.group_desc",
-                                            "object": "user"
+                                            "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                            "object": "creator-user-account"
                                         },
                                         "name": {
-                                            "key": "user-account.extensions.aws-account-ext.group_name",
-                                            "object": "user"
+                                            "key": "user-account.extensions.x-accessor-ext.group_name",
+                                            "object": "creator-user-account"
                                         },
                                         "privileges": {
-                                            "key": "user-account.extensions.aws-account-ext.group_privileges",
-                                            "object": "user"
+                                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                            "object": "creator-user-account"
                                         },
                                         "type": {
-                                            "key": "user-account.extensions.aws-account-ext.group_type",
-                                            "object": "user"
+                                            "key": "user-account.extensions.x-accessor-ext.group_type",
+                                            "object": "creator-user-account"
                                         },
                                         "uid": {
-                                            "key": "user-account.extensions.aws-account-ext.group_uid",
-                                            "object": "user"
+                                            "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                            "object": "creator-user-account"
                                         }
                                     },
                                     "name": {
                                         "key": "user-account.display_name",
-                                        "object": "user"
+                                        "object": "creator-user-account"
                                     },
                                     "org_uid": {
-                                        "key": "user-account.extensions.aws-account-ext.org_uid",
-                                        "object": "user"
+                                        "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                        "object": "creator-user-account"
                                     },
                                     "session_uid": {
-                                        "key": "user-account.extensions.aws-account-ext.session_uid",
-                                        "object": "user"
+                                        "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                        "object": "creator-user-account"
                                     },
                                     "session_uuid": {
-                                        "key": "user-account.extensions.aws-account-ext.session_uuid",
-                                        "object": "user"
+                                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                        "object": "creator-user-account"
                                     },
                                     "type": {
-                                        "key": "user-account.extensions.aws-account-ext.type",
-                                        "object": "user"
+                                        "key": "user-account.extensions.x-accessor-ext.type",
+                                        "object": "creator-user-account"
                                     },
                                     "type_id": {
-                                        "key": "user-account.extensions.aws-account-ext.type_id",
-                                        "object": "user",
-                                        "transformer": "ToInteger"
+                                        "key": "user-account.extensions.x-accessor-ext.type_id",
+                                        "object": "creator-user-account"
                                     },
                                     "uid": {
-                                        "key": "user-account.extensions.aws-account-ext.uid",
-                                        "object": "user"
+                                        "key": "user-account.user_id",
+                                        "object": "creator-user-account"
                                     },
                                     "uuid": {
-                                        "key": "user-account.extensions.aws-account-ext.uuid",
-                                        "object": "user"
+                                        "key": "user-account.extensions.x-accessor-ext.uuid",
+                                        "object": "creator-user-account"
                                     }
-                                }
-                            },
-                            "malware": {
-                                "classification_ids": {
-                                    "key": "x-ocsf-malware.classification_ids",
-                                    "object": "malware"
                                 },
-                                "classifications": {
-                                    "key": "x-ocsf-malware.classifications",
-                                    "object": "malware"
+                                "desc": {
+                                    "key": "file.extensions.x-ocsf-file-ext.description",
+                                    "object": "file"
                                 },
-                                "cves": {
-                                    "created_time": {
-                                        "key": "x-ocsf-malware.created_time",
-                                        "object": "malware"
+                                "hashes": {
+                                    "CTPH": {
+                                        "key": "file.hashes.CTPH",
+                                        "object": "file"
                                     },
-                                    "cvss": {
-                                        "base_score": {
-                                            "key": "x-ocsf-malware.base_score",
-                                            "object": "malware"
-                                        },
-                                        "depth": {
-                                            "key": "x-ocsf-malware.depth",
-                                            "object": "malware"
-                                        },
-                                        "metrics": {
-                                            "name": {
-                                                "key": "x-ocsf-malware.name",
-                                                "object": "malware"
-                                            },
-                                            "value": {
-                                                "key": "x-ocsf-malware.value",
-                                                "object": "malware"
-                                            }
+                                    "MD5": {
+                                        "key": "file.hashes.MD5",
+                                        "object": "file"
+                                    },
+                                    "Other": {
+                                        "key": "file.hashes.Other",
+                                        "object": "file"
+                                    },
+                                    "SHA-1": {
+                                        "key": "file.hashes.SHA-1",
+                                        "object": "file"
+                                    },
+                                    "SHA-256": {
+                                        "key": "file.hashes.SHA-256",
+                                        "object": "file"
+                                    },
+                                    "SHA-512": {
+                                        "key": "file.hashes.SHA-512",
+                                        "object": "file"
+                                    },
+                                    "Unknown": {
+                                        "key": "file.hashes.Unknown",
+                                        "object": "file"
+                                    }
+                                },
+                                "is_system": {
+                                    "key": "process.extensions.x-ocsf-process-ext.is_system",
+                                    "object": "process"
+                                },
+                                "mime_type": {
+                                    "key": "process.mime_type",
+                                    "object": "process"
+                                },
+                                "modified_time": {
+                                    "key": "process.extensions.x-ocsf-process-ext.modified_time",
+                                    "object": "process"
+                                },
+                                "modifier": {
+                                    "account_type": {
+                                        "key": "user-account.account_type",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "account_type_id": {
+                                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "account_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "credential_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "domain": {
+                                        "key": "user-account.extensions.x-accessor-ext.domain",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "email_addr": {
+                                        "key": "email-addr.value",
+                                        "object": "modifier-email-addr"
+                                    },
+                                    "groups": {
+                                        "desc": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                            "object": "modifier-user-account"
                                         },
-                                        "overall_score": {
-                                            "key": "x-ocsf-malware.overall_score",
-                                            "object": "malware"
+                                        "name": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_name",
+                                            "object": "modifier-user-account"
                                         },
-                                        "severity": {
-                                            "key": "x-ocsf-malware.severity",
-                                            "object": "malware"
+                                        "privileges": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                            "object": "modifier-user-account"
                                         },
-                                        "vector_string": {
-                                            "key": "x-ocsf-malware.vector_string",
-                                            "object": "malware"
+                                        "type": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_type",
+                                            "object": "modifier-user-account"
                                         },
-                                        "version": {
-                                            "key": "x-ocsf-malware.version",
-                                            "object": "malware"
+                                        "uid": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                            "object": "modifier-user-account"
                                         }
                                     },
-                                    "cwe_uid": {
-                                        "key": "x-ocsf-malware.cwe_uid",
-                                        "object": "malware"
+                                    "name": {
+                                        "key": "user-account.display_name",
+                                        "object": "modifier-user-account"
                                     },
-                                    "cwe_url": {
-                                        "key": "x-ocsf-malware.cwe_url",
-                                        "object": "malware"
+                                    "org_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                        "object": "modifier-user-account"
                                     },
-                                    "modified_time": {
-                                        "key": "x-ocsf-malware.modified_time",
-                                        "object": "malware"
+                                    "session_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                        "object": "modifier-user-account"
                                     },
-                                    "product": {
-                                        "feature": {
-                                            "name": {
-                                                "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                                "object": "malware-software"
-                                            },
-                                            "uid": {
-                                                "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                                "object": "malware-software"
-                                            },
-                                            "version": {
-                                                "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                                "object": "malware-software"
-                                            }
-                                        },
-                                        "lang": {
-                                            "key": "software.languages",
-                                            "object": "malware-software"
+                                    "session_uuid": {
+                                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "type": {
+                                        "key": "user-account.extensions.x-accessor-ext.type",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "type_id": {
+                                        "key": "user-account.extensions.x-accessor-ext.type_id",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "uid": {
+                                        "key": "user-account.user_id",
+                                        "object": "modifier-user-account"
+                                    },
+                                    "uuid": {
+                                        "key": "user-account.extensions.x-accessor-ext.uuid",
+                                        "object": "modifier-user-account"
+                                    }
+                                },
+                                "name": [
+                                    {
+                                        "key": "file.name",
+                                        "object": "file"
+                                    },
+                                    {
+                                        "key": "process.binary_ref",
+                                        "object": "process",
+                                        "references": "file"
+                                    }
+                                ],
+                                "owner": {
+                                    "account_type": {
+                                        "key": "user-account.account_type",
+                                        "object": "owner-user-account"
+                                    },
+                                    "account_type_id": {
+                                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                        "object": "owner-user-account"
+                                    },
+                                    "account_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                        "object": "owner-user-account"
+                                    },
+                                    "credential_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                        "object": "owner-user-account"
+                                    },
+                                    "domain": {
+                                        "key": "user-account.extensions.x-accessor-ext.domain",
+                                        "object": "owner-user-account"
+                                    },
+                                    "email_addr": {
+                                        "key": "email-addr.value",
+                                        "object": "owner-user-account"
+                                    },
+                                    "groups": {
+                                        "desc": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                            "object": "owner-user-account"
                                         },
                                         "name": {
-                                            "key": "software.name",
-                                            "object": "malware-software"
-                                        },
-                                        "path": {
-                                            "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                            "object": "malware-software"
+                                            "key": "user-account.extensions.x-accessor-ext.group_name",
+                                            "object": "owner-user-account"
                                         },
-                                        "uid": {
-                                            "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                            "object": "malware-software"
+                                        "privileges": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                            "object": "owner-user-account"
                                         },
-                                        "vendor_name": {
-                                            "key": "software.vendor",
-                                            "object": "malware-software"
+                                        "type": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_type",
+                                            "object": "owner-user-account"
                                         },
-                                        "version": {
-                                            "key": "software.version",
-                                            "object": "malware-software"
+                                        "uid": {
+                                            "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                            "object": "owner-user-account"
                                         }
                                     },
+                                    "name": {
+                                        "key": "user-account.display_name",
+                                        "object": "owner-user-account"
+                                    },
+                                    "org_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                        "object": "owner-user-account"
+                                    },
+                                    "session_uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                        "object": "owner-user-account"
+                                    },
+                                    "session_uuid": {
+                                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                        "object": "owner-user-account"
+                                    },
                                     "type": {
-                                        "key": "x-ocsf-malware.type",
-                                        "object": "malware"
+                                        "key": "user-account.extensions.x-accessor-ext.type",
+                                        "object": "owner-user-account"
+                                    },
+                                    "type_id": {
+                                        "key": "user-account.extensions.x-accessor-ext.type_id",
+                                        "object": "owner-user-account"
                                     },
                                     "uid": {
-                                        "key": "x-ocsf-malware.uid",
-                                        "object": "malware"
+                                        "key": "user-account.user_id",
+                                        "object": "owner-user-account"
+                                    },
+                                    "uuid": {
+                                        "key": "user-account.extensions.x-accessor-ext.uuid",
+                                        "object": "owner-user-account"
                                     }
                                 },
-                                "name": {
-                                    "key": "x-ocsf-malware.name",
-                                    "object": "malware"
-                                },
+                                "parent_folder": [
+                                    {
+                                        "key": "directory.path",
+                                        "object": "directory"
+                                    },
+                                    {
+                                        "key": "file.parent_directory_ref",
+                                        "object": "file",
+                                        "references": "directory"
+                                    }
+                                ],
                                 "path": {
-                                    "key": "x-ocsf-malware.path",
-                                    "object": "malware"
-                                },
-                                "provider": {
-                                    "key": "x-ocsf-malware.provider",
-                                    "object": "malware"
-                                },
-                                "uid": {
-                                    "key": "x-ocsf-malware.uid",
-                                    "object": "malware"
-                                }
-                            },
-                            "message": {
-                                "key": "x-ocsf-cloud.message",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "metadata": {
-                                "correlation_uid": {
-                                    "key": "x-ocsf-metadata.correlation_uid",
-                                    "object": "metadata"
-                                },
-                                "labels": {
-                                    "key": "x-ocsf-metadata.labels",
-                                    "object": "metadata"
-                                },
-                                "logged_time": {
-                                    "key": "x-ocsf-metadata.logged_time",
-                                    "object": "metadata"
-                                },
-                                "modified_time": {
-                                    "key": "x-ocsf-metadata.modified_time",
-                                    "object": "metadata"
-                                },
-                                "processed_time": {
-                                    "key": "x-ocsf-metadata.processed_time",
-                                    "object": "metadata"
+                                    "key": "file.extensions.x-ocsf-file-ext.path",
+                                    "object": "file"
                                 },
                                 "product": {
                                     "feature": {
                                         "name": {
                                             "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                            "object": "metadata-software"
+                                            "object": "file1-software"
                                         },
                                         "uid": {
                                             "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                            "object": "metadata-software"
+                                            "object": "file1-software"
                                         },
                                         "version": {
                                             "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                            "object": "metadata-software"
+                                            "object": "file1-software"
                                         }
                                     },
                                     "lang": {
                                         "key": "software.languages",
-                                        "object": "metadata-software"
+                                        "object": "file1-software"
                                     },
                                     "name": {
                                         "key": "software.name",
-                                        "object": "metadata-software"
+                                        "object": "file1-software"
                                     },
                                     "path": {
                                         "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                        "object": "metadata-software"
+                                        "object": "file1-software"
                                     },
                                     "uid": {
                                         "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                        "object": "metadata-software"
+                                        "object": "file1-software"
                                     },
                                     "vendor_name": {
                                         "key": "software.vendor",
-                                        "object": "metadata-software"
+                                        "object": "file1-software"
                                     },
                                     "version": {
                                         "key": "software.version",
-                                        "object": "metadata-software"
+                                        "object": "file1-software"
                                     }
                                 },
-                                "sequence": {
-                                    "key": "x-ocsf-metadata.sequence",
-                                    "object": "metadata",
-                                    "transformer": "ToInteger"
-                                },
-                                "uid": {
-                                    "key": "x-ocsf-metadata.uid",
-                                    "object": "metadata"
+                                "security_descriptor": {
+                                    "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
+                                    "object": "file"
+                                },
+                                "signature": {
+                                    "key": "file.extensions.x-ocsf-file-ext.signature",
+                                    "object": "file"
+                                },
+                                "size": {
+                                    "key": "file.size",
+                                    "object": "file"
                                 },
-                                "version": {
-                                    "key": "x-ocsf-metadata.version",
-                                    "object": "metadata"
-                                }
-                            },
-                            "observables": {
-                                "name": [
-                                    {
-                                        "key": "x-ibm-observables.name",
-                                        "object": "observables"
-                                    },
-                                    {
-                                        "key": "x-ibm-finding.ioc_refs",
-                                        "object": "ibm_finding",
-                                        "references": [
-                                            "observables"
-                                        ]
-                                    }
-                                ],
                                 "type": {
-                                    "key": "x-ibm-observables.finding_type",
-                                    "object": "observables"
+                                    "key": "file.extensions.x-ocsf-file-ext.type",
+                                    "object": "file"
                                 },
                                 "type_id": {
-                                    "key": "x-ibm-observables.alert_id",
-                                    "object": "observables",
-                                    "transformer": "ToInteger"
+                                    "key": "file.extensions.x-ocsf-file-ext.type_id",
+                                    "object": "file"
                                 },
-                                "value": {
-                                    "key": "x-ibm-observables.description",
-                                    "object": "observables"
+                                "uid": {
+                                    "key": "file.extensions.x-ocsf-file-ext.uid",
+                                    "object": "file"
+                                },
+                                "version": {
+                                    "key": "file.extensions.x-ocsf-file-ext.version",
+                                    "object": "file"
+                                },
+                                "xattributes": {
+                                    "key": "process.extensions.x-ocsf-process-ext.xattributes",
+                                    "object": "process"
                                 }
                             },
-                            "process": {
+                            "integrity": {
+                                "key": "process.extensions.x-ocsf-process-ext.integrity",
+                                "object": "process"
+                            },
+                            "integrity_id": {
+                                "key": "process.extensions.x-ocsf-process-ext.integrity_id",
+                                "object": "process"
+                            },
+                            "lineage": {
+                                "key": "process.extensions.x-ocsf-process-ext.lineage",
+                                "object": "process"
+                            },
+                            "loaded_modules": {
+                                "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
+                                "object": "process"
+                            },
+                            "name": {
+                                "key": "process.name",
+                                "object": "process"
+                            },
+                            "parent_process": {
                                 "cmd_line": {
                                     "key": "process.command_line",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "created_time": {
                                     "key": "process.created",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "file": {
                                     "accessed_time": {
                                         "key": "file.accessed",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "accessor": {
                                         "account_type": {
                                             "key": "user-account.account_type",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "account_type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "account_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "credential_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "domain": {
                                             "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "email_addr": {
                                             "key": "email-addr.value",
-                                            "object": "email-addr"
+                                            "object": "parent-email-addr"
                                         },
                                         "groups": {
                                             "desc": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "accessor-user-account"
+                                                "object": "parent-accessor-user-account"
                                             },
                                             "name": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "accessor-user-account"
+                                                "object": "parent-accessor-user-account"
                                             },
                                             "privileges": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "accessor-user-account"
+                                                "object": "parent-accessor-user-account"
                                             },
                                             "type": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "accessor-user-account"
+                                                "object": "parent-accessor-user-account"
                                             },
                                             "uid": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "accessor-user-account"
+                                                "object": "parent-accessor-user-account"
                                             }
                                         },
                                         "name": {
                                             "key": "user-account.display_name",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "org_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "session_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "session_uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.user_id",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         },
                                         "uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "accessor-user-account"
+                                            "object": "parent-accessor-user-account"
                                         }
                                     },
                                     "attributes": {
                                         "key": "file.extensions.x-ocsf-file-ext.attributes",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "company_name": {
                                         "key": "file.extensions.x-ocsf-file-ext.company_name",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "confidentiality": {
                                         "key": "file.extensions.x-ocsf-file-ext.confidentiality",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "confidentiality_id": {
                                         "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "created_time": {
                                         "key": "file.created",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "creator": {
                                         "account_type": {
                                             "key": "user-account.account_type",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "account_type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "account_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "credential_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "domain": {
                                             "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "email_addr": {
                                             "key": "email-addr.value",
-                                            "object": "creator-email-addr"
+                                            "object": "parent-creator-email-addr"
                                         },
                                         "groups": {
                                             "desc": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "creator-user-account"
+                                                "object": "parent-creator-user-account"
                                             },
                                             "name": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "creator-user-account"
+                                                "object": "parent-creator-user-account"
                                             },
                                             "privileges": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "creator-user-account"
+                                                "object": "parent-creator-user-account"
                                             },
                                             "type": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "creator-user-account"
+                                                "object": "parent-creator-user-account"
                                             },
                                             "uid": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "creator-user-account"
+                                                "object": "parent-creator-user-account"
                                             }
                                         },
                                         "name": {
                                             "key": "user-account.display_name",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "org_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "session_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "session_uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.user_id",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         },
                                         "uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "creator-user-account"
+                                            "object": "parent-creator-user-account"
                                         }
                                     },
                                     "desc": {
                                         "key": "file.extensions.x-ocsf-file-ext.description",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "hashes": {
                                         "CTPH": {
                                             "key": "file.hashes.CTPH",
-                                            "object": "file"
+                                            "object": "parent-file"
                                         },
                                         "MD5": {
                                             "key": "file.hashes.MD5",
-                                            "object": "file"
+                                            "object": "parent-file"
                                         },
                                         "Other": {
                                             "key": "file.hashes.Other",
-                                            "object": "file"
+                                            "object": "parent-file"
                                         },
                                         "SHA-1": {
                                             "key": "file.hashes.SHA-1",
-                                            "object": "file"
+                                            "object": "parent-file"
                                         },
                                         "SHA-256": {
                                             "key": "file.hashes.SHA-256",
-                                            "object": "file"
+                                            "object": "parent-file"
                                         },
                                         "SHA-512": {
                                             "key": "file.hashes.SHA-512",
-                                            "object": "file"
+                                            "object": "parent-file"
                                         },
                                         "Unknown": {
                                             "key": "file.hashes.Unknown",
-                                            "object": "file"
+                                            "object": "parent-file"
                                         }
                                     },
                                     "is_system": {
                                         "key": "process.extensions.x-ocsf-process-ext.is_system",
-                                        "object": "process"
+                                        "object": "parent-process"
                                     },
                                     "mime_type": {
                                         "key": "process.mime_type",
-                                        "object": "process"
+                                        "object": "parent-process"
                                     },
                                     "modified_time": {
                                         "key": "process.extensions.x-ocsf-process-ext.modified_time",
-                                        "object": "process"
+                                        "object": "parent-process"
                                     },
                                     "modifier": {
                                         "account_type": {
                                             "key": "user-account.account_type",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "account_type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "account_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "credential_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "domain": {
                                             "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "email_addr": {
                                             "key": "email-addr.value",
-                                            "object": "modifier-email-addr"
+                                            "object": "parent-modifier-email-addr"
                                         },
                                         "groups": {
                                             "desc": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "modifier-user-account"
+                                                "object": "parent-modifier-user-account"
                                             },
                                             "name": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "modifier-user-account"
+                                                "object": "parent-modifier-user-account"
                                             },
                                             "privileges": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "modifier-user-account"
+                                                "object": "parent-modifier-user-account"
                                             },
                                             "type": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "modifier-user-account"
+                                                "object": "parent-modifier-user-account"
                                             },
                                             "uid": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "modifier-user-account"
+                                                "object": "parent-modifier-user-account"
                                             }
                                         },
                                         "name": {
                                             "key": "user-account.display_name",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "org_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "session_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "session_uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.user_id",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         },
                                         "uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "modifier-user-account"
+                                            "object": "parent-modifier-user-account"
                                         }
                                     },
                                     "name": [
                                         {
                                             "key": "file.name",
-                                            "object": "file"
+                                            "object": "parent-file"
                                         },
                                         {
                                             "key": "process.binary_ref",
-                                            "object": "process",
-                                            "references": "file"
+                                            "object": "parent-process",
+                                            "references": "parent-file"
                                         }
                                     ],
                                     "owner": {
                                         "account_type": {
                                             "key": "user-account.account_type",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "account_type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "account_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "credential_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "domain": {
                                             "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "email_addr": {
                                             "key": "email-addr.value",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-email-addr"
                                         },
                                         "groups": {
                                             "desc": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "owner-user-account"
+                                                "object": "parent-owner-user-account"
                                             },
                                             "name": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "owner-user-account"
+                                                "object": "parent-owner-user-account"
                                             },
                                             "privileges": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "owner-user-account"
+                                                "object": "parent-owner-user-account"
                                             },
                                             "type": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "owner-user-account"
+                                                "object": "parent-owner-user-account"
                                             },
                                             "uid": {
                                                 "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "owner-user-account"
+                                                "object": "parent-owner-user-account"
                                             }
                                         },
                                         "name": {
                                             "key": "user-account.display_name",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "org_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "session_uid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "session_uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "type_id": {
                                             "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.user_id",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         },
                                         "uuid": {
                                             "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "owner-user-account"
+                                            "object": "parent-owner-user-account"
                                         }
                                     },
                                     "parent_folder": [
                                         {
                                             "key": "directory.path",
-                                            "object": "directory"
+                                            "object": "parent-directory"
                                         },
                                         {
                                             "key": "file.parent_directory_ref",
-                                            "object": "file",
-                                            "references": "directory"
+                                            "object": "parent-file",
+                                            "references": "parent-directory"
                                         }
                                     ],
                                     "path": {
                                         "key": "file.extensions.x-ocsf-file-ext.path",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "product": {
                                         "feature": {
                                             "name": {
                                                 "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                                "object": "file1-software"
+                                                "object": "file-software"
                                             },
                                             "uid": {
                                                 "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                                "object": "file1-software"
+                                                "object": "file-software"
                                             },
                                             "version": {
                                                 "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                                "object": "file1-software"
+                                                "object": "file-software"
                                             }
                                         },
                                         "lang": {
                                             "key": "software.languages",
-                                            "object": "file1-software"
+                                            "object": "file-software"
                                         },
                                         "name": {
                                             "key": "software.name",
-                                            "object": "file1-software"
+                                            "object": "file-software"
                                         },
                                         "path": {
                                             "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                            "object": "file1-software"
+                                            "object": "file-software"
                                         },
                                         "uid": {
                                             "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                            "object": "file1-software"
+                                            "object": "file-software"
                                         },
                                         "vendor_name": {
                                             "key": "software.vendor",
-                                            "object": "file1-software"
+                                            "object": "file-software"
                                         },
                                         "version": {
                                             "key": "software.version",
-                                            "object": "file1-software"
+                                            "object": "file-software"
                                         }
                                     },
                                     "security_descriptor": {
                                         "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "signature": {
                                         "key": "file.extensions.x-ocsf-file-ext.signature",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "size": {
                                         "key": "file.size",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "type": {
                                         "key": "file.extensions.x-ocsf-file-ext.type",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "type_id": {
                                         "key": "file.extensions.x-ocsf-file-ext.type_id",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "uid": {
                                         "key": "file.extensions.x-ocsf-file-ext.uid",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "version": {
                                         "key": "file.extensions.x-ocsf-file-ext.version",
-                                        "object": "file"
+                                        "object": "parent-file"
                                     },
                                     "xattributes": {
                                         "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                                        "object": "process"
+                                        "object": "parent-process"
                                     }
                                 },
                                 "integrity": {
                                     "key": "process.extensions.x-ocsf-process-ext.integrity",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "integrity_id": {
                                     "key": "process.extensions.x-ocsf-process-ext.integrity_id",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "lineage": {
                                     "key": "process.extensions.x-ocsf-process-ext.lineage",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "loaded_modules": {
                                     "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "name": {
                                     "key": "process.name",
-                                    "object": "process"
-                                },
-                                "parent_process": {
-                                    "cmd_line": {
-                                        "key": "process.command_line",
-                                        "object": "parent-process"
-                                    },
-                                    "created_time": {
-                                        "key": "process.created",
-                                        "object": "parent-process"
-                                    },
-                                    "file": {
-                                        "accessed_time": {
-                                            "key": "file.accessed",
-                                            "object": "parent-file"
-                                        },
-                                        "accessor": {
-                                            "account_type": {
-                                                "key": "user-account.account_type",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "account_type_id": {
-                                                "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "account_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "credential_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "domain": {
-                                                "key": "user-account.extensions.x-accessor-ext.domain",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "email_addr": {
-                                                "key": "email-addr.value",
-                                                "object": "parent-email-addr"
-                                            },
-                                            "groups": {
-                                                "desc": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                    "object": "parent-accessor-user-account"
-                                                },
-                                                "name": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                    "object": "parent-accessor-user-account"
-                                                },
-                                                "privileges": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                    "object": "parent-accessor-user-account"
-                                                },
-                                                "type": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                    "object": "parent-accessor-user-account"
-                                                },
-                                                "uid": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                    "object": "parent-accessor-user-account"
-                                                }
-                                            },
-                                            "name": {
-                                                "key": "user-account.display_name",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "org_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "session_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "session_uuid": {
-                                                "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "type": {
-                                                "key": "user-account.extensions.x-accessor-ext.type",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "type_id": {
-                                                "key": "user-account.extensions.x-accessor-ext.type_id",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "uid": {
-                                                "key": "user-account.user_id",
-                                                "object": "parent-accessor-user-account"
-                                            },
-                                            "uuid": {
-                                                "key": "user-account.extensions.x-accessor-ext.uuid",
-                                                "object": "parent-accessor-user-account"
-                                            }
-                                        },
-                                        "attributes": {
-                                            "key": "file.extensions.x-ocsf-file-ext.attributes",
-                                            "object": "parent-file"
-                                        },
-                                        "company_name": {
-                                            "key": "file.extensions.x-ocsf-file-ext.company_name",
-                                            "object": "parent-file"
-                                        },
-                                        "confidentiality": {
-                                            "key": "file.extensions.x-ocsf-file-ext.confidentiality",
-                                            "object": "parent-file"
-                                        },
-                                        "confidentiality_id": {
-                                            "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
-                                            "object": "parent-file"
-                                        },
-                                        "created_time": {
-                                            "key": "file.created",
-                                            "object": "parent-file"
-                                        },
-                                        "creator": {
-                                            "account_type": {
-                                                "key": "user-account.account_type",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "account_type_id": {
-                                                "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "account_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "credential_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "domain": {
-                                                "key": "user-account.extensions.x-accessor-ext.domain",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "email_addr": {
-                                                "key": "email-addr.value",
-                                                "object": "parent-creator-email-addr"
-                                            },
-                                            "groups": {
-                                                "desc": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                    "object": "parent-creator-user-account"
-                                                },
-                                                "name": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                    "object": "parent-creator-user-account"
-                                                },
-                                                "privileges": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                    "object": "parent-creator-user-account"
-                                                },
-                                                "type": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                    "object": "parent-creator-user-account"
-                                                },
-                                                "uid": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                    "object": "parent-creator-user-account"
-                                                }
-                                            },
-                                            "name": {
-                                                "key": "user-account.display_name",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "org_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "session_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "session_uuid": {
-                                                "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "type": {
-                                                "key": "user-account.extensions.x-accessor-ext.type",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "type_id": {
-                                                "key": "user-account.extensions.x-accessor-ext.type_id",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "uid": {
-                                                "key": "user-account.user_id",
-                                                "object": "parent-creator-user-account"
-                                            },
-                                            "uuid": {
-                                                "key": "user-account.extensions.x-accessor-ext.uuid",
-                                                "object": "parent-creator-user-account"
-                                            }
-                                        },
-                                        "desc": {
-                                            "key": "file.extensions.x-ocsf-file-ext.description",
-                                            "object": "parent-file"
-                                        },
-                                        "hashes": {
-                                            "CTPH": {
-                                                "key": "file.hashes.CTPH",
-                                                "object": "parent-file"
-                                            },
-                                            "MD5": {
-                                                "key": "file.hashes.MD5",
-                                                "object": "parent-file"
-                                            },
-                                            "Other": {
-                                                "key": "file.hashes.Other",
-                                                "object": "parent-file"
-                                            },
-                                            "SHA-1": {
-                                                "key": "file.hashes.SHA-1",
-                                                "object": "parent-file"
-                                            },
-                                            "SHA-256": {
-                                                "key": "file.hashes.SHA-256",
-                                                "object": "parent-file"
-                                            },
-                                            "SHA-512": {
-                                                "key": "file.hashes.SHA-512",
-                                                "object": "parent-file"
-                                            },
-                                            "Unknown": {
-                                                "key": "file.hashes.Unknown",
-                                                "object": "parent-file"
-                                            }
-                                        },
-                                        "is_system": {
-                                            "key": "process.extensions.x-ocsf-process-ext.is_system",
-                                            "object": "parent-process"
-                                        },
-                                        "mime_type": {
-                                            "key": "process.mime_type",
-                                            "object": "parent-process"
-                                        },
-                                        "modified_time": {
-                                            "key": "process.extensions.x-ocsf-process-ext.modified_time",
-                                            "object": "parent-process"
-                                        },
-                                        "modifier": {
-                                            "account_type": {
-                                                "key": "user-account.account_type",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "account_type_id": {
-                                                "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "account_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "credential_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "domain": {
-                                                "key": "user-account.extensions.x-accessor-ext.domain",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "email_addr": {
-                                                "key": "email-addr.value",
-                                                "object": "parent-modifier-email-addr"
-                                            },
-                                            "groups": {
-                                                "desc": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                    "object": "parent-modifier-user-account"
-                                                },
-                                                "name": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                    "object": "parent-modifier-user-account"
-                                                },
-                                                "privileges": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                    "object": "parent-modifier-user-account"
-                                                },
-                                                "type": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                    "object": "parent-modifier-user-account"
-                                                },
-                                                "uid": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                    "object": "parent-modifier-user-account"
-                                                }
-                                            },
-                                            "name": {
-                                                "key": "user-account.display_name",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "org_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "session_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "session_uuid": {
-                                                "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "type": {
-                                                "key": "user-account.extensions.x-accessor-ext.type",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "type_id": {
-                                                "key": "user-account.extensions.x-accessor-ext.type_id",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "uid": {
-                                                "key": "user-account.user_id",
-                                                "object": "parent-modifier-user-account"
-                                            },
-                                            "uuid": {
-                                                "key": "user-account.extensions.x-accessor-ext.uuid",
-                                                "object": "parent-modifier-user-account"
-                                            }
-                                        },
-                                        "name": [
-                                            {
-                                                "key": "file.name",
-                                                "object": "parent-file"
-                                            },
-                                            {
-                                                "key": "process.binary_ref",
-                                                "object": "parent-process",
-                                                "references": "parent-file"
-                                            }
-                                        ],
-                                        "owner": {
-                                            "account_type": {
-                                                "key": "user-account.account_type",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "account_type_id": {
-                                                "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "account_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "credential_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "domain": {
-                                                "key": "user-account.extensions.x-accessor-ext.domain",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "email_addr": {
-                                                "key": "email-addr.value",
-                                                "object": "parent-owner-email-addr"
-                                            },
-                                            "groups": {
-                                                "desc": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                    "object": "parent-owner-user-account"
-                                                },
-                                                "name": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                    "object": "parent-owner-user-account"
-                                                },
-                                                "privileges": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                    "object": "parent-owner-user-account"
-                                                },
-                                                "type": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                    "object": "parent-owner-user-account"
-                                                },
-                                                "uid": {
-                                                    "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                    "object": "parent-owner-user-account"
-                                                }
-                                            },
-                                            "name": {
-                                                "key": "user-account.display_name",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "org_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "session_uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "session_uuid": {
-                                                "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "type": {
-                                                "key": "user-account.extensions.x-accessor-ext.type",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "type_id": {
-                                                "key": "user-account.extensions.x-accessor-ext.type_id",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "uid": {
-                                                "key": "user-account.user_id",
-                                                "object": "parent-owner-user-account"
-                                            },
-                                            "uuid": {
-                                                "key": "user-account.extensions.x-accessor-ext.uuid",
-                                                "object": "parent-owner-user-account"
-                                            }
-                                        },
-                                        "parent_folder": [
-                                            {
-                                                "key": "directory.path",
-                                                "object": "parent-directory"
-                                            },
-                                            {
-                                                "key": "file.parent_directory_ref",
-                                                "object": "parent-file",
-                                                "references": "parent-directory"
-                                            }
-                                        ],
-                                        "path": {
-                                            "key": "file.extensions.x-ocsf-file-ext.path",
-                                            "object": "parent-file"
-                                        },
-                                        "product": {
-                                            "feature": {
-                                                "name": {
-                                                    "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                                    "object": "file-software"
-                                                },
-                                                "uid": {
-                                                    "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                                    "object": "file-software"
-                                                },
-                                                "version": {
-                                                    "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                                    "object": "file-software"
-                                                }
-                                            },
-                                            "lang": {
-                                                "key": "software.languages",
-                                                "object": "file-software"
-                                            },
-                                            "name": {
-                                                "key": "software.name",
-                                                "object": "file-software"
-                                            },
-                                            "path": {
-                                                "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                                                "object": "file-software"
-                                            },
-                                            "uid": {
-                                                "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                                "object": "file-software"
-                                            },
-                                            "vendor_name": {
-                                                "key": "software.vendor",
-                                                "object": "file-software"
-                                            },
-                                            "version": {
-                                                "key": "software.version",
-                                                "object": "file-software"
-                                            }
-                                        },
-                                        "security_descriptor": {
-                                            "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
-                                            "object": "parent-file"
-                                        },
-                                        "signature": {
-                                            "key": "file.extensions.x-ocsf-file-ext.signature",
-                                            "object": "parent-file"
-                                        },
-                                        "size": {
-                                            "key": "file.size",
-                                            "object": "parent-file"
-                                        },
-                                        "type": {
-                                            "key": "file.extensions.x-ocsf-file-ext.type",
-                                            "object": "parent-file"
-                                        },
-                                        "type_id": {
-                                            "key": "file.extensions.x-ocsf-file-ext.type_id",
-                                            "object": "parent-file"
-                                        },
-                                        "uid": {
-                                            "key": "file.extensions.x-ocsf-file-ext.uid",
-                                            "object": "parent-file"
-                                        },
-                                        "version": {
-                                            "key": "file.extensions.x-ocsf-file-ext.version",
-                                            "object": "parent-file"
-                                        },
-                                        "xattributes": {
-                                            "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                                            "object": "parent-process"
-                                        }
-                                    },
-                                    "integrity": {
-                                        "key": "process.extensions.x-ocsf-process-ext.integrity",
-                                        "object": "parent-process"
-                                    },
-                                    "integrity_id": {
-                                        "key": "process.extensions.x-ocsf-process-ext.integrity_id",
-                                        "object": "parent-process"
-                                    },
-                                    "lineage": {
-                                        "key": "process.extensions.x-ocsf-process-ext.lineage",
-                                        "object": "parent-process"
-                                    },
-                                    "loaded_modules": {
-                                        "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                                        "object": "parent-process"
-                                    },
-                                    "name": {
-                                        "key": "process.name",
-                                        "object": "parent-process"
-                                    },
-                                    "pid": [
-                                        {
-                                            "key": "process.pid",
-                                            "object": "parent-process"
-                                        },
-                                        {
-                                            "key": "process.child_refs",
-                                            "object": "parent-process",
-                                            "references": [
-                                                "process"
-                                            ]
-                                        }
-                                    ],
-                                    "sandbox": {
-                                        "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                                        "object": "parent-process"
-                                    },
-                                    "terminated_time": {
-                                        "key": "process.extensions.x-ocsf-process-ext.terminated_time",
-                                        "object": "parent-process"
-                                    },
-                                    "tid": {
-                                        "key": "process.extensions.x-ocsf-process-ext.tid",
-                                        "object": "parent-process"
-                                    },
-                                    "uid": {
-                                        "key": "process.x_unique_id",
-                                        "object": "parent-process"
-                                    },
-                                    "user": {
-                                        "account_type": {
-                                            "key": "user-account.account_type",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "account_type_id": {
-                                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "account_uid": {
-                                            "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "credential_uid": {
-                                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "domain": {
-                                            "key": "user-account.extensions.x-accessor-ext.domain",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "email_addr": {
-                                            "key": "email-addr.value",
-                                            "object": "parent-process-email-addr"
-                                        },
-                                        "groups": {
-                                            "desc": {
-                                                "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                                "object": "parent-process-user-account"
-                                            },
-                                            "name": {
-                                                "key": "user-account.extensions.x-accessor-ext.group_name",
-                                                "object": "parent-process-user-account"
-                                            },
-                                            "privileges": {
-                                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                                "object": "parent-process-user-account"
-                                            },
-                                            "type": {
-                                                "key": "user-account.extensions.x-accessor-ext.group_type",
-                                                "object": "parent-process-user-account"
-                                            },
-                                            "uid": {
-                                                "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                                "object": "parent-process-user-account"
-                                            }
-                                        },
-                                        "name": {
-                                            "key": "user-account.display_name",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "org_uid": {
-                                            "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "session_uid": {
-                                            "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "session_uuid": {
-                                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "type": {
-                                            "key": "user-account.extensions.x-accessor-ext.type",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "type_id": {
-                                            "key": "user-account.extensions.x-accessor-ext.type_id",
-                                            "object": "parent-process-user-account"
-                                        },
-                                        "uid": [
-                                            {
-                                                "key": "user-account.user_id",
-                                                "object": "parent-process-user-account"
-                                            },
-                                            {
-                                                "key": "user-account.creator_user_ref",
-                                                "object": "parent-process",
-                                                "references": "process-user-account"
-                                            }
-                                        ],
-                                        "uuid": {
-                                            "key": "user-account.extensions.x-accessor-ext.uuid",
-                                            "object": "parent-process-user-account"
-                                        }
-                                    },
-                                    "xattributes": {
-                                        "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                                        "object": "parent-process"
-                                    }
+                                    "object": "parent-process"
                                 },
                                 "pid": [
                                     {
                                         "key": "process.pid",
-                                        "object": "process"
+                                        "object": "parent-process"
                                     },
                                     {
-                                        "key": "process.parent_ref",
-                                        "object": "process",
+                                        "key": "process.child_refs",
+                                        "object": "parent-process",
                                         "references": [
-                                            "parent-process"
+                                            "process"
                                         ]
                                     }
                                 ],
                                 "sandbox": {
                                     "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "terminated_time": {
                                     "key": "process.extensions.x-ocsf-process-ext.terminated_time",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "tid": {
                                     "key": "process.extensions.x-ocsf-process-ext.tid",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "uid": {
                                     "key": "process.x_unique_id",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 },
                                 "user": {
                                     "account_type": {
                                         "key": "user-account.account_type",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "account_type_id": {
                                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "account_uid": {
                                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "credential_uid": {
                                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "domain": {
                                         "key": "user-account.extensions.x-accessor-ext.domain",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "email_addr": {
                                         "key": "email-addr.value",
-                                        "object": "process-email-addr"
+                                        "object": "parent-process-email-addr"
                                     },
                                     "groups": {
                                         "desc": {
                                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                            "object": "process-user-account"
+                                            "object": "parent-process-user-account"
                                         },
                                         "name": {
                                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                                            "object": "process-user-account"
+                                            "object": "parent-process-user-account"
                                         },
                                         "privileges": {
                                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                            "object": "process-user-account"
+                                            "object": "parent-process-user-account"
                                         },
                                         "type": {
                                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                                            "object": "process-user-account"
+                                            "object": "parent-process-user-account"
                                         },
                                         "uid": {
                                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                            "object": "process-user-account"
+                                            "object": "parent-process-user-account"
                                         }
                                     },
                                     "name": {
                                         "key": "user-account.display_name",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "org_uid": {
                                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "session_uid": {
                                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "session_uuid": {
                                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "type": {
                                         "key": "user-account.extensions.x-accessor-ext.type",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "type_id": {
                                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     },
                                     "uid": [
                                         {
                                             "key": "user-account.user_id",
-                                            "object": "process-user-account"
+                                            "object": "parent-process-user-account"
                                         },
                                         {
                                             "key": "user-account.creator_user_ref",
-                                            "object": "process",
+                                            "object": "parent-process",
                                             "references": "process-user-account"
                                         }
                                     ],
                                     "uuid": {
                                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                                        "object": "process-user-account"
+                                        "object": "parent-process-user-account"
                                     }
                                 },
                                 "xattributes": {
                                     "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                                    "object": "process"
+                                    "object": "parent-process"
                                 }
                             },
-                            "profiles": {
-                                "key": "x-ocsf-cloud.profiles",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "raw_data": {
-                                "key": "x-ocsf-cloud.raw_data",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "ref_event_code": {
-                                "key": "x-ocsf-cloud.ref_event_code",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "ref_event_name": {
-                                "key": "x-ocsf-cloud.ref_event_name",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "ref_event_uid": {
-                                "key": "x-ocsf-cloud.ref_event_uid",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "ref_time": {
-                                "key": "x-ocsf-cloud.ref_time",
-                                "object": "ocsf_cloud_api"
+                            "pid": [
+                                {
+                                    "key": "process.pid",
+                                    "object": "process"
+                                },
+                                {
+                                    "key": "process.parent_ref",
+                                    "object": "process",
+                                    "references": [
+                                        "parent-process"
+                                    ]
+                                }
+                            ],
+                            "sandbox": {
+                                "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
+                                "object": "process"
+                            },
+                            "terminated_time": {
+                                "key": "process.extensions.x-ocsf-process-ext.terminated_time",
+                                "object": "process"
+                            },
+                            "tid": {
+                                "key": "process.extensions.x-ocsf-process-ext.tid",
+                                "object": "process"
+                            },
+                            "uid": {
+                                "key": "process.x_unique_id",
+                                "object": "process"
                             },
-                            "resources": {
-                                "account_uid": [
-                                    {
-                                        "key": "x-ocsf-resources.account_uid",
-                                        "object": "resources"
-                                    },
-                                    {
-                                        "key": "x-ocsf-resources.cloud_api_ref",
-                                        "object": "resources",
-                                        "references": "ocsf_cloud_api"
-                                    }
-                                ],
-                                "cloud_partition": {
-                                    "key": "x-ocsf-resources.cloud_partition",
-                                    "object": "resources"
+                            "user": {
+                                "account_type": {
+                                    "key": "user-account.account_type",
+                                    "object": "process-user-account"
                                 },
-                                "criticality": {
-                                    "key": "x-ocsf-resources.criticality",
-                                    "object": "resources"
+                                "account_type_id": {
+                                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                                    "object": "process-user-account"
                                 },
-                                "details": {
-                                    "key": "x-ocsf-resources.details",
-                                    "object": "resources"
+                                "account_uid": {
+                                    "key": "user-account.extensions.x-accessor-ext.account_uid",
+                                    "object": "process-user-account"
                                 },
-                                "group_name": {
-                                    "key": "x-ocsf-resources.group_name",
-                                    "object": "resources"
+                                "credential_uid": {
+                                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                                    "object": "process-user-account"
+                                },
+                                "domain": {
+                                    "key": "user-account.extensions.x-accessor-ext.domain",
+                                    "object": "process-user-account"
+                                },
+                                "email_addr": {
+                                    "key": "email-addr.value",
+                                    "object": "process-email-addr"
                                 },
-                                "labels": {
-                                    "key": "x-ocsf-resources.labels",
-                                    "object": "resources"
+                                "groups": {
+                                    "desc": {
+                                        "key": "user-account.extensions.x-accessor-ext.group_desc",
+                                        "object": "process-user-account"
+                                    },
+                                    "name": {
+                                        "key": "user-account.extensions.x-accessor-ext.group_name",
+                                        "object": "process-user-account"
+                                    },
+                                    "privileges": {
+                                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                                        "object": "process-user-account"
+                                    },
+                                    "type": {
+                                        "key": "user-account.extensions.x-accessor-ext.group_type",
+                                        "object": "process-user-account"
+                                    },
+                                    "uid": {
+                                        "key": "user-account.extensions.x-accessor-ext.group_uid",
+                                        "object": "process-user-account"
+                                    }
                                 },
                                 "name": {
-                                    "key": "x-ocsf-resources.name",
-                                    "object": "resources"
+                                    "key": "user-account.display_name",
+                                    "object": "process-user-account"
                                 },
-                                "owner": {
-                                    "key": "x-ocsf-resources.owner",
-                                    "object": "resources"
+                                "org_uid": {
+                                    "key": "user-account.extensions.x-accessor-ext.org_uid",
+                                    "object": "process-user-account"
                                 },
-                                "region": {
-                                    "key": "x-ocsf-resources.region",
-                                    "object": "resources"
+                                "session_uid": {
+                                    "key": "user-account.extensions.x-accessor-ext.session_uid",
+                                    "object": "process-user-account"
+                                },
+                                "session_uuid": {
+                                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                                    "object": "process-user-account"
                                 },
                                 "type": {
-                                    "key": "x-ocsf-resources.type",
-                                    "object": "resources"
+                                    "key": "user-account.extensions.x-accessor-ext.type",
+                                    "object": "process-user-account"
                                 },
-                                "uid": {
-                                    "key": "x-ocsf-resources.uid",
-                                    "object": "resources"
-                                }
-                            },
-                            "severity": {
-                                "key": "x-ocsf-cloud.severity",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "severity_id": {
-                                "key": "x-ibm-finding.severity",
-                                "object": "ibm_finding",
-                                "transformer": "ToInteger"
-                            },
-                            "src_endpoint": {
-                                "instance_uid": {
-                                    "key": "x-oca-asset.extensions.x-src-endpoint.instance_uid",
-                                    "object": "asset"
-                                },
-                                "interface_uid": {
-                                    "key": "x-oca-asset.extensions.x-src-endpoint.interface_uid",
-                                    "object": "asset"
+                                "type_id": {
+                                    "key": "user-account.extensions.x-accessor-ext.type_id",
+                                    "object": "process-user-account"
                                 },
-                                "intermediate_ips": [
-                                    {
-                                        "key": "ipv4-addr.value",
-                                        "object": "src_ipv4",
-                                        "transformer": "FilterIPv4List",
-                                        "unwrap": true
-                                    },
-                                    {
-                                        "key": "ipv6-addr.value",
-                                        "object": "src_ipv6",
-                                        "transformer": "FilterIPv6List",
-                                        "unwrap": true
-                                    },
-                                    {
-                                        "key": "x-oca-asset.ip_refs",
-                                        "object": "asset",
-                                        "references": [
-                                            "src_ipv4",
-                                            "src_ipv6"
-                                        ],
-                                        "unwrap": true
-                                    }
-                                ],
-                                "ip": [
-                                    {
-                                        "key": "ipv4-addr.value",
-                                        "object": "src_ip",
-                                        "transformer": "CheckIPv4"
-                                    },
-                                    {
-                                        "key": "ipv6-addr.value",
-                                        "object": "src_ip",
-                                        "transformer": "CheckIPv6"
-                                    },
-                                    {
-                                        "key": "network-traffic.src_ref",
-                                        "object": "nt",
-                                        "references": "src_ip"
-                                    },
-                                    {
-                                        "key": "x-ibm-finding.src_ip_ref",
-                                        "object": "ibm_finding",
-                                        "references": "src_ip"
-                                    },
+                                "uid": [
                                     {
-                                        "group": true,
-                                        "key": "x-oca-asset.ip_refs",
-                                        "object": "host",
-                                        "references": [
-                                            "src_ip"
-                                        ]
+                                        "key": "user-account.user_id",
+                                        "object": "process-user-account"
                                     },
                                     {
-                                        "key": "x-oca-event.network_ref",
-                                        "object": "event",
-                                        "references": "nt"
+                                        "key": "user-account.creator_user_ref",
+                                        "object": "process",
+                                        "references": "process-user-account"
                                     }
                                 ],
-                                "name": {
-                                    "key": "x-oca-asset.name",
-                                    "object": "asset"
-                                },
-                                "port": {
-                                    "key": "network-traffic.src_port",
-                                    "object": "nt",
-                                    "transformer": "ToInteger"
-                                },
-                                "subnet_uid": {
-                                    "key": "x-oca-asset.extensions.x-src-endpoint.subnet_uid",
-                                    "object": "asset"
-                                },
-                                "svc_name": {
-                                    "key": "x-oca-asset.extensions.x-src-endpoint.svc_name",
-                                    "object": "asset"
-                                },
-                                "vpc_uid": {
-                                    "key": "x-oca-asset.extensions.x-src-endpoint.vpc_uid",
-                                    "object": "asset"
+                                "uuid": {
+                                    "key": "user-account.extensions.x-accessor-ext.uuid",
+                                    "object": "process-user-account"
                                 }
                             },
-                            "start_time": {
-                                "key": "first_observed",
-                                "transformer": "EpochToTimestamp"
+                            "xattributes": {
+                                "key": "process.extensions.x-ocsf-process-ext.xattributes",
+                                "object": "process"
+                            }
+                        },
+                        "profiles": {
+                            "key": "x-ocsf-cloud.profiles",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "raw_data": {
+                            "key": "x-ocsf-cloud.raw_data",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "ref_event_code": {
+                            "key": "x-ocsf-cloud.ref_event_code",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "ref_event_name": {
+                            "key": "x-ocsf-cloud.ref_event_name",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "ref_event_uid": {
+                            "key": "x-ocsf-cloud.ref_event_uid",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "ref_time": {
+                            "key": "x-ocsf-cloud.ref_time",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "resources": {
+                            "account_uid": [
+                                {
+                                    "key": "x-ocsf-resources.account_uid",
+                                    "object": "resources"
+                                },
+                                {
+                                    "key": "x-ocsf-resources.cloud_api_ref",
+                                    "object": "resources",
+                                    "references": "ocsf_cloud_api"
+                                }
+                            ],
+                            "cloud_partition": {
+                                "key": "x-ocsf-resources.cloud_partition",
+                                "object": "resources"
+                            },
+                            "criticality": {
+                                "key": "x-ocsf-resources.criticality",
+                                "object": "resources"
+                            },
+                            "details": {
+                                "key": "x-ocsf-resources.details",
+                                "object": "resources"
+                            },
+                            "group_name": {
+                                "key": "x-ocsf-resources.group_name",
+                                "object": "resources"
+                            },
+                            "labels": {
+                                "key": "x-ocsf-resources.labels",
+                                "object": "resources"
                             },
-                            "status": {
-                                "key": "x-ocsf-cloud.status",
-                                "object": "ocsf_cloud_api"
+                            "name": {
+                                "key": "x-ocsf-resources.name",
+                                "object": "resources"
                             },
-                            "status_code": {
-                                "key": "x-ocsf-cloud.status_code",
-                                "object": "ocsf_cloud_api"
+                            "owner": {
+                                "key": "x-ocsf-resources.owner",
+                                "object": "resources"
                             },
-                            "status_detail": {
-                                "key": "x-ocsf-cloud.status_detail",
-                                "object": "ocsf_cloud_api"
+                            "region": {
+                                "key": "x-ocsf-resources.region",
+                                "object": "resources"
                             },
-                            "status_id": {
-                                "key": "x-ocsf-cloud.status_id",
-                                "object": "ocsf_cloud_api",
-                                "transformer": "ToInteger"
+                            "type": {
+                                "key": "x-ocsf-resources.type",
+                                "object": "resources"
                             },
-                            "time": {
-                                "key": "x-oca-event.created",
-                                "object": "x_oca_event"
-                            },
-                            "timezone_offset": {
-                                "key": "x-oca-event.timezone",
-                                "object": "x_oca_event",
-                                "transformer": "ToInteger"
+                            "uid": {
+                                "key": "x-ocsf-resources.uid",
+                                "object": "resources"
+                            }
+                        },
+                        "severity": {
+                            "key": "x-ocsf-cloud.severity",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "severity_id": {
+                            "key": "x-ibm-finding.severity",
+                            "object": "ibm_finding",
+                            "transformer": "ToInteger"
+                        },
+                        "src_endpoint": {
+                            "instance_uid": {
+                                "key": "x-oca-asset.extensions.x-src-endpoint.instance_uid",
+                                "object": "asset"
+                            },
+                            "interface_uid": {
+                                "key": "x-oca-asset.extensions.x-src-endpoint.interface_uid",
+                                "object": "asset"
                             },
-                            "traffic": {
-                                "bytes": {
-                                    "key": "network-traffic.extensions.x-network-ext.bytes",
-                                    "object": "nt"
-                                },
-                                "bytes_in": {
-                                    "key": "network-traffic.dst_byte_count",
-                                    "object": "nt"
-                                },
-                                "bytes_out": {
-                                    "key": "network-traffic.src_byte_count",
-                                    "object": "nt"
-                                },
-                                "packets": {
-                                    "key": "network-traffic.extensions.x-network-ext.packets",
-                                    "object": "nt"
-                                },
-                                "packets_in": {
-                                    "key": "network-traffic.dst_packets",
-                                    "object": "nt"
-                                },
-                                "packets_out": {
-                                    "key": "network-traffic.src_packets",
-                                    "object": "nt"
+                            "intermediate_ips": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "src_ipv4",
+                                    "transformer": "FilterIPv4List",
+                                    "unwrap": true
+                                },
+                                {
+                                    "key": "ipv6-addr.value",
+                                    "object": "src_ipv6",
+                                    "transformer": "FilterIPv6List",
+                                    "unwrap": true
+                                },
+                                {
+                                    "key": "x-oca-asset.ip_refs",
+                                    "object": "asset",
+                                    "references": [
+                                        "src_ipv4",
+                                        "src_ipv6"
+                                    ],
+                                    "unwrap": true
                                 }
+                            ],
+                            "ip": [
+                                {
+                                    "key": "ipv4-addr.value",
+                                    "object": "src_ip",
+                                    "transformer": "CheckIPv4"
+                                },
+                                {
+                                    "key": "ipv6-addr.value",
+                                    "object": "src_ip",
+                                    "transformer": "CheckIPv6"
+                                },
+                                {
+                                    "key": "network-traffic.src_ref",
+                                    "object": "nt",
+                                    "references": "src_ip"
+                                },
+                                {
+                                    "key": "x-ibm-finding.src_ip_ref",
+                                    "object": "ibm_finding",
+                                    "references": "src_ip"
+                                },
+                                {
+                                    "group": true,
+                                    "key": "x-oca-asset.ip_refs",
+                                    "object": "host",
+                                    "references": [
+                                        "src_ip"
+                                    ]
+                                },
+                                {
+                                    "key": "x-oca-event.network_ref",
+                                    "object": "event",
+                                    "references": "nt"
+                                }
+                            ],
+                            "name": {
+                                "key": "x-oca-asset.name",
+                                "object": "asset"
                             },
-                            "type_name": {
-                                "key": "x-ocsf-cloud.type_name",
-                                "object": "ocsf_cloud_api"
-                            },
-                            "type_uid": {
-                                "key": "x-ocsf-cloud.type_uid",
-                                "object": "ocsf_cloud_api",
+                            "port": {
+                                "key": "network-traffic.src_port",
+                                "object": "nt",
                                 "transformer": "ToInteger"
                             },
-                            "vulnerabilities": {
-                                "cve": {
-                                    "created_time": {
-                                        "key": "x-ocsf-vulnerabilities.created_time",
+                            "subnet_uid": {
+                                "key": "x-oca-asset.extensions.x-src-endpoint.subnet_uid",
+                                "object": "asset"
+                            },
+                            "svc_name": {
+                                "key": "x-oca-asset.extensions.x-src-endpoint.svc_name",
+                                "object": "asset"
+                            },
+                            "vpc_uid": {
+                                "key": "x-oca-asset.extensions.x-src-endpoint.vpc_uid",
+                                "object": "asset"
+                            }
+                        },
+                        "start_time": {
+                            "key": "first_observed",
+                            "transformer": "EpochToTimestamp"
+                        },
+                        "status": {
+                            "key": "x-ocsf-cloud.status",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "status_code": {
+                            "key": "x-ocsf-cloud.status_code",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "status_detail": {
+                            "key": "x-ocsf-cloud.status_detail",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "status_id": {
+                            "key": "x-ocsf-cloud.status_id",
+                            "object": "ocsf_cloud_api",
+                            "transformer": "ToInteger"
+                        },
+                        "time": {
+                            "key": "x-oca-event.created",
+                            "object": "x_oca_event"
+                        },
+                        "timezone_offset": {
+                            "key": "x-oca-event.timezone",
+                            "object": "x_oca_event",
+                            "transformer": "ToInteger"
+                        },
+                        "traffic": {
+                            "bytes": {
+                                "key": "network-traffic.extensions.x-network-ext.bytes",
+                                "object": "nt"
+                            },
+                            "bytes_in": {
+                                "key": "network-traffic.dst_byte_count",
+                                "object": "nt"
+                            },
+                            "bytes_out": {
+                                "key": "network-traffic.src_byte_count",
+                                "object": "nt"
+                            },
+                            "packets": {
+                                "key": "network-traffic.extensions.x-network-ext.packets",
+                                "object": "nt"
+                            },
+                            "packets_in": {
+                                "key": "network-traffic.dst_packets",
+                                "object": "nt"
+                            },
+                            "packets_out": {
+                                "key": "network-traffic.src_packets",
+                                "object": "nt"
+                            }
+                        },
+                        "type_name": {
+                            "key": "x-ocsf-cloud.type_name",
+                            "object": "ocsf_cloud_api"
+                        },
+                        "type_uid": {
+                            "key": "x-ocsf-cloud.type_uid",
+                            "object": "ocsf_cloud_api",
+                            "transformer": "ToInteger"
+                        },
+                        "vulnerabilities": {
+                            "cve": {
+                                "created_time": {
+                                    "key": "x-ocsf-vulnerabilities.created_time",
+                                    "object": "vulnerabilities"
+                                },
+                                "cvss": {
+                                    "base_score": {
+                                        "key": "x-ocsf-vulnerabilities.base_score",
                                         "object": "vulnerabilities"
                                     },
-                                    "cvss": {
-                                        "base_score": {
-                                            "key": "x-ocsf-vulnerabilities.base_score",
-                                            "object": "vulnerabilities"
-                                        },
-                                        "depth": {
-                                            "key": "x-ocsf-vulnerabilities.depth",
-                                            "object": "vulnerabilities"
-                                        },
-                                        "metrics": {
-                                            "name": {
-                                                "key": "x-ocsf-vulnerabilities.name",
-                                                "object": "vulnerabilities"
-                                            },
-                                            "value": {
-                                                "key": "x-ocsf-vulnerabilities.value",
-                                                "object": "vulnerabilities"
-                                            }
-                                        },
-                                        "overall_score": {
-                                            "key": "x-ocsf-vulnerabilities.overall_score",
-                                            "object": "vulnerabilities"
-                                        },
-                                        "severity": {
-                                            "key": "x-ocsf-vulnerabilities.severity",
-                                            "object": "vulnerabilities"
-                                        },
-                                        "vector_string": {
-                                            "key": "x-ocsf-vulnerabilities.vector_string",
+                                    "depth": {
+                                        "key": "x-ocsf-vulnerabilities.depth",
+                                        "object": "vulnerabilities"
+                                    },
+                                    "metrics": {
+                                        "name": {
+                                            "key": "x-ocsf-vulnerabilities.name",
                                             "object": "vulnerabilities"
                                         },
-                                        "version": {
-                                            "key": "x-ocsf-vulnerabilities.version",
+                                        "value": {
+                                            "key": "x-ocsf-vulnerabilities.value",
                                             "object": "vulnerabilities"
                                         }
                                     },
-                                    "cwe_uid": {
-                                        "key": "x-ocsf-vulnerabilities.cwe_uid",
+                                    "overall_score": {
+                                        "key": "x-ocsf-vulnerabilities.overall_score",
                                         "object": "vulnerabilities"
                                     },
-                                    "cwe_url": {
-                                        "key": "x-ocsf-vulnerabilities.cwe_url",
+                                    "severity": {
+                                        "key": "x-ocsf-vulnerabilities.severity",
                                         "object": "vulnerabilities"
                                     },
-                                    "modified_time": {
-                                        "key": "x-ocsf-vulnerabilities.modified_time",
+                                    "vector_string": {
+                                        "key": "x-ocsf-vulnerabilities.vector_string",
                                         "object": "vulnerabilities"
                                     },
-                                    "product": {
-                                        "feature": {
-                                            "name": {
-                                                "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                                "object": "vulnerabilities-software"
-                                            },
-                                            "uid": {
-                                                "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                                "object": "vulnerabilities-software"
-                                            },
-                                            "version": {
-                                                "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                                "object": "vulnerabilities-software"
-                                            }
-                                        },
-                                        "lang": {
-                                            "key": "software.languages",
-                                            "object": "vulnerabilities-software"
-                                        },
+                                    "version": {
+                                        "key": "x-ocsf-vulnerabilities.version",
+                                        "object": "vulnerabilities"
+                                    }
+                                },
+                                "cwe_uid": {
+                                    "key": "x-ocsf-vulnerabilities.cwe_uid",
+                                    "object": "vulnerabilities"
+                                },
+                                "cwe_url": {
+                                    "key": "x-ocsf-vulnerabilities.cwe_url",
+                                    "object": "vulnerabilities"
+                                },
+                                "modified_time": {
+                                    "key": "x-ocsf-vulnerabilities.modified_time",
+                                    "object": "vulnerabilities"
+                                },
+                                "product": {
+                                    "feature": {
                                         "name": {
-                                            "key": "software.name",
-                                            "object": "vulnerabilities-software"
-                                        },
-                                        "path": {
-                                            "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                                            "key": "software.extensions.x-ocsf-product-ext.feature_name",
                                             "object": "vulnerabilities-software"
                                         },
                                         "uid": {
-                                            "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                                            "object": "vulnerabilities-software"
-                                        },
-                                        "vendor_name": {
-                                            "key": "software.vendor",
+                                            "key": "software.extensions.x-ocsf-product-ext.feature_uid",
                                             "object": "vulnerabilities-software"
                                         },
                                         "version": {
-                                            "key": "software.version",
+                                            "key": "software.extensions.x-ocsf-product-ext.feature_version",
                                             "object": "vulnerabilities-software"
                                         }
                                     },
-                                    "type": {
-                                        "key": "x-ocsf-vulnerabilities.type",
-                                        "object": "vulnerabilities"
-                                    },
-                                    "uid": {
-                                        "key": "x-ocsf-vulnerabilities.uid",
-                                        "object": "vulnerabilities"
-                                    }
-                                },
-                                "desc": {
-                                    "key": "x-ocsf-vulnerabilities.desc",
-                                    "object": "vulnerabilities"
-                                },
-                                "kb_articles": {
-                                    "key": "x-ocsf-vulnerabilities.kb_articles",
-                                    "object": "vulnerabilities"
-                                },
-                                "packages": {
-                                    "architecture": {
-                                        "key": "x-ocsf-vulnerabilities.packages_architecture",
-                                        "object": "vulnerabilities"
+                                    "lang": {
+                                        "key": "software.languages",
+                                        "object": "vulnerabilities-software"
                                     },
-                                    "epoch": {
-                                        "key": "x-ocsf-vulnerabilities.packages_epoch",
-                                        "object": "vulnerabilities"
+                                    "name": {
+                                        "key": "software.name",
+                                        "object": "vulnerabilities-software"
                                     },
-                                    "license": {
-                                        "key": "x-ocsf-vulnerabilities.packages_license",
-                                        "object": "vulnerabilities"
+                                    "path": {
+                                        "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                                        "object": "vulnerabilities-software"
                                     },
-                                    "name": {
-                                        "key": "x-ocsf-vulnerabilities.packages_name",
-                                        "object": "vulnerabilities"
+                                    "uid": {
+                                        "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                                        "object": "vulnerabilities-software"
                                     },
-                                    "release": {
-                                        "key": "x-ocsf-vulnerabilities.packages_release",
-                                        "object": "vulnerabilities"
+                                    "vendor_name": {
+                                        "key": "software.vendor",
+                                        "object": "vulnerabilities-software"
                                     },
                                     "version": {
-                                        "key": "x-ocsf-vulnerabilities.packages_version",
-                                        "object": "vulnerabilities"
+                                        "key": "software.version",
+                                        "object": "vulnerabilities-software"
                                     }
                                 },
-                                "references": {
-                                    "key": "x-ocsf-vulnerabilities.references",
+                                "type": {
+                                    "key": "x-ocsf-vulnerabilities.type",
                                     "object": "vulnerabilities"
                                 },
-                                "related_vulnerabilities": {
-                                    "key": "x-ocsf-vulnerabilities.related_vulnerabilities",
+                                "uid": {
+                                    "key": "x-ocsf-vulnerabilities.uid",
                                     "object": "vulnerabilities"
-                                },
-                                "severity": {
-                                    "key": "x-ocsf-vulnerabilities.severity",
+                                }
+                            },
+                            "desc": {
+                                "key": "x-ocsf-vulnerabilities.desc",
+                                "object": "vulnerabilities"
+                            },
+                            "kb_articles": {
+                                "key": "x-ocsf-vulnerabilities.kb_articles",
+                                "object": "vulnerabilities"
+                            },
+                            "packages": {
+                                "architecture": {
+                                    "key": "x-ocsf-vulnerabilities.packages_architecture",
                                     "object": "vulnerabilities"
                                 },
-                                "title": {
-                                    "key": "x-ocsf-vulnerabilities.title",
+                                "epoch": {
+                                    "key": "x-ocsf-vulnerabilities.packages_epoch",
                                     "object": "vulnerabilities"
                                 },
-                                "vendor_name": {
-                                    "key": "x-ocsf-vulnerabilities.vendor_name",
+                                "license": {
+                                    "key": "x-ocsf-vulnerabilities.packages_license",
                                     "object": "vulnerabilities"
-                                }
-                            }
-                        },
-                        "vpcflow": {
-                            "account": [
-                                {
-                                    "key": "x-aws-details.account_id",
-                                    "object": "accountid"
-                                }
-                            ],
-                            "action": {
-                                "key": "x-ibm-finding.finding_type",
-                                "object": "ibm_finding"
-                            },
-                            "destinationaddress": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "dst_ip"
                                 },
-                                {
-                                    "key": "ipv6-addr.value",
-                                    "object": "dst_ip"
-                                },
-                                {
-                                    "key": "x-ibm-finding.dst_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "dst_ip"
-                                },
-                                {
-                                    "key": "network-traffic.dst_ref",
-                                    "object": "nt",
-                                    "references": "dst_ip"
-                                }
-                            ],
-                            "destinationport": [
-                                {
-                                    "key": "network-traffic.dst_port",
-                                    "object": "nt",
-                                    "transformer": "ToInteger"
-                                }
-                            ],
-                            "endtime": [
-                                {
-                                    "key": "network-traffic.end",
-                                    "object": "nt",
-                                    "transformer": "EpochSecondsToTimestamp"
+                                "name": {
+                                    "key": "x-ocsf-vulnerabilities.packages_name",
+                                    "object": "vulnerabilities"
                                 },
-                                {
-                                    "key": "x-ibm-finding.end",
-                                    "object": "ibm_finding",
-                                    "transformer": "EpochSecondsToTimestamp"
+                                "release": {
+                                    "key": "x-ocsf-vulnerabilities.packages_release",
+                                    "object": "vulnerabilities"
                                 },
-                                {
-                                    "key": "last_observed",
-                                    "transformer": "EpochToTimestamp"
+                                "version": {
+                                    "key": "x-ocsf-vulnerabilities.packages_version",
+                                    "object": "vulnerabilities"
                                 }
-                            ],
-                            "name": {
-                                "key": "x-ibm-finding.name",
-                                "object": "ibm_finding"
                             },
-                            "protocol": [
-                                {
-                                    "key": "network-traffic.protocols",
-                                    "object": "nt",
-                                    "transformer": "ToLowercaseArray"
-                                }
-                            ],
-                            "sourceaddress": [
-                                {
-                                    "key": "ipv4-addr.value",
-                                    "object": "src_ip"
-                                },
-                                {
-                                    "key": "ipv6-addr.value",
-                                    "object": "src_ip"
-                                },
-                                {
-                                    "key": "network-traffic.src_ref",
-                                    "object": "nt",
-                                    "references": "src_ip"
-                                },
-                                {
-                                    "key": "x-ibm-finding.src_ip_ref",
-                                    "object": "ibm_finding",
-                                    "references": "src_ip"
-                                },
-                                {
-                                    "ds_key": "interfaceid",
-                                    "key": "ipv4-addr.x_aws_interface_id",
-                                    "object": "src_ip"
-                                },
-                                {
-                                    "ds_key": "interfaceid",
-                                    "key": "ipv6-addr.x_aws_interface_id",
-                                    "object": "src_ip"
-                                }
-                            ],
-                            "sourceport": [
-                                {
-                                    "key": "network-traffic.src_port",
-                                    "object": "nt",
-                                    "transformer": "ToInteger"
-                                }
-                            ],
-                            "starttime": [
-                                {
-                                    "key": "network-traffic.start",
-                                    "object": "nt",
-                                    "transformer": "EpochSecondsToTimestamp"
-                                },
-                                {
-                                    "key": "x-ibm-finding.start",
-                                    "object": "ibm_finding",
-                                    "transformer": "EpochSecondsToTimestamp"
-                                },
-                                {
-                                    "key": "first_observed",
-                                    "transformer": "EpochSecondsToTimestamp"
-                                }
-                            ]
+                            "references": {
+                                "key": "x-ocsf-vulnerabilities.references",
+                                "object": "vulnerabilities"
+                            },
+                            "related_vulnerabilities": {
+                                "key": "x-ocsf-vulnerabilities.related_vulnerabilities",
+                                "object": "vulnerabilities"
+                            },
+                            "severity": {
+                                "key": "x-ocsf-vulnerabilities.severity",
+                                "object": "vulnerabilities"
+                            },
+                            "title": {
+                                "key": "x-ocsf-vulnerabilities.title",
+                                "object": "vulnerabilities"
+                            },
+                            "vendor_name": {
+                                "key": "x-ocsf-vulnerabilities.vendor_name",
+                                "object": "vulnerabilities"
+                            }
                         }
                     },
+                    "operators": {
+                        "ComparisonComparators.Equal": "=",
+                        "ComparisonComparators.GreaterThan": ">",
+                        "ComparisonComparators.GreaterThanOrEqual": ">=",
+                        "ComparisonComparators.In": "IN",
+                        "ComparisonComparators.LessThan": "<",
+                        "ComparisonComparators.LessThanOrEqual": "<=",
+                        "ComparisonComparators.Like": "LIKE",
+                        "ComparisonComparators.Matches": "REGEXP_LIKE",
+                        "ComparisonComparators.NotEqual": "!=",
+                        "ComparisonExpressionOperators.And": "AND",
+                        "ComparisonExpressionOperators.Or": "OR",
+                        "ObservationOperators.And": "INTERSECT",
+                        "ObservationOperators.Or": "UNION"
+                    },
                     "vpcflow_from_stix_map": {
                         "ipv4-addr": {
                             "fields": {
                                 "value": [
-                                    "sourceaddress",
-                                    "destinationaddress"
+                                    "srcaddr",
+                                    "dstaddr"
                                 ],
                                 "x_aws_interface_id": [
-                                    "interfaceId"
+                                    "interface_id"
                                 ]
                             }
                         },
                         "ipv6-addr": {
                             "fields": {
                                 "value": [
-                                    "sourceaddress",
-                                    "destinationaddress"
+                                    "srcaddr",
+                                    "dstaddr"
                                 ],
                                 "x_aws_interface_id": [
-                                    "interfaceid"
+                                    "interface_id"
                                 ]
                             }
                         },
                         "network-traffic": {
                             "fields": {
                                 "dst_port": [
-                                    "destinationport"
+                                    "dstport"
                                 ],
                                 "dst_ref.value": [
-                                    "destinationaddress"
+                                    "dstaddr"
                                 ],
                                 "end": [
                                     "endtime"
                                 ],
                                 "protocols[*]": [
                                     "protocol"
                                 ],
                                 "src_port": [
-                                    "sourceport"
+                                    "srcport"
                                 ],
                                 "src_ref.value": [
-                                    "sourceaddress"
+                                    "srcaddr"
                                 ],
                                 "start": [
                                     "starttime"
                                 ]
                             }
                         },
                         "x-aws-details": {
@@ -4468,30 +4347,149 @@
                                     "account"
                                 ]
                             }
                         },
                         "x-ibm-finding": {
                             "fields": {
                                 "dst_ip_ref.value": [
-                                    "destinationaddress"
+                                    "dstaddr"
                                 ],
                                 "end": [
                                     "endtime"
                                 ],
                                 "finding_type": [
                                     "action"
                                 ],
                                 "src_ip_ref.value": [
-                                    "sourceaddress"
+                                    "srcaddr"
                                 ],
                                 "start": [
                                     "starttime"
                                 ]
                             }
                         }
+                    },
+                    "vpcflow_to_stix_map": {
+                        "account": [
+                            {
+                                "key": "x-aws-details.account_id",
+                                "object": "accountid"
+                            }
+                        ],
+                        "action": {
+                            "key": "x-ibm-finding.finding_type",
+                            "object": "ibm_finding"
+                        },
+                        "dstaddr": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "dst_ip"
+                            },
+                            {
+                                "key": "ipv6-addr.value",
+                                "object": "dst_ip"
+                            },
+                            {
+                                "key": "x-ibm-finding.dst_ip_ref",
+                                "object": "ibm_finding",
+                                "references": "dst_ip"
+                            },
+                            {
+                                "key": "network-traffic.dst_ref",
+                                "object": "nt",
+                                "references": "dst_ip"
+                            }
+                        ],
+                        "dstport": [
+                            {
+                                "key": "network-traffic.dst_port",
+                                "object": "nt",
+                                "transformer": "ToInteger"
+                            }
+                        ],
+                        "endtime": [
+                            {
+                                "key": "network-traffic.end",
+                                "object": "nt",
+                                "transformer": "EpochSecondsToTimestamp"
+                            },
+                            {
+                                "key": "x-ibm-finding.end",
+                                "object": "ibm_finding",
+                                "transformer": "EpochSecondsToTimestamp"
+                            },
+                            {
+                                "key": "last_observed",
+                                "transformer": "EpochToTimestamp"
+                            }
+                        ],
+                        "name": {
+                            "key": "x-ibm-finding.name",
+                            "object": "ibm_finding"
+                        },
+                        "protocol": [
+                            {
+                                "key": "network-traffic.protocols",
+                                "object": "nt",
+                                "transformer": "ToLowercaseArray"
+                            }
+                        ],
+                        "srcaddr": [
+                            {
+                                "key": "ipv4-addr.value",
+                                "object": "src_ip"
+                            },
+                            {
+                                "key": "ipv6-addr.value",
+                                "object": "src_ip"
+                            },
+                            {
+                                "key": "network-traffic.src_ref",
+                                "object": "nt",
+                                "references": "src_ip"
+                            },
+                            {
+                                "key": "x-ibm-finding.src_ip_ref",
+                                "object": "ibm_finding",
+                                "references": "src_ip"
+                            },
+                            {
+                                "ds_key": "interface_id",
+                                "key": "ipv4-addr.x_aws_interface_id",
+                                "object": "src_ip"
+                            },
+                            {
+                                "ds_key": "interface_id",
+                                "key": "ipv6-addr.x_aws_interface_id",
+                                "object": "src_ip"
+                            }
+                        ],
+                        "srcport": [
+                            {
+                                "key": "network-traffic.src_port",
+                                "object": "nt",
+                                "transformer": "ToInteger"
+                            }
+                        ],
+                        "starttime": [
+                            {
+                                "key": "network-traffic.start",
+                                "object": "nt",
+                                "transformer": "EpochSecondsToTimestamp"
+                            },
+                            {
+                                "key": "x-ibm-finding.start",
+                                "object": "ibm_finding",
+                                "transformer": "EpochSecondsToTimestamp"
+                            },
+                            {
+                                "key": "first_observed",
+                                "transformer": "EpochSecondsToTimestamp"
+                            }
+                        ]
                     }
                 },
                 "optional": true,
                 "previous": "connection.mapping",
                 "type": "json"
             },
             "result_limit": {
```

## stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py

```diff
@@ -118,22 +118,22 @@
                 if not match(str(stix_value)):
                     return False
             return True
         except Exception as e:
             self.logger.debug("Failed to validate STIX property '{}' with value '{}'. Exception: {}".format(observable_key, stix_value, e))
             return False
 
-    def _compose_value_object(self, value, key_list, observable_key=None, object_tag_ref_map=None, transformer=None, references=None, unwrap=False):
+    def _compose_value_object(self, value, key_list, observable_key=None, object_tag_ref_map=None, transformer=None, references=None, unwrap=False, is_group_ref=False):
         """
         Converts the value of the data to STIX valid value
         """
         try:
             return_value = {}
             for key in key_list:
-                return_value[key] = self._compose_value_object(value, key_list[1:], observable_key=observable_key, object_tag_ref_map=object_tag_ref_map, transformer=transformer, references=references, unwrap=unwrap)
+                return_value[key] = self._compose_value_object(value, key_list[1:], observable_key=observable_key, object_tag_ref_map=object_tag_ref_map, transformer=transformer, references=references, unwrap=unwrap, is_group_ref=is_group_ref)
                 break
             else:
                 if transformer:
                     try: 
                         value = transformer.transform(value)
                         if value is None:
                             return None
@@ -141,21 +141,39 @@
                         return None
                 
                 if references:
                     if isinstance(references, list):
                         return_value = []
                         for ref in references:
                             if not isinstance(value, list):
-                                value = [value]
-                            for i, _ in enumerate(value):
-                                parent_key_ind = self._get_tag_ind(ref, object_tag_ref_map, create_on_absence=False, unwrap=i)
+                                # Fetch the index of reference object name which has a single value.
+                                parent_key_ind = self._get_tag_ind(ref, object_tag_ref_map, create_on_absence=False)
                                 if parent_key_ind:
                                     return_value.append(parent_key_ind)
+                            else:
+                                for i, _ in enumerate(value):
+                                    parent_key_ind = self._get_tag_ind(ref, object_tag_ref_map, create_on_absence=False, unwrap=str(i))
+                                    if parent_key_ind:
+                                        return_value.append(parent_key_ind)
+                                    # Iterate through the object_tag_ref_map to fetch the index, for grouping
+                                    # reference objects of nested type through group_ref.
+                                    elif is_group_ref:
+                                        list_parent_ind = ref + '_' + str(i)
+                                        for key, val in object_tag_ref_map['tags'].items():
+                                            if key.startswith(list_parent_ind):
+                                                return_value.append(
+                                                    self._get_tag_ind(key, object_tag_ref_map, create_on_absence=False))
+
                     else:
-                        return_value = self._get_tag_ind(references, object_tag_ref_map, create_on_absence=False)
+                        # Fetch first object (index 0) for single reference when the value is of type list .
+                        if isinstance(value, list):
+                            return_value = self._get_tag_ind(references, object_tag_ref_map, create_on_absence=False,
+                                                             unwrap='0')
+                        else:
+                            return_value = self._get_tag_ind(references, object_tag_ref_map, create_on_absence=False)
                         # if the property has unwrap true and is not a list, convert to list
                         if unwrap is True and not isinstance(return_value, list):
                             return_value = [return_value]
 
                     if not return_value:
                         return None
                 else:
@@ -247,28 +265,38 @@
                 if isinstance(to_stix_config_prop, dict) and to_stix_config_prop.get('key') is not None and not isinstance(to_stix_config_prop.get('key'), dict):
                     # data variable is the final value, process in bulk
                     self._handle_value(data, parent_data, ds_sub_key, to_stix_config_prop, objects, object_tag_ref_map, object_key_ind)
 
                 elif isinstance(data, list):
                     for i, d in enumerate(data):
                         if isinstance(d, list) or isinstance(d, dict):
-                            self._handle_properties(to_stix_config_prop, d, objects, object_tag_ref_map, data, ds_sub_key, i)
+                            # Added parent key indexes to inner objects in order to handle nested lists of
+                            # dictionaries and lists. For Example, if a list of IP address is present inside
+                            # a list of network objects, then without adding this code, only the IP address information
+                            # in the first network object will be created and the rest are not created.
+                            if object_key_ind:
+                                i = str(object_key_ind) + '_' + str(i)
+                            # Inorder to include 0th index, the integer field 'i' is converted to string.
+                            self._handle_properties(to_stix_config_prop, d, objects, object_tag_ref_map, data, ds_sub_key, str(i))
                         else:
                             # data variable is the final value, process in bulk
                             self._handle_value(data, parent_data, ds_sub_key, to_stix_config_prop, objects, object_tag_ref_map, object_key_ind)
                             break
                     # group the references of list of dictionary field
                     if isinstance(to_stix_config_prop, dict):
                         group_refs = [key for key, value in to_stix_config_prop.items() if
                                       isinstance(value, dict) and value.get('group_ref') and value.get(
                                           'references')]
                         for group_ref in group_refs:
+                            # Added a new boolean (True) parameter (is_group_ref) to indicate grouping of references
+                            # through group_ref key in mapping
                             self._handle_value(data, to_stix_config_prop, ds_sub_key,
                                                to_stix_config_prop[group_ref],
-                                               objects, object_tag_ref_map, object_key_ind)
+                                               objects, object_tag_ref_map, object_key_ind, True)
+
                 elif isinstance(data, dict):
                     for k in data:
                         cust_prop = None
                         if k in to_stix_config_prop:
                             cust_prop = to_stix_config_prop[k]
                         elif self.options.get('unmapped_fallback') and k not in object_tag_ref_map['ds_key_cybox']:
                             cust_prop = {"key": "x-" + self.data_source.replace("_", "-") + "." + k, "object": "cust_object"}
@@ -277,15 +305,15 @@
                             self._handle_properties(cust_prop, data[k], objects, object_tag_ref_map, data, k, object_key_ind)
                 else:
                     self._handle_value(data, parent_data, ds_sub_key, to_stix_config_prop, objects, object_tag_ref_map, object_key_ind)
         except Exception as e:
             raise Exception("Error in json_to_stix_translator._handle_properties: %s" % e)
 
 
-    def _handle_value(self, data, parent_data, ds_sub_key, to_stix_config_prop, objects, object_tag_ref_map, object_key_ind=None):
+    def _handle_value(self, data, parent_data, ds_sub_key, to_stix_config_prop, objects, object_tag_ref_map, object_key_ind=None, is_group_ref=False):
         """
         Receives the raw value of a data property, converts to a STIX valid value and adds to the cached observable `objects` dictionary
         """
         try: 
             if isinstance(to_stix_config_prop, dict):
                 props = [to_stix_config_prop]
             else:
@@ -294,14 +322,29 @@
             for prop in props:
                 key = prop.get('key', None)
                 if key is None:
                     continue
 
                 transformer = self.transformers[prop['transformer']] if 'transformer' in prop else None
                 references = references = prop['references'] if 'references' in prop else None
+
+                # This check avoid using duplicate reference in the multiple objects of the same type.
+                # For example: If there are multiple source ipv4-addr and network-traffic objects then
+                # without this reference check the first source ipv4-addr object will be referenced to all network-traffic objects.
+                if references:
+                    if isinstance(references, str):
+                        if object_key_ind:
+                            references = references + '_' + str(object_key_ind)
+                        elif not isinstance(data, list):
+                            references = references + '_' + '0'
+                    elif isinstance(references, list):
+                        if object_key_ind:
+                            references = [ref + '_' + str(object_key_ind) for ref in references]
+                        elif not isinstance(data, list):
+                            references = [ref + '_' + '0' for ref in references]
                 # unwrap array of stix values to separate stix objects
                 unwrap = True if 'unwrap' in prop and isinstance(data, list) else False
                 if "." in key:
                     cybox = True
                 else:
                     cybox = False
                 
@@ -334,33 +377,44 @@
                     if False is cybox and not substitute_key:
                         value = self._compose_value_object(data, config_keys[2:], observable_key=key, object_tag_ref_map=object_tag_ref_map, transformer=transformer, references=references, unwrap=unwrap)
                         self._add_property(type_name, property_key, type_name, value, object_tag_ref_map['out_cybox'], cybox=False)
                         continue
 
                     if object_key_ind:
                         parent_key = parent_key + '_' + str(object_key_ind)
+                    # Adding _0 as a tag index for the following
+                    # 1. For object name of non-list type data or unwrapped data
+                    # 2. For the object name containing references to list type of data.
+                    # For Example, when a single IP address value and references to the list of domain values, needs
+                    # to be added to a single custom object, the 0th index is added to the custom object to have ip
+                    # address and references to list of domains under the same custom object.
+                    elif (isinstance(data, list) and not unwrap and not references) \
+                            or (isinstance(data, list) and references) or (not isinstance(data, list)):
+                        parent_key = parent_key + '_' + '0'
 
                     # use the hard-coded value in the mapping
                     if 'value' in prop:
                         value = prop['value']
                     else:
                         if substitute_key and parent_data:
                             data = parent_data.get(substitute_key)
 
                             if False is cybox:
                                 object_tag_ref_map['ds_key_cybox'][substitute_key] = True
                         
-                        value = self._compose_value_object(data, config_keys[2:], observable_key=key, object_tag_ref_map=object_tag_ref_map, transformer=transformer, references=references, unwrap=unwrap)
+                        value = self._compose_value_object(data, config_keys[2:], observable_key=key, object_tag_ref_map=object_tag_ref_map, transformer=transformer, references=references, unwrap=unwrap, is_group_ref=is_group_ref)
 
-                    if value is None or value == '':
+                    # Remove the values which has empty list brackets.
+                    if value is None or value in ('', []):
                         continue
 
                     if not references and unwrap and isinstance(value, list):
                         for i, val_el in enumerate(value):
-                            parent_key_ind = self._get_tag_ind(parent_key, object_tag_ref_map, create_on_absence=True, unwrap=i, property_key=property_key)
+                            # Inorder to include 0th index, the integer field 'i' is converted to string.
+                            parent_key_ind = self._get_tag_ind(parent_key, object_tag_ref_map, create_on_absence=True, unwrap=str(i), property_key=property_key)
                             self._add_property(type_name, property_key, parent_key_ind, val_el, objects, group=group)
                     else:
                         parent_key_ind = self._get_tag_ind(parent_key, object_tag_ref_map, create_on_absence=True, property_key=property_key)
                         self._add_property(type_name, property_key, parent_key_ind, value, objects, group=group)
         except Exception as e:
             raise Exception("Error in json_to_stix_translator._handle_value: %s : %s" % (e, e.__traceback__.tb_lineno))
```

## stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json

### Pretty-printed

 * *Similarity: 0.9257142857142858%*

 * *Differences: {"'ipv4-addr'": "{'fields': {'value': ['srcaddr', 'dstaddr'], 'x_aws_interface_id': "*

 * *                "['interface_id']}}",*

 * * "'ipv6-addr'": "{'fields': {'value': ['srcaddr', 'dstaddr'], 'x_aws_interface_id': "*

 * *                "['interface_id']}}",*

 * * "'network-traffic'": "{'fields': {'src_port': ['srcport'], 'dst_port': ['dstport'], "*

 * *                      "'src_ref.value': ['srcaddr'], 'dst_ref.value': ['dstaddr']}}",*

 * * "'x-ibm-finding'": "{'fields': {'src_ip_ref.value': ['srcaddr'], 'dst_ip_ref.value': "*

 * *    […]*

```diff
@@ -1,49 +1,49 @@
 {
     "ipv4-addr": {
         "fields": {
             "value": [
-                "sourceaddress",
-                "destinationaddress"
+                "srcaddr",
+                "dstaddr"
             ],
             "x_aws_interface_id": [
-                "interfaceId"
+                "interface_id"
             ]
         }
     },
     "ipv6-addr": {
         "fields": {
             "value": [
-                "sourceaddress",
-                "destinationaddress"
+                "srcaddr",
+                "dstaddr"
             ],
             "x_aws_interface_id": [
-                "interfaceid"
+                "interface_id"
             ]
         }
     },
     "network-traffic": {
         "fields": {
             "dst_port": [
-                "destinationport"
+                "dstport"
             ],
             "dst_ref.value": [
-                "destinationaddress"
+                "dstaddr"
             ],
             "end": [
                 "endtime"
             ],
             "protocols[*]": [
                 "protocol"
             ],
             "src_port": [
-                "sourceport"
+                "srcport"
             ],
             "src_ref.value": [
-                "sourceaddress"
+                "srcaddr"
             ],
             "start": [
                 "starttime"
             ]
         }
     },
     "x-aws-details": {
@@ -52,24 +52,24 @@
                 "account"
             ]
         }
     },
     "x-ibm-finding": {
         "fields": {
             "dst_ip_ref.value": [
-                "destinationaddress"
+                "dstaddr"
             ],
             "end": [
                 "endtime"
             ],
             "finding_type": [
                 "action"
             ],
             "src_ip_ref.value": [
-                "sourceaddress"
+                "srcaddr"
             ],
             "start": [
                 "starttime"
             ]
         }
     }
 }
```

## stix_shifter_modules/aws_athena/stix_transmission/results_connector.py

```diff
@@ -1,11 +1,13 @@
 import json
 from stix_shifter_utils.modules.base.stix_transmission.base_json_results_connector import BaseJsonResultsConnector
 from stix_shifter_utils.utils.error_response import ErrorResponder
+from stix_shifter_utils.utils.file_helper import read_json
 from stix_shifter_utils.utils import logger
+
 from flatten_json import flatten
 from os import path
 import os
 import six
 from collections.abc import Iterable
 
 
@@ -193,54 +195,80 @@
         :param flatten_result_cleansed: list, flattened results
         :param service_type: str, service name
         :return: list, formatted result
         """
         formatted_result = []
         transmit_basepath = os.path.abspath(__file__)
         translate_basepath = transmit_basepath.split(os.sep)[:-2]
-        filepath = os.sep.join([*translate_basepath, "stix_translation", "json", 'to_stix_map.json'])
+        filepath = os.sep.join([*translate_basepath, "stix_translation", "json", service_type + '_to_stix_map.json'])
         map_file = open(filepath).read()
         map_data = json.loads(map_file)
-        map_data_keys = list(map_data[service_type].keys())
+        map_data_keys = list(map_data.keys())
         ds_key_values = self.gen_dict_extract(key_to_search='ds_key', var=map_data)
         map_data_keys.extend(ds_key_values)
         flattened_obj = dict()
         obj_to_unflatten = dict()
         singular_obj = dict()
-        service_log_dict = dict()
         for obj in flatten_result_cleansed:
             for key, value in obj.items():
                 if key.replace('#', '_') in map_data_keys:
                     flattened_obj[key.replace('#', '_')] = value
                 else:
                     if value not in flattened_obj.values():
                         obj_to_unflatten[key] = value
             unflatten_obj = self.unflatten(obj_to_unflatten, '#')
             flattened_obj.update(unflatten_obj)
             flattened_obj.update(singular_obj)
-            service_log_dict = service_log_dict.copy()
             if flattened_obj:
-                service_log_dict[service_type] = flattened_obj
-                formatted_result.append(service_log_dict)
+                formatted_result.append(flattened_obj)
             flattened_obj = dict()
             obj_to_unflatten = dict()
         return formatted_result
 
     def format_result_ocsf(self, results):
         formatted_result = []
         for obj in results:
             json_obj = {}
             for k, v in obj.items():
                 try:
                     json_obj[k] = json.loads(v)
                 except Exception:
                     json_obj[k] = v
-            formatted_result.append({'ocsf': json_obj} )
+            
+            process_obj = json_obj.get('process')
+            if process_obj:
+                file_obj = process_obj.get('file')
+                if file_obj:
+                    file_obj['hashes'] = self.update_hash_mapping(file_obj)
+            
+                parent_process = process_obj.get('parent_process')
+                if parent_process:
+                    file_obj = parent_process.get('file')
+                    if file_obj:
+                        file_obj['hashes'] = self.update_hash_mapping(file_obj)
+  
+            formatted_result.append(json_obj)
         return formatted_result
 
+    def update_hash_mapping(self, file_obj):
+        transmit_basepath = os.path.abspath(__file__)
+        translate_basepath = transmit_basepath.split(os.sep)
+        hash_algorithm_map = os.sep.join([*translate_basepath, "stix_translation", "json", "hash_algorithm_map.json"])
+        hash_names = read_json(hash_algorithm_map, options={})
+
+        hashes = {}
+        fingerprints_objs =file_obj.get('fingerprints')
+        
+        for fingerprint in fingerprints_objs:
+            hash_name = hash_names[str(fingerprint.get('algorithm_id'))]
+
+            hashes[hash_name] = fingerprint.get('value')
+
+        return hashes
+
     def gen_dict_extract(self, key_to_search, var):
         """
         Get nested data source keys in mapping file
         :param key_to_search: str, data source key
         :param var: dict, to stix mapping
         :return: object
         """
```

## Comparing `stix_shifter_modules/aws_athena/stix_translation/json/to_stix_map.json` & `stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json`

 * *Files 9% similar despite different names*

### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('_time', [OrderedDict([('key', 'first_observed'), ('transformer', "*

 * *            "'EpochToTimestamp')]), OrderedDict([('key', 'last_observed'), ('transformer', "*

 * *            "'EpochToTimestamp')]), OrderedDict([('key', 'x-ibm-finding.time_observed'), "*

 * *            "('object', 'ibm_finding'), ('transformer', 'EpochToTimestamp')])]), ('activity', "*

 * *            "OrderedDict([('key', 'x-oca-event.action'), ('object', 'x_oca_event')])), "*

 * *            "('activity_id', OrderedDict([('key' […]*

```diff
@@ -1,3105 +1,2601 @@
 {
-    "guardduty": {
-        "accountid": {
-            "key": "x-aws-details.account_id",
-            "object": "aws_details"
+    "_time": [
+        {
+            "key": "first_observed",
+            "transformer": "EpochToTimestamp"
         },
-        "description": {
-            "key": "x-ibm-finding.description",
-            "object": "ibm_finding"
+        {
+            "key": "last_observed",
+            "transformer": "EpochToTimestamp"
         },
-        "dnsrequest_resource_instancedetails_networkinterfaces_0_privateipaddress": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "dns_private_ip1"
-            },
-            {
-                "key": "domain-name.resolves_to_refs",
-                "object": "private_dns_name",
-                "references": [
-                    "dns_private_ip1"
-                ]
-            },
-            {
-                "key": "x-ibm-finding.src_ip_ref",
-                "object": "ibm_finding",
-                "references": "dns_private_ip1"
-            },
-            {
-                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                "key": "ipv4-addr.x_aws_interface_id",
-                "object": "dns_private_ip1"
+        {
+            "key": "x-ibm-finding.time_observed",
+            "object": "ibm_finding",
+            "transformer": "EpochToTimestamp"
+        }
+    ],
+    "activity": {
+        "key": "x-oca-event.action",
+        "object": "x_oca_event"
+    },
+    "activity_id": {
+        "key": "x-oca-event.code",
+        "object": "x_oca_event",
+        "transformer": "ToString"
+    },
+    "activity_name": {
+        "key": "x-oca-event.action",
+        "object": "x_oca_event"
+    },
+    "api": {
+        "operation": {
+            "key": "x-ocsf-cloud.operation",
+            "object": "ocsf_cloud_api"
+        },
+        "request": {
+            "flags": {
+                "key": "x-ocsf-cloud.request_flags",
+                "object": "ocsf_cloud_api",
+                "transformer": "ToLowercaseArray"
             },
-            {
-                "key": "ipv4-addr.x_aws_ip_type",
-                "object": "dns_private_ip1",
-                "value": "private"
+            "uid": {
+                "key": "x-ocsf-cloud.request_uid",
+                "object": "ocsf_cloud_api"
             }
-        ],
-        "portprobe_resource_instancedetails_networkinterfaces_0_privateipaddress": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "pp_private_ip1"
+        },
+        "response": {
+            "code": {
+                "key": "x-ocsf-cloud.response_code",
+                "object": "ocsf_cloud_api",
+                "transformer": "ToInteger"
             },
-            {
-                "key": "domain-name.resolves_to_refs",
-                "object": "private_dns_name",
-                "references": [
-                    "pp_private_ip1"
-                ]
+            "error": {
+                "key": "x-ocsf-cloud.response_error",
+                "object": "ocsf_cloud_api"
             },
-            {
-                "key": "x-ibm-finding.src_ip_ref",
-                "object": "ibm_finding",
-                "references": "pp_private_ip1"
+            "error_message": {
+                "key": "x-ocsf-cloud.response_error_message",
+                "object": "ocsf_cloud_api"
             },
-            {
-                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                "key": "ipv4-addr.x_aws_interface_id",
-                "object": "pp_private_ip1"
+            "flags": {
+                "key": "x-ocsf-cloud.response_flags",
+                "object": "ocsf_cloud_api",
+                "transformer": "ToLowercaseArray"
             },
-            {
-                "key": "ipv4-addr.x_aws_ip_type",
-                "object": "pp_private_ip1",
-                "value": "private"
+            "message": {
+                "key": "x-ocsf-cloud.response_message",
+                "object": "ocsf_cloud_api"
             }
-        ],
-        "region": {
-            "key": "x-aws-details.region",
-            "object": "aws_details"
-        },
-        "resource_accesskeydetails_accesskeyid": {
-            "key": "x-aws-api.access_key_id",
-            "object": "api_details"
-        },
-        "resource_accesskeydetails_principalid": {
-            "key": "user-account.user_id",
-            "object": "api_user"
-        },
-        "resource_accesskeydetails_username": {
-            "key": "user-account.account_login",
-            "object": "api_user"
-        },
-        "resource_instancedetails_availabilityzone": {
-            "key": "x-aws-instance.availability_zone",
-            "object": "instance"
-        },
-        "resource_instancedetails_imageid": {
-            "key": "x-aws-instance.image_id",
-            "object": "instance"
-        },
-        "resource_instancedetails_instanceid": {
-            "key": "x-aws-instance.instance_id",
-            "object": "instance"
         },
-        "resource_instancedetails_networkinterfaces_0_ipv6addresses_0": [
-            {
-                "key": "ipv6-addr.value",
-                "object": "nc_ipv6_ip"
-            },
-            {
-                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                "key": "ipv6-addr.x_aws_interface_id",
-                "object": "nc_ipv6_ip"
-            }
-        ],
-        "resource_instancedetails_networkinterfaces_0_privatednsname": [
-            {
-                "key": "domain-name.value",
-                "object": "private_dns_name"
-            }
-        ],
-        "resource_instancedetails_networkinterfaces_0_privateipaddress": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "nc_private_ip1"
-            },
-            {
-                "key": "network-traffic.src_ref",
-                "object": "nc_nt",
-                "references": "nc_private_ip1"
-            },
-            {
-                "key": "domain-name.resolves_to_refs",
-                "object": "private_dns_name",
-                "references": [
-                    "nc_private_ip1"
-                ]
+        "service": {
+            "labels": {
+                "key": "x-ocsf-cloud.service_labels",
+                "object": "ocsf_cloud_api",
+                "transformer": "ToLowercaseArray"
             },
-            {
-                "key": "x-ibm-finding.src_ip_ref",
-                "object": "ibm_finding",
-                "references": "nc_private_ip1"
+            "name": {
+                "key": "x-ocsf-cloud.service_name",
+                "object": "ocsf_cloud_api"
             },
-            {
-                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                "key": "ipv4-addr.x_aws_interface_id",
-                "object": "nc_private_ip1"
+            "uid": {
+                "key": "x-ocsf-cloud.service_uid",
+                "object": "ocsf_cloud_api"
             },
-            {
-                "key": "ipv4-addr.x_aws_ip_type",
-                "object": "nc_private_ip1",
-                "value": "private"
-            }
-        ],
-        "resource_instancedetails_networkinterfaces_0_publicdnsname": [
-            {
-                "key": "domain-name.value",
-                "object": "nc_public_name"
+            "version": {
+                "key": "x-ocsf-cloud.service_uid",
+                "object": "ocsf_cloud_api"
             }
-        ],
-        "resource_instancedetails_networkinterfaces_0_publicip": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "nc_public_ip"
-            },
-            {
-                "key": "domain-name.resolves_to_refs",
-                "object": "nc_public_name",
-                "references": [
-                    "nc_public_ip"
-                ]
-            },
-            {
-                "ds_key": "resource_instancedetails_networkinterfaces_0_networkinterfaceid",
-                "key": "ipv4-addr.x_aws_interface_id",
-                "object": "nc_public_ip"
+        },
+        "version": {
+            "key": "x-ocsf-cloud.api_version",
+            "object": "ocsf_cloud_api"
+        }
+    },
+    "attacks": {
+        "tactics": {
+            "name": {
+                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_name",
+                "object": "ttp-tagging"
             },
-            {
-                "key": "ipv4-addr.x_aws_ip_type",
-                "object": "nc_public_ip",
-                "value": "public"
+            "uid": {
+                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_id",
+                "object": "ttp-tagging"
             }
-        ],
-        "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupid": {
-            "key": "x-aws-vpc.security_group_id",
-            "object": "vpc"
-        },
-        "resource_instancedetails_networkinterfaces_0_securitygroups_0_groupname": {
-            "key": "x-aws-vpc.security_group_name",
-            "object": "vpc"
-        },
-        "resource_instancedetails_networkinterfaces_0_subnetid": {
-            "key": "x-aws-vpc.subnet_id",
-            "object": "vpc"
-        },
-        "resource_instancedetails_networkinterfaces_0_vpcid": {
-            "key": "x-aws-vpc.vpc_id",
-            "object": "vpc"
         },
-        "resource_instancedetails_networkinterfaces_1_privatednsname": [
-            {
-                "key": "domain-name.value",
-                "object": "nc_private_name2"
+        "technique": {
+            "name": [
+                {
+                    "key": "x-ibm-ttp-tagging.name",
+                    "object": "ttp-tagging"
+                },
+                {
+                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_name",
+                    "object": "ttp-tagging"
+                },
+                {
+                    "key": "x-ibm-finding.ttp_tagging_refs",
+                    "object": "ibm_finding",
+                    "references": [
+                        "ttp-tagging"
+                    ]
+                }
+            ],
+            "uid": {
+                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_id",
+                "object": "ttp-tagging"
             }
-        ],
-        "resource_instancedetails_networkinterfaces_1_privateipaddress": [
+        },
+        "version": {
+            "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.versoin",
+            "object": "ttp-tagging"
+        }
+    },
+    "category_name": {
+        "key": "x-oca-event.category",
+        "object": "x_oca_event"
+    },
+    "category_uid": {
+        "key": "x-oca-event.code",
+        "object": "x_oca_event",
+        "transformer": "ToString"
+    },
+    "class_name": {
+        "key": "x-oca-event.module",
+        "object": "x_oca_event"
+    },
+    "class_uid": {
+        "key": "x-oca-event.extensions.x-cloud-api.class_uid",
+        "object": "x_oca_event",
+        "transformer": "ToInteger"
+    },
+    "cloud": {
+        "account_type": {
+            "key": "x-ocsf-cloud.account_type",
+            "object": "ocsf_cloud_api"
+        },
+        "account_type_id": {
+            "key": "x-ocsf-cloud.account_type_id",
+            "object": "ocsf_cloud_api",
+            "transformer": "ToInteger"
+        },
+        "account_uid": {
+            "key": "x-ocsf-cloud.account_uid",
+            "object": "ocsf_cloud_api"
+        },
+        "org_uid": {
+            "key": "x-ocsf-cloud.org_uid",
+            "object": "ocsf_cloud_api"
+        },
+        "project_uid": {
+            "key": "x-ocsf-cloud.project_uid",
+            "object": "ocsf_cloud_api"
+        },
+        "provider": {
+            "key": "x-ocsf-cloud.provider",
+            "object": "ocsf_cloud_api"
+        },
+        "region": {
+            "key": "x-ocsf-cloud.region",
+            "object": "ocsf_cloud_api"
+        },
+        "resource_uid": {
+            "key": "x-ocsf-cloud.resource_uid",
+            "object": "ocsf_cloud_api"
+        },
+        "zone": {
+            "key": "x-ocsf-cloud.zone",
+            "object": "ocsf_cloud_api"
+        }
+    },
+    "compliance": {
+        "requirements": {
+            "key": "x-ocsf-compliance.requirements",
+            "object": "compliance"
+        },
+        "status": {
+            "key": "x-ocsf-compliance.status",
+            "object": "compliance"
+        },
+        "status_detail": {
+            "key": "x-ocsf-compliance.status_detail",
+            "object": "compliance"
+        }
+    },
+    "confidence": {
+        "key": "x-oca-event.confidence",
+        "object": "x-oca-event"
+    },
+    "connection_info": {
+        "boundary": {
+            "key": "network-traffic.extensions.x-network-ext.boundary",
+            "object": "nt"
+        },
+        "boundary_id": {
+            "key": "network-traffic.extensions.x-network-ext.boundary_id",
+            "object": "nt"
+        },
+        "direction": {
+            "key": "network-traffic.extensions.x-network-ext.direction",
+            "object": "nt"
+        },
+        "direction_id": {
+            "key": "network-traffic.extensions.x-network-ext.direction_id",
+            "object": "nt"
+        },
+        "protocol_name": {
+            "key": "network-traffic.extensions.x-network-ext.protocol_name",
+            "object": "nt"
+        },
+        "protocol_num": {
+            "group": true,
+            "key": "network-traffic.protocols",
+            "object": "nt",
+            "transformer": "ProtocolNumToName"
+        },
+        "protocol_ver": {
+            "group": true,
+            "key": "network-traffic.protocols",
+            "object": "nt",
+            "transformer": "ToLowercaseArray"
+        },
+        "protocol_ver_id": {
+            "key": "network-traffic.extensions.x-network-ext.protocol_ver_id",
+            "object": "nt"
+        },
+        "tcp_flags": {
+            "key": "network-traffic.extensions.tcp-ext.src_flags_hex",
+            "object": "nt"
+        }
+    },
+    "count": [
+        {
+            "key": "number_observed",
+            "transformer": "ToInteger"
+        },
+        {
+            "key": "x-ibm-finding.event_count",
+            "object": "ibm_finding",
+            "transformer": "ToInteger"
+        }
+    ],
+    "data": {
+        "key": "x-oca-event.extensions.x-ocsf-data.data",
+        "object": "x-oca-event"
+    },
+    "dst_endpoint": {
+        "instance_uid": {
+            "key": "x-oca-asset.extensions.x-dst-endpoint.instance_uid",
+            "object": "asset"
+        },
+        "interface_uid": {
+            "key": "x-oca-asset.extensions.x-dst-endpoint.interface_uid",
+            "object": "asset"
+        },
+        "intermediate_ips": [
             {
                 "key": "ipv4-addr.value",
-                "object": "nc_private_ip2"
-            },
-            {
-                "key": "domain-name.resolves_to_refs",
-                "object": "nc_private_name2",
-                "references": [
-                    "nc_private_ip2"
-                ]
-            },
-            {
-                "ds_key": "resource_instancedetails_networkinterfaces_1_networkinterfaceid",
-                "key": "ipv4-addr.x_aws_interface_id",
-                "object": "nc_private_ip2"
+                "object": "dst_ipv4",
+                "transformer": "FilterIPv4List",
+                "unwrap": true
             },
             {
-                "key": "ipv4-addr.x_aws_ip_type",
-                "object": "nc_private_ip2",
-                "value": "private"
-            }
-        ],
-        "resource_instancedetails_platform": [
-            {
-                "key": "software.name",
-                "object": "software"
+                "key": "ipv6-addr.value",
+                "object": "dst_ipv6",
+                "transformer": "FilterIPv6List",
+                "unwrap": true
             },
             {
-                "key": "x-ibm-finding.src_os_ref",
-                "object": "ibm_finding",
-                "references": "software"
+                "key": "x-oca-asset.ip_refs",
+                "object": "asset",
+                "references": [
+                    "dst_ipv4",
+                    "dst_ipv6"
+                ],
+                "unwrap": true
             }
         ],
-        "service_action_awsapicallaction_api": {
-            "key": "x-aws-api.api",
-            "object": "api_details"
-        },
-        "service_action_awsapicallaction_remoteipdetails_ipaddressv4": [
+        "ip": [
             {
                 "key": "ipv4-addr.value",
-                "object": "api_remote_ip"
-            },
-            {
-                "key": "x-ibm-finding.dst_ip_ref",
-                "object": "ibm_finding",
-                "references": "api_remote_ip"
-            },
-            {
-                "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
-                "key": "x-ibm-finding.dst_geolocation",
-                "object": "ibm_finding"
-            },
-            {
-                "ds_key": "service_action_awsapicallaction_remoteipdetails_city_cityname",
-                "key": "ipv4-addr.x_aws_remote_city_name",
-                "object": "api_remote_ip"
+                "object": "dst_ip",
+                "transformer": "CheckIPv4"
             },
             {
-                "ds_key": "service_action_awsapicallaction_remoteipdetails_country_countryname",
-                "key": "ipv4-addr.x_aws_remote_country_name",
-                "object": "api_remote_ip"
-            }
-        ],
-        "service_action_awsapicallaction_servicename": {
-            "key": "x-aws-api.service_name",
-            "object": "api_details"
-        },
-        "service_action_dnsrequestaction_domain": [
-            {
-                "key": "domain-name.value",
-                "object": "dns_domain_name"
-            }
-        ],
-        "service_action_networkconnectionaction_localportdetails_port": [
-            {
-                "key": "network-traffic.src_port",
-                "object": "nc_nt",
-                "transformer": "ToInteger"
-            }
-        ],
-        "service_action_networkconnectionaction_protocol": [
-            {
-                "key": "network-traffic.protocols",
-                "object": "nc_nt",
-                "transformer": "ToLowercaseArray"
-            }
-        ],
-        "service_action_networkconnectionaction_remoteipdetails_ipaddressv4": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "nc_remote_ip"
+                "key": "ipv6-addr.value",
+                "object": "dst_ip",
+                "transformer": "CheckIPv6"
             },
             {
                 "key": "network-traffic.dst_ref",
-                "object": "nc_nt",
-                "references": "nc_remote_ip"
+                "object": "nt",
+                "references": "dst_ip"
             },
             {
                 "key": "x-ibm-finding.dst_ip_ref",
                 "object": "ibm_finding",
-                "references": "nc_remote_ip"
-            },
-            {
-                "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
-                "key": "x-ibm-finding.dst_geolocation",
-                "object": "ibm_finding"
+                "references": "dst_ip"
             },
             {
-                "ds_key": "service_action_networkconnectionaction_remoteipdetails_city_cityname",
-                "key": "ipv4-addr.x_aws_remote_city_name",
-                "object": "nc_remote_ip"
+                "group": true,
+                "key": "x-oca-asset.ip_refs",
+                "object": "host",
+                "references": [
+                    "dst_ip"
+                ]
             },
             {
-                "ds_key": "service_action_networkconnectionaction_remoteipdetails_country_countryname",
-                "key": "ipv4-addr.x_aws_remote_country_name",
-                "object": "nc_remote_ip"
-            }
-        ],
-        "service_action_networkconnectionaction_remoteportdetails_port": [
-            {
-                "key": "network-traffic.dst_port",
-                "object": "nc_nt",
-                "transformer": "ToInteger"
+                "key": "x-oca-event.network_ref",
+                "object": "event",
+                "references": "nt"
             }
         ],
-        "service_action_portprobeaction_portprobedetails_0_localportdetails_port": [
-            {
-                "key": "x-ibm-finding.probe_port",
+        "name": {
+            "key": "x-oca-asset.name",
+            "object": "asset"
+        },
+        "port": {
+            "key": "network-traffic.dst_port",
+            "object": "nt",
+            "transformer": "ToInteger"
+        },
+        "subnet_uid": {
+            "key": "x-oca-asset.extensions.x-dst-endpoint.subnet_uid",
+            "object": "asset"
+        },
+        "svc_name": {
+            "key": "x-oca-asset.extensions.x-dst-endpoint.svc_name",
+            "object": "asset"
+        },
+        "vpc_uid": {
+            "key": "x-oca-asset.extensions.x-dst-endpoint.vpc_uid",
+            "object": "asset"
+        }
+    },
+    "duration": {
+        "key": "x-oca-event.duration",
+        "object": "x_oca_event",
+        "transformer": "ToInteger"
+    },
+    "end_time": [
+        {
+            "key": "x-ibm-finding.end",
+            "object": "ibm_finding",
+            "transformer": "EpochToTimestamp"
+        },
+        {
+            "key": "last_observed",
+            "transformer": "EpochToTimestamp"
+        }
+    ],
+    "enrichments": {
+        "data": {
+            "key": "x-ocsf-enrichments.data",
+            "object": "enrichments"
+        },
+        "name": {
+            "key": "x-ocsf-enrichments.name",
+            "object": "enrichments"
+        },
+        "provider": {
+            "key": "x-ocsf-enrichments.provider",
+            "object": "enrichments"
+        },
+        "type": {
+            "key": "x-ocsf-enrichments.type",
+            "object": "enrichments"
+        },
+        "value": {
+            "key": "x-ocsf-enrichments.value",
+            "object": "enrichments"
+        }
+    },
+    "finding": {
+        "created_time": {
+            "key": "x-ibm-finding.start",
+            "object": "ibm_finding"
+        },
+        "desc": {
+            "key": "x-ibm-finding.description",
+            "object": "ibm_finding"
+        },
+        "first_seen_time": {
+            "key": "x-ibm-finding.time_observed",
+            "object": "ibm_finding"
+        },
+        "last_seen_time": {
+            "key": "x-ibm-finding.extensions.x-ocsf-findings.last_seen_time",
+            "object": "ibm_finding"
+        },
+        "modified_time": {
+            "key": "x-ibm-finding.extensions.x-ocsf-findings.modified_time",
+            "object": "ibm_finding"
+        },
+        "product_uid": {
+            "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
+            "object": "ibm_finding"
+        },
+        "related_events": {
+            "product_uid": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
                 "object": "ibm_finding"
-            }
-        ],
-        "service_action_portprobeaction_portprobedetails_0_remoteipdetails_ipaddressv4": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "pp_remote_ip"
-            },
-            {
-                "key": "x-ibm-finding.dst_ip_ref",
-                "object": "ibm_finding",
-                "references": "pp_remote_ip"
             },
-            {
-                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
-                "key": "x-ibm-finding.dst_geolocation",
+            "type": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.type",
                 "object": "ibm_finding"
             },
-            {
-                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_city_cityname",
-                "key": "ipv4-addr.x_aws_remote_city_name",
-                "object": "pp_remote_ip"
-            },
-            {
-                "ds_key": "service_action_portprobeaction_portprobedetails_0_remoteipdetails_country_countryname",
-                "key": "ipv4-addr.x_aws_remote_country_name",
-                "object": "pp_remote_ip"
-            }
-        ],
-        "service_eventfirstseen": [
-            {
-                "key": "first_observed"
+            "type_uid": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.type_uid",
+                "object": "ibm_finding"
             },
-            {
-                "key": "x-ibm-finding.start",
+            "uid": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.uid",
                 "object": "ibm_finding"
             }
-        ],
-        "service_eventlastseen": [
-            {
-                "key": "last_observed"
+        },
+        "remediation": {
+            "desc": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_desc",
+                "object": "ibm_finding"
             },
-            {
-                "key": "x-ibm-finding.end",
+            "kb_articles": {
+                "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_kb_articles",
                 "object": "ibm_finding"
             }
-        ],
-        "severity": {
-            "key": "x-ibm-finding.severity",
+        },
+        "src_url": {
+            "key": "x-ibm-finding.extensions.x-ocsf-findings.src_url",
+            "object": "ibm_finding"
+        },
+        "supporting_data": {
+            "key": "x-ibm-finding.extensions.x-ocsf-findings.upporting_data",
             "object": "ibm_finding"
         },
         "title": {
             "key": "x-ibm-finding.name",
             "object": "ibm_finding"
         },
-        "type": {
-            "key": "x-ibm-finding.finding_type",
+        "types": {
+            "key": "x-ibm-finding.types",
+            "object": "ibm_finding"
+        },
+        "uid": {
+            "key": "x-ibm-finding.alert_id",
             "object": "ibm_finding"
         }
     },
-    "ocsf": {
-        "_time": [
-            {
-                "key": "first_observed",
-                "transformer": "EpochToTimestamp"
-            },
-            {
-                "key": "last_observed",
-                "transformer": "EpochToTimestamp"
+    "http_request": {
+        "args": {
+            "key": "x-ocsf-http-request.value",
+            "object": "http_request"
+        },
+        "http_headers": {
+            "name": {
+                "key": "x-ocsf-http-request.http_headers_name",
+                "object": "ocsf_cloud_api"
             },
-            {
-                "key": "x-ibm-finding.time_observed",
-                "object": "ibm_finding",
-                "transformer": "EpochToTimestamp"
+            "value": {
+                "key": "x-ocsf-http-request.http_headers_value",
+                "object": "http_request"
             }
-        ],
-        "activity": {
-            "key": "x-oca-event.action",
-            "object": "x_oca_event"
-        },
-        "activity_id": {
-            "key": "x-oca-event.code",
-            "object": "x_oca_event",
-            "transformer": "ToString"
-        },
-        "activity_name": {
-            "key": "x-oca-event.action",
-            "object": "x_oca_event"
-        },
-        "api": {
-            "operation": {
-                "key": "x-ocsf-cloud.operation",
-                "object": "ocsf_cloud_api"
+        },
+        "http_method": {
+            "key": "x-ocsf-http-request.http_method",
+            "object": "http_request"
+        },
+        "prefix": {
+            "key": "x-ocsf-http-request.prefix",
+            "object": "http_request"
+        },
+        "referrer": {
+            "key": "x-ocsf-http-request.referrer",
+            "object": "http_request"
+        },
+        "uid": {
+            "key": "x-ocsf-http-request.uid",
+            "object": "http_request"
+        },
+        "url": {
+            "key": "url.value",
+            "object": "url"
+        },
+        "user_agent": {
+            "key": "x-ocsf-http-request.user_agent",
+            "object": "http_request"
+        },
+        "version": {
+            "key": "x-ocsf-http-request.version",
+            "object": "http_request"
+        },
+        "x_forwarded_for": {
+            "key": "x-ocsf-http-request.x_forwarded_for",
+            "object": "http_request"
+        }
+    },
+    "identity": {
+        "authorizations": {
+            "decision": {
+                "key": "x-ocsf-identity.authorizations.decision",
+                "object": "x-ocsf-identity"
             },
-            "request": {
-                "flags": {
-                    "key": "x-ocsf-cloud.request_flags",
-                    "object": "ocsf_cloud_api",
-                    "transformer": "ToLowercaseArray"
+            "policy": {
+                "desc": {
+                    "key": "x-ocsf-identity.authorizations.policy_desc",
+                    "object": "x-ocsf-identity"
                 },
-                "uid": {
-                    "key": "x-ocsf-cloud.request_uid",
-                    "object": "ocsf_cloud_api"
-                }
-            },
-            "response": {
-                "code": {
-                    "key": "x-ocsf-cloud.response_code",
-                    "object": "ocsf_cloud_api",
-                    "transformer": "ToInteger"
-                },
-                "error": {
-                    "key": "x-ocsf-cloud.response_error",
-                    "object": "ocsf_cloud_api"
-                },
-                "error_message": {
-                    "key": "x-ocsf-cloud.response_error_message",
-                    "object": "ocsf_cloud_api"
-                },
-                "flags": {
-                    "key": "x-ocsf-cloud.response_flags",
-                    "object": "ocsf_cloud_api",
-                    "transformer": "ToLowercaseArray"
-                },
-                "message": {
-                    "key": "x-ocsf-cloud.response_message",
-                    "object": "ocsf_cloud_api"
-                }
-            },
-            "service": {
-                "labels": {
-                    "key": "x-ocsf-cloud.service_labels",
-                    "object": "ocsf_cloud_api",
-                    "transformer": "ToLowercaseArray"
+                "group": {
+                    "desc": {
+                        "key": "x-ocsf-identity.authorizations.policy_group_desc",
+                        "object": "x-ocsf-identity"
+                    },
+                    "name": {
+                        "key": "x-ocsf-identity.authorizations.policy_group_namee",
+                        "object": "x-ocsf-identity"
+                    },
+                    "privileges": {
+                        "key": "x-ocsf-identity.authorizations.policy_group_privileges",
+                        "object": "x-ocsf-identity"
+                    },
+                    "type": {
+                        "key": "x-ocsf-identity.authorizations.policy_group_type",
+                        "object": "x-ocsf-identity"
+                    },
+                    "uid": {
+                        "key": "x-ocsf-identity.authorizations.policy_group_uid",
+                        "object": "x-ocsf-identity"
+                    }
                 },
                 "name": {
-                    "key": "x-ocsf-cloud.service_name",
-                    "object": "ocsf_cloud_api"
+                    "key": "x-ocsf-identity.authorizations.name",
+                    "object": "x-ocsf-identity"
                 },
                 "uid": {
-                    "key": "x-ocsf-cloud.service_uid",
-                    "object": "ocsf_cloud_api"
+                    "key": "x-ocsf-identity.authorizations.uid",
+                    "object": "x-ocsf-identity"
                 },
                 "version": {
-                    "key": "x-ocsf-cloud.service_uid",
-                    "object": "ocsf_cloud_api"
+                    "key": "x-ocsf-identity.authorizations.version",
+                    "object": "x-ocsf-identity"
                 }
-            },
-            "version": {
-                "key": "x-ocsf-cloud.api_version",
-                "object": "ocsf_cloud_api"
             }
         },
-        "attacks": {
-            "tactics": {
-                "name": {
-                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_name",
-                    "object": "ttp-tagging"
-                },
-                "uid": {
-                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.tactic_id",
-                    "object": "ttp-tagging"
-                }
-            },
-            "technique": {
-                "name": [
-                    {
-                        "key": "x-ibm-ttp-tagging.name",
-                        "object": "ttp-tagging"
-                    },
-                    {
-                        "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_name",
-                        "object": "ttp-tagging"
-                    },
-                    {
-                        "key": "x-ibm-finding.ttp_tagging_refs",
-                        "object": "ibm_finding",
-                        "references": [
-                            "ttp-tagging"
-                        ]
-                    }
-                ],
-                "uid": {
-                    "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.technique_id",
-                    "object": "ttp-tagging"
-                }
+        "idp": {
+            "name": {
+                "key": "x-ocsf-identity.idp.name",
+                "object": "x-ocsf-identity"
             },
-            "version": {
-                "key": "x-ibm-ttp-tagging.extensions.mitre-attack-ext.versoin",
-                "object": "ttp-tagging"
+            "uid": {
+                "key": "x-ocsf-identity.idp.uid",
+                "object": "x-ocsf-identity"
             }
         },
-        "category_name": {
-            "key": "x-oca-event.category",
-            "object": "x_oca_event"
-        },
-        "category_uid": {
-            "key": "x-oca-event.code",
-            "object": "x_oca_event",
-            "transformer": "ToString"
-        },
-        "class_name": {
-            "key": "x-oca-event.module",
-            "object": "x_oca_event"
-        },
-        "class_uid": {
-            "key": "x-oca-event.extensions.x-cloud-api.class_uid",
-            "object": "x_oca_event",
-            "transformer": "ToInteger"
+        "invoked_by": {
+            "key": "x-ocsf-identity.invoked_by",
+            "object": "x-ocsf-identity"
         },
-        "cloud": {
-            "account_type": {
-                "key": "x-ocsf-cloud.account_type",
-                "object": "ocsf_cloud_api"
-            },
-            "account_type_id": {
-                "key": "x-ocsf-cloud.account_type_id",
-                "object": "ocsf_cloud_api",
-                "transformer": "ToInteger"
-            },
-            "account_uid": {
-                "key": "x-ocsf-cloud.account_uid",
-                "object": "ocsf_cloud_api"
-            },
-            "org_uid": {
-                "key": "x-ocsf-cloud.org_uid",
-                "object": "ocsf_cloud_api"
+        "message": {
+            "key": "x-ocsf-identity.message",
+            "object": "x-ocsf-identity"
+        },
+        "session": {
+            "created_time": {
+                "key": "x-ocsf-identity.session.created_time",
+                "object": "x-ocsf-identity"
             },
-            "project_uid": {
-                "key": "x-ocsf-cloud.project_uid",
-                "object": "ocsf_cloud_api"
+            "credential_uid": {
+                "key": "x-ocsf-identity.session.credential_uid",
+                "object": "x-ocsf-identity"
             },
-            "provider": {
-                "key": "x-ocsf-cloud.provider",
-                "object": "ocsf_cloud_api"
+            "expiration_time": {
+                "key": "x-ocsf-identity.session.expiration_time",
+                "object": "x-ocsf-identity"
             },
-            "region": {
-                "key": "x-ocsf-cloud.region",
-                "object": "ocsf_cloud_api"
+            "issuer": {
+                "key": "x-ocsf-identity.session.issuer",
+                "object": "x-ocsf-identity"
             },
-            "resource_uid": {
-                "key": "x-ocsf-cloud.resource_uid",
-                "object": "ocsf_cloud_api"
+            "mfa": {
+                "key": "x-ocsf-identity.session.mfa",
+                "object": "x-ocsf-identity"
             },
-            "zone": {
-                "key": "x-ocsf-cloud.zone",
-                "object": "ocsf_cloud_api"
+            "uid": {
+                "key": "x-ocsf-identity.session.uid",
+                "object": "x-ocsf-identity"
             }
         },
-        "compliance": {
-            "requirements": {
-                "key": "x-ocsf-compliance.requirements",
-                "object": "compliance"
-            },
-            "status": {
-                "key": "x-ocsf-compliance.status",
-                "object": "compliance"
-            },
-            "status_detail": {
-                "key": "x-ocsf-compliance.status_detail",
-                "object": "compliance"
-            }
-        },
-        "confidence": {
-            "key": "x-oca-event.confidence",
-            "object": "x-oca-event"
-        },
-        "connection_info": {
-            "boundary": {
-                "key": "network-traffic.extensions.x-network-ext.boundary",
-                "object": "nt"
-            },
-            "boundary_id": {
-                "key": "network-traffic.extensions.x-network-ext.boundary_id",
-                "object": "nt"
-            },
-            "direction": {
-                "key": "network-traffic.extensions.x-network-ext.direction",
-                "object": "nt"
-            },
-            "direction_id": {
-                "key": "network-traffic.extensions.x-network-ext.direction_id",
-                "object": "nt"
-            },
-            "protocol_name": {
-                "key": "network-traffic.extensions.x-network-ext.protocol_name",
-                "object": "nt"
-            },
-            "protocol_num": {
-                "group": true,
-                "key": "network-traffic.protocols",
-                "object": "nt",
-                "transformer": "ProtocolNumToName"
-            },
-            "protocol_ver": {
-                "group": true,
-                "key": "network-traffic.protocols",
-                "object": "nt",
-                "transformer": "ToLowercaseArray"
-            },
-            "protocol_ver_id": {
-                "key": "network-traffic.extensions.x-network-ext.protocol_ver_id",
-                "object": "nt"
+        "user": {
+            "account_type": {
+                "key": "user-account.account_type",
+                "object": "user"
             },
-            "tcp_flags": {
-                "key": "network-traffic.extensions.tcp-ext.src_flags_hex",
-                "object": "nt"
-            }
-        },
-        "count": [
-            {
-                "key": "number_observed",
+            "account_type_id": {
+                "key": "user-account.extensions.aws-account-ext.account_type_id",
+                "object": "user",
                 "transformer": "ToInteger"
             },
-            {
-                "key": "x-ibm-finding.event_count",
-                "object": "ibm_finding",
-                "transformer": "ToInteger"
-            }
-        ],
-        "data": {
-            "key": "x-oca-event.extensions.x-ocsf-data.data",
-            "object": "x-oca-event"
-        },
-        "dst_endpoint": {
-            "instance_uid": {
-                "key": "x-oca-asset.extensions.x-dst-endpoint.instance_uid",
-                "object": "asset"
-            },
-            "interface_uid": {
-                "key": "x-oca-asset.extensions.x-dst-endpoint.interface_uid",
-                "object": "asset"
+            "account_uid": {
+                "key": "user-account.user_id",
+                "object": "user"
             },
-            "intermediate_ips": [
-                {
-                    "key": "ipv4-addr.value",
-                    "object": "dst_ipv4",
-                    "transformer": "FilterIPv4List",
-                    "unwrap": true
-                },
-                {
-                    "key": "ipv6-addr.value",
-                    "object": "dst_ipv6",
-                    "transformer": "FilterIPv6List",
-                    "unwrap": true
-                },
-                {
-                    "key": "x-oca-asset.ip_refs",
-                    "object": "asset",
-                    "references": [
-                        "dst_ipv4",
-                        "dst_ipv6"
-                    ],
-                    "unwrap": true
-                }
-            ],
-            "ip": [
-                {
-                    "key": "ipv4-addr.value",
-                    "object": "dst_ip",
-                    "transformer": "CheckIPv4"
-                },
-                {
-                    "key": "ipv6-addr.value",
-                    "object": "dst_ip",
-                    "transformer": "CheckIPv6"
+            "credential_uid": {
+                "key": "user-account.extensions.aws-account-ext.credential_uid",
+                "object": "user"
+            },
+            "domain": {
+                "key": "user-account.extensions.aws-account-ext.domain",
+                "object": "user"
+            },
+            "email_addr": {
+                "key": "email-addr.value",
+                "object": "email_addr"
+            },
+            "groups": {
+                "desc": {
+                    "key": "user-account.extensions.aws-account-ext.group_desc",
+                    "object": "user"
                 },
-                {
-                    "key": "network-traffic.dst_ref",
-                    "object": "nt",
-                    "references": "dst_ip"
+                "name": {
+                    "key": "user-account.extensions.aws-account-ext.group_name",
+                    "object": "user"
                 },
-                {
-                    "key": "x-ibm-finding.dst_ip_ref",
-                    "object": "ibm_finding",
-                    "references": "dst_ip"
+                "privileges": {
+                    "key": "user-account.extensions.aws-account-ext.group_privileges",
+                    "object": "user"
                 },
-                {
-                    "group": true,
-                    "key": "x-oca-asset.ip_refs",
-                    "object": "host",
-                    "references": [
-                        "dst_ip"
-                    ]
+                "type": {
+                    "key": "user-account.extensions.aws-account-ext.group_type",
+                    "object": "user"
                 },
-                {
-                    "key": "x-oca-event.network_ref",
-                    "object": "event",
-                    "references": "nt"
+                "uid": {
+                    "key": "user-account.extensions.aws-account-ext.group_uid",
+                    "object": "user"
                 }
-            ],
-            "name": {
-                "key": "x-oca-asset.name",
-                "object": "asset"
             },
-            "port": {
-                "key": "network-traffic.dst_port",
-                "object": "nt",
-                "transformer": "ToInteger"
+            "name": {
+                "key": "user-account.display_name",
+                "object": "user"
             },
-            "subnet_uid": {
-                "key": "x-oca-asset.extensions.x-dst-endpoint.subnet_uid",
-                "object": "asset"
-            },
-            "svc_name": {
-                "key": "x-oca-asset.extensions.x-dst-endpoint.svc_name",
-                "object": "asset"
-            },
-            "vpc_uid": {
-                "key": "x-oca-asset.extensions.x-dst-endpoint.vpc_uid",
-                "object": "asset"
-            }
-        },
-        "duration": {
-            "key": "x-oca-event.duration",
-            "object": "x_oca_event",
-            "transformer": "ToInteger"
-        },
-        "end_time": [
-            {
-                "key": "x-ibm-finding.end",
-                "object": "ibm_finding",
-                "transformer": "EpochToTimestamp"
+            "org_uid": {
+                "key": "user-account.extensions.aws-account-ext.org_uid",
+                "object": "user"
             },
-            {
-                "key": "last_observed",
-                "transformer": "EpochToTimestamp"
-            }
-        ],
-        "enrichments": {
-            "data": {
-                "key": "x-ocsf-enrichments.data",
-                "object": "enrichments"
+            "session_uid": {
+                "key": "user-account.extensions.aws-account-ext.session_uid",
+                "object": "user"
+            },
+            "session_uuid": {
+                "key": "user-account.extensions.aws-account-ext.session_uuid",
+                "object": "user"
             },
-            "name": {
-                "key": "x-ocsf-enrichments.name",
-                "object": "enrichments"
+            "type": {
+                "key": "user-account.extensions.aws-account-ext.type",
+                "object": "user"
             },
-            "provider": {
-                "key": "x-ocsf-enrichments.provider",
-                "object": "enrichments"
+            "type_id": {
+                "key": "user-account.extensions.aws-account-ext.type_id",
+                "object": "user",
+                "transformer": "ToInteger"
             },
-            "type": {
-                "key": "x-ocsf-enrichments.type",
-                "object": "enrichments"
+            "uid": {
+                "key": "user-account.extensions.aws-account-ext.uid",
+                "object": "user"
             },
-            "value": {
-                "key": "x-ocsf-enrichments.value",
-                "object": "enrichments"
+            "uuid": {
+                "key": "user-account.extensions.aws-account-ext.uuid",
+                "object": "user"
             }
+        }
+    },
+    "malware": {
+        "classification_ids": {
+            "key": "x-ocsf-malware.classification_ids",
+            "object": "malware"
+        },
+        "classifications": {
+            "key": "x-ocsf-malware.classifications",
+            "object": "malware"
         },
-        "finding": {
+        "cves": {
             "created_time": {
-                "key": "x-ibm-finding.start",
-                "object": "ibm_finding"
+                "key": "x-ocsf-malware.created_time",
+                "object": "malware"
             },
-            "desc": {
-                "key": "x-ibm-finding.description",
-                "object": "ibm_finding"
+            "cvss": {
+                "base_score": {
+                    "key": "x-ocsf-malware.base_score",
+                    "object": "malware"
+                },
+                "depth": {
+                    "key": "x-ocsf-malware.depth",
+                    "object": "malware"
+                },
+                "metrics": {
+                    "name": {
+                        "key": "x-ocsf-malware.name",
+                        "object": "malware"
+                    },
+                    "value": {
+                        "key": "x-ocsf-malware.value",
+                        "object": "malware"
+                    }
+                },
+                "overall_score": {
+                    "key": "x-ocsf-malware.overall_score",
+                    "object": "malware"
+                },
+                "severity": {
+                    "key": "x-ocsf-malware.severity",
+                    "object": "malware"
+                },
+                "vector_string": {
+                    "key": "x-ocsf-malware.vector_string",
+                    "object": "malware"
+                },
+                "version": {
+                    "key": "x-ocsf-malware.version",
+                    "object": "malware"
+                }
             },
-            "first_seen_time": {
-                "key": "x-ibm-finding.time_observed",
-                "object": "ibm_finding"
+            "cwe_uid": {
+                "key": "x-ocsf-malware.cwe_uid",
+                "object": "malware"
             },
-            "last_seen_time": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.last_seen_time",
-                "object": "ibm_finding"
+            "cwe_url": {
+                "key": "x-ocsf-malware.cwe_url",
+                "object": "malware"
             },
             "modified_time": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.modified_time",
-                "object": "ibm_finding"
-            },
-            "product_uid": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
-                "object": "ibm_finding"
+                "key": "x-ocsf-malware.modified_time",
+                "object": "malware"
             },
-            "related_events": {
-                "product_uid": {
-                    "key": "x-ibm-finding.extensions.x-ocsf-findings.product_uid",
-                    "object": "ibm_finding"
+            "product": {
+                "feature": {
+                    "name": {
+                        "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                        "object": "malware-software"
+                    },
+                    "uid": {
+                        "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                        "object": "malware-software"
+                    },
+                    "version": {
+                        "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                        "object": "malware-software"
+                    }
                 },
-                "type": {
-                    "key": "x-ibm-finding.extensions.x-ocsf-findings.type",
-                    "object": "ibm_finding"
+                "lang": {
+                    "key": "software.languages",
+                    "object": "malware-software"
                 },
-                "type_uid": {
-                    "key": "x-ibm-finding.extensions.x-ocsf-findings.type_uid",
-                    "object": "ibm_finding"
+                "name": {
+                    "key": "software.name",
+                    "object": "malware-software"
+                },
+                "path": {
+                    "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                    "object": "malware-software"
                 },
                 "uid": {
-                    "key": "x-ibm-finding.extensions.x-ocsf-findings.uid",
-                    "object": "ibm_finding"
-                }
-            },
-            "remediation": {
-                "desc": {
-                    "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_desc",
-                    "object": "ibm_finding"
+                    "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                    "object": "malware-software"
+                },
+                "vendor_name": {
+                    "key": "software.vendor",
+                    "object": "malware-software"
                 },
-                "kb_articles": {
-                    "key": "x-ibm-finding.extensions.x-ocsf-findings.remediation_kb_articles",
-                    "object": "ibm_finding"
+                "version": {
+                    "key": "software.version",
+                    "object": "malware-software"
                 }
             },
-            "src_url": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.src_url",
-                "object": "ibm_finding"
-            },
-            "supporting_data": {
-                "key": "x-ibm-finding.extensions.x-ocsf-findings.upporting_data",
-                "object": "ibm_finding"
-            },
-            "title": {
-                "key": "x-ibm-finding.name",
-                "object": "ibm_finding"
-            },
-            "types": {
-                "key": "x-ibm-finding.types",
-                "object": "ibm_finding"
+            "type": {
+                "key": "x-ocsf-malware.type",
+                "object": "malware"
             },
             "uid": {
-                "key": "x-ibm-finding.alert_id",
-                "object": "ibm_finding"
+                "key": "x-ocsf-malware.uid",
+                "object": "malware"
             }
         },
-        "http_request": {
-            "args": {
-                "key": "x-ocsf-http-request.value",
-                "object": "http_request"
-            },
-            "http_headers": {
+        "name": {
+            "key": "x-ocsf-malware.name",
+            "object": "malware"
+        },
+        "path": {
+            "key": "x-ocsf-malware.path",
+            "object": "malware"
+        },
+        "provider": {
+            "key": "x-ocsf-malware.provider",
+            "object": "malware"
+        },
+        "uid": {
+            "key": "x-ocsf-malware.uid",
+            "object": "malware"
+        }
+    },
+    "message": {
+        "key": "x-ocsf-cloud.message",
+        "object": "ocsf_cloud_api"
+    },
+    "metadata": {
+        "correlation_uid": {
+            "key": "x-ocsf-metadata.correlation_uid",
+            "object": "metadata"
+        },
+        "labels": {
+            "key": "x-ocsf-metadata.labels",
+            "object": "metadata"
+        },
+        "logged_time": {
+            "key": "x-ocsf-metadata.logged_time",
+            "object": "metadata"
+        },
+        "modified_time": {
+            "key": "x-ocsf-metadata.modified_time",
+            "object": "metadata"
+        },
+        "processed_time": {
+            "key": "x-ocsf-metadata.processed_time",
+            "object": "metadata"
+        },
+        "product": {
+            "feature": {
                 "name": {
-                    "key": "x-ocsf-http-request.http_headers_name",
-                    "object": "ocsf_cloud_api"
+                    "key": "software.extensions.x-ocsf-product-ext.feature_name",
+                    "object": "metadata-software"
                 },
-                "value": {
-                    "key": "x-ocsf-http-request.http_headers_value",
-                    "object": "http_request"
+                "uid": {
+                    "key": "software.extensions.x-ocsf-product-ext.feature_uid",
+                    "object": "metadata-software"
+                },
+                "version": {
+                    "key": "software.extensions.x-ocsf-product-ext.feature_version",
+                    "object": "metadata-software"
                 }
             },
-            "http_method": {
-                "key": "x-ocsf-http-request.http_method",
-                "object": "http_request"
+            "lang": {
+                "key": "software.languages",
+                "object": "metadata-software"
             },
-            "prefix": {
-                "key": "x-ocsf-http-request.prefix",
-                "object": "http_request"
+            "name": {
+                "key": "software.name",
+                "object": "metadata-software"
             },
-            "referrer": {
-                "key": "x-ocsf-http-request.referrer",
-                "object": "http_request"
+            "path": {
+                "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                "object": "metadata-software"
             },
             "uid": {
-                "key": "x-ocsf-http-request.uid",
-                "object": "http_request"
-            },
-            "url": {
-                "key": "url.value",
-                "object": "url"
+                "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                "object": "metadata-software"
             },
-            "user_agent": {
-                "key": "x-ocsf-http-request.user_agent",
-                "object": "http_request"
+            "vendor_name": {
+                "key": "software.vendor",
+                "object": "metadata-software"
             },
             "version": {
-                "key": "x-ocsf-http-request.version",
-                "object": "http_request"
+                "key": "software.version",
+                "object": "metadata-software"
+            }
+        },
+        "sequence": {
+            "key": "x-ocsf-metadata.sequence",
+            "object": "metadata",
+            "transformer": "ToInteger"
+        },
+        "uid": {
+            "key": "x-ocsf-metadata.uid",
+            "object": "metadata"
+        },
+        "version": {
+            "key": "x-ocsf-metadata.version",
+            "object": "metadata"
+        }
+    },
+    "observables": {
+        "name": [
+            {
+                "key": "x-ibm-observables.name",
+                "object": "observables"
             },
-            "x_forwarded_for": {
-                "key": "x-ocsf-http-request.x_forwarded_for",
-                "object": "http_request"
+            {
+                "key": "x-ibm-finding.ioc_refs",
+                "object": "ibm_finding",
+                "references": [
+                    "observables"
+                ]
             }
+        ],
+        "type": {
+            "key": "x-ibm-observables.finding_type",
+            "object": "observables"
         },
-        "identity": {
-            "authorizations": {
-                "decision": {
-                    "key": "x-ocsf-identity.authorizations.decision",
-                    "object": "x-ocsf-identity"
+        "type_id": {
+            "key": "x-ibm-observables.alert_id",
+            "object": "observables",
+            "transformer": "ToInteger"
+        },
+        "value": {
+            "key": "x-ibm-observables.description",
+            "object": "observables"
+        }
+    },
+    "process": {
+        "cmd_line": {
+            "key": "process.command_line",
+            "object": "process"
+        },
+        "created_time": {
+            "key": "process.created",
+            "object": "process"
+        },
+        "file": {
+            "accessed_time": {
+                "key": "file.accessed",
+                "object": "file"
+            },
+            "accessor": {
+                "account_type": {
+                    "key": "user-account.account_type",
+                    "object": "accessor-user-account"
                 },
-                "policy": {
+                "account_type_id": {
+                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                    "object": "accessor-user-account"
+                },
+                "account_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.account_uid",
+                    "object": "accessor-user-account"
+                },
+                "credential_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                    "object": "accessor-user-account"
+                },
+                "domain": {
+                    "key": "user-account.extensions.x-accessor-ext.domain",
+                    "object": "accessor-user-account"
+                },
+                "email_addr": {
+                    "key": "email-addr.value",
+                    "object": "email-addr"
+                },
+                "groups": {
                     "desc": {
-                        "key": "x-ocsf-identity.authorizations.policy_desc",
-                        "object": "x-ocsf-identity"
-                    },
-                    "group": {
-                        "desc": {
-                            "key": "x-ocsf-identity.authorizations.policy_group_desc",
-                            "object": "x-ocsf-identity"
-                        },
-                        "name": {
-                            "key": "x-ocsf-identity.authorizations.policy_group_namee",
-                            "object": "x-ocsf-identity"
-                        },
-                        "privileges": {
-                            "key": "x-ocsf-identity.authorizations.policy_group_privileges",
-                            "object": "x-ocsf-identity"
-                        },
-                        "type": {
-                            "key": "x-ocsf-identity.authorizations.policy_group_type",
-                            "object": "x-ocsf-identity"
-                        },
-                        "uid": {
-                            "key": "x-ocsf-identity.authorizations.policy_group_uid",
-                            "object": "x-ocsf-identity"
-                        }
+                        "key": "user-account.extensions.x-accessor-ext.group_desc",
+                        "object": "accessor-user-account"
                     },
                     "name": {
-                        "key": "x-ocsf-identity.authorizations.name",
-                        "object": "x-ocsf-identity"
+                        "key": "user-account.extensions.x-accessor-ext.group_name",
+                        "object": "accessor-user-account"
                     },
-                    "uid": {
-                        "key": "x-ocsf-identity.authorizations.uid",
-                        "object": "x-ocsf-identity"
+                    "privileges": {
+                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                        "object": "accessor-user-account"
                     },
-                    "version": {
-                        "key": "x-ocsf-identity.authorizations.version",
-                        "object": "x-ocsf-identity"
+                    "type": {
+                        "key": "user-account.extensions.x-accessor-ext.group_type",
+                        "object": "accessor-user-account"
+                    },
+                    "uid": {
+                        "key": "user-account.extensions.x-accessor-ext.group_uid",
+                        "object": "accessor-user-account"
                     }
-                }
-            },
-            "idp": {
+                },
                 "name": {
-                    "key": "x-ocsf-identity.idp.name",
-                    "object": "x-ocsf-identity"
+                    "key": "user-account.display_name",
+                    "object": "accessor-user-account"
                 },
-                "uid": {
-                    "key": "x-ocsf-identity.idp.uid",
-                    "object": "x-ocsf-identity"
-                }
-            },
-            "invoked_by": {
-                "key": "x-ocsf-identity.invoked_by",
-                "object": "x-ocsf-identity"
-            },
-            "message": {
-                "key": "x-ocsf-identity.message",
-                "object": "x-ocsf-identity"
-            },
-            "session": {
-                "created_time": {
-                    "key": "x-ocsf-identity.session.created_time",
-                    "object": "x-ocsf-identity"
+                "org_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.org_uid",
+                    "object": "accessor-user-account"
                 },
-                "credential_uid": {
-                    "key": "x-ocsf-identity.session.credential_uid",
-                    "object": "x-ocsf-identity"
+                "session_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.session_uid",
+                    "object": "accessor-user-account"
                 },
-                "expiration_time": {
-                    "key": "x-ocsf-identity.session.expiration_time",
-                    "object": "x-ocsf-identity"
+                "session_uuid": {
+                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                    "object": "accessor-user-account"
                 },
-                "issuer": {
-                    "key": "x-ocsf-identity.session.issuer",
-                    "object": "x-ocsf-identity"
+                "type": {
+                    "key": "user-account.extensions.x-accessor-ext.type",
+                    "object": "accessor-user-account"
                 },
-                "mfa": {
-                    "key": "x-ocsf-identity.session.mfa",
-                    "object": "x-ocsf-identity"
+                "type_id": {
+                    "key": "user-account.extensions.x-accessor-ext.type_id",
+                    "object": "accessor-user-account"
                 },
                 "uid": {
-                    "key": "x-ocsf-identity.session.uid",
-                    "object": "x-ocsf-identity"
+                    "key": "user-account.user_id",
+                    "object": "accessor-user-account"
+                },
+                "uuid": {
+                    "key": "user-account.extensions.x-accessor-ext.uuid",
+                    "object": "accessor-user-account"
                 }
             },
-            "user": {
+            "attributes": {
+                "key": "file.extensions.x-ocsf-file-ext.attributes",
+                "object": "file"
+            },
+            "company_name": {
+                "key": "file.extensions.x-ocsf-file-ext.company_name",
+                "object": "file"
+            },
+            "confidentiality": {
+                "key": "file.extensions.x-ocsf-file-ext.confidentiality",
+                "object": "file"
+            },
+            "confidentiality_id": {
+                "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
+                "object": "file"
+            },
+            "created_time": {
+                "key": "file.created",
+                "object": "file"
+            },
+            "creator": {
                 "account_type": {
                     "key": "user-account.account_type",
-                    "object": "user"
+                    "object": "creator-user-account"
                 },
                 "account_type_id": {
-                    "key": "user-account.extensions.aws-account-ext.account_type_id",
-                    "object": "user",
-                    "transformer": "ToInteger"
+                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                    "object": "creator-user-account"
                 },
                 "account_uid": {
-                    "key": "user-account.user_id",
-                    "object": "user"
+                    "key": "user-account.extensions.x-accessor-ext.account_uid",
+                    "object": "creator-user-account"
                 },
                 "credential_uid": {
-                    "key": "user-account.extensions.aws-account-ext.credential_uid",
-                    "object": "user"
+                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                    "object": "creator-user-account"
                 },
                 "domain": {
-                    "key": "user-account.extensions.aws-account-ext.domain",
-                    "object": "user"
+                    "key": "user-account.extensions.x-accessor-ext.domain",
+                    "object": "creator-user-account"
                 },
                 "email_addr": {
                     "key": "email-addr.value",
-                    "object": "email_addr"
+                    "object": "creator-email-addr"
                 },
                 "groups": {
                     "desc": {
-                        "key": "user-account.extensions.aws-account-ext.group_desc",
-                        "object": "user"
+                        "key": "user-account.extensions.x-accessor-ext.group_desc",
+                        "object": "creator-user-account"
                     },
                     "name": {
-                        "key": "user-account.extensions.aws-account-ext.group_name",
-                        "object": "user"
+                        "key": "user-account.extensions.x-accessor-ext.group_name",
+                        "object": "creator-user-account"
                     },
                     "privileges": {
-                        "key": "user-account.extensions.aws-account-ext.group_privileges",
-                        "object": "user"
+                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                        "object": "creator-user-account"
                     },
                     "type": {
-                        "key": "user-account.extensions.aws-account-ext.group_type",
-                        "object": "user"
+                        "key": "user-account.extensions.x-accessor-ext.group_type",
+                        "object": "creator-user-account"
                     },
                     "uid": {
-                        "key": "user-account.extensions.aws-account-ext.group_uid",
-                        "object": "user"
+                        "key": "user-account.extensions.x-accessor-ext.group_uid",
+                        "object": "creator-user-account"
                     }
                 },
                 "name": {
                     "key": "user-account.display_name",
-                    "object": "user"
+                    "object": "creator-user-account"
                 },
                 "org_uid": {
-                    "key": "user-account.extensions.aws-account-ext.org_uid",
-                    "object": "user"
+                    "key": "user-account.extensions.x-accessor-ext.org_uid",
+                    "object": "creator-user-account"
                 },
                 "session_uid": {
-                    "key": "user-account.extensions.aws-account-ext.session_uid",
-                    "object": "user"
+                    "key": "user-account.extensions.x-accessor-ext.session_uid",
+                    "object": "creator-user-account"
                 },
                 "session_uuid": {
-                    "key": "user-account.extensions.aws-account-ext.session_uuid",
-                    "object": "user"
+                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                    "object": "creator-user-account"
                 },
                 "type": {
-                    "key": "user-account.extensions.aws-account-ext.type",
-                    "object": "user"
+                    "key": "user-account.extensions.x-accessor-ext.type",
+                    "object": "creator-user-account"
                 },
                 "type_id": {
-                    "key": "user-account.extensions.aws-account-ext.type_id",
-                    "object": "user",
-                    "transformer": "ToInteger"
+                    "key": "user-account.extensions.x-accessor-ext.type_id",
+                    "object": "creator-user-account"
                 },
                 "uid": {
-                    "key": "user-account.extensions.aws-account-ext.uid",
-                    "object": "user"
+                    "key": "user-account.user_id",
+                    "object": "creator-user-account"
                 },
                 "uuid": {
-                    "key": "user-account.extensions.aws-account-ext.uuid",
-                    "object": "user"
+                    "key": "user-account.extensions.x-accessor-ext.uuid",
+                    "object": "creator-user-account"
                 }
-            }
-        },
-        "malware": {
-            "classification_ids": {
-                "key": "x-ocsf-malware.classification_ids",
-                "object": "malware"
             },
-            "classifications": {
-                "key": "x-ocsf-malware.classifications",
-                "object": "malware"
+            "desc": {
+                "key": "file.extensions.x-ocsf-file-ext.description",
+                "object": "file"
             },
-            "cves": {
-                "created_time": {
-                    "key": "x-ocsf-malware.created_time",
-                    "object": "malware"
+            "hashes": {
+                "CTPH": {
+                    "key": "file.hashes.CTPH",
+                    "object": "file"
                 },
-                "cvss": {
-                    "base_score": {
-                        "key": "x-ocsf-malware.base_score",
-                        "object": "malware"
-                    },
-                    "depth": {
-                        "key": "x-ocsf-malware.depth",
-                        "object": "malware"
-                    },
-                    "metrics": {
-                        "name": {
-                            "key": "x-ocsf-malware.name",
-                            "object": "malware"
-                        },
-                        "value": {
-                            "key": "x-ocsf-malware.value",
-                            "object": "malware"
-                        }
+                "MD5": {
+                    "key": "file.hashes.MD5",
+                    "object": "file"
+                },
+                "Other": {
+                    "key": "file.hashes.Other",
+                    "object": "file"
+                },
+                "SHA-1": {
+                    "key": "file.hashes.SHA-1",
+                    "object": "file"
+                },
+                "SHA-256": {
+                    "key": "file.hashes.SHA-256",
+                    "object": "file"
+                },
+                "SHA-512": {
+                    "key": "file.hashes.SHA-512",
+                    "object": "file"
+                },
+                "Unknown": {
+                    "key": "file.hashes.Unknown",
+                    "object": "file"
+                }
+            },
+            "is_system": {
+                "key": "process.extensions.x-ocsf-process-ext.is_system",
+                "object": "process"
+            },
+            "mime_type": {
+                "key": "process.mime_type",
+                "object": "process"
+            },
+            "modified_time": {
+                "key": "process.extensions.x-ocsf-process-ext.modified_time",
+                "object": "process"
+            },
+            "modifier": {
+                "account_type": {
+                    "key": "user-account.account_type",
+                    "object": "modifier-user-account"
+                },
+                "account_type_id": {
+                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                    "object": "modifier-user-account"
+                },
+                "account_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.account_uid",
+                    "object": "modifier-user-account"
+                },
+                "credential_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                    "object": "modifier-user-account"
+                },
+                "domain": {
+                    "key": "user-account.extensions.x-accessor-ext.domain",
+                    "object": "modifier-user-account"
+                },
+                "email_addr": {
+                    "key": "email-addr.value",
+                    "object": "modifier-email-addr"
+                },
+                "groups": {
+                    "desc": {
+                        "key": "user-account.extensions.x-accessor-ext.group_desc",
+                        "object": "modifier-user-account"
                     },
-                    "overall_score": {
-                        "key": "x-ocsf-malware.overall_score",
-                        "object": "malware"
+                    "name": {
+                        "key": "user-account.extensions.x-accessor-ext.group_name",
+                        "object": "modifier-user-account"
                     },
-                    "severity": {
-                        "key": "x-ocsf-malware.severity",
-                        "object": "malware"
+                    "privileges": {
+                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                        "object": "modifier-user-account"
                     },
-                    "vector_string": {
-                        "key": "x-ocsf-malware.vector_string",
-                        "object": "malware"
+                    "type": {
+                        "key": "user-account.extensions.x-accessor-ext.group_type",
+                        "object": "modifier-user-account"
                     },
-                    "version": {
-                        "key": "x-ocsf-malware.version",
-                        "object": "malware"
+                    "uid": {
+                        "key": "user-account.extensions.x-accessor-ext.group_uid",
+                        "object": "modifier-user-account"
                     }
                 },
-                "cwe_uid": {
-                    "key": "x-ocsf-malware.cwe_uid",
-                    "object": "malware"
+                "name": {
+                    "key": "user-account.display_name",
+                    "object": "modifier-user-account"
                 },
-                "cwe_url": {
-                    "key": "x-ocsf-malware.cwe_url",
-                    "object": "malware"
+                "org_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.org_uid",
+                    "object": "modifier-user-account"
                 },
-                "modified_time": {
-                    "key": "x-ocsf-malware.modified_time",
-                    "object": "malware"
+                "session_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.session_uid",
+                    "object": "modifier-user-account"
                 },
-                "product": {
-                    "feature": {
-                        "name": {
-                            "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                            "object": "malware-software"
-                        },
-                        "uid": {
-                            "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                            "object": "malware-software"
-                        },
-                        "version": {
-                            "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                            "object": "malware-software"
-                        }
-                    },
-                    "lang": {
-                        "key": "software.languages",
-                        "object": "malware-software"
+                "session_uuid": {
+                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                    "object": "modifier-user-account"
+                },
+                "type": {
+                    "key": "user-account.extensions.x-accessor-ext.type",
+                    "object": "modifier-user-account"
+                },
+                "type_id": {
+                    "key": "user-account.extensions.x-accessor-ext.type_id",
+                    "object": "modifier-user-account"
+                },
+                "uid": {
+                    "key": "user-account.user_id",
+                    "object": "modifier-user-account"
+                },
+                "uuid": {
+                    "key": "user-account.extensions.x-accessor-ext.uuid",
+                    "object": "modifier-user-account"
+                }
+            },
+            "name": [
+                {
+                    "key": "file.name",
+                    "object": "file"
+                },
+                {
+                    "key": "process.binary_ref",
+                    "object": "process",
+                    "references": "file"
+                }
+            ],
+            "owner": {
+                "account_type": {
+                    "key": "user-account.account_type",
+                    "object": "owner-user-account"
+                },
+                "account_type_id": {
+                    "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                    "object": "owner-user-account"
+                },
+                "account_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.account_uid",
+                    "object": "owner-user-account"
+                },
+                "credential_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                    "object": "owner-user-account"
+                },
+                "domain": {
+                    "key": "user-account.extensions.x-accessor-ext.domain",
+                    "object": "owner-user-account"
+                },
+                "email_addr": {
+                    "key": "email-addr.value",
+                    "object": "owner-user-account"
+                },
+                "groups": {
+                    "desc": {
+                        "key": "user-account.extensions.x-accessor-ext.group_desc",
+                        "object": "owner-user-account"
                     },
                     "name": {
-                        "key": "software.name",
-                        "object": "malware-software"
-                    },
-                    "path": {
-                        "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                        "object": "malware-software"
+                        "key": "user-account.extensions.x-accessor-ext.group_name",
+                        "object": "owner-user-account"
                     },
-                    "uid": {
-                        "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                        "object": "malware-software"
+                    "privileges": {
+                        "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                        "object": "owner-user-account"
                     },
-                    "vendor_name": {
-                        "key": "software.vendor",
-                        "object": "malware-software"
+                    "type": {
+                        "key": "user-account.extensions.x-accessor-ext.group_type",
+                        "object": "owner-user-account"
                     },
-                    "version": {
-                        "key": "software.version",
-                        "object": "malware-software"
+                    "uid": {
+                        "key": "user-account.extensions.x-accessor-ext.group_uid",
+                        "object": "owner-user-account"
                     }
                 },
+                "name": {
+                    "key": "user-account.display_name",
+                    "object": "owner-user-account"
+                },
+                "org_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.org_uid",
+                    "object": "owner-user-account"
+                },
+                "session_uid": {
+                    "key": "user-account.extensions.x-accessor-ext.session_uid",
+                    "object": "owner-user-account"
+                },
+                "session_uuid": {
+                    "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                    "object": "owner-user-account"
+                },
                 "type": {
-                    "key": "x-ocsf-malware.type",
-                    "object": "malware"
+                    "key": "user-account.extensions.x-accessor-ext.type",
+                    "object": "owner-user-account"
+                },
+                "type_id": {
+                    "key": "user-account.extensions.x-accessor-ext.type_id",
+                    "object": "owner-user-account"
                 },
                 "uid": {
-                    "key": "x-ocsf-malware.uid",
-                    "object": "malware"
+                    "key": "user-account.user_id",
+                    "object": "owner-user-account"
+                },
+                "uuid": {
+                    "key": "user-account.extensions.x-accessor-ext.uuid",
+                    "object": "owner-user-account"
                 }
             },
-            "name": {
-                "key": "x-ocsf-malware.name",
-                "object": "malware"
-            },
+            "parent_folder": [
+                {
+                    "key": "directory.path",
+                    "object": "directory"
+                },
+                {
+                    "key": "file.parent_directory_ref",
+                    "object": "file",
+                    "references": "directory"
+                }
+            ],
             "path": {
-                "key": "x-ocsf-malware.path",
-                "object": "malware"
-            },
-            "provider": {
-                "key": "x-ocsf-malware.provider",
-                "object": "malware"
-            },
-            "uid": {
-                "key": "x-ocsf-malware.uid",
-                "object": "malware"
-            }
-        },
-        "message": {
-            "key": "x-ocsf-cloud.message",
-            "object": "ocsf_cloud_api"
-        },
-        "metadata": {
-            "correlation_uid": {
-                "key": "x-ocsf-metadata.correlation_uid",
-                "object": "metadata"
-            },
-            "labels": {
-                "key": "x-ocsf-metadata.labels",
-                "object": "metadata"
-            },
-            "logged_time": {
-                "key": "x-ocsf-metadata.logged_time",
-                "object": "metadata"
-            },
-            "modified_time": {
-                "key": "x-ocsf-metadata.modified_time",
-                "object": "metadata"
-            },
-            "processed_time": {
-                "key": "x-ocsf-metadata.processed_time",
-                "object": "metadata"
+                "key": "file.extensions.x-ocsf-file-ext.path",
+                "object": "file"
             },
             "product": {
                 "feature": {
                     "name": {
                         "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                        "object": "metadata-software"
+                        "object": "file1-software"
                     },
                     "uid": {
                         "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                        "object": "metadata-software"
+                        "object": "file1-software"
                     },
                     "version": {
                         "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                        "object": "metadata-software"
+                        "object": "file1-software"
                     }
                 },
                 "lang": {
                     "key": "software.languages",
-                    "object": "metadata-software"
+                    "object": "file1-software"
                 },
                 "name": {
                     "key": "software.name",
-                    "object": "metadata-software"
+                    "object": "file1-software"
                 },
                 "path": {
                     "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                    "object": "metadata-software"
+                    "object": "file1-software"
                 },
                 "uid": {
                     "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                    "object": "metadata-software"
+                    "object": "file1-software"
                 },
                 "vendor_name": {
                     "key": "software.vendor",
-                    "object": "metadata-software"
+                    "object": "file1-software"
                 },
                 "version": {
                     "key": "software.version",
-                    "object": "metadata-software"
+                    "object": "file1-software"
                 }
             },
-            "sequence": {
-                "key": "x-ocsf-metadata.sequence",
-                "object": "metadata",
-                "transformer": "ToInteger"
+            "security_descriptor": {
+                "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
+                "object": "file"
             },
-            "uid": {
-                "key": "x-ocsf-metadata.uid",
-                "object": "metadata"
+            "signature": {
+                "key": "file.extensions.x-ocsf-file-ext.signature",
+                "object": "file"
+            },
+            "size": {
+                "key": "file.size",
+                "object": "file"
             },
-            "version": {
-                "key": "x-ocsf-metadata.version",
-                "object": "metadata"
-            }
-        },
-        "observables": {
-            "name": [
-                {
-                    "key": "x-ibm-observables.name",
-                    "object": "observables"
-                },
-                {
-                    "key": "x-ibm-finding.ioc_refs",
-                    "object": "ibm_finding",
-                    "references": [
-                        "observables"
-                    ]
-                }
-            ],
             "type": {
-                "key": "x-ibm-observables.finding_type",
-                "object": "observables"
+                "key": "file.extensions.x-ocsf-file-ext.type",
+                "object": "file"
             },
             "type_id": {
-                "key": "x-ibm-observables.alert_id",
-                "object": "observables",
-                "transformer": "ToInteger"
+                "key": "file.extensions.x-ocsf-file-ext.type_id",
+                "object": "file"
             },
-            "value": {
-                "key": "x-ibm-observables.description",
-                "object": "observables"
+            "uid": {
+                "key": "file.extensions.x-ocsf-file-ext.uid",
+                "object": "file"
+            },
+            "version": {
+                "key": "file.extensions.x-ocsf-file-ext.version",
+                "object": "file"
+            },
+            "xattributes": {
+                "key": "process.extensions.x-ocsf-process-ext.xattributes",
+                "object": "process"
             }
         },
-        "process": {
+        "integrity": {
+            "key": "process.extensions.x-ocsf-process-ext.integrity",
+            "object": "process"
+        },
+        "integrity_id": {
+            "key": "process.extensions.x-ocsf-process-ext.integrity_id",
+            "object": "process"
+        },
+        "lineage": {
+            "key": "process.extensions.x-ocsf-process-ext.lineage",
+            "object": "process"
+        },
+        "loaded_modules": {
+            "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
+            "object": "process"
+        },
+        "name": {
+            "key": "process.name",
+            "object": "process"
+        },
+        "parent_process": {
             "cmd_line": {
                 "key": "process.command_line",
-                "object": "process"
+                "object": "parent-process"
             },
             "created_time": {
                 "key": "process.created",
-                "object": "process"
+                "object": "parent-process"
             },
             "file": {
                 "accessed_time": {
                     "key": "file.accessed",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "accessor": {
                     "account_type": {
                         "key": "user-account.account_type",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "account_type_id": {
                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "account_uid": {
                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "credential_uid": {
                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "domain": {
                         "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "email_addr": {
                         "key": "email-addr.value",
-                        "object": "email-addr"
+                        "object": "parent-email-addr"
                     },
                     "groups": {
                         "desc": {
                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "accessor-user-account"
+                            "object": "parent-accessor-user-account"
                         },
                         "name": {
                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "accessor-user-account"
+                            "object": "parent-accessor-user-account"
                         },
                         "privileges": {
                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "accessor-user-account"
+                            "object": "parent-accessor-user-account"
                         },
                         "type": {
                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "accessor-user-account"
+                            "object": "parent-accessor-user-account"
                         },
                         "uid": {
                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "accessor-user-account"
+                            "object": "parent-accessor-user-account"
                         }
                     },
                     "name": {
                         "key": "user-account.display_name",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "org_uid": {
                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "session_uid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "session_uuid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "type_id": {
                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "uid": {
                         "key": "user-account.user_id",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     },
                     "uuid": {
                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "accessor-user-account"
+                        "object": "parent-accessor-user-account"
                     }
                 },
                 "attributes": {
                     "key": "file.extensions.x-ocsf-file-ext.attributes",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "company_name": {
                     "key": "file.extensions.x-ocsf-file-ext.company_name",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "confidentiality": {
                     "key": "file.extensions.x-ocsf-file-ext.confidentiality",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "confidentiality_id": {
                     "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "created_time": {
                     "key": "file.created",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "creator": {
                     "account_type": {
                         "key": "user-account.account_type",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "account_type_id": {
                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "account_uid": {
                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "credential_uid": {
                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "domain": {
                         "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "email_addr": {
                         "key": "email-addr.value",
-                        "object": "creator-email-addr"
+                        "object": "parent-creator-email-addr"
                     },
                     "groups": {
                         "desc": {
                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "creator-user-account"
+                            "object": "parent-creator-user-account"
                         },
                         "name": {
                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "creator-user-account"
+                            "object": "parent-creator-user-account"
                         },
                         "privileges": {
                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "creator-user-account"
+                            "object": "parent-creator-user-account"
                         },
                         "type": {
                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "creator-user-account"
+                            "object": "parent-creator-user-account"
                         },
                         "uid": {
                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "creator-user-account"
+                            "object": "parent-creator-user-account"
                         }
                     },
                     "name": {
                         "key": "user-account.display_name",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "org_uid": {
                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "session_uid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "session_uuid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "type_id": {
                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "uid": {
                         "key": "user-account.user_id",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     },
                     "uuid": {
                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "creator-user-account"
+                        "object": "parent-creator-user-account"
                     }
                 },
                 "desc": {
                     "key": "file.extensions.x-ocsf-file-ext.description",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "hashes": {
                     "CTPH": {
                         "key": "file.hashes.CTPH",
-                        "object": "file"
+                        "object": "parent-file"
                     },
                     "MD5": {
                         "key": "file.hashes.MD5",
-                        "object": "file"
+                        "object": "parent-file"
                     },
                     "Other": {
                         "key": "file.hashes.Other",
-                        "object": "file"
+                        "object": "parent-file"
                     },
                     "SHA-1": {
                         "key": "file.hashes.SHA-1",
-                        "object": "file"
+                        "object": "parent-file"
                     },
                     "SHA-256": {
                         "key": "file.hashes.SHA-256",
-                        "object": "file"
+                        "object": "parent-file"
                     },
                     "SHA-512": {
                         "key": "file.hashes.SHA-512",
-                        "object": "file"
+                        "object": "parent-file"
                     },
                     "Unknown": {
                         "key": "file.hashes.Unknown",
-                        "object": "file"
+                        "object": "parent-file"
                     }
                 },
                 "is_system": {
                     "key": "process.extensions.x-ocsf-process-ext.is_system",
-                    "object": "process"
+                    "object": "parent-process"
                 },
                 "mime_type": {
                     "key": "process.mime_type",
-                    "object": "process"
+                    "object": "parent-process"
                 },
                 "modified_time": {
                     "key": "process.extensions.x-ocsf-process-ext.modified_time",
-                    "object": "process"
+                    "object": "parent-process"
                 },
                 "modifier": {
                     "account_type": {
                         "key": "user-account.account_type",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "account_type_id": {
                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "account_uid": {
                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "credential_uid": {
                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "domain": {
                         "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "email_addr": {
                         "key": "email-addr.value",
-                        "object": "modifier-email-addr"
+                        "object": "parent-modifier-email-addr"
                     },
                     "groups": {
                         "desc": {
                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "modifier-user-account"
+                            "object": "parent-modifier-user-account"
                         },
                         "name": {
                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "modifier-user-account"
+                            "object": "parent-modifier-user-account"
                         },
                         "privileges": {
                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "modifier-user-account"
+                            "object": "parent-modifier-user-account"
                         },
                         "type": {
                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "modifier-user-account"
+                            "object": "parent-modifier-user-account"
                         },
                         "uid": {
                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "modifier-user-account"
+                            "object": "parent-modifier-user-account"
                         }
                     },
                     "name": {
                         "key": "user-account.display_name",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "org_uid": {
                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "session_uid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "session_uuid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "type_id": {
                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "uid": {
                         "key": "user-account.user_id",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     },
                     "uuid": {
                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "modifier-user-account"
+                        "object": "parent-modifier-user-account"
                     }
                 },
                 "name": [
                     {
                         "key": "file.name",
-                        "object": "file"
+                        "object": "parent-file"
                     },
                     {
                         "key": "process.binary_ref",
-                        "object": "process",
-                        "references": "file"
+                        "object": "parent-process",
+                        "references": "parent-file"
                     }
                 ],
                 "owner": {
                     "account_type": {
                         "key": "user-account.account_type",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "account_type_id": {
                         "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "account_uid": {
                         "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "credential_uid": {
                         "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "domain": {
                         "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "email_addr": {
                         "key": "email-addr.value",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-email-addr"
                     },
                     "groups": {
                         "desc": {
                             "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "owner-user-account"
+                            "object": "parent-owner-user-account"
                         },
                         "name": {
                             "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "owner-user-account"
+                            "object": "parent-owner-user-account"
                         },
                         "privileges": {
                             "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "owner-user-account"
+                            "object": "parent-owner-user-account"
                         },
                         "type": {
                             "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "owner-user-account"
+                            "object": "parent-owner-user-account"
                         },
                         "uid": {
                             "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "owner-user-account"
+                            "object": "parent-owner-user-account"
                         }
                     },
                     "name": {
                         "key": "user-account.display_name",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "org_uid": {
                         "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "session_uid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "session_uuid": {
                         "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "type_id": {
                         "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "uid": {
                         "key": "user-account.user_id",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     },
                     "uuid": {
                         "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "owner-user-account"
+                        "object": "parent-owner-user-account"
                     }
                 },
                 "parent_folder": [
                     {
                         "key": "directory.path",
-                        "object": "directory"
+                        "object": "parent-directory"
                     },
                     {
                         "key": "file.parent_directory_ref",
-                        "object": "file",
-                        "references": "directory"
+                        "object": "parent-file",
+                        "references": "parent-directory"
                     }
                 ],
                 "path": {
                     "key": "file.extensions.x-ocsf-file-ext.path",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "product": {
                     "feature": {
                         "name": {
                             "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                            "object": "file1-software"
+                            "object": "file-software"
                         },
                         "uid": {
                             "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                            "object": "file1-software"
+                            "object": "file-software"
                         },
                         "version": {
                             "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                            "object": "file1-software"
+                            "object": "file-software"
                         }
                     },
                     "lang": {
                         "key": "software.languages",
-                        "object": "file1-software"
+                        "object": "file-software"
                     },
                     "name": {
                         "key": "software.name",
-                        "object": "file1-software"
+                        "object": "file-software"
                     },
                     "path": {
                         "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                        "object": "file1-software"
+                        "object": "file-software"
                     },
                     "uid": {
                         "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                        "object": "file1-software"
+                        "object": "file-software"
                     },
                     "vendor_name": {
                         "key": "software.vendor",
-                        "object": "file1-software"
+                        "object": "file-software"
                     },
                     "version": {
                         "key": "software.version",
-                        "object": "file1-software"
+                        "object": "file-software"
                     }
                 },
                 "security_descriptor": {
                     "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "signature": {
                     "key": "file.extensions.x-ocsf-file-ext.signature",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "size": {
                     "key": "file.size",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "type": {
                     "key": "file.extensions.x-ocsf-file-ext.type",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "type_id": {
                     "key": "file.extensions.x-ocsf-file-ext.type_id",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "uid": {
                     "key": "file.extensions.x-ocsf-file-ext.uid",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "version": {
                     "key": "file.extensions.x-ocsf-file-ext.version",
-                    "object": "file"
+                    "object": "parent-file"
                 },
                 "xattributes": {
                     "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                    "object": "process"
+                    "object": "parent-process"
                 }
             },
             "integrity": {
                 "key": "process.extensions.x-ocsf-process-ext.integrity",
-                "object": "process"
+                "object": "parent-process"
             },
             "integrity_id": {
                 "key": "process.extensions.x-ocsf-process-ext.integrity_id",
-                "object": "process"
+                "object": "parent-process"
             },
             "lineage": {
                 "key": "process.extensions.x-ocsf-process-ext.lineage",
-                "object": "process"
+                "object": "parent-process"
             },
             "loaded_modules": {
                 "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                "object": "process"
+                "object": "parent-process"
             },
             "name": {
                 "key": "process.name",
-                "object": "process"
-            },
-            "parent_process": {
-                "cmd_line": {
-                    "key": "process.command_line",
-                    "object": "parent-process"
-                },
-                "created_time": {
-                    "key": "process.created",
-                    "object": "parent-process"
-                },
-                "file": {
-                    "accessed_time": {
-                        "key": "file.accessed",
-                        "object": "parent-file"
-                    },
-                    "accessor": {
-                        "account_type": {
-                            "key": "user-account.account_type",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "account_type_id": {
-                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "account_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.account_uid",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "credential_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "domain": {
-                            "key": "user-account.extensions.x-accessor-ext.domain",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "email_addr": {
-                            "key": "email-addr.value",
-                            "object": "parent-email-addr"
-                        },
-                        "groups": {
-                            "desc": {
-                                "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                "object": "parent-accessor-user-account"
-                            },
-                            "name": {
-                                "key": "user-account.extensions.x-accessor-ext.group_name",
-                                "object": "parent-accessor-user-account"
-                            },
-                            "privileges": {
-                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                "object": "parent-accessor-user-account"
-                            },
-                            "type": {
-                                "key": "user-account.extensions.x-accessor-ext.group_type",
-                                "object": "parent-accessor-user-account"
-                            },
-                            "uid": {
-                                "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                "object": "parent-accessor-user-account"
-                            }
-                        },
-                        "name": {
-                            "key": "user-account.display_name",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "org_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.org_uid",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "session_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.session_uid",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "session_uuid": {
-                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "type": {
-                            "key": "user-account.extensions.x-accessor-ext.type",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "type_id": {
-                            "key": "user-account.extensions.x-accessor-ext.type_id",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "uid": {
-                            "key": "user-account.user_id",
-                            "object": "parent-accessor-user-account"
-                        },
-                        "uuid": {
-                            "key": "user-account.extensions.x-accessor-ext.uuid",
-                            "object": "parent-accessor-user-account"
-                        }
-                    },
-                    "attributes": {
-                        "key": "file.extensions.x-ocsf-file-ext.attributes",
-                        "object": "parent-file"
-                    },
-                    "company_name": {
-                        "key": "file.extensions.x-ocsf-file-ext.company_name",
-                        "object": "parent-file"
-                    },
-                    "confidentiality": {
-                        "key": "file.extensions.x-ocsf-file-ext.confidentiality",
-                        "object": "parent-file"
-                    },
-                    "confidentiality_id": {
-                        "key": "file.extensions.x-ocsf-file-ext.confidentiality_id",
-                        "object": "parent-file"
-                    },
-                    "created_time": {
-                        "key": "file.created",
-                        "object": "parent-file"
-                    },
-                    "creator": {
-                        "account_type": {
-                            "key": "user-account.account_type",
-                            "object": "parent-creator-user-account"
-                        },
-                        "account_type_id": {
-                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                            "object": "parent-creator-user-account"
-                        },
-                        "account_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.account_uid",
-                            "object": "parent-creator-user-account"
-                        },
-                        "credential_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                            "object": "parent-creator-user-account"
-                        },
-                        "domain": {
-                            "key": "user-account.extensions.x-accessor-ext.domain",
-                            "object": "parent-creator-user-account"
-                        },
-                        "email_addr": {
-                            "key": "email-addr.value",
-                            "object": "parent-creator-email-addr"
-                        },
-                        "groups": {
-                            "desc": {
-                                "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                "object": "parent-creator-user-account"
-                            },
-                            "name": {
-                                "key": "user-account.extensions.x-accessor-ext.group_name",
-                                "object": "parent-creator-user-account"
-                            },
-                            "privileges": {
-                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                "object": "parent-creator-user-account"
-                            },
-                            "type": {
-                                "key": "user-account.extensions.x-accessor-ext.group_type",
-                                "object": "parent-creator-user-account"
-                            },
-                            "uid": {
-                                "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                "object": "parent-creator-user-account"
-                            }
-                        },
-                        "name": {
-                            "key": "user-account.display_name",
-                            "object": "parent-creator-user-account"
-                        },
-                        "org_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.org_uid",
-                            "object": "parent-creator-user-account"
-                        },
-                        "session_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.session_uid",
-                            "object": "parent-creator-user-account"
-                        },
-                        "session_uuid": {
-                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                            "object": "parent-creator-user-account"
-                        },
-                        "type": {
-                            "key": "user-account.extensions.x-accessor-ext.type",
-                            "object": "parent-creator-user-account"
-                        },
-                        "type_id": {
-                            "key": "user-account.extensions.x-accessor-ext.type_id",
-                            "object": "parent-creator-user-account"
-                        },
-                        "uid": {
-                            "key": "user-account.user_id",
-                            "object": "parent-creator-user-account"
-                        },
-                        "uuid": {
-                            "key": "user-account.extensions.x-accessor-ext.uuid",
-                            "object": "parent-creator-user-account"
-                        }
-                    },
-                    "desc": {
-                        "key": "file.extensions.x-ocsf-file-ext.description",
-                        "object": "parent-file"
-                    },
-                    "hashes": {
-                        "CTPH": {
-                            "key": "file.hashes.CTPH",
-                            "object": "parent-file"
-                        },
-                        "MD5": {
-                            "key": "file.hashes.MD5",
-                            "object": "parent-file"
-                        },
-                        "Other": {
-                            "key": "file.hashes.Other",
-                            "object": "parent-file"
-                        },
-                        "SHA-1": {
-                            "key": "file.hashes.SHA-1",
-                            "object": "parent-file"
-                        },
-                        "SHA-256": {
-                            "key": "file.hashes.SHA-256",
-                            "object": "parent-file"
-                        },
-                        "SHA-512": {
-                            "key": "file.hashes.SHA-512",
-                            "object": "parent-file"
-                        },
-                        "Unknown": {
-                            "key": "file.hashes.Unknown",
-                            "object": "parent-file"
-                        }
-                    },
-                    "is_system": {
-                        "key": "process.extensions.x-ocsf-process-ext.is_system",
-                        "object": "parent-process"
-                    },
-                    "mime_type": {
-                        "key": "process.mime_type",
-                        "object": "parent-process"
-                    },
-                    "modified_time": {
-                        "key": "process.extensions.x-ocsf-process-ext.modified_time",
-                        "object": "parent-process"
-                    },
-                    "modifier": {
-                        "account_type": {
-                            "key": "user-account.account_type",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "account_type_id": {
-                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "account_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.account_uid",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "credential_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "domain": {
-                            "key": "user-account.extensions.x-accessor-ext.domain",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "email_addr": {
-                            "key": "email-addr.value",
-                            "object": "parent-modifier-email-addr"
-                        },
-                        "groups": {
-                            "desc": {
-                                "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                "object": "parent-modifier-user-account"
-                            },
-                            "name": {
-                                "key": "user-account.extensions.x-accessor-ext.group_name",
-                                "object": "parent-modifier-user-account"
-                            },
-                            "privileges": {
-                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                "object": "parent-modifier-user-account"
-                            },
-                            "type": {
-                                "key": "user-account.extensions.x-accessor-ext.group_type",
-                                "object": "parent-modifier-user-account"
-                            },
-                            "uid": {
-                                "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                "object": "parent-modifier-user-account"
-                            }
-                        },
-                        "name": {
-                            "key": "user-account.display_name",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "org_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.org_uid",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "session_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.session_uid",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "session_uuid": {
-                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "type": {
-                            "key": "user-account.extensions.x-accessor-ext.type",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "type_id": {
-                            "key": "user-account.extensions.x-accessor-ext.type_id",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "uid": {
-                            "key": "user-account.user_id",
-                            "object": "parent-modifier-user-account"
-                        },
-                        "uuid": {
-                            "key": "user-account.extensions.x-accessor-ext.uuid",
-                            "object": "parent-modifier-user-account"
-                        }
-                    },
-                    "name": [
-                        {
-                            "key": "file.name",
-                            "object": "parent-file"
-                        },
-                        {
-                            "key": "process.binary_ref",
-                            "object": "parent-process",
-                            "references": "parent-file"
-                        }
-                    ],
-                    "owner": {
-                        "account_type": {
-                            "key": "user-account.account_type",
-                            "object": "parent-owner-user-account"
-                        },
-                        "account_type_id": {
-                            "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                            "object": "parent-owner-user-account"
-                        },
-                        "account_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.account_uid",
-                            "object": "parent-owner-user-account"
-                        },
-                        "credential_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                            "object": "parent-owner-user-account"
-                        },
-                        "domain": {
-                            "key": "user-account.extensions.x-accessor-ext.domain",
-                            "object": "parent-owner-user-account"
-                        },
-                        "email_addr": {
-                            "key": "email-addr.value",
-                            "object": "parent-owner-email-addr"
-                        },
-                        "groups": {
-                            "desc": {
-                                "key": "user-account.extensions.x-accessor-ext.group_desc",
-                                "object": "parent-owner-user-account"
-                            },
-                            "name": {
-                                "key": "user-account.extensions.x-accessor-ext.group_name",
-                                "object": "parent-owner-user-account"
-                            },
-                            "privileges": {
-                                "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                                "object": "parent-owner-user-account"
-                            },
-                            "type": {
-                                "key": "user-account.extensions.x-accessor-ext.group_type",
-                                "object": "parent-owner-user-account"
-                            },
-                            "uid": {
-                                "key": "user-account.extensions.x-accessor-ext.group_uid",
-                                "object": "parent-owner-user-account"
-                            }
-                        },
-                        "name": {
-                            "key": "user-account.display_name",
-                            "object": "parent-owner-user-account"
-                        },
-                        "org_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.org_uid",
-                            "object": "parent-owner-user-account"
-                        },
-                        "session_uid": {
-                            "key": "user-account.extensions.x-accessor-ext.session_uid",
-                            "object": "parent-owner-user-account"
-                        },
-                        "session_uuid": {
-                            "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                            "object": "parent-owner-user-account"
-                        },
-                        "type": {
-                            "key": "user-account.extensions.x-accessor-ext.type",
-                            "object": "parent-owner-user-account"
-                        },
-                        "type_id": {
-                            "key": "user-account.extensions.x-accessor-ext.type_id",
-                            "object": "parent-owner-user-account"
-                        },
-                        "uid": {
-                            "key": "user-account.user_id",
-                            "object": "parent-owner-user-account"
-                        },
-                        "uuid": {
-                            "key": "user-account.extensions.x-accessor-ext.uuid",
-                            "object": "parent-owner-user-account"
-                        }
-                    },
-                    "parent_folder": [
-                        {
-                            "key": "directory.path",
-                            "object": "parent-directory"
-                        },
-                        {
-                            "key": "file.parent_directory_ref",
-                            "object": "parent-file",
-                            "references": "parent-directory"
-                        }
-                    ],
-                    "path": {
-                        "key": "file.extensions.x-ocsf-file-ext.path",
-                        "object": "parent-file"
-                    },
-                    "product": {
-                        "feature": {
-                            "name": {
-                                "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                                "object": "file-software"
-                            },
-                            "uid": {
-                                "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                                "object": "file-software"
-                            },
-                            "version": {
-                                "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                                "object": "file-software"
-                            }
-                        },
-                        "lang": {
-                            "key": "software.languages",
-                            "object": "file-software"
-                        },
-                        "name": {
-                            "key": "software.name",
-                            "object": "file-software"
-                        },
-                        "path": {
-                            "key": "software.extensions.x-ocsf-product-ext.installed_path",
-                            "object": "file-software"
-                        },
-                        "uid": {
-                            "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                            "object": "file-software"
-                        },
-                        "vendor_name": {
-                            "key": "software.vendor",
-                            "object": "file-software"
-                        },
-                        "version": {
-                            "key": "software.version",
-                            "object": "file-software"
-                        }
-                    },
-                    "security_descriptor": {
-                        "key": "file.extensions.x-ocsf-file-ext.security_descriptor",
-                        "object": "parent-file"
-                    },
-                    "signature": {
-                        "key": "file.extensions.x-ocsf-file-ext.signature",
-                        "object": "parent-file"
-                    },
-                    "size": {
-                        "key": "file.size",
-                        "object": "parent-file"
-                    },
-                    "type": {
-                        "key": "file.extensions.x-ocsf-file-ext.type",
-                        "object": "parent-file"
-                    },
-                    "type_id": {
-                        "key": "file.extensions.x-ocsf-file-ext.type_id",
-                        "object": "parent-file"
-                    },
-                    "uid": {
-                        "key": "file.extensions.x-ocsf-file-ext.uid",
-                        "object": "parent-file"
-                    },
-                    "version": {
-                        "key": "file.extensions.x-ocsf-file-ext.version",
-                        "object": "parent-file"
-                    },
-                    "xattributes": {
-                        "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                        "object": "parent-process"
-                    }
-                },
-                "integrity": {
-                    "key": "process.extensions.x-ocsf-process-ext.integrity",
-                    "object": "parent-process"
-                },
-                "integrity_id": {
-                    "key": "process.extensions.x-ocsf-process-ext.integrity_id",
-                    "object": "parent-process"
-                },
-                "lineage": {
-                    "key": "process.extensions.x-ocsf-process-ext.lineage",
-                    "object": "parent-process"
-                },
-                "loaded_modules": {
-                    "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                    "object": "parent-process"
-                },
-                "name": {
-                    "key": "process.name",
-                    "object": "parent-process"
-                },
-                "pid": [
-                    {
-                        "key": "process.pid",
-                        "object": "parent-process"
-                    },
-                    {
-                        "key": "process.child_refs",
-                        "object": "parent-process",
-                        "references": [
-                            "process"
-                        ]
-                    }
-                ],
-                "sandbox": {
-                    "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                    "object": "parent-process"
-                },
-                "terminated_time": {
-                    "key": "process.extensions.x-ocsf-process-ext.terminated_time",
-                    "object": "parent-process"
-                },
-                "tid": {
-                    "key": "process.extensions.x-ocsf-process-ext.tid",
-                    "object": "parent-process"
-                },
-                "uid": {
-                    "key": "process.x_unique_id",
-                    "object": "parent-process"
-                },
-                "user": {
-                    "account_type": {
-                        "key": "user-account.account_type",
-                        "object": "parent-process-user-account"
-                    },
-                    "account_type_id": {
-                        "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                        "object": "parent-process-user-account"
-                    },
-                    "account_uid": {
-                        "key": "user-account.extensions.x-accessor-ext.account_uid",
-                        "object": "parent-process-user-account"
-                    },
-                    "credential_uid": {
-                        "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                        "object": "parent-process-user-account"
-                    },
-                    "domain": {
-                        "key": "user-account.extensions.x-accessor-ext.domain",
-                        "object": "parent-process-user-account"
-                    },
-                    "email_addr": {
-                        "key": "email-addr.value",
-                        "object": "parent-process-email-addr"
-                    },
-                    "groups": {
-                        "desc": {
-                            "key": "user-account.extensions.x-accessor-ext.group_desc",
-                            "object": "parent-process-user-account"
-                        },
-                        "name": {
-                            "key": "user-account.extensions.x-accessor-ext.group_name",
-                            "object": "parent-process-user-account"
-                        },
-                        "privileges": {
-                            "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                            "object": "parent-process-user-account"
-                        },
-                        "type": {
-                            "key": "user-account.extensions.x-accessor-ext.group_type",
-                            "object": "parent-process-user-account"
-                        },
-                        "uid": {
-                            "key": "user-account.extensions.x-accessor-ext.group_uid",
-                            "object": "parent-process-user-account"
-                        }
-                    },
-                    "name": {
-                        "key": "user-account.display_name",
-                        "object": "parent-process-user-account"
-                    },
-                    "org_uid": {
-                        "key": "user-account.extensions.x-accessor-ext.org_uid",
-                        "object": "parent-process-user-account"
-                    },
-                    "session_uid": {
-                        "key": "user-account.extensions.x-accessor-ext.session_uid",
-                        "object": "parent-process-user-account"
-                    },
-                    "session_uuid": {
-                        "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                        "object": "parent-process-user-account"
-                    },
-                    "type": {
-                        "key": "user-account.extensions.x-accessor-ext.type",
-                        "object": "parent-process-user-account"
-                    },
-                    "type_id": {
-                        "key": "user-account.extensions.x-accessor-ext.type_id",
-                        "object": "parent-process-user-account"
-                    },
-                    "uid": [
-                        {
-                            "key": "user-account.user_id",
-                            "object": "parent-process-user-account"
-                        },
-                        {
-                            "key": "user-account.creator_user_ref",
-                            "object": "parent-process",
-                            "references": "process-user-account"
-                        }
-                    ],
-                    "uuid": {
-                        "key": "user-account.extensions.x-accessor-ext.uuid",
-                        "object": "parent-process-user-account"
-                    }
-                },
-                "xattributes": {
-                    "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                    "object": "parent-process"
-                }
+                "object": "parent-process"
             },
             "pid": [
                 {
                     "key": "process.pid",
-                    "object": "process"
+                    "object": "parent-process"
                 },
                 {
-                    "key": "process.parent_ref",
-                    "object": "process",
+                    "key": "process.child_refs",
+                    "object": "parent-process",
                     "references": [
-                        "parent-process"
+                        "process"
                     ]
                 }
             ],
             "sandbox": {
                 "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
-                "object": "process"
+                "object": "parent-process"
             },
             "terminated_time": {
                 "key": "process.extensions.x-ocsf-process-ext.terminated_time",
-                "object": "process"
+                "object": "parent-process"
             },
             "tid": {
                 "key": "process.extensions.x-ocsf-process-ext.tid",
-                "object": "process"
+                "object": "parent-process"
             },
             "uid": {
                 "key": "process.x_unique_id",
-                "object": "process"
+                "object": "parent-process"
             },
             "user": {
                 "account_type": {
                     "key": "user-account.account_type",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "account_type_id": {
                     "key": "user-account.extensions.x-accessor-ext.account_type_id",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "account_uid": {
                     "key": "user-account.extensions.x-accessor-ext.account_uid",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "credential_uid": {
                     "key": "user-account.extensions.x-accessor-ext.credential_uid",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "domain": {
                     "key": "user-account.extensions.x-accessor-ext.domain",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "email_addr": {
                     "key": "email-addr.value",
-                    "object": "process-email-addr"
+                    "object": "parent-process-email-addr"
                 },
                 "groups": {
                     "desc": {
                         "key": "user-account.extensions.x-accessor-ext.group_desc",
-                        "object": "process-user-account"
+                        "object": "parent-process-user-account"
                     },
                     "name": {
                         "key": "user-account.extensions.x-accessor-ext.group_name",
-                        "object": "process-user-account"
+                        "object": "parent-process-user-account"
                     },
                     "privileges": {
                         "key": "user-account.extensions.x-accessor-ext.group_privileges",
-                        "object": "process-user-account"
+                        "object": "parent-process-user-account"
                     },
                     "type": {
                         "key": "user-account.extensions.x-accessor-ext.group_type",
-                        "object": "process-user-account"
+                        "object": "parent-process-user-account"
                     },
                     "uid": {
                         "key": "user-account.extensions.x-accessor-ext.group_uid",
-                        "object": "process-user-account"
+                        "object": "parent-process-user-account"
                     }
                 },
                 "name": {
                     "key": "user-account.display_name",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "org_uid": {
                     "key": "user-account.extensions.x-accessor-ext.org_uid",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "session_uid": {
                     "key": "user-account.extensions.x-accessor-ext.session_uid",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "session_uuid": {
                     "key": "user-account.extensions.x-accessor-ext.session_uuid",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "type": {
                     "key": "user-account.extensions.x-accessor-ext.type",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "type_id": {
                     "key": "user-account.extensions.x-accessor-ext.type_id",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 },
                 "uid": [
                     {
                         "key": "user-account.user_id",
-                        "object": "process-user-account"
+                        "object": "parent-process-user-account"
                     },
                     {
                         "key": "user-account.creator_user_ref",
-                        "object": "process",
+                        "object": "parent-process",
                         "references": "process-user-account"
                     }
                 ],
                 "uuid": {
                     "key": "user-account.extensions.x-accessor-ext.uuid",
-                    "object": "process-user-account"
+                    "object": "parent-process-user-account"
                 }
             },
             "xattributes": {
                 "key": "process.extensions.x-ocsf-process-ext.xattributes",
-                "object": "process"
+                "object": "parent-process"
             }
         },
-        "profiles": {
-            "key": "x-ocsf-cloud.profiles",
-            "object": "ocsf_cloud_api"
-        },
-        "raw_data": {
-            "key": "x-ocsf-cloud.raw_data",
-            "object": "ocsf_cloud_api"
-        },
-        "ref_event_code": {
-            "key": "x-ocsf-cloud.ref_event_code",
-            "object": "ocsf_cloud_api"
-        },
-        "ref_event_name": {
-            "key": "x-ocsf-cloud.ref_event_name",
-            "object": "ocsf_cloud_api"
-        },
-        "ref_event_uid": {
-            "key": "x-ocsf-cloud.ref_event_uid",
-            "object": "ocsf_cloud_api"
-        },
-        "ref_time": {
-            "key": "x-ocsf-cloud.ref_time",
-            "object": "ocsf_cloud_api"
+        "pid": [
+            {
+                "key": "process.pid",
+                "object": "process"
+            },
+            {
+                "key": "process.parent_ref",
+                "object": "process",
+                "references": [
+                    "parent-process"
+                ]
+            }
+        ],
+        "sandbox": {
+            "key": "process.extensions.x-ocsf-process-ext.loaded_modules",
+            "object": "process"
+        },
+        "terminated_time": {
+            "key": "process.extensions.x-ocsf-process-ext.terminated_time",
+            "object": "process"
+        },
+        "tid": {
+            "key": "process.extensions.x-ocsf-process-ext.tid",
+            "object": "process"
+        },
+        "uid": {
+            "key": "process.x_unique_id",
+            "object": "process"
         },
-        "resources": {
-            "account_uid": [
-                {
-                    "key": "x-ocsf-resources.account_uid",
-                    "object": "resources"
-                },
-                {
-                    "key": "x-ocsf-resources.cloud_api_ref",
-                    "object": "resources",
-                    "references": "ocsf_cloud_api"
-                }
-            ],
-            "cloud_partition": {
-                "key": "x-ocsf-resources.cloud_partition",
-                "object": "resources"
+        "user": {
+            "account_type": {
+                "key": "user-account.account_type",
+                "object": "process-user-account"
             },
-            "criticality": {
-                "key": "x-ocsf-resources.criticality",
-                "object": "resources"
+            "account_type_id": {
+                "key": "user-account.extensions.x-accessor-ext.account_type_id",
+                "object": "process-user-account"
             },
-            "details": {
-                "key": "x-ocsf-resources.details",
-                "object": "resources"
+            "account_uid": {
+                "key": "user-account.extensions.x-accessor-ext.account_uid",
+                "object": "process-user-account"
             },
-            "group_name": {
-                "key": "x-ocsf-resources.group_name",
-                "object": "resources"
+            "credential_uid": {
+                "key": "user-account.extensions.x-accessor-ext.credential_uid",
+                "object": "process-user-account"
+            },
+            "domain": {
+                "key": "user-account.extensions.x-accessor-ext.domain",
+                "object": "process-user-account"
+            },
+            "email_addr": {
+                "key": "email-addr.value",
+                "object": "process-email-addr"
             },
-            "labels": {
-                "key": "x-ocsf-resources.labels",
-                "object": "resources"
+            "groups": {
+                "desc": {
+                    "key": "user-account.extensions.x-accessor-ext.group_desc",
+                    "object": "process-user-account"
+                },
+                "name": {
+                    "key": "user-account.extensions.x-accessor-ext.group_name",
+                    "object": "process-user-account"
+                },
+                "privileges": {
+                    "key": "user-account.extensions.x-accessor-ext.group_privileges",
+                    "object": "process-user-account"
+                },
+                "type": {
+                    "key": "user-account.extensions.x-accessor-ext.group_type",
+                    "object": "process-user-account"
+                },
+                "uid": {
+                    "key": "user-account.extensions.x-accessor-ext.group_uid",
+                    "object": "process-user-account"
+                }
             },
             "name": {
-                "key": "x-ocsf-resources.name",
-                "object": "resources"
+                "key": "user-account.display_name",
+                "object": "process-user-account"
             },
-            "owner": {
-                "key": "x-ocsf-resources.owner",
-                "object": "resources"
+            "org_uid": {
+                "key": "user-account.extensions.x-accessor-ext.org_uid",
+                "object": "process-user-account"
             },
-            "region": {
-                "key": "x-ocsf-resources.region",
-                "object": "resources"
+            "session_uid": {
+                "key": "user-account.extensions.x-accessor-ext.session_uid",
+                "object": "process-user-account"
+            },
+            "session_uuid": {
+                "key": "user-account.extensions.x-accessor-ext.session_uuid",
+                "object": "process-user-account"
             },
             "type": {
-                "key": "x-ocsf-resources.type",
-                "object": "resources"
+                "key": "user-account.extensions.x-accessor-ext.type",
+                "object": "process-user-account"
             },
-            "uid": {
-                "key": "x-ocsf-resources.uid",
-                "object": "resources"
-            }
-        },
-        "severity": {
-            "key": "x-ocsf-cloud.severity",
-            "object": "ocsf_cloud_api"
-        },
-        "severity_id": {
-            "key": "x-ibm-finding.severity",
-            "object": "ibm_finding",
-            "transformer": "ToInteger"
-        },
-        "src_endpoint": {
-            "instance_uid": {
-                "key": "x-oca-asset.extensions.x-src-endpoint.instance_uid",
-                "object": "asset"
-            },
-            "interface_uid": {
-                "key": "x-oca-asset.extensions.x-src-endpoint.interface_uid",
-                "object": "asset"
+            "type_id": {
+                "key": "user-account.extensions.x-accessor-ext.type_id",
+                "object": "process-user-account"
             },
-            "intermediate_ips": [
-                {
-                    "key": "ipv4-addr.value",
-                    "object": "src_ipv4",
-                    "transformer": "FilterIPv4List",
-                    "unwrap": true
-                },
+            "uid": [
                 {
-                    "key": "ipv6-addr.value",
-                    "object": "src_ipv6",
-                    "transformer": "FilterIPv6List",
-                    "unwrap": true
-                },
-                {
-                    "key": "x-oca-asset.ip_refs",
-                    "object": "asset",
-                    "references": [
-                        "src_ipv4",
-                        "src_ipv6"
-                    ],
-                    "unwrap": true
-                }
-            ],
-            "ip": [
-                {
-                    "key": "ipv4-addr.value",
-                    "object": "src_ip",
-                    "transformer": "CheckIPv4"
-                },
-                {
-                    "key": "ipv6-addr.value",
-                    "object": "src_ip",
-                    "transformer": "CheckIPv6"
-                },
-                {
-                    "key": "network-traffic.src_ref",
-                    "object": "nt",
-                    "references": "src_ip"
-                },
-                {
-                    "key": "x-ibm-finding.src_ip_ref",
-                    "object": "ibm_finding",
-                    "references": "src_ip"
-                },
-                {
-                    "group": true,
-                    "key": "x-oca-asset.ip_refs",
-                    "object": "host",
-                    "references": [
-                        "src_ip"
-                    ]
+                    "key": "user-account.user_id",
+                    "object": "process-user-account"
                 },
                 {
-                    "key": "x-oca-event.network_ref",
-                    "object": "event",
-                    "references": "nt"
+                    "key": "user-account.creator_user_ref",
+                    "object": "process",
+                    "references": "process-user-account"
                 }
             ],
-            "name": {
-                "key": "x-oca-asset.name",
-                "object": "asset"
-            },
-            "port": {
-                "key": "network-traffic.src_port",
-                "object": "nt",
-                "transformer": "ToInteger"
-            },
-            "subnet_uid": {
-                "key": "x-oca-asset.extensions.x-src-endpoint.subnet_uid",
-                "object": "asset"
-            },
-            "svc_name": {
-                "key": "x-oca-asset.extensions.x-src-endpoint.svc_name",
-                "object": "asset"
-            },
-            "vpc_uid": {
-                "key": "x-oca-asset.extensions.x-src-endpoint.vpc_uid",
-                "object": "asset"
+            "uuid": {
+                "key": "user-account.extensions.x-accessor-ext.uuid",
+                "object": "process-user-account"
             }
         },
-        "start_time": {
-            "key": "first_observed",
-            "transformer": "EpochToTimestamp"
+        "xattributes": {
+            "key": "process.extensions.x-ocsf-process-ext.xattributes",
+            "object": "process"
+        }
+    },
+    "profiles": {
+        "key": "x-ocsf-cloud.profiles",
+        "object": "ocsf_cloud_api"
+    },
+    "raw_data": {
+        "key": "x-ocsf-cloud.raw_data",
+        "object": "ocsf_cloud_api"
+    },
+    "ref_event_code": {
+        "key": "x-ocsf-cloud.ref_event_code",
+        "object": "ocsf_cloud_api"
+    },
+    "ref_event_name": {
+        "key": "x-ocsf-cloud.ref_event_name",
+        "object": "ocsf_cloud_api"
+    },
+    "ref_event_uid": {
+        "key": "x-ocsf-cloud.ref_event_uid",
+        "object": "ocsf_cloud_api"
+    },
+    "ref_time": {
+        "key": "x-ocsf-cloud.ref_time",
+        "object": "ocsf_cloud_api"
+    },
+    "resources": {
+        "account_uid": [
+            {
+                "key": "x-ocsf-resources.account_uid",
+                "object": "resources"
+            },
+            {
+                "key": "x-ocsf-resources.cloud_api_ref",
+                "object": "resources",
+                "references": "ocsf_cloud_api"
+            }
+        ],
+        "cloud_partition": {
+            "key": "x-ocsf-resources.cloud_partition",
+            "object": "resources"
+        },
+        "criticality": {
+            "key": "x-ocsf-resources.criticality",
+            "object": "resources"
+        },
+        "details": {
+            "key": "x-ocsf-resources.details",
+            "object": "resources"
+        },
+        "group_name": {
+            "key": "x-ocsf-resources.group_name",
+            "object": "resources"
+        },
+        "labels": {
+            "key": "x-ocsf-resources.labels",
+            "object": "resources"
         },
-        "status": {
-            "key": "x-ocsf-cloud.status",
-            "object": "ocsf_cloud_api"
+        "name": {
+            "key": "x-ocsf-resources.name",
+            "object": "resources"
         },
-        "status_code": {
-            "key": "x-ocsf-cloud.status_code",
-            "object": "ocsf_cloud_api"
+        "owner": {
+            "key": "x-ocsf-resources.owner",
+            "object": "resources"
         },
-        "status_detail": {
-            "key": "x-ocsf-cloud.status_detail",
-            "object": "ocsf_cloud_api"
+        "region": {
+            "key": "x-ocsf-resources.region",
+            "object": "resources"
         },
-        "status_id": {
-            "key": "x-ocsf-cloud.status_id",
-            "object": "ocsf_cloud_api",
-            "transformer": "ToInteger"
+        "type": {
+            "key": "x-ocsf-resources.type",
+            "object": "resources"
         },
-        "time": {
-            "key": "x-oca-event.created",
-            "object": "x_oca_event"
-        },
-        "timezone_offset": {
-            "key": "x-oca-event.timezone",
-            "object": "x_oca_event",
-            "transformer": "ToInteger"
+        "uid": {
+            "key": "x-ocsf-resources.uid",
+            "object": "resources"
+        }
+    },
+    "severity": {
+        "key": "x-ocsf-cloud.severity",
+        "object": "ocsf_cloud_api"
+    },
+    "severity_id": {
+        "key": "x-ibm-finding.severity",
+        "object": "ibm_finding",
+        "transformer": "ToInteger"
+    },
+    "src_endpoint": {
+        "instance_uid": {
+            "key": "x-oca-asset.extensions.x-src-endpoint.instance_uid",
+            "object": "asset"
+        },
+        "interface_uid": {
+            "key": "x-oca-asset.extensions.x-src-endpoint.interface_uid",
+            "object": "asset"
         },
-        "traffic": {
-            "bytes": {
-                "key": "network-traffic.extensions.x-network-ext.bytes",
-                "object": "nt"
-            },
-            "bytes_in": {
-                "key": "network-traffic.dst_byte_count",
-                "object": "nt"
-            },
-            "bytes_out": {
-                "key": "network-traffic.src_byte_count",
-                "object": "nt"
-            },
-            "packets": {
-                "key": "network-traffic.extensions.x-network-ext.packets",
-                "object": "nt"
-            },
-            "packets_in": {
-                "key": "network-traffic.dst_packets",
-                "object": "nt"
-            },
-            "packets_out": {
-                "key": "network-traffic.src_packets",
-                "object": "nt"
+        "intermediate_ips": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "src_ipv4",
+                "transformer": "FilterIPv4List",
+                "unwrap": true
+            },
+            {
+                "key": "ipv6-addr.value",
+                "object": "src_ipv6",
+                "transformer": "FilterIPv6List",
+                "unwrap": true
+            },
+            {
+                "key": "x-oca-asset.ip_refs",
+                "object": "asset",
+                "references": [
+                    "src_ipv4",
+                    "src_ipv6"
+                ],
+                "unwrap": true
             }
+        ],
+        "ip": [
+            {
+                "key": "ipv4-addr.value",
+                "object": "src_ip",
+                "transformer": "CheckIPv4"
+            },
+            {
+                "key": "ipv6-addr.value",
+                "object": "src_ip",
+                "transformer": "CheckIPv6"
+            },
+            {
+                "key": "network-traffic.src_ref",
+                "object": "nt",
+                "references": "src_ip"
+            },
+            {
+                "key": "x-ibm-finding.src_ip_ref",
+                "object": "ibm_finding",
+                "references": "src_ip"
+            },
+            {
+                "group": true,
+                "key": "x-oca-asset.ip_refs",
+                "object": "host",
+                "references": [
+                    "src_ip"
+                ]
+            },
+            {
+                "key": "x-oca-event.network_ref",
+                "object": "event",
+                "references": "nt"
+            }
+        ],
+        "name": {
+            "key": "x-oca-asset.name",
+            "object": "asset"
         },
-        "type_name": {
-            "key": "x-ocsf-cloud.type_name",
-            "object": "ocsf_cloud_api"
-        },
-        "type_uid": {
-            "key": "x-ocsf-cloud.type_uid",
-            "object": "ocsf_cloud_api",
+        "port": {
+            "key": "network-traffic.src_port",
+            "object": "nt",
             "transformer": "ToInteger"
         },
-        "vulnerabilities": {
-            "cve": {
-                "created_time": {
-                    "key": "x-ocsf-vulnerabilities.created_time",
+        "subnet_uid": {
+            "key": "x-oca-asset.extensions.x-src-endpoint.subnet_uid",
+            "object": "asset"
+        },
+        "svc_name": {
+            "key": "x-oca-asset.extensions.x-src-endpoint.svc_name",
+            "object": "asset"
+        },
+        "vpc_uid": {
+            "key": "x-oca-asset.extensions.x-src-endpoint.vpc_uid",
+            "object": "asset"
+        }
+    },
+    "start_time": {
+        "key": "first_observed",
+        "transformer": "EpochToTimestamp"
+    },
+    "status": {
+        "key": "x-ocsf-cloud.status",
+        "object": "ocsf_cloud_api"
+    },
+    "status_code": {
+        "key": "x-ocsf-cloud.status_code",
+        "object": "ocsf_cloud_api"
+    },
+    "status_detail": {
+        "key": "x-ocsf-cloud.status_detail",
+        "object": "ocsf_cloud_api"
+    },
+    "status_id": {
+        "key": "x-ocsf-cloud.status_id",
+        "object": "ocsf_cloud_api",
+        "transformer": "ToInteger"
+    },
+    "time": {
+        "key": "x-oca-event.created",
+        "object": "x_oca_event"
+    },
+    "timezone_offset": {
+        "key": "x-oca-event.timezone",
+        "object": "x_oca_event",
+        "transformer": "ToInteger"
+    },
+    "traffic": {
+        "bytes": {
+            "key": "network-traffic.extensions.x-network-ext.bytes",
+            "object": "nt"
+        },
+        "bytes_in": {
+            "key": "network-traffic.dst_byte_count",
+            "object": "nt"
+        },
+        "bytes_out": {
+            "key": "network-traffic.src_byte_count",
+            "object": "nt"
+        },
+        "packets": {
+            "key": "network-traffic.extensions.x-network-ext.packets",
+            "object": "nt"
+        },
+        "packets_in": {
+            "key": "network-traffic.dst_packets",
+            "object": "nt"
+        },
+        "packets_out": {
+            "key": "network-traffic.src_packets",
+            "object": "nt"
+        }
+    },
+    "type_name": {
+        "key": "x-ocsf-cloud.type_name",
+        "object": "ocsf_cloud_api"
+    },
+    "type_uid": {
+        "key": "x-ocsf-cloud.type_uid",
+        "object": "ocsf_cloud_api",
+        "transformer": "ToInteger"
+    },
+    "vulnerabilities": {
+        "cve": {
+            "created_time": {
+                "key": "x-ocsf-vulnerabilities.created_time",
+                "object": "vulnerabilities"
+            },
+            "cvss": {
+                "base_score": {
+                    "key": "x-ocsf-vulnerabilities.base_score",
                     "object": "vulnerabilities"
                 },
-                "cvss": {
-                    "base_score": {
-                        "key": "x-ocsf-vulnerabilities.base_score",
-                        "object": "vulnerabilities"
-                    },
-                    "depth": {
-                        "key": "x-ocsf-vulnerabilities.depth",
-                        "object": "vulnerabilities"
-                    },
-                    "metrics": {
-                        "name": {
-                            "key": "x-ocsf-vulnerabilities.name",
-                            "object": "vulnerabilities"
-                        },
-                        "value": {
-                            "key": "x-ocsf-vulnerabilities.value",
-                            "object": "vulnerabilities"
-                        }
-                    },
-                    "overall_score": {
-                        "key": "x-ocsf-vulnerabilities.overall_score",
-                        "object": "vulnerabilities"
-                    },
-                    "severity": {
-                        "key": "x-ocsf-vulnerabilities.severity",
-                        "object": "vulnerabilities"
-                    },
-                    "vector_string": {
-                        "key": "x-ocsf-vulnerabilities.vector_string",
+                "depth": {
+                    "key": "x-ocsf-vulnerabilities.depth",
+                    "object": "vulnerabilities"
+                },
+                "metrics": {
+                    "name": {
+                        "key": "x-ocsf-vulnerabilities.name",
                         "object": "vulnerabilities"
                     },
-                    "version": {
-                        "key": "x-ocsf-vulnerabilities.version",
+                    "value": {
+                        "key": "x-ocsf-vulnerabilities.value",
                         "object": "vulnerabilities"
                     }
                 },
-                "cwe_uid": {
-                    "key": "x-ocsf-vulnerabilities.cwe_uid",
+                "overall_score": {
+                    "key": "x-ocsf-vulnerabilities.overall_score",
                     "object": "vulnerabilities"
                 },
-                "cwe_url": {
-                    "key": "x-ocsf-vulnerabilities.cwe_url",
+                "severity": {
+                    "key": "x-ocsf-vulnerabilities.severity",
                     "object": "vulnerabilities"
                 },
-                "modified_time": {
-                    "key": "x-ocsf-vulnerabilities.modified_time",
+                "vector_string": {
+                    "key": "x-ocsf-vulnerabilities.vector_string",
                     "object": "vulnerabilities"
                 },
-                "product": {
-                    "feature": {
-                        "name": {
-                            "key": "software.extensions.x-ocsf-product-ext.feature_name",
-                            "object": "vulnerabilities-software"
-                        },
-                        "uid": {
-                            "key": "software.extensions.x-ocsf-product-ext.feature_uid",
-                            "object": "vulnerabilities-software"
-                        },
-                        "version": {
-                            "key": "software.extensions.x-ocsf-product-ext.feature_version",
-                            "object": "vulnerabilities-software"
-                        }
-                    },
-                    "lang": {
-                        "key": "software.languages",
-                        "object": "vulnerabilities-software"
-                    },
+                "version": {
+                    "key": "x-ocsf-vulnerabilities.version",
+                    "object": "vulnerabilities"
+                }
+            },
+            "cwe_uid": {
+                "key": "x-ocsf-vulnerabilities.cwe_uid",
+                "object": "vulnerabilities"
+            },
+            "cwe_url": {
+                "key": "x-ocsf-vulnerabilities.cwe_url",
+                "object": "vulnerabilities"
+            },
+            "modified_time": {
+                "key": "x-ocsf-vulnerabilities.modified_time",
+                "object": "vulnerabilities"
+            },
+            "product": {
+                "feature": {
                     "name": {
-                        "key": "software.name",
-                        "object": "vulnerabilities-software"
-                    },
-                    "path": {
-                        "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                        "key": "software.extensions.x-ocsf-product-ext.feature_name",
                         "object": "vulnerabilities-software"
                     },
                     "uid": {
-                        "key": "software.extensions.x-ocsf-product-ext.product_uid",
-                        "object": "vulnerabilities-software"
-                    },
-                    "vendor_name": {
-                        "key": "software.vendor",
+                        "key": "software.extensions.x-ocsf-product-ext.feature_uid",
                         "object": "vulnerabilities-software"
                     },
                     "version": {
-                        "key": "software.version",
+                        "key": "software.extensions.x-ocsf-product-ext.feature_version",
                         "object": "vulnerabilities-software"
                     }
                 },
-                "type": {
-                    "key": "x-ocsf-vulnerabilities.type",
-                    "object": "vulnerabilities"
-                },
-                "uid": {
-                    "key": "x-ocsf-vulnerabilities.uid",
-                    "object": "vulnerabilities"
-                }
-            },
-            "desc": {
-                "key": "x-ocsf-vulnerabilities.desc",
-                "object": "vulnerabilities"
-            },
-            "kb_articles": {
-                "key": "x-ocsf-vulnerabilities.kb_articles",
-                "object": "vulnerabilities"
-            },
-            "packages": {
-                "architecture": {
-                    "key": "x-ocsf-vulnerabilities.packages_architecture",
-                    "object": "vulnerabilities"
+                "lang": {
+                    "key": "software.languages",
+                    "object": "vulnerabilities-software"
                 },
-                "epoch": {
-                    "key": "x-ocsf-vulnerabilities.packages_epoch",
-                    "object": "vulnerabilities"
+                "name": {
+                    "key": "software.name",
+                    "object": "vulnerabilities-software"
                 },
-                "license": {
-                    "key": "x-ocsf-vulnerabilities.packages_license",
-                    "object": "vulnerabilities"
+                "path": {
+                    "key": "software.extensions.x-ocsf-product-ext.installed_path",
+                    "object": "vulnerabilities-software"
                 },
-                "name": {
-                    "key": "x-ocsf-vulnerabilities.packages_name",
-                    "object": "vulnerabilities"
+                "uid": {
+                    "key": "software.extensions.x-ocsf-product-ext.product_uid",
+                    "object": "vulnerabilities-software"
                 },
-                "release": {
-                    "key": "x-ocsf-vulnerabilities.packages_release",
-                    "object": "vulnerabilities"
+                "vendor_name": {
+                    "key": "software.vendor",
+                    "object": "vulnerabilities-software"
                 },
                 "version": {
-                    "key": "x-ocsf-vulnerabilities.packages_version",
-                    "object": "vulnerabilities"
+                    "key": "software.version",
+                    "object": "vulnerabilities-software"
                 }
             },
-            "references": {
-                "key": "x-ocsf-vulnerabilities.references",
+            "type": {
+                "key": "x-ocsf-vulnerabilities.type",
                 "object": "vulnerabilities"
             },
-            "related_vulnerabilities": {
-                "key": "x-ocsf-vulnerabilities.related_vulnerabilities",
+            "uid": {
+                "key": "x-ocsf-vulnerabilities.uid",
                 "object": "vulnerabilities"
-            },
-            "severity": {
-                "key": "x-ocsf-vulnerabilities.severity",
+            }
+        },
+        "desc": {
+            "key": "x-ocsf-vulnerabilities.desc",
+            "object": "vulnerabilities"
+        },
+        "kb_articles": {
+            "key": "x-ocsf-vulnerabilities.kb_articles",
+            "object": "vulnerabilities"
+        },
+        "packages": {
+            "architecture": {
+                "key": "x-ocsf-vulnerabilities.packages_architecture",
                 "object": "vulnerabilities"
             },
-            "title": {
-                "key": "x-ocsf-vulnerabilities.title",
+            "epoch": {
+                "key": "x-ocsf-vulnerabilities.packages_epoch",
                 "object": "vulnerabilities"
             },
-            "vendor_name": {
-                "key": "x-ocsf-vulnerabilities.vendor_name",
+            "license": {
+                "key": "x-ocsf-vulnerabilities.packages_license",
                 "object": "vulnerabilities"
-            }
-        }
-    },
-    "vpcflow": {
-        "account": [
-            {
-                "key": "x-aws-details.account_id",
-                "object": "accountid"
-            }
-        ],
-        "action": {
-            "key": "x-ibm-finding.finding_type",
-            "object": "ibm_finding"
-        },
-        "destinationaddress": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "dst_ip"
-            },
-            {
-                "key": "ipv6-addr.value",
-                "object": "dst_ip"
             },
-            {
-                "key": "x-ibm-finding.dst_ip_ref",
-                "object": "ibm_finding",
-                "references": "dst_ip"
-            },
-            {
-                "key": "network-traffic.dst_ref",
-                "object": "nt",
-                "references": "dst_ip"
-            }
-        ],
-        "destinationport": [
-            {
-                "key": "network-traffic.dst_port",
-                "object": "nt",
-                "transformer": "ToInteger"
-            }
-        ],
-        "endtime": [
-            {
-                "key": "network-traffic.end",
-                "object": "nt",
-                "transformer": "EpochSecondsToTimestamp"
+            "name": {
+                "key": "x-ocsf-vulnerabilities.packages_name",
+                "object": "vulnerabilities"
             },
-            {
-                "key": "x-ibm-finding.end",
-                "object": "ibm_finding",
-                "transformer": "EpochSecondsToTimestamp"
+            "release": {
+                "key": "x-ocsf-vulnerabilities.packages_release",
+                "object": "vulnerabilities"
             },
-            {
-                "key": "last_observed",
-                "transformer": "EpochToTimestamp"
+            "version": {
+                "key": "x-ocsf-vulnerabilities.packages_version",
+                "object": "vulnerabilities"
             }
-        ],
-        "name": {
-            "key": "x-ibm-finding.name",
-            "object": "ibm_finding"
         },
-        "protocol": [
-            {
-                "key": "network-traffic.protocols",
-                "object": "nt",
-                "transformer": "ToLowercaseArray"
-            }
-        ],
-        "sourceaddress": [
-            {
-                "key": "ipv4-addr.value",
-                "object": "src_ip"
-            },
-            {
-                "key": "ipv6-addr.value",
-                "object": "src_ip"
-            },
-            {
-                "key": "network-traffic.src_ref",
-                "object": "nt",
-                "references": "src_ip"
-            },
-            {
-                "key": "x-ibm-finding.src_ip_ref",
-                "object": "ibm_finding",
-                "references": "src_ip"
-            },
-            {
-                "ds_key": "interfaceid",
-                "key": "ipv4-addr.x_aws_interface_id",
-                "object": "src_ip"
-            },
-            {
-                "ds_key": "interfaceid",
-                "key": "ipv6-addr.x_aws_interface_id",
-                "object": "src_ip"
-            }
-        ],
-        "sourceport": [
-            {
-                "key": "network-traffic.src_port",
-                "object": "nt",
-                "transformer": "ToInteger"
-            }
-        ],
-        "starttime": [
-            {
-                "key": "network-traffic.start",
-                "object": "nt",
-                "transformer": "EpochSecondsToTimestamp"
-            },
-            {
-                "key": "x-ibm-finding.start",
-                "object": "ibm_finding",
-                "transformer": "EpochSecondsToTimestamp"
-            },
-            {
-                "key": "first_observed",
-                "transformer": "EpochSecondsToTimestamp"
-            }
-        ]
+        "references": {
+            "key": "x-ocsf-vulnerabilities.references",
+            "object": "vulnerabilities"
+        },
+        "related_vulnerabilities": {
+            "key": "x-ocsf-vulnerabilities.related_vulnerabilities",
+            "object": "vulnerabilities"
+        },
+        "severity": {
+            "key": "x-ocsf-vulnerabilities.severity",
+            "object": "vulnerabilities"
+        },
+        "title": {
+            "key": "x-ocsf-vulnerabilities.title",
+            "object": "vulnerabilities"
+        },
+        "vendor_name": {
+            "key": "x-ocsf-vulnerabilities.vendor_name",
+            "object": "vulnerabilities"
+        }
     }
 }
```

## Comparing `stix_shifter_modules_aws_athena-5.3.1.dist-info/LICENSE.md` & `stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-5.3.1.dist-info/METADATA` & `stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stix-shifter-modules-aws-athena
-Version: 5.3.1
+Version: 6.0.0.dev74
 Summary: Tools and interface to translate STIX formatted results and queries to different data source formats and to set up appropriate connection strings for invoking and triggering actions in openwhisk
 Home-page: https://github.com/opencybersecurityalliance/stix-shifter
 Author: ibm
 Author-email: 
 Project-URL: Source, https://github.com/opencybersecurityalliance/stix-shifter
 Keywords: datasource stix translate transform transmit
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `stix_shifter_modules_aws_athena-5.3.1.dist-info/NOTICE` & `stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-5.3.1.dist-info/RECORD` & `stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 stix_shifter_modules/aws_athena/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stix_shifter_modules/aws_athena/entry_point.py,sha256=FHXjqiWmrOdq31iDqyFzooZyxBGxqUIp3RqWcxcfiOY,1374
-stix_shifter_modules/aws_athena/configuration/config.json,sha256=CB4hBMR-yhGfE1ZPXQxOmDXDyR7sMY82pXFIX9BBtJA,252493
+stix_shifter_modules/aws_athena/configuration/config.json,sha256=n2kQH9RXi6jhNTXV60V7mZb8O63N97Xgzl9RVHcbWGQ,239955
 stix_shifter_modules/aws_athena/configuration/dialects.json,sha256=2nYaixArRUIgorTTWC7QzuuNiHti6tF3gb6y0y91x7Q,229
 stix_shifter_modules/aws_athena/configuration/lang_en.json,sha256=J4SXpSel1epi9EKGVppvLYfXPkbIxfxwJcJ-xwyc2ww,4766
 stix_shifter_modules/aws_athena/stix_translation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py,sha256=vffR1MRpwX6NMwXy0MldaTecIIzvVSZIlcqXOM8Nx7I,22646
+stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py,sha256=mlzibasm2UfSGhYqHoH2hMFHlx7XCy35VSlzzFTWpjc,27024
 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py,sha256=IsWNLisRsvduCgv1OrQ05x6llobayfUapumqGLOrZRo,24044
 stix_shifter_modules/aws_athena/stix_translation/query_translator.py,sha256=QyXnF8HPZWYYmNM1WrFqoH3ZaW8S4fOh0oxZFSgmYaE,1024
-stix_shifter_modules/aws_athena/stix_translation/results_translator.py,sha256=SkMabFdZ2PxhXy6OZKjf45XRttP-LveVPhzi9ZyAD3s,1522
 stix_shifter_modules/aws_athena/stix_translation/transformers.py,sha256=RmmyKJwXx3XMgvCLKAex2ZgTwmg14REONa-Ai_D2AqE,1075
 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json,sha256=leAlSRCH2F-6GtOewVbFfkaXV_fUY_B3qA-QcQyoOQM,4765
 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json,sha256=qdbHf8p71aOUgH29SiCgbW-bm7tyz6TkMVKVJ1XfljY,1894
+stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json,sha256=PKWe5DnziFhFqZzQCyMqLLJXWUvMvRj6fs0SBz43PTY,10146
 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json,sha256=Mjh6Jl4D14CKVwuQh2ksTIh69hYg-ygZrUBuOigG8pQ,139
 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json,sha256=Kv22JuyDwUdrLxnhj_789NmXsE9aTRvNKlPM95_Hb5s,2439
 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json,sha256=aCIzFD7g24EseM4-VviVumdn6oWvQSjYv4-2ZdefiVQ,18300
+stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json,sha256=Pfn8IsRiGR_oP_nvbzbsS03PPmdF5CFqrG_vQL415II,75601
 stix_shifter_modules/aws_athena/stix_translation/json/operators.json,sha256=jLCjazSAKvuvKzZhibBK3_PccQGu0TGF5inbzzzkoR0,591
-stix_shifter_modules/aws_athena/stix_translation/json/to_stix_map.json,sha256=pCgXzJQa5luba0_sJZhl3ovdvfy-2j0WT5_dQOLUEV8,94369
-stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json,sha256=TDiBsk4GtUH98mK6_KBKfFcDoOo1UzF08lyFpHF9XqM,891
+stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json,sha256=qmXsj5YwOGFlh1y7dyjk1rEsFpvT9k2VzPie95CLIus,814
+stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json,sha256=j9I7Yh01JvT0ODg04rNU1dcqb3YHTFWsLpwTYSCDQ5I,2350
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json,sha256=qdbHf8p71aOUgH29SiCgbW-bm7tyz6TkMVKVJ1XfljY,1894
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json,sha256=_lKZSQdQjm7yJZ5ZDCww8rC4QVFtS75cqdUmnQrpBKw,18297
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json,sha256=Q3hVrbhWXE9i0jn9iaaswGXhRsR7B5QGSPSv-Vw3rxM,93792
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json,sha256=TDiBsk4GtUH98mK6_KBKfFcDoOo1UzF08lyFpHF9XqM,891
 stix_shifter_modules/aws_athena/stix_transmission/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py,sha256=4hVUN_O77rghatKexuLOPsTGvzi2fHInpFfgYBuTPkM,4173
 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py,sha256=D2A5li6TWgZvqpnDGLXVveLqYHlWI1evVWKYKeXT60M,1207
 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py,sha256=u2IkHTEccByBayyajth6iudtzWy3tIxRDnbpPIX_610,1959
 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py,sha256=HkcSFvDlW71v6tBtMTcvAd_jQqit6Uh3YknjBu7YKmw,1370
 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py,sha256=eOK6mHRwtASq4gZxOyqmSUvDDThxkDhhbdYQ8jOTweY,7443
-stix_shifter_modules/aws_athena/stix_transmission/results_connector.py,sha256=RJw9nNCr7FCIqqRJOSUG55k8a9uo0wdk7tYc27NHg7c,14478
+stix_shifter_modules/aws_athena/stix_transmission/results_connector.py,sha256=3J_nfleKOrrSbOGyxDYVxs4qWG1dFWY-qnJBR8jwhZY,15539
 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py,sha256=G-JPjia6t91hGEtvAgImHpoGdO2DNI9ERZB4AAzqf7s,3175
-stix_shifter_modules_aws_athena-5.3.1.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
-stix_shifter_modules_aws_athena-5.3.1.dist-info/METADATA,sha256=z0WuGk4nUZggs85XWEdagoyNnRJlXhodTBuheTj8Fdc,8040
-stix_shifter_modules_aws_athena-5.3.1.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
-stix_shifter_modules_aws_athena-5.3.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-stix_shifter_modules_aws_athena-5.3.1.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
-stix_shifter_modules_aws_athena-5.3.1.dist-info/RECORD,,
+stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
+stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/METADATA,sha256=hgWUwd9QBMC1la_U7d5vyZ9f133f-DFxx-AdnM1rRdc,8046
+stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
+stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
+stix_shifter_modules_aws_athena-6.0.0.dev74.dist-info/RECORD,,
```

