# Comparing `tmp/fixie-proto-0.1.0.tar.gz` & `tmp/fixie-proto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixie-proto-0.1.0.tar", max compression
+gzip compressed data, was "fixie-proto-0.1.1.tar", max compression
```

## Comparing `fixie-proto-0.1.0.tar` & `fixie-proto-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      727 2023-07-20 00:17:30.813317 fixie-proto-0.1.0/README.md
--rw-r--r--   0        0        0      328 2023-07-19 22:36:00.207003 fixie-proto-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 fixie-proto-0.1.0/setup.py
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 fixie-proto-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2460 2023-07-20 16:55:13.038944 fixie-proto-0.1.1/README.md
+-rw-r--r--   0        0        0      333 2023-07-20 17:56:29.824895 fixie-proto-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 fixie-proto-0.1.1/setup.py
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 fixie-proto-0.1.1/PKG-INFO
```

### Comparing `fixie-proto-0.1.0/setup.py` & `fixie-proto-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['python']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['protobuf>=4.23.4,<5.0.0']
+['protobuf>=4.21.1,<5']
 
 setup_kwargs = {
     'name': 'fixie-proto',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '# fixie-proto\nRepository containing protos. The intention is for this to define our public-facing APIs. Tooling in this repository should then make it easy to use the *already compiled* protos in various languages.\n\nFor languages supported by the Buf Schema Registry, instructions for adding these protos like a normal dependency can be found [here](https://buf.build/fixie-ai/fixie/assets/main).  For example, to add a TypeScript dependency using yarn:\n\n```\nyarn config set npmScopes.buf.npmRegistryServer https://buf.build/gen/npm/v1/\nyarn add @buf/fixie-ai_fixie.bufbuild_connect-es@latest\n```\n\nWe also support additional languages (albeit with fewer options) directly. In particular, Python is available via pip: [PyPI]().\n',
+    'long_description': "# fixie-proto\nThis repository contains protocol buffer definitions for working with the Fixie platform. The intention is for this to define our public-facing APIs. Tooling in this repository should then make it easy to use the *already compiled* protos in various languages.\n\n## Buf Schema Registry (BSR)\n\nFor languages supported by the Buf Schema Registry, instructions for adding these protos like a normal dependency can be found [here](https://buf.build/fixie-ai/fixie/assets/main).  For example, to add a TypeScript dependency using yarn:\n\n```\nyarn config set npmScopes.buf.npmRegistryServer https://buf.build/gen/npm/v1/\nyarn add @buf/fixie-ai_fixie.bufbuild_connect-es@latest\n```\n\nAs of July 2023, BSR has support for JavaScript/Typscript, Go, JVM-based languages like Java and Kotlin, and Swift.\n\n## Directly supported languages\n\nWe also support additional languages (albeit with fewer options) directly. In particular, Python is available via pip: [PyPI](https://pypi.org/project/fixie-proto/).\n\n```\npip install fixie-proto\n```\n\n## Including Fixie protos in a proto library\n\nThe easiest way to depend on Fixie protos for your own proto library is by building with [Buf](https://buf.build/docs/introduction/) and adding `buf.build/fixie-ai/fixie` as a dependency in your buf.yaml.\n\nIf you're using protoc instead, consider including this repository as a submodule in your own repository.\n\n\n## Other languages\n\nBuf can be used to easily compile our protos in other languages too, including: Ruby, Objective-C, PHP, C#, Scala, C++, Dart, and Rust.  You'll need to create a [buf.gen.yaml file](https://buf.build/docs/generate/overview/) that uses the relevant protoc plugin for your language. You can also define language-specific proto options without modifying the proto files themselves using [managed mode](https://buf.build/docs/generate/managed-mode/#managed). You can then compile the protos in your language of choice by running:\n\n```\nbuf generate --template buf.gen.yaml buf.build/fixie-ai/fixie\n```\n\nIf you'd prefer to use protoc, see the advice above about including Fixie protos in your own proto library.\n\n## Using JSON instead\n\nIf you'd prefer not to deal with protos, we've got you covered! All of our APIs can accept and return JSON instead. Just set your Content-Type header to `application/json` instead of `application/proto`.\n\n<!-- TODO(mdepinet): Figure out how/where to publish the generated OpenAPI and then link to that here. -->\n\n",
     'author': 'Fixie.ai Team',
     'author_email': 'founders@fixie.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

