# Comparing `tmp/dbt_copilot_tools-0.1.7.tar.gz` & `tmp/dbt_copilot_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_tools-0.1.7.tar", max compression
+gzip compressed data, was "dbt_copilot_tools-0.1.8.tar", max compression
```

## Comparing `dbt_copilot_tools-0.1.7.tar` & `dbt_copilot_tools-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.7/LICENSE
--rw-r--r--   0        0        0    12476 2023-07-19 16:03:49.302241 dbt_copilot_tools-0.1.7/commands/COMMANDS.md
--rw-r--r--   0        0        0     1737 2023-06-27 16:14:10.422751 dbt_copilot_tools-0.1.7/commands/README.md
--rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.7/commands/__init__.py
--rwxr-xr-x   0        0        0     9834 2023-06-30 15:36:41.153299 dbt_copilot_tools-0.1.7/commands/bootstrap_cli.py
--rwxr-xr-x   0        0        0     2563 2023-07-14 15:07:33.244634 dbt_copilot_tools-0.1.7/commands/check_cloudformation.py
--rwxr-xr-x   0        0        0    13567 2023-07-19 15:44:35.418970 dbt_copilot_tools-0.1.7/commands/codebuild_cli.py
--rwxr-xr-x   0        0        0     6991 2023-06-28 16:19:20.994539 dbt_copilot_tools-0.1.7/commands/copilot_cli.py
--rwxr-xr-x   0        0        0    20986 2023-07-14 15:07:33.244923 dbt_copilot_tools-0.1.7/commands/dns_cli.py
--rw-r--r--   0        0        0     1081 2023-07-19 15:42:25.200193 dbt_copilot_tools-0.1.7/commands/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      412 2023-07-19 15:42:25.200367 dbt_copilot_tools-0.1.7/commands/templates/addons/README.md
--rw-r--r--   0        0        0      529 2023-07-19 15:42:25.200528 dbt_copilot_tools-0.1.7/commands/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0     6148 2023-07-19 15:42:25.200665 dbt_copilot_tools-0.1.7/commands/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     8690 2023-07-19 15:42:25.200830 dbt_copilot_tools-0.1.7/commands/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0     4612 2023-07-19 15:42:25.200972 dbt_copilot_tools-0.1.7/commands/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     4062 2023-07-19 15:42:25.201064 dbt_copilot_tools-0.1.7/commands/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     2168 2023-07-19 15:42:25.201210 dbt_copilot_tools-0.1.7/commands/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     1778 2023-07-19 15:42:25.201386 dbt_copilot_tools-0.1.7/commands/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0     1836 2023-07-19 15:42:25.201495 dbt_copilot_tools-0.1.7/commands/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2023-07-19 15:42:25.201570 dbt_copilot_tools-0.1.7/commands/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2023-07-19 15:42:25.201676 dbt_copilot_tools-0.1.7/commands/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      728 2023-07-19 15:42:25.201841 dbt_copilot_tools-0.1.7/commands/templates/env/manifest.yml
--rw-r--r--   0        0        0     2721 2023-07-19 15:42:25.201945 dbt_copilot_tools-0.1.7/commands/templates/instructions.txt
--rw-r--r--   0        0        0      610 2023-07-19 15:42:25.202051 dbt_copilot_tools-0.1.7/commands/templates/storage-instructions.txt
--rw-r--r--   0        0        0     1852 2023-07-19 15:42:25.202226 dbt_copilot_tools-0.1.7/commands/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3119 2023-07-19 15:42:25.202376 dbt_copilot_tools-0.1.7/commands/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0     5894 2023-07-19 15:45:04.448343 dbt_copilot_tools-0.1.7/commands/utils.py
--rw-r--r--   0        0        0     6007 2023-07-14 15:07:33.245135 dbt_copilot_tools-0.1.7/commands/waf_cli.py
--rwxr-xr-x   0        0        0      970 2023-06-28 12:16:25.470546 dbt_copilot_tools-0.1.7/copilot_helper.py
--rw-r--r--   0        0        0     1102 2023-07-19 15:55:33.669207 dbt_copilot_tools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.8/LICENSE
+-rw-r--r--   0        0        0    12476 2023-07-20 14:40:32.289038 dbt_copilot_tools-0.1.8/commands/COMMANDS.md
+-rw-r--r--   0        0        0     1737 2023-06-27 16:14:10.422751 dbt_copilot_tools-0.1.8/commands/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.8/commands/__init__.py
+-rwxr-xr-x   0        0        0     9834 2023-06-30 15:36:41.153299 dbt_copilot_tools-0.1.8/commands/bootstrap_cli.py
+-rwxr-xr-x   0        0        0     2563 2023-07-14 15:07:33.244634 dbt_copilot_tools-0.1.8/commands/check_cloudformation.py
+-rwxr-xr-x   0        0        0    13567 2023-07-20 11:58:54.500816 dbt_copilot_tools-0.1.8/commands/codebuild_cli.py
+-rwxr-xr-x   0        0        0     7006 2023-07-20 14:52:58.636758 dbt_copilot_tools-0.1.8/commands/copilot_cli.py
+-rw-r--r--   0        0        0      221 2023-07-20 14:52:58.637154 dbt_copilot_tools-0.1.8/commands/default-storage.yml
+-rwxr-xr-x   0        0        0    20986 2023-07-14 15:07:33.244923 dbt_copilot_tools-0.1.8/commands/dns_cli.py
+-rw-r--r--   0        0        0    10705 2023-07-20 14:52:58.637346 dbt_copilot_tools-0.1.8/commands/schemas/storage-schema.json
+-rw-r--r--   0        0        0     4141 2023-07-20 14:52:58.638060 dbt_copilot_tools-0.1.8/commands/storage-plans.yml
+-rw-r--r--   0        0        0     1081 2023-07-20 11:58:54.501083 dbt_copilot_tools-0.1.8/commands/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      412 2023-07-20 11:58:54.501306 dbt_copilot_tools-0.1.8/commands/templates/addons/README.md
+-rw-r--r--   0        0        0      529 2023-07-20 14:52:58.638828 dbt_copilot_tools-0.1.8/commands/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0     6148 2023-07-20 11:58:54.501686 dbt_copilot_tools-0.1.8/commands/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     8690 2023-07-20 14:52:58.639317 dbt_copilot_tools-0.1.8/commands/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0     4622 2023-07-20 13:18:17.158455 dbt_copilot_tools-0.1.8/commands/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     4062 2023-07-20 11:58:54.502157 dbt_copilot_tools-0.1.8/commands/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     3945 2023-07-20 13:18:17.158705 dbt_copilot_tools-0.1.8/commands/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     1778 2023-07-20 11:58:54.502526 dbt_copilot_tools-0.1.8/commands/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0     1836 2023-07-20 11:58:54.502669 dbt_copilot_tools-0.1.8/commands/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2023-07-20 11:58:54.502781 dbt_copilot_tools-0.1.8/commands/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2023-07-20 11:58:54.502929 dbt_copilot_tools-0.1.8/commands/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      728 2023-07-20 14:52:58.639746 dbt_copilot_tools-0.1.8/commands/templates/env/manifest.yml
+-rw-r--r--   0        0        0     2721 2023-07-20 11:58:54.503273 dbt_copilot_tools-0.1.8/commands/templates/instructions.txt
+-rw-r--r--   0        0        0      610 2023-07-20 11:58:54.503399 dbt_copilot_tools-0.1.8/commands/templates/storage-instructions.txt
+-rw-r--r--   0        0        0     1848 2023-07-20 13:18:17.159484 dbt_copilot_tools-0.1.8/commands/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3115 2023-07-20 13:18:17.159767 dbt_copilot_tools-0.1.8/commands/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0     5894 2023-07-20 11:58:54.504032 dbt_copilot_tools-0.1.8/commands/utils.py
+-rw-r--r--   0        0        0     6007 2023-07-14 15:07:33.245135 dbt_copilot_tools-0.1.8/commands/waf_cli.py
+-rwxr-xr-x   0        0        0      970 2023-06-28 12:16:25.470546 dbt_copilot_tools-0.1.8/copilot_helper.py
+-rw-r--r--   0        0        0     1102 2023-07-20 14:52:58.640166 dbt_copilot_tools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2830 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.8/PKG-INFO
```

### Comparing `dbt_copilot_tools-0.1.7/LICENSE` & `dbt_copilot_tools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/COMMANDS.md` & `dbt_copilot_tools-0.1.8/commands/COMMANDS.md`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/README.md` & `dbt_copilot_tools-0.1.8/commands/README.md`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/bootstrap_cli.py` & `dbt_copilot_tools-0.1.8/commands/bootstrap_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/check_cloudformation.py` & `dbt_copilot_tools-0.1.8/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/codebuild_cli.py` & `dbt_copilot_tools-0.1.8/commands/codebuild_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/copilot_cli.py` & `dbt_copilot_tools-0.1.8/commands/copilot_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .utils import SSM_BASE_PATH
 from .utils import camel_case
 from .utils import ensure_cwd_is_repo_root
 from .utils import mkdir
 from .utils import mkfile
 from .utils import setup_templates
 
-BASE_DIR = Path(__file__).parent.parent
+PACKAGE_DIR = Path(__file__).resolve().parent
 
 WAF_ACL_ARN_KEY = "waf-acl-arn"
 
 
 def list_copilot_local_environments():
     return [path.parent.parts[-1] for path in Path("./copilot/environments/").glob("*/manifest.yml")]
 
@@ -44,18 +44,18 @@
         conf.update(env_conf)
 
         return conf
 
     def _normalise_keys(source: dict):
         return {k.replace("-", "_"): v for k, v in source.items()}
 
-    with open(BASE_DIR / "storage-plans.yml", "r") as fd:
+    with open(PACKAGE_DIR / "storage-plans.yml", "r") as fd:
         storage_plans = yaml.safe_load(fd)
 
-    with open(BASE_DIR / "schemas/storage-schema.json", "r") as fd:
+    with open(PACKAGE_DIR / "schemas/storage-schema.json", "r") as fd:
         schema = json.load(fd)
 
     # load and validate config
     with open(config_file, "r") as fd:
         config = yaml.safe_load(fd)
 
     # empty file
@@ -130,15 +130,15 @@
     overwrite = True
     output_dir = Path(".").absolute()
 
     ensure_cwd_is_repo_root()
 
     templates = setup_templates()
 
-    config = _validate_and_normalise_config(BASE_DIR / "default-storage.yml")
+    config = _validate_and_normalise_config(PACKAGE_DIR / "default-storage.yml")
 
     project_config = _validate_and_normalise_config("storage.yml")
 
     config.update(project_config)
 
     click.echo("\n>>> Generating storage cloudformation\n")
```

### Comparing `dbt_copilot_tools-0.1.7/commands/dns_cli.py` & `dbt_copilot_tools-0.1.8/commands/dns_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/COMMANDS.md.jinja` & `dbt_copilot_tools-0.1.8/commands/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/addons/env/addons.parameters.yml` & `dbt_copilot_tools-0.1.8/commands/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/addons/env/aurora-postgres.yml` & `dbt_copilot_tools-0.1.8/commands/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/addons/env/opensearch.yml` & `dbt_copilot_tools-0.1.8/commands/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/addons/env/rds-postgres.yml` & `dbt_copilot_tools-0.1.8/commands/templates/addons/env/rds-postgres.yml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 Mappings:
   {{ service.prefix }}EnvScalingConfigurationMap:
     {% for env_name, config in service.environments.items() %}
     {{ env_name }}:
       DBInstanceClass: '{{ config.instance }}'
       MultiAZ: {% if config.replicas %} true {% else %} false {% endif %}
       AllocatedStorage: {{ config.volume_size }}
-      MaxAllocatedStorage: {{ config.volume_size * 1.26 }}
+      MaxAllocatedStorage: {{ (config.volume_size * 1.26)|round|int }}
       StorageType: {% if env_name == "prod" %} io1 {% else %} gp3 {% endif %}
 
     {% endfor %}
 
 Resources:
   # Subnet group to control where the DB gets placed
   DBSubnetGroup:
@@ -69,15 +69,15 @@
     Metadata:
       'aws:copilot:description': 'DB cluster'
     Type: AWS::RDS::DBInstance
     Properties:
       AutoMinorVersionUpgrade: true
       EnablePerformanceInsights: true
       Engine: postgres
-      EngineVersion: '13.4'
+      EngineVersion: '13'
       DBInstanceClass: !FindInMap [{{ service.prefix }}EnvScalingConfigurationMap, !Ref Env, DBInstanceClass]
       AllocatedStorage: !FindInMap [{{ service.prefix }}EnvScalingConfigurationMap, !Ref Env, AllocatedStorage]
       MaxAllocatedStorage: !FindInMap [{{ service.prefix }}EnvScalingConfigurationMap, !Ref Env, MaxAllocatedStorage]
       StorageType: !FindInMap [{{ service.prefix }}EnvScalingConfigurationMap, !Ref Env, StorageType]
       MultiAZ: !FindInMap [{{ service.prefix }}EnvScalingConfigurationMap, !Ref Env, MultiAZ]
       AllowMajorVersionUpgrade: false
       BackupRetentionPeriod: 7
```

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/addons/env/redis-cluster.yml` & `dbt_copilot_tools-0.1.8/commands/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/addons/env/s3.yml` & `dbt_copilot_tools-0.1.8/commands/templates/addons/svc/s3-policy.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata:
+  cfn-lint:
+    config:
+      ignore_checks:
+        - W2001 # Parameter not used
+
 Parameters:
   # Copilot required Parameters...
   App:
     Type: String
     Description: Your application's name.
   Env:
     Type: String
@@ -15,55 +21,37 @@
     # Create an entry for each environment
     {% for env_name, config in service.environments.items() %}
     {{ env_name }}:
       BucketName: '{{ config.bucket_name }}'
     {% endfor %}
 
 Resources:
-  {{ service.prefix }}Bucket:
+  {{ service.prefix }}S3AccessPolicy:
     Metadata:
-      'aws:copilot:description': 'An Amazon S3 bucket to store and retrieve objects for {{ service.prefix }}'
-    Type: AWS::S3::Bucket
-    Properties:
-      BucketName: !FindInMap [{{ service.prefix }}BucketNameMap, !Ref Env, BucketName]
-      AccessControl: Private
-      BucketEncryption:
-        ServerSideEncryptionConfiguration:
-        - ServerSideEncryptionByDefault:
-            SSEAlgorithm: AES256
-      PublicAccessBlockConfiguration:
-        BlockPublicAcls: true
-        BlockPublicPolicy: true
-      Tags:
-        - Key: Copilot-application
-          Value: !Ref App
-        - Key: Copilot-environment
-          Value: !Ref Env
-        - Key: Copilot-name
-          Value: !Ref Name
-
-  {{ service.prefix }}BucketPolicy:
-    Metadata:
-      'aws:copilot:description': 'A bucket policy to deny unencrypted access to the bucket and its contents'
-    Type: AWS::S3::BucketPolicy
-    DeletionPolicy: Retain
-    UpdateReplacePolicy: Retain
+      'aws:copilot:description': 'An IAM ManagedPolicy for your service to access the bucket'
+    Type: AWS::IAM::ManagedPolicy
     Properties:
+      Description: Grants Read access to the S3 bucket.
       PolicyDocument:
-        Version: '2012-10-17'
+        Version: 2012-10-17
         Statement:
-          - Sid: ForceHTTPS
-            Effect: Deny
-            Principal: '*'
-            Action: 's3:*'
-            Resource:
-              - !Sub ${ {{ service.prefix }}Bucket.Arn}/*
-              - !Sub ${ {{ service.prefix }}Bucket.Arn}
-            Condition:
-              Bool:
-                "aws:SecureTransport": false
-      Bucket: !Ref {{ service.prefix }}Bucket
-
+          - Sid: S3ObjectActions
+            Effect: Allow
+            Action:
+{%- if service.readonly %}
+              - s3:GetObject
+{% else %}
+              - s3:*Object
+{% endif %}
+            Resource: !Sub
+              - "arn:aws:s3:::${ bucket_name }/*"
+              - bucket_name: !FindInMap [{{ service.prefix }}BucketNameMap, !Ref Env, BucketName]
+          - Sid: S3ListAction
+            Effect: Allow
+            Action: s3:ListBucket
+            Resource: !Sub
+              - "arn:aws:s3:::${ bucket_name }"
+              - bucket_name: !FindInMap [{{ service.prefix }}BucketNameMap, !Ref Env, BucketName]
 Outputs:
-  {{ service.prefix }}Name:
-    Description: "The name of a user-defined bucket."
-    Value: !Ref {{ service.prefix }}Bucket
+  {{ service.prefix }}AccessPolicy:
+    Description: "The IAM::ManagedPolicy to attach to the task role"
+    Value: !Ref {{ service.prefix }}S3AccessPolicy
```

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/ci-codebuild-role-policy.json` & `dbt_copilot_tools-0.1.8/commands/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/custom-codebuild-role-policy.json` & `dbt_copilot_tools-0.1.8/commands/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/env/manifest.yml` & `dbt_copilot_tools-0.1.8/commands/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/instructions.txt` & `dbt_copilot_tools-0.1.8/commands/templates/instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/storage-instructions.txt` & `dbt_copilot_tools-0.1.8/commands/templates/storage-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/svc/manifest-backend.yml` & `dbt_copilot_tools-0.1.8/commands/templates/svc/manifest-backend.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
   range: 2-10
   cooldown:
     in: 120s
     out: 60s
   cpu_percentage: 50
 exec: true     # Enable running commands in your container.
 
-# storage:
-  # readonly_fs: true       # Limit to read-only access to mounted root filesystems.
+storage:
+  readonly_fs: true       # Limit to read-only access to mounted root filesystems.
 
 variables:                    # Pass environment variables as key value pairs.
   PORT: 8080                  # The bootstrap container requires a $PORT env var
   {%- for envvar, value in env_vars %}
   {{ envvar }}:
   {% endfor %}
```

### Comparing `dbt_copilot_tools-0.1.7/commands/templates/svc/manifest-public.yml` & `dbt_copilot_tools-0.1.8/commands/templates/svc/manifest-public.yml`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     in: 120s
     out: 60s
   cpu_percentage: 50
 exec: true     # Enable running commands in your container.
 network:
   connect: true # Enable Service Connect for intra-environment traffic between services.
 
-# storage:
-  # readonly_fs: true       # Limit to read-only access to mounted root filesystems.
+storage:
+  readonly_fs: true       # Limit to read-only access to mounted root filesystems.
 
 # Optional fields for more advanced use-cases.
 #
 variables:                    # Pass environment variables as key value pairs.
   PORT: 8080
   {%- for envvar, value in env_vars.items() %}
   {{ envvar }}:
```

### Comparing `dbt_copilot_tools-0.1.7/commands/utils.py` & `dbt_copilot_tools-0.1.8/commands/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/commands/waf_cli.py` & `dbt_copilot_tools-0.1.8/commands/waf_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/copilot_helper.py` & `dbt_copilot_tools-0.1.8/copilot_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.7/pyproject.toml` & `dbt_copilot_tools-0.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry]
 name = "dbt-copilot-tools"
-version = "0.1.7"
+version = "0.1.8"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "commands/README.md"
 packages = [
     { include = "commands" },
     { include = "copilot_helper.py" }
```

### Comparing `dbt_copilot_tools-0.1.7/PKG-INFO` & `dbt_copilot_tools-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

