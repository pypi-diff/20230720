# Comparing `tmp/network-config-analyzer-1.9.3.tar.gz` & `tmp/network-config-analyzer-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-config-analyzer-1.9.3.tar", last modified: Mon Jul 10 14:10:26 2023, max compression
+gzip compressed data, was "network-config-analyzer-1.9.4.tar", last modified: Thu Jul 20 11:11:19 2023, max compression
```

## Comparing `network-config-analyzer-1.9.3.tar` & `network-config-analyzer-1.9.4.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.936906 network-config-analyzer-1.9.3/nca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.944906 network-config-analyzer-1.9.3/nca/CoreDS/
--rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/CanonicalHyperCubeSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/CanonicalIntervalSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ConnectionSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ConnectivityCube.py
--rw-r--r--   0 runner    (1001) docker     (123)    23486 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ConnectivityProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/DimensionsManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/MethodSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/MinDFA.py
--rw-r--r--   0 runner    (1001) docker     (123)    30879 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/Peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/PortSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ProtocolNameResolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ProtocolSet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.944906 network-config-analyzer-1.9.3/nca/FWRules/
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/ClusterInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    28220 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/ConnectivityGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/DotGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    28290 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/FWRule.py
--rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/InteractiveConnectivityGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/MinimizeFWRules.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.948907 network-config-analyzer-1.9.3/nca/FileScanners/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/DirScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/GenericTreeScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/GitScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/HelmScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.952906 network-config-analyzer-1.9.3/nca/NetworkConfig/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.932906 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.952906 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/dns/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/dns/dns_pods.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.952906 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/ingress_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/ingress_controller/ingress_controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.952906 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/istio_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/istio_gateway/istio_custom_gateway.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/istio_gateway/istio_gateway.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)   113771 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfigQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfigQueryRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24609 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/PeerContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/PoliciesFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/QueryOutputHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/ResourcesHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/TopologyObjectsFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.956906 network-config-analyzer-1.9.3/nca/Parsers/
--rw-r--r--   0 runner    (1001) docker     (123)    37209 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/CalicoPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/GenericIngressLikeYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/GenericYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IngressPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioGenericYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    29222 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioServiceEntryYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioSidecarYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioTrafficResourcesYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24720 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/K8sPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/K8sServiceYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.960907 network-config-analyzer-1.9.3/nca/Resources/
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/CalicoNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/IngressPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/IstioNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/IstioSidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/IstioTrafficResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/K8sNamespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/K8sNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/K8sService.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/NetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/SchemeRunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/nca/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/CmdlineRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    23062 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/ExplTracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/NcaLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/OutputConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/OutputFilesFlags.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/nca_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.738948 network-config-analyzer-1.9.4/nca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.738948 network-config-analyzer-1.9.4/nca/CoreDS/
+-rw-r--r--   0 runner    (1001) docker     (123)    41884 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/CanonicalHyperCubeSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/CanonicalIntervalSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ConnectionSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ConnectivityCube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23486 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ConnectivityProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/DimensionsManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/MethodSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/MinDFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30879 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/Peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/PortSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ProtocolNameResolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/ProtocolSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/CoreDS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.738948 network-config-analyzer-1.9.4/nca/FWRules/
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/ClusterInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28220 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/ConnectivityGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/DotGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28290 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/FWRule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/InteractiveConnectivityGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/MinimizeFWRules.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FWRules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/FileScanners/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/DirScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/GenericTreeScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/GitScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/HelmScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/FileScanners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/NetworkConfig/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.734948 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/dns/dns_pods.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/ingress_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/ingress_controller/ingress_controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.742948 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/istio_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/istio_gateway/istio_custom_gateway.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/LiveSim/istio_gateway/istio_gateway.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115210 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfigQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfigQueryRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24609 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/PeerContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/PoliciesFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/QueryOutputHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/ResourcesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/TopologyObjectsFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/NetworkConfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/nca/Parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)    37209 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/CalicoPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/GenericIngressLikeYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/GenericYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IngressPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioGenericYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29222 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioServiceEntryYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioSidecarYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20741 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/IstioTrafficResourcesYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24720 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/K8sPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/K8sServiceYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/nca/Resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/CalicoNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/IngressPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/IstioNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/IstioSidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/IstioTrafficResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/K8sNamespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/K8sNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/K8sService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/NetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/SchemeRunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/nca/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/CmdlineRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/ExplTracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/NcaLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/OutputConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/OutputFilesFlags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/nca/nca_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 11:11:19.000000 network-config-analyzer-1.9.4/network_config_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 11:09:39.000000 network-config-analyzer-1.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 11:11:19.746948 network-config-analyzer-1.9.4/setup.cfg
```

### Comparing `network-config-analyzer-1.9.3/LICENSE` & `network-config-analyzer-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/PKG-INFO` & `network-config-analyzer-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-config-analyzer
-Version: 1.9.3
+Version: 1.9.4
 Summary: An analyzer for Network Policies and other connectivity-configuration resources
 Home-page: https://github.com/IBM/network-config-analyzer
 Author: Ziv Nevo
 Author-email: nevo@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/network-config-analyzer/issues
 Project-URL: NP-Guard Home, https://np-guard.github.io
 Classifier: Programming Language :: Python :: 3
```

### Comparing `network-config-analyzer-1.9.3/README.md` & `network-config-analyzer-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/CanonicalHyperCubeSet.py` & `network-config-analyzer-1.9.4/nca/CoreDS/CanonicalHyperCubeSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -537,28 +537,31 @@
         for layer in self.layers:
             current_layer_0 = self._copy_layer_elem(layer)
             for other_layer in other.layers:
                 other_sub_elem = other.layers[other_layer]
                 common_part = current_layer_0 & other_layer
                 has_common_part = bool(common_part)
                 if has_common_part:
+                    # if it's not last dim for both self and other, determine containment recursively
                     if not self._is_last_dimension() and not other._is_last_dimension() and \
                             not (self.layers[layer])._contained_in_aux(other_sub_elem, all_active_dims[1:]):
                         return False
+                    # if it's last dim for self but not for other: the remaining of other should be entire cube
+                    if self._is_last_dimension() and not other._is_last_dimension() and \
+                            not other_sub_elem._is_sub_elem_entire_sub_space():
+                        return False
+                    # if it's the last dim for other but not for self -> containment is satisfied on this part
+                    # at this point, sub-object from common_part is contained
                     remaining = current_layer_0 - common_part
                     if remaining:
                         # continue exploring other's cubes for containment of the remaining part from self
                         current_layer_0 = remaining
                     else:
-                        if self._is_last_dimension() and not other._is_last_dimension():
-                            # if it's last dim for self but not for other: the remaining of other should be entire cube
-                            if other_sub_elem._is_sub_elem_entire_sub_space():
-                                is_subset_count += 1
-                        else:
-                            is_subset_count += 1
+                        # count current cube (from current_layer_0) as contained in other
+                        is_subset_count += 1
                         break
         return is_subset_count == len(self.layers)
 
     def get_first_item(self, relevant_dimensions=None):
         """
         :param list relevant_dimensions: list of dimensions to include in the result item
         get an item of values within one of self's cubes.
```

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/CanonicalIntervalSet.py` & `network-config-analyzer-1.9.4/nca/CoreDS/CanonicalIntervalSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/ConnectionSet.py` & `network-config-analyzer-1.9.4/nca/CoreDS/ConnectionSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/ConnectivityCube.py` & `network-config-analyzer-1.9.4/nca/CoreDS/ConnectivityCube.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/ConnectivityProperties.py` & `network-config-analyzer-1.9.4/nca/CoreDS/ConnectivityProperties.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/DimensionsManager.py` & `network-config-analyzer-1.9.4/nca/CoreDS/DimensionsManager.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/MethodSet.py` & `network-config-analyzer-1.9.4/nca/CoreDS/MethodSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/MinDFA.py` & `network-config-analyzer-1.9.4/nca/CoreDS/MinDFA.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/Peer.py` & `network-config-analyzer-1.9.4/nca/CoreDS/Peer.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/PortSet.py` & `network-config-analyzer-1.9.4/nca/CoreDS/PortSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/ProtocolNameResolver.py` & `network-config-analyzer-1.9.4/nca/CoreDS/ProtocolNameResolver.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/CoreDS/ProtocolSet.py` & `network-config-analyzer-1.9.4/nca/CoreDS/ProtocolSet.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FWRules/ClusterInfo.py` & `network-config-analyzer-1.9.4/nca/FWRules/ClusterInfo.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FWRules/ConnectivityGraph.py` & `network-config-analyzer-1.9.4/nca/FWRules/ConnectivityGraph.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FWRules/DotGraph.py` & `network-config-analyzer-1.9.4/nca/FWRules/DotGraph.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FWRules/FWRule.py` & `network-config-analyzer-1.9.4/nca/FWRules/FWRule.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FWRules/InteractiveConnectivityGraph.py` & `network-config-analyzer-1.9.4/nca/FWRules/InteractiveConnectivityGraph.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FWRules/MinimizeFWRules.py` & `network-config-analyzer-1.9.4/nca/FWRules/MinimizeFWRules.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FileScanners/DirScanner.py` & `network-config-analyzer-1.9.4/nca/FileScanners/DirScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FileScanners/GenericTreeScanner.py` & `network-config-analyzer-1.9.4/nca/FileScanners/GenericTreeScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FileScanners/GitScanner.py` & `network-config-analyzer-1.9.4/nca/FileScanners/GitScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/FileScanners/HelmScanner.py` & `network-config-analyzer-1.9.4/nca/FileScanners/HelmScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfig.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfig.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfigQuery.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfigQuery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1011,16 +1011,16 @@
 
     def _txt_no_fw_rules_format_from_connections_dict(self, connections, peers, connectivity_restriction=None):
         """
         :param dict connections: the connections' dict (map from connection-set to peer pairs)
         :param PeerSet peers: the peers to consider for dot output
         :param Union[str,None] connectivity_restriction: specify if connectivity is restricted to TCP / non-TCP , or not
         :rtype:  str
-        :return the connectivity map in txt_no_fw_rules format: the connections between peers excluding connections between
-        workload to itself (without grouping as fw-rules).
+        :return the connectivity map in txt_no_fw_rules format: the connections between peers excluding connections
+        between workload to itself (without grouping as fw-rules).
         """
         conn_graph = self._get_conn_graph(connections, peers)
         return conn_graph.get_connections_without_fw_rules_txt_format(connectivity_restriction)
 
     def dot_format_from_connections_dict(self, connections, peers, connectivity_restriction=None):
         """
         :param dict connections: the connections' dict (map from connection-set to peer pairs)
@@ -1126,16 +1126,16 @@
             tcp_conns = ConnectionSet(True)  # all connections in terms of TCP
 
         return tcp_conns, non_tcp_conns
 
     @staticmethod
     def convert_props_to_split_by_tcp(props):
         """
-        given the ConnectivityProperties properties set, convert it to two properties sets, one for TCP only, and the other
-        for non-TCP only.
+        given the ConnectivityProperties properties set, convert it to two properties sets, one for TCP only,
+        and the other for non-TCP only.
         :param ConnectivityProperties props: properties describing allowed connections
         :return: a tuple of the two properties sets: first for TCP, second for non-TCP
         :rtype: tuple(ConnectivityProperties, ConnectivityProperties)
         """
         tcp_protocol = ProtocolSet.get_protocol_set_with_single_protocol('TCP')
         tcp_props = props & ConnectivityProperties.make_conn_props_from_dict({"protocols": tcp_protocol})
         non_tcp_props = props - tcp_props
@@ -1218,14 +1218,43 @@
         peers_to_compare.filter_ipv6_blocks(ip_blocks_mask)
         conns_filter = ConnectivityProperties.make_conn_props_from_dict({"src_peers": peers_to_compare,
                                                                          "dst_peers": peers_to_compare})
         res_conns1 = self.config1.filter_conns_by_peer_types(conns1, peers_to_compare) & conns_filter
         res_conns2 = self.config2.filter_conns_by_peer_types(conns2, peers_to_compare) & conns_filter
         return res_conns1, res_conns2
 
+    def _append_different_conns_to_list(self, conn_diff_props, different_conns_list, props_based_on_config1=True):
+        """
+        Adds difference between config1 and config2 connectivities into the list of differences
+        :param ConnectivityProperties conn_diff_props: connectivity properties representing a difference
+         between config1 and config2 connections (or between config2 and config1 connections)
+        :param list different_conns_list: the list to add differences to
+        :param bool props_based_on_config1: whether conn_diff_props represent connections present in config1 but not in config2
+        (the value True) or connections present in config2 but not in config1 (the value False)
+        """
+        no_conns = ConnectionSet()
+        for cube in conn_diff_props:
+            conn_cube = conn_diff_props.get_connectivity_cube(cube)
+            conns, src_peers, dst_peers = \
+                ConnectionSet.get_connection_set_and_peers_from_cube(conn_cube, self.config1.peer_container)
+            conns1 = conns if props_based_on_config1 else no_conns
+            conns2 = no_conns if props_based_on_config1 else conns
+            if self.output_config.fullExplanation:
+                if self.config1.optimized_run == 'true':
+                    different_conns_list.append(PeersAndConnections(str(src_peers), str(dst_peers), conns1, conns2))
+                else:  # 'debug': produce the same output format as in the original implementation (per peer pairs)
+                    for src_peer in src_peers:
+                        for dst_peer in dst_peers:
+                            if src_peer != dst_peer:
+                                different_conns_list.append(PeersAndConnections(str(src_peer), str(dst_peer),
+                                                                                conns1, conns2))
+            else:
+                different_conns_list.append(PeersAndConnections(src_peers.rep(), dst_peers.rep(), conns1, conns2))
+                return
+
     @staticmethod
     def clone_without_ingress(config):
         """
         Clone config without ingress policies
         :param NetworkConfig config: the config to clone
         :return: resulting config without ingress policies
         :rtype: NetworkConfig
@@ -1287,41 +1316,14 @@
 
         if different_conns_list:
             return self._query_answer_with_relevant_explanation(sorted(different_conns_list))
 
         return QueryAnswer(True, self.name1 + ' and ' + self.name2 + ' are semantically equivalent.',
                            numerical_result=0)
 
-    def _append_different_conns_to_list(self, conn_props, different_conns_list, props_based_on_config1):
-        """
-        Adds difference between config1 and config2 connectivities into the list of differences
-        :param ConnectivityProperties conn_props: connectivity properties representing a difference between config1 and config2
-        :param list different_conns_list: the list to add differences to
-        :param bool props_based_on_config1: whether conn_props represent connections present in config1 but not in config2
-        (the value True) or connections present in config2 but not in config1 (the value False)
-        """
-        no_conns = ConnectionSet()
-        for cube in conn_props:
-            conn_cube = conn_props.get_connectivity_cube(cube)
-            conns, src_peers, dst_peers = \
-                ConnectionSet.get_connection_set_and_peers_from_cube(conn_cube, self.config1.peer_container)
-            conns1 = conns if props_based_on_config1 else no_conns
-            conns2 = no_conns if props_based_on_config1 else conns
-            if self.output_config.fullExplanation:
-                if self.config1.optimized_run == 'true':
-                    different_conns_list.append(PeersAndConnections(str(src_peers), str(dst_peers), conns1, conns2))
-                else:  # 'debug': produce the same output format as in the original implementation (per peer pairs)
-                    for src_peer in src_peers:
-                        for dst_peer in dst_peers:
-                            if src_peer != dst_peer:
-                                different_conns_list.append(PeersAndConnections(str(src_peer), str(dst_peer),
-                                                                                conns1, conns2))
-            else:
-                different_conns_list.append(PeersAndConnections(src_peers.rep(), dst_peers.rep(), conns1, conns2))
-
     def check_equivalence_optimized(self, layer_name=None):
         conn_props1 = self.config1.allowed_connections_optimized(layer_name)
         conn_props2 = self.config2.allowed_connections_optimized(layer_name)
         all_conns1, all_conns2 = self.filter_conns_by_input_or_internal_constraints(conn_props1.all_allowed_conns,
                                                                                     conn_props2.all_allowed_conns)
         if all_conns1 == all_conns2:
             return QueryAnswer(True, self.name1 + ' and ' + self.name2 + ' are semantically equivalent.',
@@ -1718,14 +1720,21 @@
             peers_list = [str(e) for e in peers_in_config1_not_in_config2]
             final_explanation = \
                 PodsListsExplanations(explanation_description=f'Peers in {self.name1} which are not in {self.name2}',
                                       pods_list=sorted(peers_list))
             return QueryAnswer(False, f'{self.name1} is not contained in {self.name2} ',
                                output_explanation=[final_explanation], numerical_result=0 if not cmd_line_flag else 1)
 
+        if self.config1.optimized_run == 'false':
+            return self.check_containment_original(cmd_line_flag, only_captured)
+        else:
+            return self.check_containment_optimized(cmd_line_flag, only_captured)
+
+    def check_containment_original(self, cmd_line_flag=False, only_captured=False):
+        config1_peers = self.config1.peer_container.get_all_peers_group(include_dns_entries=True)
         peers_to_compare = config1_peers | self.disjoint_referenced_ip_blocks()
         captured_pods = self.config1.get_captured_pods() | self.config2.get_captured_pods()
         not_contained_list = []
         for peer1 in peers_to_compare:
             for peer2 in peers_to_compare if peer1 in captured_pods else captured_pods:
                 if peer1 == peer2:
                     continue
@@ -1741,14 +1750,29 @@
                     if not self.output_config.fullExplanation:
                         return self._query_answer_with_relevant_explanation(not_contained_list, cmd_line_flag)
         if not_contained_list:
             return self._query_answer_with_relevant_explanation(sorted(not_contained_list), cmd_line_flag)
         return QueryAnswer(True, self.name1 + ' is contained in ' + self.name2,
                            numerical_result=1 if not cmd_line_flag else 0)
 
+    def check_containment_optimized(self, cmd_line_flag=False, only_captured=False):
+        conn_props1 = self.config1.allowed_connections_optimized()
+        conn_props2 = self.config2.allowed_connections_optimized()
+        conns1, conns2 = self.filter_conns_by_input_or_internal_constraints(
+            conn_props1.allowed_conns if only_captured else conn_props1.all_allowed_conns,
+            conn_props2.all_allowed_conns)
+        if conns1.contained_in(conns2):
+            return QueryAnswer(True, self.name1 + ' is contained in ' + self.name2,
+                               numerical_result=1 if not cmd_line_flag else 0)
+
+        conns1_not_in_conns2 = conns1 - conns2
+        different_conns_list = []
+        self._append_different_conns_to_list(conns1_not_in_conns2, different_conns_list)
+        return self._query_answer_with_relevant_explanation(sorted(different_conns_list), cmd_line_flag)
+
     def _query_answer_with_relevant_explanation(self, explanation_list, cmd_line_flag):
         output_result = f'{self.name1} is not contained in {self.name2}'
         explanation_description = f'Connections allowed in {self.name1} which are not a subset of those in {self.name2}'
         final_explanation = ConnectionsDiffExplanation(explanation_description=explanation_description,
                                                        peers_diff_connections_list=explanation_list)
         return QueryAnswer(False, output_result, output_explanation=[final_explanation],
                            numerical_result=0 if not cmd_line_flag else 1)
```

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfigQueryRunner.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkConfigQueryRunner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkLayer.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/NetworkLayer.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/PeerContainer.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/PeerContainer.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/PoliciesFinder.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/PoliciesFinder.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/QueryOutputHandler.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/QueryOutputHandler.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/ResourcesHandler.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/ResourcesHandler.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/NetworkConfig/TopologyObjectsFinder.py` & `network-config-analyzer-1.9.4/nca/NetworkConfig/TopologyObjectsFinder.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/CalicoPolicyYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/CalicoPolicyYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/GenericIngressLikeYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/GenericIngressLikeYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/GenericYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/GenericYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/IngressPolicyYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/IngressPolicyYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/IstioGenericYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/IstioGenericYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/IstioPolicyYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/IstioPolicyYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/IstioServiceEntryYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/IstioServiceEntryYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/IstioSidecarYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/IstioSidecarYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/IstioTrafficResourcesYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/IstioTrafficResourcesYamlParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             return None  # Not an Istio VirtualService object
         vs_namespace = self.peer_container.get_namespace(vs_ns)
         vs = VirtualService(vs_name, vs_namespace)
 
         vs_spec = vs_resource['spec']
         self.check_fields_validity(vs_spec, f'VirtualService {vs.full_name()}',
                                    {'hosts': [0, list], 'gateways': [0, list], 'http': 0, 'tls': 3, 'tcp': 3,
-                                    'exportTo': [3, str]})
+                                    'exportTo': [3, list]})
         hosts = vs_spec.get('hosts')
         for host in hosts or []:
             host_dfa = self.parse_host_value(host, vs_resource)
             if host_dfa:
                 vs.add_host_dfa(host_dfa)
 
         self.parse_vs_gateways(vs, vs_spec)
```

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/K8sPolicyYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/K8sPolicyYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Parsers/K8sServiceYamlParser.py` & `network-config-analyzer-1.9.4/nca/Parsers/K8sServiceYamlParser.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Resources/CalicoNetworkPolicy.py` & `network-config-analyzer-1.9.4/nca/Resources/CalicoNetworkPolicy.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,34 +83,34 @@
             self.order == other.order
 
     def _update_opt_props_by_order(self, is_ingress):
         # handle the order of rules
         for rule in self.ingress_rules if is_ingress else self.egress_rules:
             props = rule.optimized_props.copy()
             if rule.action == CalicoPolicyRule.ActionType.Allow:
-                props -= self.optimized_deny_ingress_props if is_ingress else self.optimized_deny_egress_props
-                props -= self.optimized_pass_ingress_props if is_ingress else self.optimized_pass_egress_props
+                props -= self._optimized_deny_ingress_props if is_ingress else self._optimized_deny_egress_props
+                props -= self._optimized_pass_ingress_props if is_ingress else self._optimized_pass_egress_props
                 if is_ingress:
-                    self.optimized_allow_ingress_props |= props
+                    self._optimized_allow_ingress_props |= props
                 else:
-                    self.optimized_allow_egress_props |= props
+                    self._optimized_allow_egress_props |= props
             elif rule.action == CalicoPolicyRule.ActionType.Deny:
-                props -= self.optimized_allow_ingress_props if is_ingress else self.optimized_allow_egress_props
-                props -= self.optimized_pass_ingress_props if is_ingress else self.optimized_pass_egress_props
+                props -= self._optimized_allow_ingress_props if is_ingress else self._optimized_allow_egress_props
+                props -= self._optimized_pass_ingress_props if is_ingress else self._optimized_pass_egress_props
                 if is_ingress:
-                    self.optimized_deny_ingress_props |= props
+                    self._optimized_deny_ingress_props |= props
                 else:
-                    self.optimized_deny_egress_props |= props
+                    self._optimized_deny_egress_props |= props
             elif rule.action == CalicoPolicyRule.ActionType.Pass:
-                props -= self.optimized_allow_ingress_props if is_ingress else self.optimized_allow_egress_props
-                props -= self.optimized_deny_ingress_props if is_ingress else self.optimized_deny_egress_props
+                props -= self._optimized_allow_ingress_props if is_ingress else self._optimized_allow_egress_props
+                props -= self._optimized_deny_ingress_props if is_ingress else self._optimized_deny_egress_props
                 if is_ingress:
-                    self.optimized_pass_ingress_props |= props
+                    self._optimized_pass_ingress_props |= props
                 else:
-                    self.optimized_pass_egress_props |= props
+                    self._optimized_pass_egress_props |= props
 
     def sync_opt_props(self):
         """
         If optimized props of the policy are not synchronized (self.optimized_props_in_sync is False),
         compute optimized props of the policy according to the optimized props of its rules
         """
         if self.optimized_props_in_sync:
@@ -165,25 +165,24 @@
         Evaluate the set of connections this policy allows/denies/passes between any two peers
         :param bool is_ingress: whether we evaluate ingress rules only or egress rules only
         :return: A ConnectivityProperties object containing all allowed connections for relevant peers,
         ConnectivityProperties object containing all denied connections,
         and the peer set of captured peers by this policy.
         :rtype: tuple (ConnectivityProperties, ConnectivityProperties, PeerSet)
         """
-        self.sync_opt_props()
         res_conns = OptimizedPolicyConnections()
         if is_ingress:
-            res_conns.allowed_conns = self.optimized_allow_ingress_props.copy()
-            res_conns.denied_conns = self.optimized_deny_ingress_props.copy()
-            res_conns.pass_conns = self.optimized_pass_ingress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_ingress_props().copy()
+            res_conns.denied_conns = self.optimized_deny_ingress_props().copy()
+            res_conns.pass_conns = self.optimized_pass_ingress_props().copy()
             res_conns.captured = self.selected_peers if self.affects_ingress else Peer.PeerSet()
         else:
-            res_conns.allowed_conns = self.optimized_allow_egress_props.copy()
-            res_conns.denied_conns = self.optimized_deny_egress_props.copy()
-            res_conns.pass_conns = self.optimized_pass_egress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_egress_props().copy()
+            res_conns.denied_conns = self.optimized_deny_egress_props().copy()
+            res_conns.pass_conns = self.optimized_pass_egress_props().copy()
             res_conns.captured = self.selected_peers if self.affects_egress else Peer.PeerSet()
         return res_conns
 
     def clone_without_rule(self, rule_to_exclude, ingress_rule):
         """
         Makes a copy of 'self' without a given policy rule
         :param CalicoPolicyRule rule_to_exclude: The one rule not to include in the copy
```

### Comparing `network-config-analyzer-1.9.3/nca/Resources/IngressPolicy.py` & `network-config-analyzer-1.9.4/nca/Resources/IngressPolicy.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         If optimized props of the policy are not synchronized (self.optimized_props_in_sync is False),
         compute optimized props of the policy according to the optimized props of its rules
         """
         if self.optimized_props_in_sync:
             return
         self._init_opt_props()
         for rule in self.egress_rules:
-            self.optimized_allow_egress_props |= rule.optimized_props
+            self._optimized_allow_egress_props |= rule.optimized_props
         self.optimized_props_in_sync = True
 
     def allowed_connections(self, from_peer, to_peer, is_ingress):
         """
         Evaluate the set of connections this ingress resource allows between two peers
         :param Peer.Peer from_peer: The source peer
         :param Peer.Peer to_peer:  The target peer
@@ -106,21 +106,20 @@
         :param bool is_ingress: For compatibility with other policies.
          Will return the set of allowed connections only for is_ingress being False.
         :return: A ConnectivityProperties object containing all allowed connections for any peers,
         ConnectivityProperties object containing all denied connections,
         and the peer set of captured peers by this policy.
         :rtype: tuple (ConnectivityProperties, ConnectivityProperties, PeerSet)
         """
-        self.sync_opt_props()
         res_conns = OptimizedPolicyConnections()
         if is_ingress:
             res_conns.allowed_conns = ConnectivityProperties.make_empty_props()
             res_conns.captured = PeerSet()
         else:
-            res_conns.allowed_conns = self.optimized_allow_egress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_egress_props().copy()
             res_conns.captured = self.selected_peers if self.affects_egress else PeerSet()
         return res_conns
 
     def has_empty_rules(self, _config_name=''):
         """
         Checks whether the policy contains empty rules (rules that do not select any peers)
         :param str _config_name: is not used. Kept for compatibility with other policies.
```

### Comparing `network-config-analyzer-1.9.3/nca/Resources/IstioNetworkPolicy.py` & `network-config-analyzer-1.9.4/nca/Resources/IstioNetworkPolicy.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,19 +74,19 @@
         compute optimized props of the policy according to the optimized props of its rules
         """
         if self.optimized_props_in_sync:
             return
         self._init_opt_props()
         for rule in self.ingress_rules:
             if self.action == IstioNetworkPolicy.ActionType.Allow:
-                self.optimized_allow_ingress_props |= rule.optimized_props
+                self._optimized_allow_ingress_props |= rule.optimized_props
             elif self.action == IstioNetworkPolicy.ActionType.Deny:
-                self.optimized_deny_ingress_props |= rule.optimized_props
+                self._optimized_deny_ingress_props |= rule.optimized_props
 
-        self.optimized_allow_egress_props = ConnectivityProperties.get_all_conns_props_per_domain_peers()
+        self._optimized_allow_egress_props = ConnectivityProperties.get_all_conns_props_per_domain_peers()
         self.optimized_props_in_sync = True
 
     def allowed_connections(self, from_peer, to_peer, is_ingress):
         """
         Evaluate the set of connections this policy allows/denies/passes between two peers
         :param Peer.Peer from_peer: The source peer
         :param Peer.Peer to_peer:  The target peer
@@ -118,23 +118,22 @@
         Evaluate the set of connections this policy allows/denied/passed between any two peers
         :param bool is_ingress: whether we evaluate ingress rules only or egress rules only
         :return: A ConnectivityProperties object containing all allowed connections for relevant peers,
         ConnectivityProperties object containing all denied connections,
         and the peer set of captured peers by this policy.
         :rtype: tuple (ConnectivityProperties, ConnectivityProperties, PeerSet)
         """
-        self.sync_opt_props()
         res_conns = OptimizedPolicyConnections()
         if is_ingress:
-            res_conns.allowed_conns = self.optimized_allow_ingress_props.copy()
-            res_conns.denied_conns = self.optimized_deny_ingress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_ingress_props().copy()
+            res_conns.denied_conns = self.optimized_deny_ingress_props().copy()
             res_conns.captured = self.selected_peers
         else:
-            res_conns.allowed_conns = self.optimized_allow_egress_props.copy()
-            res_conns.denied_conns = self.optimized_deny_egress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_egress_props().copy()
+            res_conns.denied_conns = self.optimized_deny_egress_props().copy()
             res_conns.captured = PeerSet()
         return res_conns
 
     def referenced_ip_blocks(self, exclude_ipv6=False):
         """
         :param bool exclude_ipv6: indicates if to exclude the automatically added IPv6 addresses in the referenced ip_blocks.
         IPv6 addresses that are referenced in the policy by the user will always be included
```

### Comparing `network-config-analyzer-1.9.3/nca/Resources/IstioSidecar.py` & `network-config-analyzer-1.9.4/nca/Resources/IstioSidecar.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,17 @@
         """
         If optimized props of the policy are not synchronized (self.optimized_props_in_sync is False),
         compute optimized props of the policy according to the optimized props of its rules
         """
         if self.optimized_props_in_sync:
             return
         self._init_opt_props()
-        self.optimized_allow_ingress_props = ConnectivityProperties.get_all_conns_props_per_domain_peers()
+        self._optimized_allow_ingress_props = ConnectivityProperties.get_all_conns_props_per_domain_peers()
         for rule in self.egress_rules:
-            self.optimized_allow_egress_props |= rule.optimized_props
+            self._optimized_allow_egress_props |= rule.optimized_props
         self.optimized_props_in_sync = True
 
     def allowed_connections(self, from_peer, to_peer, is_ingress):
         """
         Evaluate the set of connections this policy allows/denies/passes between two peers
         :param Peer.Peer from_peer: The source peer
         :param Peer.Peer to_peer:  The target peer
@@ -96,23 +96,22 @@
                 return PolicyConnections(True, allowed_conns=ConnectionSet(True))
 
         # egress from from_peer to to_peer is not allowed : if to_peer not been captured in the rules' egress_peer_set,
         # or if the sidecar is global and to_peer is not in same namespace of from_peer while rule host's ns is '.'
         return PolicyConnections(True, allowed_conns=ConnectionSet())
 
     def allowed_connections_optimized(self, is_ingress):
-        self.sync_opt_props()
         res_conns = OptimizedPolicyConnections()
         if is_ingress:
-            res_conns.allowed_conns = self.optimized_allow_ingress_props.copy()
-            res_conns.denied_conns = self.optimized_deny_ingress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_ingress_props().copy()
+            res_conns.denied_conns = self.optimized_deny_ingress_props().copy()
             res_conns.captured = PeerSet()
         else:
-            res_conns.allowed_conns = self.optimized_allow_egress_props.copy()
-            res_conns.denied_conns = self.optimized_deny_egress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_egress_props().copy()
+            res_conns.denied_conns = self.optimized_deny_egress_props().copy()
             res_conns.captured = self.selected_peers if self.affects_egress else PeerSet()
         return res_conns
 
     def has_empty_rules(self, config_name=''):
         """
         Checks whether the sidecar contains empty rules (rules that do not select any peers)
         :param str config_name: (optional) the name of the NetworkConfig object
```

### Comparing `network-config-analyzer-1.9.3/nca/Resources/IstioTrafficResources.py` & `network-config-analyzer-1.9.4/nca/Resources/IstioTrafficResources.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Resources/K8sNamespace.py` & `network-config-analyzer-1.9.4/nca/Resources/K8sNamespace.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Resources/K8sNetworkPolicy.py` & `network-config-analyzer-1.9.4/nca/Resources/K8sNetworkPolicy.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,17 @@
         If optimized props of the policy are not synchronized (self.optimized_props_in_sync is False),
         compute optimized props of the policy according to the optimized props of its rules
         """
         if self.optimized_props_in_sync:
             return
         self._init_opt_props()
         for rule in self.ingress_rules:
-            self.optimized_allow_ingress_props |= rule.optimized_props
+            self._optimized_allow_ingress_props |= rule.optimized_props
         for rule in self.egress_rules:
-            self.optimized_allow_egress_props |= rule.optimized_props
+            self._optimized_allow_egress_props |= rule.optimized_props
         self.optimized_props_in_sync = True
 
     def allowed_connections(self, from_peer, to_peer, is_ingress):
         """
         Evaluate the set of connections this policy allows between two peers
         (either the allowed ingress into to_peer or the allowed egress from from_peer).
         :param Peer.Peer from_peer: The source peer
@@ -85,21 +85,20 @@
         (either ingress or egress).
         :param bool is_ingress: whether we evaluate ingress rules only or egress rules only
         :return: A ConnectivityProperties object containing all allowed connections for relevant peers,
         None for denied connections (K8s does not have denied),
         and the peer set of captured peers by this policy.
         :rtype: tuple (ConnectivityProperties, ConnectivityProperties, PeerSet)
         """
-        self.sync_opt_props()
         res_conns = OptimizedPolicyConnections()
         if is_ingress:
-            res_conns.allowed_conns = self.optimized_allow_ingress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_ingress_props().copy()
             res_conns.captured = self.selected_peers if self.affects_ingress else Peer.PeerSet()
         else:
-            res_conns.allowed_conns = self.optimized_allow_egress_props.copy()
+            res_conns.allowed_conns = self.optimized_allow_egress_props().copy()
             res_conns.captured = self.selected_peers if self.affects_egress else Peer.PeerSet()
         return res_conns
 
     def clone_without_rule(self, rule_to_exclude, ingress_rule):
         """
         Makes a copy of 'self' without a given policy rule
         :param K8sPolicyRule rule_to_exclude: The one rule not to include in the copy
```

### Comparing `network-config-analyzer-1.9.3/nca/Resources/K8sService.py` & `network-config-analyzer-1.9.4/nca/Resources/K8sService.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Resources/NetworkPolicy.py` & `network-config-analyzer-1.9.4/nca/Resources/NetworkPolicy.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,41 +68,75 @@
         self.policy_kind = NetworkPolicy.PolicyType.Unknown
         self.has_ipv6_addresses = False  # whether the policy referenced ip addresses (by user)
         # if this flag is False, excluding ipv6 addresses from the query results will be enabled
 
     def _init_opt_props(self):
         """
         The members below are used for lazy evaluation of policy connectivity properties.
+        NOTE: THEY CANNOT BE ACCESSED DIRECTLY, ONLY BY 'GETTER' METHODS BELOW!
         """
-        self.optimized_allow_ingress_props = ConnectivityProperties.make_empty_props()
-        self.optimized_deny_ingress_props = ConnectivityProperties.make_empty_props()
-        self.optimized_pass_ingress_props = ConnectivityProperties.make_empty_props()
-        self.optimized_allow_egress_props = ConnectivityProperties.make_empty_props()
-        self.optimized_deny_egress_props = ConnectivityProperties.make_empty_props()
-        self.optimized_pass_egress_props = ConnectivityProperties.make_empty_props()
+        self._optimized_allow_ingress_props = ConnectivityProperties.make_empty_props()
+        self._optimized_deny_ingress_props = ConnectivityProperties.make_empty_props()
+        self._optimized_pass_ingress_props = ConnectivityProperties.make_empty_props()
+        self._optimized_allow_egress_props = ConnectivityProperties.make_empty_props()
+        self._optimized_deny_egress_props = ConnectivityProperties.make_empty_props()
+        self._optimized_pass_egress_props = ConnectivityProperties.make_empty_props()
+
+    def optimized_allow_ingress_props(self):
+        self.sync_opt_props()
+        return self._optimized_allow_ingress_props
+
+    def optimized_deny_ingress_props(self):
+        self.sync_opt_props()
+        return self._optimized_deny_ingress_props
+
+    def optimized_pass_ingress_props(self):
+        self.sync_opt_props()
+        return self._optimized_pass_ingress_props
+
+    def optimized_allow_egress_props(self):
+        self.sync_opt_props()
+        return self._optimized_allow_egress_props
+
+    def optimized_deny_egress_props(self):
+        self.sync_opt_props()
+        return self._optimized_deny_egress_props
+
+    def optimized_pass_egress_props(self):
+        self.sync_opt_props()
+        return self._optimized_pass_egress_props
+
+    def sync_opt_props(self):
+        """
+        Implemented by derived policies to compute optimized props of the policy according to the optimized props
+        of its rules, in case optimized props are not currently synchronized.
+        """
+        return NotImplemented
 
     def __str__(self):
         return self.full_name()
 
     def __eq__(self, other):
         if type(self) == type(other):
+            self.sync_opt_props()
+            other.sync_opt_props()
             return \
                 self.name == other.name and \
                 self.namespace == other.namespace and \
                 self.affects_egress == other.affects_egress and \
                 self.affects_ingress == other.affects_ingress and \
                 self.selected_peers == other.selected_peers and \
                 self.ingress_rules == other.ingress_rules and \
                 self.egress_rules == other.egress_rules and \
-                self.optimized_allow_ingress_props == other.optimized_allow_ingress_props and \
-                self.optimized_deny_ingress_props == other.optimized_deny_ingress_props and \
-                self.optimized_pass_ingress_props == other.optimized_pass_ingress_props and \
-                self.optimized_allow_egress_props == other.optimized_allow_egress_props and \
-                self.optimized_deny_egress_props == other.optimized_deny_egress_props and \
-                self.optimized_pass_egress_props == other.optimized_pass_egress_props
+                self._optimized_allow_ingress_props == other._optimized_allow_ingress_props and \
+                self._optimized_deny_ingress_props == other._optimized_deny_ingress_props and \
+                self._optimized_pass_ingress_props == other._optimized_pass_ingress_props and \
+                self._optimized_allow_egress_props == other._optimized_allow_egress_props and \
+                self._optimized_deny_egress_props == other._optimized_deny_egress_props and \
+                self._optimized_pass_egress_props == other._optimized_pass_egress_props
         return False
 
     def __lt__(self, other):  # required so we can evaluate the policies according to their order
         if not isinstance(other, NetworkPolicy):
             return False
         # TODO - should add the condition below to make the comparison stable.
         # This makes some tests to fail because the order of output is different
```

### Comparing `network-config-analyzer-1.9.3/nca/SchemeRunner.py` & `network-config-analyzer-1.9.4/nca/SchemeRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 
 class SchemeRunner(GenericYamlParser):
     """
     This class takes a scheme file, build all its network configurations and runs all its queries
     """
 
-    implemented_opt_queries = {'connectivityMap', 'equivalence', 'vacuity', 'redundancy', 'strongEquivalence'}
+    implemented_opt_queries = {'connectivityMap', 'equivalence', 'vacuity', 'redundancy',
+                               'strongEquivalence', 'containment', 'twoWayContainment', 'permits'}
 
     def __init__(self, scheme_file_name, output_format=None, output_path=None, optimized_run='false'):
         GenericYamlParser.__init__(self, scheme_file_name)
         self.network_configs = {}
         self.global_res = 0
         self.output_config_from_cli_args = dict()
         if output_format is not None:
```

### Comparing `network-config-analyzer-1.9.3/nca/Utils/CmdlineRunner.py` & `network-config-analyzer-1.9.4/nca/Utils/CmdlineRunner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Utils/ExplTracker.py` & `network-config-analyzer-1.9.4/nca/Utils/ExplTracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,18 +258,17 @@
         src_peer = self._get_peer_by_name(src)
         dst_peer = self._get_peer_by_name(dst)
 
         return True if self.all_conns & ConnectivityProperties.make_conn_props_from_dict(
             {"src_peers": PeerSet({src_peer}), "dst_peers": PeerSet({dst_peer})}) else False
 
     def add_policy_to_peers(self, policy):
-        policy.sync_opt_props()
         for peer in policy.selected_peers:
-            src_peers, _ = self.extract_peers(policy.optimized_allow_ingress_props)
-            _, dst_peers = self.extract_peers(policy.optimized_allow_egress_props)
+            src_peers, _ = self.extract_peers(policy.optimized_allow_ingress_props())
+            _, dst_peers = self.extract_peers(policy.optimized_allow_egress_props())
             peer_name = peer.full_name()
             self.add_peer_policy(peer_name, policy.name, dst_peers, src_peers)
 
     def add_default_policy(self, src, dst, is_ingress):
         """
         Add the default policy to the peers which were not affected by a specific policy.
         :param PeerSet src: the peer list for the source of the policy
```

### Comparing `network-config-analyzer-1.9.3/nca/Utils/NcaLogger.py` & `network-config-analyzer-1.9.4/nca/Utils/NcaLogger.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Utils/OutputConfiguration.py` & `network-config-analyzer-1.9.4/nca/Utils/OutputConfiguration.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/Utils/OutputFilesFlags.py` & `network-config-analyzer-1.9.4/nca/Utils/OutputFilesFlags.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/nca/nca_cli.py` & `network-config-analyzer-1.9.4/nca/nca_cli.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/network_config_analyzer.egg-info/PKG-INFO` & `network-config-analyzer-1.9.4/network_config_analyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-config-analyzer
-Version: 1.9.3
+Version: 1.9.4
 Summary: An analyzer for Network Policies and other connectivity-configuration resources
 Home-page: https://github.com/IBM/network-config-analyzer
 Author: Ziv Nevo
 Author-email: nevo@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/network-config-analyzer/issues
 Project-URL: NP-Guard Home, https://np-guard.github.io
 Classifier: Programming Language :: Python :: 3
```

### Comparing `network-config-analyzer-1.9.3/network_config_analyzer.egg-info/SOURCES.txt` & `network-config-analyzer-1.9.4/network_config_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.3/setup.cfg` & `network-config-analyzer-1.9.4/setup.cfg`

 * *Files identical despite different names*

