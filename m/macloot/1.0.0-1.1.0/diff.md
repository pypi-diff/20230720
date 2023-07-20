# Comparing `tmp/macloot-1.0.0.tar.gz` & `tmp/macloot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macloot-1.0.0.tar", last modified: Wed Jul 19 10:25:02 2023, max compression
+gzip compressed data, was "macloot-1.1.0.tar", last modified: Thu Jul 20 14:53:17 2023, max compression
```

## Comparing `macloot-1.0.0.tar` & `macloot-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mikael    (1000) mikael    (1000)        0 2023-07-19 10:25:02.225981 macloot-1.0.0/
--rw-r--r--   0 mikael    (1000) mikael    (1000)     1088 2023-07-17 11:21:42.000000 macloot-1.0.0/LICENSE
--rw-r--r--   0 mikael    (1000) mikael    (1000)     6967 2023-07-19 10:25:02.225981 macloot-1.0.0/PKG-INFO
--rw-r--r--   0 mikael    (1000) mikael    (1000)     6063 2023-07-15 14:31:00.000000 macloot-1.0.0/README.md
--rw-r--r--   0 mikael    (1000) mikael    (1000)      364 2023-07-15 14:24:00.000000 macloot-1.0.0/app_info.py
--rw-r--r--   0 mikael    (1000) mikael    (1000)    10139 2023-07-19 07:27:32.000000 macloot-1.0.0/mac.py
-drwxr-xr-x   0 mikael    (1000) mikael    (1000)        0 2023-07-19 10:25:02.225981 macloot-1.0.0/macloot.egg-info/
--rw-r--r--   0 mikael    (1000) mikael    (1000)     6967 2023-07-19 10:25:02.000000 macloot-1.0.0/macloot.egg-info/PKG-INFO
--rw-r--r--   0 mikael    (1000) mikael    (1000)      285 2023-07-19 10:25:02.000000 macloot-1.0.0/macloot.egg-info/SOURCES.txt
--rw-r--r--   0 mikael    (1000) mikael    (1000)        1 2023-07-19 10:25:02.000000 macloot-1.0.0/macloot.egg-info/dependency_links.txt
--rw-r--r--   0 mikael    (1000) mikael    (1000)       41 2023-07-19 10:25:02.000000 macloot-1.0.0/macloot.egg-info/entry_points.txt
--rw-r--r--   0 mikael    (1000) mikael    (1000)        9 2023-07-19 10:25:02.000000 macloot-1.0.0/macloot.egg-info/requires.txt
--rw-r--r--   0 mikael    (1000) mikael    (1000)       25 2023-07-19 10:25:02.000000 macloot-1.0.0/macloot.egg-info/top_level.txt
--rwxr-xr-x   0 mikael    (1000) mikael    (1000)    11714 2023-07-19 10:17:39.000000 macloot-1.0.0/macloot.py
--rw-r--r--   0 mikael    (1000) mikael    (1000)     8570 2023-07-18 18:13:55.000000 macloot-1.0.0/oui.py
--rw-r--r--   0 mikael    (1000) mikael    (1000)       38 2023-07-19 10:25:02.225981 macloot-1.0.0/setup.cfg
--rw-r--r--   0 mikael    (1000) mikael    (1000)     1251 2023-07-17 11:12:53.000000 macloot-1.0.0/setup.py
-drwxr-xr-x   0 mikael    (1000) mikael    (1000)        0 2023-07-19 10:25:02.225981 macloot-1.0.0/test/
--rw-r--r--   0 mikael    (1000) mikael    (1000)    10885 2023-07-19 07:58:57.000000 macloot-1.0.0/test/test_mac.py
--rw-r--r--   0 mikael    (1000) mikael    (1000)     8713 2023-07-19 07:59:12.000000 macloot-1.0.0/test/test_oui.py
+drwxr-xr-x   0 mikael    (1000) mikael    (1000)        0 2023-07-20 14:53:17.788191 macloot-1.1.0/
+-rw-r--r--   0 mikael    (1000) mikael    (1000)     1088 2023-07-17 11:21:42.000000 macloot-1.1.0/LICENSE
+-rw-r--r--   0 mikael    (1000) mikael    (1000)     6965 2023-07-20 14:53:17.784191 macloot-1.1.0/PKG-INFO
+-rw-r--r--   0 mikael    (1000) mikael    (1000)     6061 2023-07-20 07:02:22.000000 macloot-1.1.0/README.md
+-rw-r--r--   0 mikael    (1000) mikael    (1000)      364 2023-07-20 14:47:46.000000 macloot-1.1.0/app_info.py
+-rw-r--r--   0 mikael    (1000) mikael    (1000)    10478 2023-07-20 13:03:09.000000 macloot-1.1.0/mac.py
+drwxr-xr-x   0 mikael    (1000) mikael    (1000)        0 2023-07-20 14:53:17.784191 macloot-1.1.0/macloot.egg-info/
+-rw-r--r--   0 mikael    (1000) mikael    (1000)     6965 2023-07-20 14:53:17.000000 macloot-1.1.0/macloot.egg-info/PKG-INFO
+-rw-r--r--   0 mikael    (1000) mikael    (1000)      285 2023-07-20 14:53:17.000000 macloot-1.1.0/macloot.egg-info/SOURCES.txt
+-rw-r--r--   0 mikael    (1000) mikael    (1000)        1 2023-07-20 14:53:17.000000 macloot-1.1.0/macloot.egg-info/dependency_links.txt
+-rw-r--r--   0 mikael    (1000) mikael    (1000)       41 2023-07-20 14:53:17.000000 macloot-1.1.0/macloot.egg-info/entry_points.txt
+-rw-r--r--   0 mikael    (1000) mikael    (1000)        9 2023-07-20 14:53:17.000000 macloot-1.1.0/macloot.egg-info/requires.txt
+-rw-r--r--   0 mikael    (1000) mikael    (1000)       25 2023-07-20 14:53:17.000000 macloot-1.1.0/macloot.egg-info/top_level.txt
+-rwxr-xr-x   0 mikael    (1000) mikael    (1000)    11168 2023-07-20 13:03:09.000000 macloot-1.1.0/macloot.py
+-rw-r--r--   0 mikael    (1000) mikael    (1000)     9382 2023-07-20 14:47:11.000000 macloot-1.1.0/oui.py
+-rw-r--r--   0 mikael    (1000) mikael    (1000)       38 2023-07-20 14:53:17.788191 macloot-1.1.0/setup.cfg
+-rw-r--r--   0 mikael    (1000) mikael    (1000)     1251 2023-07-17 11:12:53.000000 macloot-1.1.0/setup.py
+drwxr-xr-x   0 mikael    (1000) mikael    (1000)        0 2023-07-20 14:53:17.784191 macloot-1.1.0/test/
+-rw-r--r--   0 mikael    (1000) mikael    (1000)    11105 2023-07-20 13:03:09.000000 macloot-1.1.0/test/test_mac.py
+-rw-r--r--   0 mikael    (1000) mikael    (1000)     8713 2023-07-20 13:03:09.000000 macloot-1.1.0/test/test_oui.py
```

### Comparing `macloot-1.0.0/LICENSE` & `macloot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macloot-1.0.0/PKG-INFO` & `macloot-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macloot
-Version: 1.0.0
+Version: 1.1.0
 Summary: A CLI tool to lookup the Organization (OUI) of MAC addresses, from file or stdin, and/or transform between different MAC address formats.
 Home-page: https://github.com/bitcanon/macloot
 Author: Mikael Schultz
 Author-email: macloot.3jcsb@passmail.net
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -111,15 +111,15 @@
 ```
 Output:
 ```bash
 2c:c8:1b:a1:b2:c3   Routerboard.com
 ```
 
 ### Character Casing
-To modify the character casing of MAC addresses in the output, you can utilize the `-l` or `--lower-case` and `-u` or `--upper-case` arguments. Using `-l` will convert the output MAC addresses to lowercase, while `-u` will convert them to uppercase.
+To modify the character casing of MAC addresses in the output, you can utilize the `-l` or `--lowercase` and `-u` or `--uppercase` arguments. Using `-l` will convert the output MAC addresses to lowercase, while `-u` will convert them to uppercase.
 
 If neither of these arguments is provided, the original casing of the input MAC addresses will be preserved in the output.
 
 #### Uppercase
 In this example we convert a MAC address in Cisco format to the format Microsoft uses (with hyphens, in **uppercase**) by using the `-u` argument:
 ```bash
 macloot 1c1a.dfa1.b2c3 -O - -u
@@ -143,19 +143,19 @@
 To search for OUIs based on company names, you can utilize the `-s` or `--search` argument. By providing the desired company name as the argument value, such as "Cisco," "Apple," or "Microsoft," you can retrieve the corresponding OUIs associated with those companies. This feature enables easy lookup and identification of OUIs based on the names of specific organizations.
 
 ```bash
 macloot -s microsoft
 ```
 Output:
 ```bash
-70F8AE  Microsoft Corporation
-201642  Microsoft Corporation
-C461C7  Microsoft Corporation
-D8E2DF  Microsoft Corporation
-A085FC  Microsoft Corporation
+0003FF  Microsoft Corporation
+000D3A  Microsoft Corporation
+00125A  Microsoft Corporation
+00155D  Microsoft Corporation
+0017FA  Microsoft Corporation
 ... (output truncated) ...
 ```
 To make the output compatible with CSV format, you can use the `-d ";"` option here as well. 
 ## Update OUI database
 You can easily update the OUI database at any time by running the command: 
 ```bash
 macloot --update-db
```

### Comparing `macloot-1.0.0/README.md` & `macloot-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 ```
 Output:
 ```bash
 2c:c8:1b:a1:b2:c3   Routerboard.com
 ```
 
 ### Character Casing
-To modify the character casing of MAC addresses in the output, you can utilize the `-l` or `--lower-case` and `-u` or `--upper-case` arguments. Using `-l` will convert the output MAC addresses to lowercase, while `-u` will convert them to uppercase.
+To modify the character casing of MAC addresses in the output, you can utilize the `-l` or `--lowercase` and `-u` or `--uppercase` arguments. Using `-l` will convert the output MAC addresses to lowercase, while `-u` will convert them to uppercase.
 
 If neither of these arguments is provided, the original casing of the input MAC addresses will be preserved in the output.
 
 #### Uppercase
 In this example we convert a MAC address in Cisco format to the format Microsoft uses (with hyphens, in **uppercase**) by using the `-u` argument:
 ```bash
 macloot 1c1a.dfa1.b2c3 -O - -u
@@ -122,19 +122,19 @@
 To search for OUIs based on company names, you can utilize the `-s` or `--search` argument. By providing the desired company name as the argument value, such as "Cisco," "Apple," or "Microsoft," you can retrieve the corresponding OUIs associated with those companies. This feature enables easy lookup and identification of OUIs based on the names of specific organizations.
 
 ```bash
 macloot -s microsoft
 ```
 Output:
 ```bash
-70F8AE  Microsoft Corporation
-201642  Microsoft Corporation
-C461C7  Microsoft Corporation
-D8E2DF  Microsoft Corporation
-A085FC  Microsoft Corporation
+0003FF  Microsoft Corporation
+000D3A  Microsoft Corporation
+00125A  Microsoft Corporation
+00155D  Microsoft Corporation
+0017FA  Microsoft Corporation
 ... (output truncated) ...
 ```
 To make the output compatible with CSV format, you can use the `-d ";"` option here as well. 
 ## Update OUI database
 You can easily update the OUI database at any time by running the command: 
 ```bash
 macloot --update-db
```

### Comparing `macloot-1.0.0/mac.py` & `macloot-1.1.0/mac.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 """
 mac.py
 
-This module provides the `MacAddress` class and functionality for handling MAC addresses. 
-The `MacAddress` class represents a MAC address and includes methods for manipulation, formatting 
-    and analysis.
+This module provides the `MacAddress` classes and functionality for handling MAC addresses. 
+The main `MacAddress` class represents a MAC address and includes methods for manipulation,
+    formatting and analysis.
 
 Classes:
 - MacAddress: Represents a MAC address and provides various methods for MAC address handling.
-
-Usage:
-1. Import the module: `from mac import MacAddress`
-2. Create a `MacAddress` object: `mac = mac.MacAddress('00:11:22:33:44:55')`
-3. Access the MAC address and perform operations:
-   - `mac.address`: Returns the MAC address string.
-   - `mac.lowercase`: Returns the MAC address in lowercase.
-   - `mac.uppercase`: Returns the MAC address in uppercase.
-   - `mac.remove_separators()`: Returns the MAC address with separators removed.
-   - ...
+- MacCase: Enumeration class representing the character casing used by the MacAddress class.
+- MacAddressGenerator: Generates testing addresses and output in various formats.
 
 Note: The methods in the `MacAddress` class operate on well-formed MAC addresses. Ensure that the 
     MAC address string provided adheres to the standard format.
 
 For more information, refer to the documentation or relevant code comments.
 """
 import random
 import re
 
-from oui import OuiDatabase
+from enum import Enum
+from oui import OuiDatabase, OuiOrganization
+
+class MacCase(Enum):
+    """ Defines three possible character case values. """
+    ORIGINAL  = 0   # Leave as provided by input
+    UPPERCASE = 1   # Uppercase
+    LOWERCASE = 2   # Lowercase
 
 class MacAddress:
     """ Class definition of a MAC address. """
 
-    def __init__(self, mac_address: str) -> None:
+    def __init__(self, mac_address: str, case: MacCase = MacCase.ORIGINAL) -> None:
         """ Initialize a MacAddress object with the provided MAC address. """
         self.__address = MacAddress.remove_separators(mac_address)
-        self.__organization_name = None
-        self.__organization_address = None
+        self.__organization = OuiOrganization(name=None, address=None)
         self.__octet_separator = MacAddress.get_octet_separator(mac_address)
+        self.__case = case
 
     def __str__(self):
         """ Get the string representation of the MacAddress object. """
         return self.address
 
     def __eq__(self, other):
         """ Compare this MacAddress with another MacAddress object. """
         if isinstance(other, MacAddress):
             return  self.__address == other.address and \
-                    self.__organization_name == other.organization_name
+                    self.__organization.name == other.organization.name
+        return False
+
+    def __lt__(self, other):
+        """ Check if this MacAddress is 'less than' another MacAddress object. """
+        if isinstance(other, MacAddress):
+            return self.to_int() < other.to_int()
         return False
 
     def to_bytes(self):
         """ Convert the MAC address into a bytes representation. """
         # Implement logic to convert the MAC address into a bytes representation
         raise NotImplementedError
 
+    def to_int(self):
+        """ Convert the MAC address into an integer representation. """
+        return int(self.__address, 16)
+
+    def to_list(self, verbose: bool = False) -> list:
+        """ Return a subset or all printable properties of the MacAddress class as a list. """
+        if verbose:
+            return [str(self.address), str(self.__organization.name),
+                    str(self.__organization.address)]
+        return [str(self.address), str(self.__organization.name)]
+
     @classmethod
     def check_case(cls, mac_address: str) -> str:
         """ Check if the MAC address is in upper or lower case. """
 
         # Check if the MAC address contains only digits
         if mac_address.isdigit():
             return None
@@ -100,71 +116,53 @@
 
         # Regex pattern to find b00bface1337 or B00Bface1234
         hex_pattern  = re.findall(r'(?:[\da-fA-F]{12})', input_string)
 
         return common_pattern + cisco_pattern + hex_pattern
 
     @classmethod
-    def format(cls, mac: str, separator: str = ":", section_size: int = 2) -> str:
+    def format(cls, mac: str, separator: str = ":", section_size: int = 2,
+               case: MacCase = MacCase.ORIGINAL) -> str:
         """ Insert separator between octets in the MAC address string. """
         mac_octets = [mac[i:i+section_size] for i in range(0, len(mac), section_size)]
-        return separator.join(mac_octets)
+        mac_address = separator.join(mac_octets)
+        if case == MacCase.UPPERCASE:
+            mac_address = mac_address.upper()
+        elif case == MacCase.LOWERCASE:
+            mac_address = mac_address.lower()
+        return mac_address
 
     @property
     def address(self):
         """
         Return the MAC address using the delimiter from the self.__delimiter variable.
         
         If the delimiter is a . (dot) we return the address Cisco style:
          - xxxx.xxxx.xxxx
         Else we return the address "everyone else" style:
          - xx-xx-xx-xx-xx-xx
          - xx:xx:xx:xx:xx:xx
         """
         if self.octet_separator == ".":
             mac_address = MacAddress.format(self.__address, separator=self.octet_separator,
-                                            section_size=4)
+                                            section_size=4, case=self.__case)
         else:
-            mac_address = MacAddress.format(self.__address, separator=self.octet_separator)
+            mac_address = MacAddress.format(self.__address, separator=self.octet_separator,
+                                            case=self.__case)
         return mac_address
 
     @property
     def oui(self):
         """ Get the OUI part of the MAC address (the first 6 characters). """
         return self.__address[:6].upper()
 
     @property
-    def lowercase(self):
-        """ Get the MAC address in lowercase. """
-        return self.address.lower()
-
-    @property
-    def uppercase(self):
-        """ Get the MAC address in uppercase. """
-        return self.address.upper()
-
-    @property
-    def organization_name(self):
-        """ Get the organization name found in the OUI database. """
-        return self.__organization_name
-
-    @organization_name.setter
-    def organization_name(self, value):
-        """ Set the organization name found in the OUI database. """
-        self.__organization_name = value
-
-    @property
-    def organization_address(self):
-        """ Get the organization address found in the OUI database. """
-        return self.__organization_address
-
-    @organization_address.setter
-    def organization_address(self, value):
-        """ Set the organization address found in the OUI database. """
-        self.__organization_address = value
+    def organization(self):
+        """ Get the Organization data object. """
+        return self.__organization
 
     @property
     def octet_separator(self):
         """ Get the octet separator to be used between octets in the MAC address. """
         return self.__octet_separator
 
     @octet_separator.setter
@@ -176,54 +174,54 @@
     """ A MAC address generator class which outputs addresses in various formats. """
 
     def __init__(self, database: OuiDatabase):
         """ Initialize the MacAddressGenerator with the given OUI database. """
         database.load_database()
         self.__oui_list = database.get_entries()
 
-    def generate_mac_address(self):
+    def generate_mac_address(self, case: MacCase = MacCase.LOWERCASE):
         """ Generate a random and valid MAC address and return MacAddress object. """
 
         # Randomly pick a valid OUI from the OUI database (first 6 digits of MAC)
-        first_three_octets = random.choice(self.__oui_list).assignment
+        first_three_octets = random.choice(self.__oui_list).assignment.lower()
 
         # Randomly generate the last 3 octets (last 6 digits of MAC)
         last_three_octets = random.getrandbits(24)
 
         # Combine the two and return as a MacAddress object
-        return MacAddress(f"{first_three_octets}{last_three_octets:06X}")
+        return MacAddress(f"{first_three_octets}{last_three_octets:06x}", case=case)
 
-    def generate_mac_address_list(self, num: int, octet_separator: str, upper: bool = False):
+    def generate_mac_address_list(self, num: int, octet_separator: str,
+                                  case: MacCase = MacCase.LOWERCASE):
         """ Generate a list MAC addresses. """
         output = []
 
         for _ in range(num):
             # Get a random MAC address with a valid OUI
-            mac = self.generate_mac_address()
+            mac = self.generate_mac_address(case=case)
 
             # Use default octet separator ':' if none is provided
             mac.octet_separator = ':' if octet_separator is None else octet_separator
 
             # Print MAC addresses in users preferred case
-            mac_addr = mac.uppercase if upper else mac.lowercase
-            output.append(f"{mac_addr}")
+            output.append(f"{mac.address}")
         return "\n".join(output)
 
     def generate_ios_output(self, count):
         """ Generate a number of rows of Cisco IOS MAC Address Table. """
         output = []
         output.append('Mac Address Table')
         output.append('-------------------------------------------')
         output.append('Vlan    Mac Address       Type        Ports')
         output.append('----    -----------       --------    -----')
         vlan = 0
         for i in range(count):
             vlan += 1 if i % random.choice([2,4,8]) == 0 else 0
             mac = self.generate_mac_address()
-            mac_addr = MacAddress.format(mac.lowercase, '.', 4)
+            mac_addr = MacAddress.format(mac.address, '.', 4, case=MacCase.UPPERCASE)
             output.append(f" {vlan:2}     {mac_addr}    DYNAMIC     Gi0/1")
         return "\n".join(output)
 
     def generate_routeros_output(self, count):
         """ Generate a number of rows of RouterOS MAC Address Table. """
         output = []
         output.append("Flags: D - DYNAMIC; E - EXTERNAL")
@@ -244,10 +242,10 @@
         output.append("")
         output.append("MAC Address          VLAN     Type       Port")
         output.append("--------------------------------------------------")
         vlan = 0
         for i in range(count):
             vlan += 1 if i % random.choice([4,8,16]) == 0 else 0
             mac = self.generate_mac_address()
-            mac_addr = MacAddress.format(mac.lowercase)
+            mac_addr = MacAddress.format(mac.address, case=MacCase.LOWERCASE)
             output.append(f"{mac_addr}    {vlan:3}      dynamic    1/1/1")
         return "\n".join(output)
```

### Comparing `macloot-1.0.0/macloot.egg-info/PKG-INFO` & `macloot-1.1.0/macloot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macloot
-Version: 1.0.0
+Version: 1.1.0
 Summary: A CLI tool to lookup the Organization (OUI) of MAC addresses, from file or stdin, and/or transform between different MAC address formats.
 Home-page: https://github.com/bitcanon/macloot
 Author: Mikael Schultz
 Author-email: macloot.3jcsb@passmail.net
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -111,15 +111,15 @@
 ```
 Output:
 ```bash
 2c:c8:1b:a1:b2:c3   Routerboard.com
 ```
 
 ### Character Casing
-To modify the character casing of MAC addresses in the output, you can utilize the `-l` or `--lower-case` and `-u` or `--upper-case` arguments. Using `-l` will convert the output MAC addresses to lowercase, while `-u` will convert them to uppercase.
+To modify the character casing of MAC addresses in the output, you can utilize the `-l` or `--lowercase` and `-u` or `--uppercase` arguments. Using `-l` will convert the output MAC addresses to lowercase, while `-u` will convert them to uppercase.
 
 If neither of these arguments is provided, the original casing of the input MAC addresses will be preserved in the output.
 
 #### Uppercase
 In this example we convert a MAC address in Cisco format to the format Microsoft uses (with hyphens, in **uppercase**) by using the `-u` argument:
 ```bash
 macloot 1c1a.dfa1.b2c3 -O - -u
@@ -143,19 +143,19 @@
 To search for OUIs based on company names, you can utilize the `-s` or `--search` argument. By providing the desired company name as the argument value, such as "Cisco," "Apple," or "Microsoft," you can retrieve the corresponding OUIs associated with those companies. This feature enables easy lookup and identification of OUIs based on the names of specific organizations.
 
 ```bash
 macloot -s microsoft
 ```
 Output:
 ```bash
-70F8AE  Microsoft Corporation
-201642  Microsoft Corporation
-C461C7  Microsoft Corporation
-D8E2DF  Microsoft Corporation
-A085FC  Microsoft Corporation
+0003FF  Microsoft Corporation
+000D3A  Microsoft Corporation
+00125A  Microsoft Corporation
+00155D  Microsoft Corporation
+0017FA  Microsoft Corporation
 ... (output truncated) ...
 ```
 To make the output compatible with CSV format, you can use the `-d ";"` option here as well. 
 ## Update OUI database
 You can easily update the OUI database at any time by running the command: 
 ```bash
 macloot --update-db
```

### Comparing `macloot-1.0.0/macloot.py` & `macloot-1.1.0/macloot.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,21 +20,22 @@
     up-to-date information for accurate lookups.
 
 - Also: Why did the MAC address go on a diet? It wanted to shed a few colons!
 
 Let the MAC address mastery begin!
 """
 import argparse
+import csv
 import os
 import sys
 
 from dataclasses import dataclass
 from site import USER_BASE
 from oui import OuiDatabase
-from mac import MacAddress, MacAddressGenerator
+from mac import MacAddress, MacAddressGenerator, MacCase
 
 import app_info
 
 
 @dataclass
 class FormatArguments:
     """ Dataclass representing CLI arguments passed by the user. """
@@ -63,24 +64,25 @@
         formatter_class=argparse.RawTextHelpFormatter
     )
 
     # Transformation arguments
     transform_group = parser.add_argument_group('transformational arguments')
     transform_group.add_argument("-O", "--octet-separator", default=None, metavar='CHAR',
                         help="character to use between octets in output (default: keep original)")
-    transform_group.add_argument("-l", "--lower-case", action="store_true",
-                        help="output MAC addresses in lower case")
-    transform_group.add_argument("-u", "--upper-case", action="store_true",
-                        help="output MAC addresses in upper case")
+    transform_group.add_argument("-l", "--lowercase", action="store_true",
+                        help="output MAC addresses in lowercase")
+    transform_group.add_argument("-u", "--uppercase", action="store_true",
+                        help="output MAC addresses in uppercase")
 
     # Output arguments
     output_group = parser.add_argument_group('output arguments')
     output_group.add_argument("-d", "--delimiter", default=None, metavar='CHAR',
                         help="delimiting character to use between fields in output (default: TAB)")
-    output_group.add_argument("-o", "--output-file", metavar='FILE', help="write output to file")
+    output_group.add_argument("-o", "--outfile", default=os.devnull,
+                              metavar='FILE', help="write output to file")
     output_group.add_argument("-q", "--quiet", action="store_true",
                         help="suppress output to stdout")
     output_group.add_argument("-v", "--verbose", action="store_true",
                         help="include OUI information in output")
 
     # Generator arguments
     generator_group = parser.add_argument_group('generator arguments')
@@ -124,68 +126,51 @@
     else:
         # Read from file
         try:
             with open(input_string, 'r', encoding='utf-8') as file:
                 input_lines = file.readlines()
         except FileNotFoundError:
             input_lines = input_string
+        except OSError:
+            input_lines = input_string
     return input_lines
 
 def create_mac_addresses(mac_addresses_input: str, database: OuiDatabase,
-                         octet_separator: str = None) -> list:
+                         octet_separator: str = None,
+                         case: MacCase = MacCase.ORIGINAL) -> list:
     """ Create a list of MacAddress objects for every MAC address found in user input. """
 
     # Create one MacAddress instance for every MAC address in input
     mac_addresses = []
     for mac_address in mac_addresses_input:
-        mac = MacAddress(mac_address)
+        mac = MacAddress(mac_address, case)
         oui_entry = database.lookup(mac.address)
         if oui_entry:
-            mac.organization_name = oui_entry.organization_name
-            mac.organization_address = oui_entry.organization_address
+            mac.organization.name = oui_entry.organization.name
+            mac.organization.address = oui_entry.organization.address
 
         if octet_separator:
             mac.octet_separator = octet_separator
         mac_addresses.append(mac)
     return mac_addresses
 
-def print_mac_addresses(mac_addresses: list, delimiter: str = None, upper_case: bool = False,
-                        lower_case:bool = False, verbose: bool = False) -> None:
-    """ Print a list of MacAddress objects. """
-    for mac in mac_addresses:
-        delim = '\t' if delimiter is None else delimiter
-        if upper_case:
-            mac_address = mac.uppercase
-        elif lower_case:
-            mac_address = mac.lowercase
-        else:
-            mac_address = mac.address
-
-        if verbose:
-            print(f"{mac_address}{delim}{mac.organization_name}{delim}{mac.organization_address}")
-        else:
-            print(f"{mac_address}{delim}{mac.organization_name}")
+def export_list(item_list: list, delimiter: str = None, quiet: bool = False,
+                        verbose: bool = False, outfile: str = None) -> None:
+    """ Export a list of objects, implementing the to_list() method, to stdout and/or file. """
 
-def write_mac_addresses_to_file(mac_addresses: list, outfile: str, args: FormatArguments) -> None:
-    """ Write a list of MacAddress objects to file. """
+    # Export to file and stdout using '/dev/null' if no outfile is given
     with open(outfile, 'w', encoding='utf8') as file:
-        for mac in mac_addresses:
-            delim = '\t' if args.delimiter is None else args.delimiter
-            if args.upper:
-                mac_address = mac.uppercase
-            elif args.lower:
-                mac_address = mac.lowercase
-            else:
-                mac_address = mac.address
-
-            if args.verbose:
-                file.write(f"{mac_address}{delim}{mac.organization_name}" \
-                           f"{delim}{mac.organization_address}\n")
-            else:
-                file.write(f"{mac_address}{delim}{mac.organization_name}\n")
+        delim = '\t' if delimiter is None else delimiter
+        stdout_writer = csv.writer(sys.stdout, delimiter=delim)
+        file_writer   = csv.writer(file, delimiter=delim)
+        for item in item_list:
+            output = item.to_list(verbose=verbose)
+            if not quiet:
+                stdout_writer.writerow(output)
+            file_writer.writerow(output)
 
 def generate_addresses(args: list, database: str) -> None:
     """ Generate MAC addresses in various formats. """
 
     count = args.count
     count_max = 1024
     address_list = args.address_list
@@ -197,27 +182,35 @@
         sys.exit(1)
 
     macgen = MacAddressGenerator(database)
     output = None
 
     if address_list:
         output = macgen.generate_mac_address_list(num=count, octet_separator=args.octet_separator,
-                                                  upper=args.upper_case)
+                                                  case=parse_mac_case(args))
         print(output)
     elif example_tables:
         if example_tables == 'ios':
             output = macgen.generate_ios_output(count)
             print(output)
         elif example_tables == 'arubaos':
             output = macgen.generate_arubaos_output(count)
             print(output)
         else:
             output = macgen.generate_routeros_output(count)
             print(output)
 
+def parse_mac_case(args: list) -> MacCase:
+    """ Parse the argument list for -u and -l and returns the selectec character case. """
+    if args.uppercase:
+        return MacCase.UPPERCASE
+    if args.lowercase:
+        return MacCase.LOWERCASE
+    return MacCase.ORIGINAL
+
 def main():
     """ Entry point of the application. """
 
     # Initiate the OUI database
     csv_file = os.path.join(USER_BASE, f"share/{app_info.NAME}/oui.csv")
     oui_db = OuiDatabase(csv_file)
 
@@ -254,48 +247,42 @@
         sys.exit(0)
 
     # Check if the user is requesting a search
     if args.search:
         # Parse search input from stdin
         input_lines = args.INPUT
 
-        delim = '\t' if args.delimiter is None else args.delimiter
+        # Make sure search term is within length constraints
         if len(input_lines) < 3:
             print(f"{app_info.NAME}: error: argument -s/--search: search term " \
                   "must be 3 or more characters long.")
             sys.exit(1)
 
+        # Find all OuiEntry objects matching the user input
         oui_entries = oui_db.search(input_lines)
-        for entry in oui_entries:
-            try:
-                print(f"{entry.assignment}{delim}{entry.organization_name}")
-            except BrokenPipeError:
-                pass
+
+        # Export list of OuiEntry objects to stdout and/or file
+        export_list(item_list=oui_entries, delimiter=args.delimiter,
+                    quiet=args.quiet, verbose=args.verbose, outfile=args.outfile)
     else:
         # Parse input from a file or stdin
         input_lines = parse_input(args.INPUT)
 
         # Process input lines
         data_input = "".join(input_lines).strip()
 
         # Find all MAC addresses in the user input
         mac_list = MacAddress.extract_addresses(data_input)
 
         # Create a list of MacAddress instance objects
+        mac_case = parse_mac_case(args)
         mac_addresses = create_mac_addresses(mac_addresses_input=mac_list, database=oui_db,
-                                             octet_separator=args.octet_separator)
+                                             octet_separator=args.octet_separator, case=mac_case)
 
-        # Print the list of MacAddress objects
-        if not args.quiet:
-            print_mac_addresses(mac_addresses=mac_addresses, delimiter=args.delimiter,
-                                upper_case=args.upper_case, lower_case=args.lower_case,
-                                verbose=args.verbose)
-        if args.output_file:
-            arg_list = FormatArguments(delimiter=args.delimiter, upper=args.upper_case,
-                                       lower=args.lower_case, verbose=args.verbose)
-            write_mac_addresses_to_file(mac_addresses=mac_addresses, outfile=args.output_file,
-                                        args=arg_list)
+        # Export the list of MacAddress objects to stdout and/or file
+        export_list(item_list=mac_addresses, delimiter=args.delimiter,
+                    quiet=args.quiet, verbose=args.verbose, outfile=args.outfile)
 
     sys.exit(0)
 
 if __name__ == "__main__":
     main()
```

### Comparing `macloot-1.0.0/oui.py` & `macloot-1.1.0/oui.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,69 +26,90 @@
 For more information, refer to the documentation or visit the official IEEE OUI database website.
 """
 
 import csv
 import datetime
 import os
 import re
+
+from dataclasses import dataclass
+
 import requests
 
+
+@dataclass
+class OuiOrganization:
+    """ Class definition of an Organization (OUI). """
+    name: str
+    address: str
+
 class OuiEntry:
     """ Class definition of an OUI entry in the CSV database file. """
 
     def __init__(self, registry: str, assignment: str, \
                  organization_name: str, organization_address: str):
         """ Initialize an OuiEntry object with the provided fields. """
         self.__registry = registry
         self.__assignment = assignment
-        self.__organization_name = organization_name
-        self.__organization_address = organization_address
+        self.__organization= OuiOrganization(organization_name, organization_address)
 
     def __str__(self) -> str:
         """ Return a string representation of the OuiEntry. """
         return f"OuiEntry(registry='{self.registry}', assignment='{self.assignment}', " \
-               f"organization_name='{self.organization_name}', "\
-               f"organization_address='{self.organization_address}')"
+               f"organization_name='{self.organization.name}', "\
+               f"organization_address='{self.organization.address}')"
 
     def __repr__(self) -> str:
         """ Return a string representation of the OuiEntry for object re-creation. """
         return f"OuiEntry(registry='{self.registry}', assignment='{self.assignment}', " \
-               f"organization_name='{self.organization_name}', " \
-               f"organization_address='{self.organization_address}')"
+               f"organization_name='{self.organization.name}', " \
+               f"organization_address='{self.organization.address}')"
 
     def __eq__(self, other):
         """ Compare two OuiEntry objects for equality. """
         if isinstance(other, OuiEntry):
             return (
                 self.__registry == other.registry and
                 self.__assignment == other.assignment and
-                self.__organization_name == other.organization_name and
-                self.__organization_address == other.organization_address
+                self.__organization.name == other.organization.name and
+                self.__organization.address == other.organization.address
             )
         return False
 
+    def __lt__(self, other):
+        """ Check if this OuiEntry is 'less than' another OuiEntry object. """
+        if isinstance(other, OuiEntry):
+            return self.to_int() < other.to_int()
+        return False
+
+    def to_int(self):
+        """ Convert the OuiEntry Assignment (OUI) into an integer representation. """
+        return int(self.__assignment, 16)
+
+    def to_list(self, verbose: bool = False) -> list:
+        """ Return a subset or all printable properties of the OuiEntry class as a list. """
+        if verbose:
+            return [str(self.__registry), str(self.__assignment),
+                    str(self.__organization.name), str(self.__organization.address)]
+        return [str(self.__assignment), str(self.__organization.name)]
+
     @property
     def registry(self) -> str:
         """ Get the registry field of the OuiEntry. """
         return self.__registry
 
     @property
     def assignment(self) -> str:
         """ Get the assignment field of the OuiEntry. """
         return self.__assignment
 
     @property
-    def organization_name(self) -> str:
-        """ Get the organization name field of the OuiEntry. """
-        return self.__organization_name
-
-    @property
-    def organization_address(self) -> str:
-        """ Get the organization address field of the OuiEntry. """
-        return self.__organization_address
+    def organization(self) -> str:
+        """ Get the organization object of the OuiEntry. """
+        return self.__organization
 
 
 class OuiDatabase:
     """ Class definition of the OUI database. """
 
     def __init__(self, database_file: str) -> None:
         """ Constructor method for the OuiDatabase class. """
@@ -125,24 +146,27 @@
 
         # Look for an OUI entry matching the assignment ID (OUI)
         for entry in self.__oui_entries:
             if entry.assignment == assignment:
                 return entry
         return None
 
-    def search(self, organization_name: str) -> list:
+    def search(self, query: str, sort: bool = True) -> list:
         """ Search for OUIs belonging to an organization. """
 
         # List of resulting OuiEntry objects
         results = []
 
         # Look for an OUI entry matching the assignment ID (OUI)
         for entry in self.__oui_entries:
-            if organization_name.lower() in entry.organization_name.lower():
+            query = query.lower()
+            if query in entry.organization.name.lower() or query in entry.assignment.lower():
                 results.append(entry)
+        if sort:
+            results.sort()
         return results
 
     def get_entries(self) -> list:
         """ Get the list of OuiEntry items read from the database file. """
         return self.__oui_entries
 
     def update_database(self, force_update = False) -> bool:
```

### Comparing `macloot-1.0.0/setup.py` & `macloot-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `macloot-1.0.0/test/test_mac.py` & `macloot-1.1.0/test/test_mac.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Unit Testing Script for mac.py module. """
 import os
 import unittest
 
 from test_oui import OuiDatabaseTestCase
-from mac import MacAddress, MacAddressGenerator
+from mac import MacAddress, MacAddressGenerator, MacCase
 from oui import OuiDatabase
 
 
 class MacAddressTestCase(unittest.TestCase):
     """ Test cases testing the parsing capabilities of MAC addresses. """
     def test_format_mac_address(self):
         """ Test the formatting capabilitites of the format_mac_address() method. """
@@ -136,50 +136,50 @@
         self.assertEqual(result1, expected_oui1)
         self.assertEqual(result2, expected_oui2)
         self.assertEqual(result3, expected_oui3)
         self.assertEqual(result4, expected_oui4)
 
     def test_lowercase_property(self):
         """ Test the MacAddress lowercase property. """
-        mac_address1 = MacAddress('00:11:22:33:44:55')
-        mac_address2 = MacAddress('AA-BB-CC-DD-EE-FF')
-        mac_address3 = MacAddress('AaBbCcDdEeFf')
-        mac_address4 = MacAddress('a1b2.c3d4.e5f6')
+        mac_address1 = MacAddress('00:11:22:33:44:55',  case=MacCase.LOWERCASE)
+        mac_address2 = MacAddress('AA-BB-CC-DD-EE-FF',  case=MacCase.LOWERCASE)
+        mac_address3 = MacAddress('AaBbCcDdEeFf',       case=MacCase.LOWERCASE)
+        mac_address4 = MacAddress('a1b2.c3d4.e5f6',     case=MacCase.LOWERCASE)
 
         expected_lower1 = '00:11:22:33:44:55'
         expected_lower2 = 'aa-bb-cc-dd-ee-ff'
         expected_lower3 = 'aabbccddeeff'
         expected_lower4 = 'a1b2.c3d4.e5f6'
 
-        result1 = mac_address1.lowercase
-        result2 = mac_address2.lowercase
-        result3 = mac_address3.lowercase
-        result4 = mac_address4.lowercase
+        result1 = mac_address1.address
+        result2 = mac_address2.address
+        result3 = mac_address3.address
+        result4 = mac_address4.address
 
         self.assertEqual(result1, expected_lower1)
         self.assertEqual(result2, expected_lower2)
         self.assertEqual(result3, expected_lower3)
         self.assertEqual(result4, expected_lower4)
 
     def test_uppercase_property(self):
         """ Test the MacAddress uppercase property. """
-        mac_address1 = MacAddress('00:11:22:33:44:55')
-        mac_address2 = MacAddress('AA-BB-CC-DD-EE-FF')
-        mac_address3 = MacAddress('AaBbCcDdEeFf')
-        mac_address4 = MacAddress('a1b2.c3d4.e5f6')
+        mac_address1 = MacAddress('00:11:22:33:44:55',  case=MacCase.UPPERCASE)
+        mac_address2 = MacAddress('AA-BB-CC-DD-EE-FF',  case=MacCase.UPPERCASE)
+        mac_address3 = MacAddress('AaBbCcDdEeFf',       case=MacCase.UPPERCASE)
+        mac_address4 = MacAddress('a1b2.c3d4.e5f6',     case=MacCase.UPPERCASE)
 
         expected_upper1 = '00:11:22:33:44:55'
         expected_upper2 = 'AA-BB-CC-DD-EE-FF'
         expected_upper3 = 'AABBCCDDEEFF'
         expected_upper4 = 'A1B2.C3D4.E5F6'
 
-        result1 = mac_address1.uppercase
-        result2 = mac_address2.uppercase
-        result3 = mac_address3.uppercase
-        result4 = mac_address4.uppercase
+        result1 = mac_address1.address
+        result2 = mac_address2.address
+        result3 = mac_address3.address
+        result4 = mac_address4.address
 
         self.assertEqual(result1, expected_upper1)
         self.assertEqual(result2, expected_upper2)
         self.assertEqual(result3, expected_upper3)
         self.assertEqual(result4, expected_upper4)
 
     def test_octet_separator_property(self):
@@ -204,36 +204,36 @@
         self.assertEqual(result4, expected_separator4)
 
     def test_organization_name_property(self):
         """ Test the MacAddress organization name property. """
         mac_address = MacAddress('00:11:22:33:44:55')
         expected_name = 'Organization Name'
 
-        result = mac_address.organization_name
+        result = mac_address.organization.name
 
         self.assertIsNone(result)
 
-        mac_address.organization_name = expected_name
+        mac_address.organization.name = expected_name
 
-        result = mac_address.organization_name
+        result = mac_address.organization.name
 
         self.assertEqual(result, expected_name)
 
     def test_organization_address_property(self):
         """ Test the MacAddress organization address property. """
         mac_address = MacAddress('00:11:22:33:44:55')
         expected_address = 'Organization Address'
 
-        result = mac_address.organization_address
+        result = mac_address.organization.address
 
         self.assertIsNone(result)
 
-        mac_address.organization_address = expected_address
+        mac_address.organization.address = expected_address
 
-        result = mac_address.organization_address
+        result = mac_address.organization.address
 
         self.assertEqual(result, expected_address)
 
 
 class TestMacAddressGenerator(unittest.TestCase):
     """ Test cases testing the generating capabilities of the MacAddressGenerator class. """
     def setUp(self):
@@ -254,13 +254,13 @@
         mac_address = self.generator.generate_mac_address()
         self.assertIsInstance(mac_address, MacAddress)
 
     def test_generate_mac_address_list(self):
         """ Test the MAC address list generator method. """
         num = 5
         octet_separator = '-'
-        upper = True
-        mac_list = self.generator.generate_mac_address_list(num, octet_separator, upper)
+        case = MacCase.UPPERCASE
+        mac_list = self.generator.generate_mac_address_list(num, octet_separator, case)
         mac_addresses = mac_list.split('\n')
         self.assertEqual(len(mac_addresses), num)
         for mac_address in mac_addresses:
             self.assertEqual(mac_address, mac_address.upper())
```

### Comparing `macloot-1.0.0/test/test_oui.py` & `macloot-1.1.0/test/test_oui.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,16 +80,16 @@
         loaded_entries = oui_db.get_entries()
 
         # Assert that the loaded entries match the expected entries
         self.assertEqual(len(loaded_entries), len(expected_entries))
         for loaded_entry, expected_entry in zip(loaded_entries, expected_entries):
             self.assertEqual(loaded_entry.registry, expected_entry.registry)
             self.assertEqual(loaded_entry.assignment, expected_entry.assignment)
-            self.assertEqual(loaded_entry.organization_name, expected_entry.organization_name)
-            self.assertEqual(loaded_entry.organization_address, expected_entry.organization_address)
+            self.assertEqual(loaded_entry.organization.name, expected_entry.organization.name)
+            self.assertEqual(loaded_entry.organization.address, expected_entry.organization.address)
 
     def test_lookup_existing_mac(self):
         """ Test the database lookup using an existing MAC address. """
 
         # Setup the database instance
         oui_db = OuiDatabase(self.temp_file_path)
         oui_db.load_database()
@@ -127,18 +127,18 @@
         # Setup the database instance
         oui_db = OuiDatabase(self.temp_file_path)
         oui_db.load_database()
 
         # Test for an existing organization
         organization_name = 'Semsung Electronics Co.,Ltd'
         expected_results = [
-            OuiEntry(registry='MA-L', assignment='A1A1A1',
+            OuiEntry(registry='MA-L', assignment='123456',
                      organization_name='Semsung Electronics Co.,Ltd',
                      organization_address='#83-1, Imtoo-Long Gummi Gyeongbook'),
-            OuiEntry(registry='MA-L', assignment='123456',
+            OuiEntry(registry='MA-L', assignment='A1A1A1',
                      organization_name='Semsung Electronics Co.,Ltd',
                      organization_address='#83-1, Imtoo-Long Gummi Gyeongbook')
         ]
 
         # Perform the search
         results = oui_db.search(organization_name)
```

