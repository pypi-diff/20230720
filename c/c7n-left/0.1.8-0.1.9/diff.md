# Comparing `tmp/c7n_left-0.1.8-py3-none-any.whl.zip` & `tmp/c7n_left-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 19618 bytes, number of entries: 15
--rw-r--r--  2.0 unx     2977 b- defN 80-Jan-01 00:00 c7n_left/cli.py
--rw-r--r--  2.0 unx    11560 b- defN 80-Jan-01 00:00 c7n_left/core.py
+Zip file size: 19570 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     2959 b- defN 80-Jan-01 00:00 c7n_left/cli.py
+-rw-r--r--  2.0 unx    11484 b- defN 80-Jan-01 00:00 c7n_left/core.py
 -rw-r--r--  2.0 unx      142 b- defN 80-Jan-01 00:00 c7n_left/entry.py
--rw-r--r--  2.0 unx     4315 b- defN 80-Jan-01 00:00 c7n_left/filters.py
--rw-r--r--  2.0 unx    11824 b- defN 80-Jan-01 00:00 c7n_left/output.py
+-rw-r--r--  2.0 unx     4277 b- defN 80-Jan-01 00:00 c7n_left/filters.py
+-rw-r--r--  2.0 unx    11714 b- defN 80-Jan-01 00:00 c7n_left/output.py
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/__init__.py
 -rw-r--r--  2.0 unx     3282 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/graph.py
--rw-r--r--  2.0 unx     1552 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/provider.py
+-rw-r--r--  2.0 unx     1530 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/provider.py
 -rw-r--r--  2.0 unx      945 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/resource.py
--rw-r--r--  2.0 unx     7208 b- defN 80-Jan-01 00:00 c7n_left/test.py
+-rw-r--r--  2.0 unx     7178 b- defN 80-Jan-01 00:00 c7n_left/test.py
 -rw-r--r--  2.0 unx      732 b- defN 80-Jan-01 00:00 c7n_left/utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_left-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 c7n_left-0.1.8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    12065 b- defN 16-Jan-01 00:00 c7n_left-0.1.8.dist-info/METADATA
-?rw-------  2.0 unx     1206 b- defN 23-May-25 11:15 c7n_left-0.1.8.dist-info/RECORD
-15 files, 58062 bytes uncompressed, 17636 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_left-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 c7n_left-0.1.9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12065 b- defN 16-Jan-01 00:00 c7n_left-0.1.9.dist-info/METADATA
+?rw-------  2.0 unx     1206 b- defN 23-Jun-28 08:38 c7n_left-0.1.9.dist-info/RECORD
+15 files, 57768 bytes uncompressed, 17588 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: c7n_left/test.py
 Comment: 
 
 Filename: c7n_left/utils.py
 Comment: 
 
-Filename: c7n_left-0.1.8.dist-info/WHEEL
+Filename: c7n_left-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_left-0.1.8.dist-info/entry_points.txt
+Filename: c7n_left-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_left-0.1.8.dist-info/METADATA
+Filename: c7n_left-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_left-0.1.8.dist-info/RECORD
+Filename: c7n_left-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## c7n_left/cli.py

```diff
@@ -23,26 +23,22 @@
     """Shift Left Policy"""
     logging.basicConfig(level=logging.INFO)
     initialize_iac()
 
 
 @cli.command()
 @click.option("--format", default="terraform")
-@click.option(
-    "--filters", help="filter policies or resources as k=v pairs with globbing"
-)
+@click.option("--filters", help="filter policies or resources as k=v pairs with globbing")
 @click.option("-p", "--policy-dir", type=click.Path())
 @click.option("-d", "--directory", type=click.Path())
 @click.option("-o", "--output", default="cli", type=click.Choice(report_outputs.keys()))
 @click.option("--output-file", type=click.File("w"), default="-")
 @click.option("--output-query", default=None)
 @click.option("--summary", default="policy", type=click.Choice(summary_options.keys()))
-def run(
-    format, policy_dir, directory, output, output_file, output_query, summary, filters
-):
+def run(format, policy_dir, directory, output, output_file, output_query, summary, filters):
     """evaluate policies against IaC sources.
 
     c7n-left -p policy_dir -d terraform_root --filters "severity=HIGH"
 
 
     WARNING - CLI interface subject to change.
     """
@@ -64,17 +60,15 @@
     reporter = get_reporter(config)
     runner = CollectionRunner(policies, config, reporter)
     sys.exit(int(runner.run()))
 
 
 @cli.command()
 @click.option("-p", "--policy-dir", type=click.Path(), required=True)
-@click.option(
-    "--filters", help="filter policies or resources as k=v pairs with globbing"
-)
+@click.option("--filters", help="filter policies or resources as k=v pairs with globbing")
 def test(policy_dir, filters):
     """Run policy tests."""
     policy_dir = Path(policy_dir)
     source_dir = policy_dir / "tests"
 
     config = Config.empty(
         source_dir=source_dir,
```

## c7n_left/core.py

```diff
@@ -58,17 +58,15 @@
         return " ".join(self.categories)
 
     @property
     def categories(self):
         categories = self.policy.data.get("metadata", {}).get("category", [])
         if isinstance(categories, str):
             categories = [categories]
-        if not isinstance(categories, list) or (
-            categories and not isinstance(categories[0], str)
-        ):
+        if not isinstance(categories, list) or (categories and not isinstance(categories[0], str)):
             categories = []
         return categories
 
     @property
     def severity(self):
         value = self.policy.data.get("metadata", {}).get("severity", "")
         if isinstance(value, str):
@@ -126,25 +124,21 @@
 
     @classmethod
     def _validate_severities(cls, filters):
         invalid_severities = set()
         if filters["severity"]:
             invalid_severities = set(filters["severity"]).difference(SEVERITY_LEVELS)
         if invalid_severities:
-            raise ValueError(
-                "invalid severity for filtering %s" % (", ".join(invalid_severities))
-            )
+            raise ValueError("invalid severity for filtering %s" % (", ".join(invalid_severities)))
 
     def filter_attribute(self, filter_name, attribute, items):
         if not self.filters[filter_name] or not items:
             return items
         results = []
-        op_class = (
-            isinstance(items[0], dict) and operator.itemgetter or operator.attrgetter
-        )
+        op_class = isinstance(items[0], dict) and operator.itemgetter or operator.attrgetter
         op = op_class(attribute)
         for f in self.filters[filter_name]:
             for i in items:
                 v = op(i)
                 if not v:
                     continue
                 elif isinstance(v, list):
```

## c7n_left/filters.py

```diff
@@ -84,17 +84,15 @@
         return type_chain
 
     def process(self, resources, event):
         results = []
         for r in resources:
             working_set = (r,)
             for target_type in self.type_chain:
-                working_set = self.resolve_refs(
-                    target_type, working_set, event["graph"]
-                )
+                working_set = self.resolve_refs(target_type, working_set, event["graph"])
             matched = self.match_attrs(working_set)
             if not self.match_cardinality(matched):
                 continue
             if matched:
                 r[self.annotation_key] = matched
             results.append(r)
         return results
```

## c7n_left/output.py

```diff
@@ -45,26 +45,23 @@
     def __init__(self, ctx, config):
         super().__init__(ctx, config)
         self.console = Console(file=config.output_file)
         self.started = None
         self.matches = 0
 
     def on_execution_started(self, policies, graph):
-        self.console.print(
-            "Running %d policies on %d resources" % (len(policies), len(graph))
-        )
+        self.console.print("Running %d policies on %d resources" % (len(policies), len(graph)))
         self.started = time.time()
 
     def on_execution_ended(self):
         message = "[green]Success[green]"
         if self.matches:
             message = "[red]%d Failures[/red]" % self.matches
         self.console.print(
-            "Evaluation complete %0.2f seconds -> %s"
-            % (time.time() - self.started, message)
+            "Evaluation complete %0.2f seconds -> %s" % (time.time() - self.started, message)
         )
 
     def on_results(self, results):
         for r in results:
             self.console.print(RichResult(r))
         self.matches += len(results)
 
@@ -144,17 +141,15 @@
         unevaluated = sum(
             [
                 v
                 for k, v in self.counter_unevaluated_by_type.items()
                 if k not in set(self.counter_policies_by_type)
             ]
         )
-        compliant = (
-            self.count_total_resources - len(self.resource_name_matches) - unevaluated
-        )
+        compliant = self.count_total_resources - len(self.resource_name_matches) - unevaluated
         msg = "%d compliant of %d total" % (compliant, self.count_total_resources)
         if self.resource_name_matches:
             msg += ", %d resources have %d policy violations" % (
                 len(self.resource_name_matches),
                 self.count_policy_matches,
             )
 
@@ -230,17 +225,15 @@
     def __init__(self, ctx, config):
         super().__init__(ctx, config)
         self.policies = {}
         self.resource_policy_matches = {}
 
     def on_execution_started(self, policies, graph):
         super().on_execution_started(policies, graph)
-        self.policies = {
-            p.name: p for p in sorted(map(PolicyMetadata, policies), key=severity_key)
-        }
+        self.policies = {p.name: p for p in sorted(map(PolicyMetadata, policies), key=severity_key)}
 
     def on_results(self, results):
         super().on_results(results)
         for r in results:
             self.resource_policy_matches.setdefault(r.resource.name, []).append(r)
 
     def on_execution_ended(self):
@@ -352,17 +345,15 @@
 
     def on_results(self, results):
         self.results.extend(results)
 
     def on_execution_ended(self):
         formatted_results = [self.format_result(r) for r in self.results]
         if self.config.output_query:
-            formatted_results = jmespath_search(
-                self.config.output_query, formatted_results
-            )
+            formatted_results = jmespath_search(self.config.output_query, formatted_results)
         self.config.output_file.write(
             json.dumps({"results": formatted_results}, cls=JSONEncoder, indent=2)
         )
 
     def format_result(self, result):
         resource = result.resource
```

## c7n_left/providers/terraform/provider.py

```diff
@@ -39,17 +39,15 @@
 
     def initialize_policies(self, policies, options):
         for p in policies:
             p.data["mode"] = {"type": "terraform-source"}
         return policies
 
     def parse(self, source_dir):
-        graph = TerraformGraph(
-            load_from_path(source_dir, allow_downloads=True), source_dir
-        )
+        graph = TerraformGraph(load_from_path(source_dir, allow_downloads=True), source_dir)
         graph.build()
         log.debug("Loaded %d %s resources", len(graph), self.type)
         return graph
 
     def match_dir(self, source_dir):
         files = list(source_dir.glob("*.tf"))
         files += list(source_dir.glob("*.tf.json"))
```

## c7n_left/test.py

```diff
@@ -120,17 +120,15 @@
             "unused": [t for idx, t in enumerate(self.data) if idx not in self.used],
         }
 
     def initialize_matchers(self):
         cfg = Config.empty(session_factory=None, tracer=NullTracer(None), options=None)
         matchers = []
         for match_block in self.data:
-            matcher = DataMatcher(
-                cfg, {"filters": [{k: v} for k, v in match_block.items()]}
-            )
+            matcher = DataMatcher(cfg, {"filters": [{k: v} for k, v in match_block.items()]})
             for i in matcher.iter_filters():
                 i.annotate = False
             matchers.append(matcher)
         self.matchers = matchers
 
     def match(self, result):
         found = False
```

## Comparing `c7n_left-0.1.8.dist-info/METADATA` & `c7n_left-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c7n-left
-Version: 0.1.8
+Version: 0.1.9
 Summary: Custodian policies for IAAC definitions
 Home-page: https://cloudcustodian.io
 License: Apache-2
 Author: Cloud Custodian Project
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
@@ -12,33 +12,33 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: c7n (==0.9.27) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: c7n (==0.9.28) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: click (==8.1.3) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: rich (==13.3.5) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: rich (==13.4.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: tfparse (==0.5.0) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: argcomplete (==3.0.8) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: boto3 (==1.26.139) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: argcomplete (==3.1.1) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: boto3 (==1.26.157) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: docutils (==0.18.1) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: importlib-metadata (==5.2.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: jsonschema (==4.17.3) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: python-dateutil (==2.8.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pyyaml (==6.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: tabulate (==0.9.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: urllib3 (==1.26.16) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: colorama (==0.4.6) ; python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
 Requires-Dist: markdown-it-py (==2.2.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pygments (==2.15.1) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: typing-extensions (==4.6.1) ; python_version >= "3.7" and python_version < "3.9"
+Requires-Dist: typing-extensions (==4.6.3) ; python_version >= "3.7" and python_version < "3.9"
 Requires-Dist: cffi (==1.15.1) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: botocore (==1.29.139) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: botocore (==1.29.157) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: jmespath (==1.0.1) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: s3transfer (==0.6.1) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: zipp (==3.15.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: attrs (==23.1.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: importlib-resources (==5.12.0) ; python_version >= "3.7" and python_version < "3.9"
 Requires-Dist: pkgutil-resolve-name (==1.3.10) ; python_version >= "3.7" and python_version < "3.9"
 Requires-Dist: pyrsistent (==0.19.3) ; python_version >= "3.7" and python_version < "4.0"
```

