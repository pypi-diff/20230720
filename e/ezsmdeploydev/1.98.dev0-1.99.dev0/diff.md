# Comparing `tmp/ezsmdeploydev-1.98.dev0.tar.gz` & `tmp/ezsmdeploydev-1.99.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsmdeploydev-1.98.dev0.tar", last modified: Thu Jul 20 19:35:17 2023, max compression
+gzip compressed data, was "ezsmdeploydev-1.99.dev0.tar", last modified: Thu Jul 20 20:08:11 2023, max compression
```

## Comparing `ezsmdeploydev-1.98.dev0.tar` & `ezsmdeploydev-1.99.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:35:17.550236 ezsmdeploydev-1.98.dev0/
--rw-r--r--   0 chethan   (1000) chethan   (1000)       26 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/MANIFEST.in
--rw-r--r--   0 chethan   (1000) chethan   (1000)    19601 2023-07-20 19:35:17.550236 ezsmdeploydev-1.98.dev0/PKG-INFO
--rw-r--r--   0 chethan   (1000) chethan   (1000)    19108 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/README.rst
-drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:35:17.540236 ezsmdeploydev-1.98.dev0/ezsmdeploy/
--rw-r--r--   0 chethan   (1000) chethan   (1000)    48494 2023-07-20 19:34:03.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/__init__.py
-drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:35:17.540236 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/
--rw-r--r--   0 chethan   (1000) chethan   (1000)     2100 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/Dockerfile
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1934 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/Dockerfile_flask
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1390 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/build-docker.sh
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1603 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/conversation.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1361 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/cost.csv
--rw-r--r--   0 chethan   (1000) chethan   (1000)      884 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/dockerd-entrypoint.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)      576 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/instancetypes.csv
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1797 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/model_handler.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)      719 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/nginx.conf
--rw-r--r--   0 chethan   (1000) chethan   (1000)     2090 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/predictor.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)     2429 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/serve
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1409 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/smlocust.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)      432 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/train
--rw-r--r--   0 chethan   (1000) chethan   (1000)      202 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/wsgi.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)      733 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/modelscript_sklearn.py
-drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:35:17.550236 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/
--rw-r--r--   0 chethan   (1000) chethan   (1000)    19601 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/PKG-INFO
--rw-r--r--   0 chethan   (1000) chethan   (1000)      714 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/SOURCES.txt
--rw-r--r--   0 chethan   (1000) chethan   (1000)        1 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/dependency_links.txt
--rw-r--r--   0 chethan   (1000) chethan   (1000)        1 2023-07-20 19:35:05.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/not-zip-safe
--rw-r--r--   0 chethan   (1000) chethan   (1000)      129 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/requires.txt
--rw-r--r--   0 chethan   (1000) chethan   (1000)       11 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/top_level.txt
--rw-r--r--   0 chethan   (1000) chethan   (1000)       38 2023-07-20 19:35:17.550236 ezsmdeploydev-1.98.dev0/setup.cfg
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1277 2023-07-20 19:34:59.000000 ezsmdeploydev-1.98.dev0/setup.py
+drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 20:08:11.630267 ezsmdeploydev-1.99.dev0/
+-rw-r--r--   0 chethan   (1000) chethan   (1000)       26 2023-07-20 18:56:41.000000 ezsmdeploydev-1.99.dev0/MANIFEST.in
+-rw-r--r--   0 chethan   (1000) chethan   (1000)    19401 2023-07-20 20:08:11.630267 ezsmdeploydev-1.99.dev0/PKG-INFO
+-rw-r--r--   0 chethan   (1000) chethan   (1000)    18908 2023-07-20 19:44:20.000000 ezsmdeploydev-1.99.dev0/README.rst
+drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 20:08:11.620267 ezsmdeploydev-1.99.dev0/ezsmdeploy/
+-rw-r--r--   0 chethan   (1000) chethan   (1000)    48586 2023-07-20 20:00:25.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/__init__.py
+drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 20:08:11.630267 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     2095 2023-07-20 19:44:16.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/Dockerfile
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1933 2023-07-20 19:44:16.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/Dockerfile_flask
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1389 2023-07-20 19:44:20.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/build-docker.sh
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1604 2023-07-20 19:53:57.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/conversation.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1362 2023-07-20 19:44:20.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/cost.csv
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      885 2023-07-20 19:44:35.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/dockerd-entrypoint.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      577 2023-07-20 19:44:20.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/instancetypes.csv
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1713 2023-07-20 19:44:43.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/model_handler.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      717 2023-07-20 19:44:16.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/nginx.conf
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     2015 2023-07-20 19:54:20.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/predictor.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     2429 2023-07-20 18:56:41.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/serve
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1349 2023-07-20 19:55:30.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/smlocust.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      428 2023-07-20 19:44:16.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/train
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      202 2023-07-20 18:56:41.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/data/wsgi.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      707 2023-07-20 19:44:43.000000 ezsmdeploydev-1.99.dev0/ezsmdeploy/modelscript_sklearn.py
+drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 20:08:11.630267 ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/
+-rw-r--r--   0 chethan   (1000) chethan   (1000)    19401 2023-07-20 20:08:11.000000 ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/PKG-INFO
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      714 2023-07-20 20:08:11.000000 ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/SOURCES.txt
+-rw-r--r--   0 chethan   (1000) chethan   (1000)        1 2023-07-20 20:08:11.000000 ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/dependency_links.txt
+-rw-r--r--   0 chethan   (1000) chethan   (1000)        1 2023-07-20 20:06:44.000000 ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/not-zip-safe
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      129 2023-07-20 20:08:11.000000 ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/requires.txt
+-rw-r--r--   0 chethan   (1000) chethan   (1000)       11 2023-07-20 20:08:11.000000 ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/top_level.txt
+-rw-r--r--   0 chethan   (1000) chethan   (1000)       38 2023-07-20 20:08:11.630267 ezsmdeploydev-1.99.dev0/setup.cfg
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1201 2023-07-20 20:07:43.000000 ezsmdeploydev-1.99.dev0/setup.py
```

### Comparing `ezsmdeploydev-1.98.dev0/PKG-INFO` & `ezsmdeploydev-1.99.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploydev
-Version: 1.98.dev0
+Version: 1.99.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -32,16 +32,16 @@
 .. image:: https://img.shields.io/badge/Made%20With-Love-orange.svg
    :target: https://pypi.python.org/pypi/ezsmdeploy
    :alt: Made With Love
 
 .. image:: https://img.shields.io/badge/Gen-AI-8A2BE2
    :target: https://pypi.python.org/pypi/ezsmdeploy
    :alt: GenAI
-   
-   
+
+
 
 **Ezsmdeploy** python SDK helps you easily deploy Machine learning models on SageMaker. It provides a rich set of features such as deploying models from hubs (like Huggingface or SageMaker Jumpstart), passing one or more model files (even with multi-model deployments), automatically choosing an instance based on model size or based on a budget, and load testing endpoints using an intuitive API. **Ezsmdeploy** uses the SageMaker Python SDK, which is an open source library for training and deploying machine learning models on Amazon SageMaker. This SDK however focuses on further simplifying deployment from existing models, and as such, this is for you if:
 
 1.  you want to quickly deploy and try out foundational language models as an API powered by SageMaker (**New in v 2.0**)
 2.  you have a serialized model (a pickle / joblib/ json/ TF saved model/ Pytorch .pth/ etc) file and you want to deploy and test your model as an API endpoint
 3. you have a model or multiple models stored as local files, in local folders, or in S3 as tar files (model.tar.gz)
 4. you don't want to create a custom docker container for deployment and/or don't want to deal with docker
@@ -66,16 +66,16 @@
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
     - facebook/galactica-6.7b, ml.g5.16xlarge
     - CalderaAI/30B-Lazarus, ml.g5.16xlarge
     - huggyllama/llama-65b, ml.g5.16xlarge
     - ausboss/llama-30b-supercot, ml.g4dn.4xlarge
     - MetaIX/GPT4-X-Alpasta-30b, ml.g4dn.4xlarge
-    - 
-    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50) 
+    -
+    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50)
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -109,34 +109,34 @@
 
 Cleanest way to install this package is within a virtualenv:
 
 
 ::
 
     python -m venv env
-    
+
     source env/bin/activate
 
     pip install ezsmdeploy[locust]
 
 
 In some cases, installs fail due to an existing package installed called "greenlet". This is not a direct dependency of ezsmdeploy but interferes with the installation. To fix this, either install in a virtualenv as seen above, or do:
 
 ::
 
     pip install ezsmdeploy[locust] --ignore-installed greenlet
-    
-    
+
+
 If you have another way to test the endpoint, or want to manage locust on your own, just do:
 
 ::
 
     pip install ezsmdeploy
-    
-   
+
+
 
 Key Features
 ~~~~~~~~~~~~
 
 At minimum, **ezsmdeploy** requires you to provide:
 
 1. one or more model files
@@ -154,19 +154,19 @@
 
 You can also load multiple models ...
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = ['model1.pth','model2.pth'],
                   script = 'modelscript_pytorch.py',
-                  requirements = ['numpy','torch','joblib'])    
+                  requirements = ['numpy','torch','joblib'])
 
 ...  or download tar.gz models from S3
-:: 
-    
+::
+
     ezonsm = ezsmdeploy.Deploy(model = ['s3://ezsmdeploy/pytorchmnist/model.tar.gz'],
                   script = 'modelscript_pytorch.py',
                   requirements = 'path/to/requirements.txt')
 
 
 Other Features
 ~~~~~~~~~~~~~~~
@@ -198,30 +198,30 @@
     ):
 
 
 Let's take a look at each of these parameters and what they do:
 
 * You can skip passing in requirements through a file or a list if you choose a **"framework"** in ["tensorflow", "pytorch", "mxnet", "sklearn"]. If you do, these libraries are installed automatically. However it is expected that most people will not use this, given the limited installs, and will usually pass in a custom set of requirements.
 
- :: 
+ ::
 
     ezonsm = ezsmdeploy.Deploy(model = ... ,
                   script = ... ,
                   framework = 'sklearn')
 
 * Pass in a **"name"** if you want to override the random name generated by ezsmdeploy that is used to name your custom ECR image and the endpoint.
 
- :: 
+ ::
 
     ezonsm = ezsmdeploy.Deploy(model = ... ,
                   script = ... ,
                   framework = 'sklearn',
                   name = 'randomname')
-                      
-                      
+
+
 * Set **"autoscale"** to True if required to switch on autoscaling for your endpoint. By default, this sets up endpoint autoscaling with the metric *SageMakerVariantInvocationsPerInstance* and a target value of 1000. You can override this value by also passing in a value for autoscaletarget
 
 |
 
 * **"wait**" is set to True by default and can be set to False if you don't want to wait for the endpoint to deploy.
 
 |
@@ -230,19 +230,19 @@
 
 |
 
 * Pass in a sagemaker **"session"** to override the default session; for most cases this is not necessary. Also, this may interfere with local deployments as the same session cannot be used for tasks such as downloading and uploading files, and for local and remote deployments.
 
 |
 
-* If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in. 
+* If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in.
 
 |
 
-* If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe. 
+* If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe.
 
 |
 
 * Passing in an **"instance_count"** > 1 will change the initial number of instances that the model(s) is(are) deployed on.
 
 |
 
@@ -251,43 +251,43 @@
 |
 
 * Set **"monitor"** to True if you would like to turn on Datacapture for this endpoint. Currently, a sampling_percentage of 100 is used. Read more about Model monitor here - https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor.html
 
 |
 
 * You should see an output as follows for a typical deployment:
-    
+
  ::
 
    0:00:00.143132 | compressed model(s)
    0:00:00.403894 | uploaded model tarball(s) ; check returned modelpath
    0:00:00.404948 | added requirements file
    0:00:00.406745 | added source file
    0:00:00.408180 | added Dockerfile
    0:00:00.409959 | added model_handler and docker utils
    0:00:00.410072 | building docker container
    0:01:59.298091 | built docker container
    0:01:59.647986 | created model(s). Now deploying on ml.m5.xlarge
    0:09:31.904897 | deployed model
    0:09:31.905450 | estimated cost is $0.3 per hour
-   0:09:31.905805 | Done! ✔ 
+   0:09:31.905805 | Done! ✔
 
 
 * Once your model is deployed, you can use locust.io to load test your endpoint. The test reports the number of requests, number of failures, average, min, max response time in milliseconds and requests per second reached based on the number of parallel users and hatch rate entered. To load test your model (make sure you have deployed it remotely first), try:
- 
+
  ::
 
      ezonsm.test(input_data, target_model='model1.tar.gz')
- 
- or 
+
+ or
 
  ::
 
      ezonsm.test(input_data, target_model='model1.tar.gz',usercount=20,hatchrate=10,timeoutsecs=10)
-     
+
  ... to override default arguments. Read more about locust.io here https://docs.locust.io/en/stable/
 
 
 Model Script requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Make sure your model script has a load_model() and predict() function. While you can still use sagemaker's serializers and deserializers, assume that you will get a payload in bytes, and that you have to return a prediction in bytes. What you do in between is up to you. For example, your model script may look like:
@@ -300,15 +300,15 @@
 
     def predict(model, payload):
         try:
             # in remote / container based deployment, payload comes in as a stream of bytes
             out = [str(model.predict(np.frombuffer(payload[0]['body']).reshape((1,64))))]
         except Exception as e:
            out = [type(payload),str(e)] #useful for debugging!
-    
+
     return out
 
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
 Large Language models
@@ -325,30 +325,30 @@
 
 To deploy models using Jumpstart:
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
                                foundation_model=True)
-                               
-Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker                               
+
+Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker
 
 
 
 To deploy a huggingface LLM model (this uses the huggingface llm container):
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "tiiuae/falcon-40b-instruct",
                                foundation_model=True,
                                huggingface_model=True,
                                huggingface_model_task='text-generation',
                                instance_type="ml.g4dn.12xlarge"
                                )
-                               
+
 (See release notes for models we have tested so far with instances that worked)
 
 Note that at the time of writing this, officially supported model architectures for LLMs on Huggingface are currently:
 
     - BLOOM / BLOOMZ
     - MT0-XXL
     - Galactica
@@ -396,15 +396,15 @@
 You can read more about which permissions are necessary in the `AWS Documentation <https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html>`__.
 
 The SageMaker Python SDK should not require any additional permissions aside from what is required for using SageMaker.
 However, if you are using an IAM role with a path in it, you should grant permission for ``iam:GetRole``.
 
 Licensing
 ~~~~~~~~~
-Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/ 
+Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/
 
 Sample Notebooks
 ~~~~~~~~~~~~~~~~~
 https://github.com/aws-samples/easy-amazon-sagemaker-deployments/tree/master/notebooks
 
 Known Gotchas
 ~~~~~~~~~~~~~~~~~~
@@ -420,15 +420,15 @@
 
 |
 
 * Ezsmdeploy uses Locust to do endpoint testing - any restrictions of the locustio package are also expected to be seen here.
 
 |
 
-* Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU). 
+* Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU).
 
 |
 
 * The payload comes in as bytes; you can also use Sagemaker's serializer and deserializers to send in other formats of input data
 
 |
 
@@ -448,15 +448,15 @@
 
     docker system prune -a
 
 * If you encounter an "image does not exist" error, try running this script that exists after an unsuccessful run, but manually. For this, do:
 
 ::
 
-   ./src/build-docker.sh 
+   ./src/build-docker.sh
 
 * Locust load testing on local endpoint has not been tested (and may not make much sense). Please use the .test() for remote deployment
 
 |
 
 * Use instance_type "local" if you would like to test locally (this lets you test using the MMS stack). If you intend to finally deploy your model to a GPU instance, use "local_gpu" - this launches the flask-nginx stack locally and the same stack when you deploy to a GPU.
 
@@ -465,10 +465,7 @@
 * At the time of writing this guide, launching a multi-model server from sagemaker does not support GPUs (but the open source MMS repository has no such restrictions). Ezsmdeploy checks the number of models passed in, the instance type and other parameters to decide which stack to build for your endpoint.
 
 
 CONTRIBUTING
 ------------
 
 Please submit a pull request to the packages git repo
-
-
-
```

### Comparing `ezsmdeploydev-1.98.dev0/README.rst` & `ezsmdeploydev-1.99.dev0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 .. image:: https://img.shields.io/badge/Made%20With-Love-orange.svg
    :target: https://pypi.python.org/pypi/ezsmdeploy
    :alt: Made With Love
 
 .. image:: https://img.shields.io/badge/Gen-AI-8A2BE2
    :target: https://pypi.python.org/pypi/ezsmdeploy
    :alt: GenAI
-   
-   
+
+
 
 **Ezsmdeploy** python SDK helps you easily deploy Machine learning models on SageMaker. It provides a rich set of features such as deploying models from hubs (like Huggingface or SageMaker Jumpstart), passing one or more model files (even with multi-model deployments), automatically choosing an instance based on model size or based on a budget, and load testing endpoints using an intuitive API. **Ezsmdeploy** uses the SageMaker Python SDK, which is an open source library for training and deploying machine learning models on Amazon SageMaker. This SDK however focuses on further simplifying deployment from existing models, and as such, this is for you if:
 
 1.  you want to quickly deploy and try out foundational language models as an API powered by SageMaker (**New in v 2.0**)
 2.  you have a serialized model (a pickle / joblib/ json/ TF saved model/ Pytorch .pth/ etc) file and you want to deploy and test your model as an API endpoint
 3. you have a model or multiple models stored as local files, in local folders, or in S3 as tar files (model.tar.gz)
 4. you don't want to create a custom docker container for deployment and/or don't want to deal with docker
@@ -51,16 +51,16 @@
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
     - facebook/galactica-6.7b, ml.g5.16xlarge
     - CalderaAI/30B-Lazarus, ml.g5.16xlarge
     - huggyllama/llama-65b, ml.g5.16xlarge
     - ausboss/llama-30b-supercot, ml.g4dn.4xlarge
     - MetaIX/GPT4-X-Alpasta-30b, ml.g4dn.4xlarge
-    - 
-    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50) 
+    -
+    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50)
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -94,34 +94,34 @@
 
 Cleanest way to install this package is within a virtualenv:
 
 
 ::
 
     python -m venv env
-    
+
     source env/bin/activate
 
     pip install ezsmdeploy[locust]
 
 
 In some cases, installs fail due to an existing package installed called "greenlet". This is not a direct dependency of ezsmdeploy but interferes with the installation. To fix this, either install in a virtualenv as seen above, or do:
 
 ::
 
     pip install ezsmdeploy[locust] --ignore-installed greenlet
-    
-    
+
+
 If you have another way to test the endpoint, or want to manage locust on your own, just do:
 
 ::
 
     pip install ezsmdeploy
-    
-   
+
+
 
 Key Features
 ~~~~~~~~~~~~
 
 At minimum, **ezsmdeploy** requires you to provide:
 
 1. one or more model files
@@ -139,19 +139,19 @@
 
 You can also load multiple models ...
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = ['model1.pth','model2.pth'],
                   script = 'modelscript_pytorch.py',
-                  requirements = ['numpy','torch','joblib'])    
+                  requirements = ['numpy','torch','joblib'])
 
 ...  or download tar.gz models from S3
-:: 
-    
+::
+
     ezonsm = ezsmdeploy.Deploy(model = ['s3://ezsmdeploy/pytorchmnist/model.tar.gz'],
                   script = 'modelscript_pytorch.py',
                   requirements = 'path/to/requirements.txt')
 
 
 Other Features
 ~~~~~~~~~~~~~~~
@@ -183,30 +183,30 @@
     ):
 
 
 Let's take a look at each of these parameters and what they do:
 
 * You can skip passing in requirements through a file or a list if you choose a **"framework"** in ["tensorflow", "pytorch", "mxnet", "sklearn"]. If you do, these libraries are installed automatically. However it is expected that most people will not use this, given the limited installs, and will usually pass in a custom set of requirements.
 
- :: 
+ ::
 
     ezonsm = ezsmdeploy.Deploy(model = ... ,
                   script = ... ,
                   framework = 'sklearn')
 
 * Pass in a **"name"** if you want to override the random name generated by ezsmdeploy that is used to name your custom ECR image and the endpoint.
 
- :: 
+ ::
 
     ezonsm = ezsmdeploy.Deploy(model = ... ,
                   script = ... ,
                   framework = 'sklearn',
                   name = 'randomname')
-                      
-                      
+
+
 * Set **"autoscale"** to True if required to switch on autoscaling for your endpoint. By default, this sets up endpoint autoscaling with the metric *SageMakerVariantInvocationsPerInstance* and a target value of 1000. You can override this value by also passing in a value for autoscaletarget
 
 |
 
 * **"wait**" is set to True by default and can be set to False if you don't want to wait for the endpoint to deploy.
 
 |
@@ -215,19 +215,19 @@
 
 |
 
 * Pass in a sagemaker **"session"** to override the default session; for most cases this is not necessary. Also, this may interfere with local deployments as the same session cannot be used for tasks such as downloading and uploading files, and for local and remote deployments.
 
 |
 
-* If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in. 
+* If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in.
 
 |
 
-* If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe. 
+* If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe.
 
 |
 
 * Passing in an **"instance_count"** > 1 will change the initial number of instances that the model(s) is(are) deployed on.
 
 |
 
@@ -236,43 +236,43 @@
 |
 
 * Set **"monitor"** to True if you would like to turn on Datacapture for this endpoint. Currently, a sampling_percentage of 100 is used. Read more about Model monitor here - https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor.html
 
 |
 
 * You should see an output as follows for a typical deployment:
-    
+
  ::
 
    0:00:00.143132 | compressed model(s)
    0:00:00.403894 | uploaded model tarball(s) ; check returned modelpath
    0:00:00.404948 | added requirements file
    0:00:00.406745 | added source file
    0:00:00.408180 | added Dockerfile
    0:00:00.409959 | added model_handler and docker utils
    0:00:00.410072 | building docker container
    0:01:59.298091 | built docker container
    0:01:59.647986 | created model(s). Now deploying on ml.m5.xlarge
    0:09:31.904897 | deployed model
    0:09:31.905450 | estimated cost is $0.3 per hour
-   0:09:31.905805 | Done! ✔ 
+   0:09:31.905805 | Done! ✔
 
 
 * Once your model is deployed, you can use locust.io to load test your endpoint. The test reports the number of requests, number of failures, average, min, max response time in milliseconds and requests per second reached based on the number of parallel users and hatch rate entered. To load test your model (make sure you have deployed it remotely first), try:
- 
+
  ::
 
      ezonsm.test(input_data, target_model='model1.tar.gz')
- 
- or 
+
+ or
 
  ::
 
      ezonsm.test(input_data, target_model='model1.tar.gz',usercount=20,hatchrate=10,timeoutsecs=10)
-     
+
  ... to override default arguments. Read more about locust.io here https://docs.locust.io/en/stable/
 
 
 Model Script requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Make sure your model script has a load_model() and predict() function. While you can still use sagemaker's serializers and deserializers, assume that you will get a payload in bytes, and that you have to return a prediction in bytes. What you do in between is up to you. For example, your model script may look like:
@@ -285,15 +285,15 @@
 
     def predict(model, payload):
         try:
             # in remote / container based deployment, payload comes in as a stream of bytes
             out = [str(model.predict(np.frombuffer(payload[0]['body']).reshape((1,64))))]
         except Exception as e:
            out = [type(payload),str(e)] #useful for debugging!
-    
+
     return out
 
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
 Large Language models
@@ -310,30 +310,30 @@
 
 To deploy models using Jumpstart:
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
                                foundation_model=True)
-                               
-Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker                               
+
+Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker
 
 
 
 To deploy a huggingface LLM model (this uses the huggingface llm container):
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "tiiuae/falcon-40b-instruct",
                                foundation_model=True,
                                huggingface_model=True,
                                huggingface_model_task='text-generation',
                                instance_type="ml.g4dn.12xlarge"
                                )
-                               
+
 (See release notes for models we have tested so far with instances that worked)
 
 Note that at the time of writing this, officially supported model architectures for LLMs on Huggingface are currently:
 
     - BLOOM / BLOOMZ
     - MT0-XXL
     - Galactica
@@ -381,15 +381,15 @@
 You can read more about which permissions are necessary in the `AWS Documentation <https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html>`__.
 
 The SageMaker Python SDK should not require any additional permissions aside from what is required for using SageMaker.
 However, if you are using an IAM role with a path in it, you should grant permission for ``iam:GetRole``.
 
 Licensing
 ~~~~~~~~~
-Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/ 
+Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/
 
 Sample Notebooks
 ~~~~~~~~~~~~~~~~~
 https://github.com/aws-samples/easy-amazon-sagemaker-deployments/tree/master/notebooks
 
 Known Gotchas
 ~~~~~~~~~~~~~~~~~~
@@ -405,15 +405,15 @@
 
 |
 
 * Ezsmdeploy uses Locust to do endpoint testing - any restrictions of the locustio package are also expected to be seen here.
 
 |
 
-* Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU). 
+* Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU).
 
 |
 
 * The payload comes in as bytes; you can also use Sagemaker's serializer and deserializers to send in other formats of input data
 
 |
 
@@ -433,15 +433,15 @@
 
     docker system prune -a
 
 * If you encounter an "image does not exist" error, try running this script that exists after an unsuccessful run, but manually. For this, do:
 
 ::
 
-   ./src/build-docker.sh 
+   ./src/build-docker.sh
 
 * Locust load testing on local endpoint has not been tested (and may not make much sense). Please use the .test() for remote deployment
 
 |
 
 * Use instance_type "local" if you would like to test locally (this lets you test using the MMS stack). If you intend to finally deploy your model to a GPU instance, use "local_gpu" - this launches the flask-nginx stack locally and the same stack when you deploy to a GPU.
 
@@ -450,10 +450,7 @@
 * At the time of writing this guide, launching a multi-model server from sagemaker does not support GPUs (but the open source MMS repository has no such restrictions). Ezsmdeploy checks the number of models passed in, the instance type and other parameters to decide which stack to build for your endpoint.
 
 
 CONTRIBUTING
 ------------
 
 Please submit a pull request to the packages git repo
-
-
-
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/__init__.py` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,66 @@
-import sagemaker
-import shortuuid
-from yaspin import yaspin
-from yaspin.spinners import Spinners
-import time
+import ast
+import cmd
+import csv
 import datetime
-import tarfile
-import re
-import boto3
 import glob
+import json
 import os
+import pickle
+import re
 import shutil
-import pkg_resources
 import subprocess
-from sagemaker.multidatamodel import MultiDataModel
-from sagemaker.serverless import ServerlessInferenceConfig
-from sagemaker.model import Model
-import ast
-import csv
-import json
-import pickle
+import tarfile
 import time
-import cmd
 from typing import List, Optional
+
+import boto3
+import pkg_resources
+import sagemaker
+import shortuuid
+from sagemaker.model import Model
+from sagemaker.multidatamodel import MultiDataModel
 from sagemaker.predictor import Predictor
+from sagemaker.serverless import ServerlessInferenceConfig
+from yaspin import yaspin
+from yaspin.spinners import Spinners
+
+__version__ = "1.99dev"
 
 _model_env_variable_map = {
     "huggingface-text2text-flan-t5-xxl": {"TS_DEFAULT_WORKERS_PER_MODEL": "1"},
     "huggingface-text2text-flan-t5-xxl-fp16": {"TS_DEFAULT_WORKERS_PER_MODEL": "1"},
     "huggingface-text2text-flan-t5-xxl-bnb-int8": {"TS_DEFAULT_WORKERS_PER_MODEL": "1"},
     "huggingface-text2text-flan-t5-xl": {"MMS_DEFAULT_WORKERS_PER_MODEL": "1"},
     "huggingface-text2text-flan-t5-large": {"MMS_DEFAULT_WORKERS_PER_MODEL": "1"},
     "huggingface-text2text-flan-ul2-bf16": {"TS_DEFAULT_WORKERS_PER_MODEL": "1"},
     "huggingface-text2text-bigscience-t0pp": {"TS_DEFAULT_WORKERS_PER_MODEL": "1"},
     "huggingface-text2text-bigscience-t0pp-fp16": {"TS_DEFAULT_WORKERS_PER_MODEL": "1"},
-    "huggingface-text2text-bigscience-t0pp-bnb-int8": {"TS_DEFAULT_WORKERS_PER_MODEL": "1"},
-    "huggingface-textgeneration2-gpt-neoxt-chat-base-20b-fp16":{"TS_DEFAULT_WORKERS_PER_MODEL": "1"}
+    "huggingface-text2text-bigscience-t0pp-bnb-int8": {
+        "TS_DEFAULT_WORKERS_PER_MODEL": "1"
+    },
+    "huggingface-textgeneration2-gpt-neoxt-chat-base-20b-fp16": {
+        "TS_DEFAULT_WORKERS_PER_MODEL": "1"
+    },
 }
 
 
-
 class utils(object):
     def __init__(self):
         pass
+
     def list_foundation_models(self, filter_value="task == text2text"):
         from sagemaker.jumpstart.notebook_utils import list_jumpstart_models
+
         # print('\n'.join(list(_model_env_variable_map.keys())))
         text_generation_models = list_jumpstart_models(filter=filter_value)
         print("List of foundation models in Jumpstart: \n")
         print("\n".join(text_generation_models))
-    
+
+
 class Deploy(object):
     def __init__(
         self,
         model,
         script=None,
         framework=None,
         requirements=None,
@@ -60,31 +68,36 @@
         autoscale=False,
         autoscaletarget=1000,
         serverless=False,
         serverless_memory=4096,
         serverless_concurrency=10,
         wait=True,
         bucket=None,
-        prefix='',
+        prefix="",
         session=None,
         image=None,
         dockerfilepath=None,
         instance_type=None,
         instance_count=1,
         budget=100,
         ei=None,
         monitor=False,
         foundation_model=False,
-        foundation_model_version='*',
+        foundation_model_version="*",
         huggingface_model=False,
         huggingface_model_task=None,
-        huggingface_model_quantize=None
+        huggingface_model_quantize=None,
     ):
-
-        self.frameworklist = ["tensorflow", "pytorch", "mxnet", "sklearn","huggingface"]
+        self.frameworklist = [
+            "tensorflow",
+            "pytorch",
+            "mxnet",
+            "sklearn",
+            "huggingface",
+        ]
         self.frameworkinstalls = {
             "tensorflow": ["tensorflow"],
             "pytorch": ["torch"],
             "mxnet": ["mxnet", "gluon"],
             "sklearn": ["sklearn"],
         }
 
@@ -100,46 +113,45 @@
         self.deployed = False
         self.autoscaletarget = autoscaletarget
         self.foundation_model = foundation_model
         self.foundation_model_version = foundation_model_version
         self.huggingface_model = huggingface_model
         self.huggingface_model_task = huggingface_model_task
         self.serverless = serverless
-        
+
         if serverless:
             self.serverless_config = ServerlessInferenceConfig(
-                memory_size_in_mb=serverless_memory, max_concurrency=serverless_concurrency)
+                memory_size_in_mb=serverless_memory,
+                max_concurrency=serverless_concurrency,
+            )
         else:
             self.serverless_config = None
-            
+
         self.huggingface_model_quantize = huggingface_model_quantize
 
         # ------ load cost types dict ---------
         costpath = pkg_resources.resource_filename("ezsmdeploy", "data/cost.csv")
         self.costdict = {}
         with open(costpath, mode="r") as infile:
             reader = csv.reader(infile)
             for rows in reader:
                 # cost for each instance
                 self.costdict[rows[0]] = float(rows[1])
 
         # ------- basic instance type check --------
 
-        if (
-            self.instance_type == None
-        ):  # since we will not select a a GPU instance in automatic instance selection
+        # since we will not select a a GPU instance in automatic instance selection
+        if self.instance_type is None:
             self.gpu = False
             self.multimodel = True
         else:
-
             if (
                 (self.instance_type in list(self.costdict.keys()))
                 or "local" in self.instance_type
-            ) and self.instance_type != None:
-
+            ) and self.instance_type is not None:
                 if "local" in self.instance_type:
                     if (
                         self.instance_type == "local_gpu"
                     ):  # useful if you intend to do local testing. No change vs. local
                         self.gpu = True
                         self.multimodel = False
                         self.instance_type == "local"
@@ -171,32 +183,32 @@
         if type(model) == str:
             self.model = [model]
             self.multimodel = False
 
         elif type(model) == list:
             self.model = model
             self.multimodel = True
-        elif model == None:  # assume you are loading from a hub or from a dockerfile
+        elif model is None:  # assume you are loading from a hub or from a dockerfile
             with open("tmpmodel", "w") as fp:
                 pass
             self.model = ["tmpmodel"]
             self.multimodel = False
         else:
             raise ValueError(
                 "model must be a single serialized file (like 'model.pkl') or a \
                 list of files ([model.pkl, model2.pkl]). If you are downloading a model in the script \
                 or packaging with the container, pass in model = None"
             )
-            
+
         # if self.huggingface_model:
         #     # if self.huggingface_model_task == None:
         #     #     print("Using None as task type")
         #     # else:
         #     #     pr
-                # raise ValueError("Please specify huggingface_model_task. For example: question-answering")
+        # raise ValueError("Please specify huggingface_model_task. For example: question-answering")
 
         # ------- Script checks ---------
         if not (self.foundation_model or self.huggingface_model):
             if script[-2:] != "py":
                 raise ValueError(
                     "please provide a valid python script with .py extension. "
                     + script
@@ -204,31 +216,33 @@
                 )
             else:
                 self.script = script
 
             filename = self.script
             with open(filename) as file:
                 node = ast.parse(file.read())
-                functions = [n.name for n in node.body if isinstance(n, ast.FunctionDef)]
+                functions = [
+                    n.name for n in node.body if isinstance(n, ast.FunctionDef)
+                ]
 
             if ("load_model" not in functions) and ("predict" not in functions):
                 raise ValueError(
                     "please implement a load_model(modelpath) that \
                     returns a loaded model, and predict(inputdata) function that returns a prediction in your"
                     + script
                 )
 
         # ------- session checks --------
-        if session == None:
+        if session is None:
             self.session = sagemaker.session.Session()
         else:
             self.session = session  # leave session as none since users may want to do local testing.
 
         # ------- name checks --------
-        if name == None:
+        if name is None:
             self.name = shortuuid.uuid().lower()
         elif type(name) == str:
             self.name = name
             if name.islower() == False:
                 raise ValueError(
                     "please enter a name with lower case letters; we will be using this name for s3 bucket prefixes, model names, ECR repository names etc. that have various restrictions"
                 )
@@ -236,186 +250,206 @@
         else:
             raise ValueError(
                 "enter string for a name or don't pass in a name; type of name passed in is "
                 + str(type(name))
             )
 
         # ------- bucket checks --------
-        if bucket == None:
+        if bucket is None:
             self.bucket = self.session.default_bucket()
         else:
             self.bucket = bucket
 
         self.requirements = requirements
 
         # ------- framework --------
-        if requirements == None and framework in self.frameworklist:
+        if requirements is None and framework in self.frameworklist:
             self.framework = framework
             self.requirements = self.frameworkinstalls[framework]
-        elif requirements == None and framework not in self.frameworklist and not self.foundation_model and not self.huggingface_model:
+        elif (
+            requirements == None
+            and framework not in self.frameworklist
+            and not self.foundation_model
+            and not self.huggingface_model
+        ):
             raise ValueError(
                 "If requirements=None, please provide a value for framework; \
                     choice should be one of 'tensorflow','pytorch','mxnet','sklearn'"
             )
 
         self.autoscale = autoscale
 
         self.wait = wait
         self.deploy()
 
-    
-    
     def deploy_huggingface_model(self):
-        
-        if self.instance_type == None and not self.serverless:
+        if self.instance_type is None and not self.serverless:
             raise ValueError("Please enter a valid instance type, not [None]")
-        
+
         # from sagemaker.huggingface.model import HuggingFaceModel, get_huggingface_llm_image_uri
-        from sagemaker.huggingface import HuggingFaceModel, get_huggingface_llm_image_uri
-        
+        from sagemaker.huggingface import (
+            HuggingFaceModel,
+            get_huggingface_llm_image_uri,
+        )
+
         self.model = self.model[0]
         hub = {
-            'HF_MODEL_ID':self.model,                # model_id from hf.co/models
+            "HF_MODEL_ID": self.model,  # model_id from hf.co/models
         }
-        
-        
+
         if self.huggingface_model_task is not None:
-             hub['HF_TASK'] = self.huggingface_model_task    # NLP task you want to use for predictions
-        
-        if not self.serverless: #ignore instance type checks, and ignore fallback. Also ignore quantization
+            hub[
+                "HF_TASK"
+            ] = self.huggingface_model_task  # NLP task you want to use for predictions
+
+        if (
+            not self.serverless
+        ):  # ignore instance type checks, and ignore fallback. Also ignore quantization
             try:
                 ec2_client = boto3.client("ec2")
-                resp = ec2_client.describe_instance_types(InstanceTypes=[self.instance_type.strip("ml.")])['InstanceTypes'][0]
-                if 'GpuInfo' in resp:
-                    hub['SM_NUM_GPUS']= json.dumps(resp['GpuInfo']['Gpus'][0]['Count'])
+                resp = ec2_client.describe_instance_types(
+                    InstanceTypes=[self.instance_type.strip("ml.")]
+                )["InstanceTypes"][0]
+                if "GpuInfo" in resp:
+                    hub["SM_NUM_GPUS"] = json.dumps(resp["GpuInfo"]["Gpus"][0]["Count"])
                 else:
                     pass
             except Exception as e:
                 print(e, end=" ... ")
-                print("Trying fallback to figure out number of GPUs in the instance type you chose - ")
-                hub['SM_NUM_GPUS']= json.dumps(0) # Use at least 0 GPU by default. else:
-                if 'g' in self.instance_type:
-                    hub['SM_NUM_GPUS']= json.dumps(1)
-                    if '12x' in self.instance_type:
-                        hub['SM_NUM_GPUS']= json.dumps(4)
-                    elif '24x' in self.instance_type:
-                        hub['SM_NUM_GPUS']= json.dumps(4)
-                    elif '48x' in self.instance_type:
-                        hub['SM_NUM_GPUS']= json.dumps(4)
-                elif 'p2' in self.instance_type:
-                    hub['SM_NUM_GPUS']= json.dumps(1)
-                    if '8x' in self.instance_type:
-                        hub['SM_NUM_GPUS']=json.dumps(8)
-                    elif '16x' in self.instance_type:
-                        hub['SM_NUM_GPUS']=json.dumps(16)
-                elif 'p3' in self.instance_type:
-                    hub['SM_NUM_GPUS']= json.dumps(1)
-                    if '8x' in self.instance_type:
-                        hub['SM_NUM_GPUS']=json.dumps(4)
-                    elif '16x' in self.instance_type:
-                        hub['SM_NUM_GPUS']=json.dumps(8)
-                    elif '24x' in self.instance_type:
-                        hub['SM_NUM_GPUS']=json.dumps(8)
-                elif 'p4' in self.instance_type:
-                    hub['SM_NUM_GPUS']=json.dumps(8)
-
-
-
-
-            if self.huggingface_model_quantize in ['bitsandbytes', 'gptq']:
-                hub['HF_MODEL_QUANTIZE'] = self.huggingface_model_quantize
-            elif self.huggingface_model_quantize==None:
+                print(
+                    "Trying fallback to figure out number of GPUs in the instance type you chose - "
+                )
+                hub["SM_NUM_GPUS"] = json.dumps(
+                    0
+                )  # Use at least 0 GPU by default. else:
+                if "g" in self.instance_type:
+                    hub["SM_NUM_GPUS"] = json.dumps(1)
+                    if "12x" in self.instance_type:
+                        hub["SM_NUM_GPUS"] = json.dumps(4)
+                    elif "24x" in self.instance_type:
+                        hub["SM_NUM_GPUS"] = json.dumps(4)
+                    elif "48x" in self.instance_type:
+                        hub["SM_NUM_GPUS"] = json.dumps(4)
+                elif "p2" in self.instance_type:
+                    hub["SM_NUM_GPUS"] = json.dumps(1)
+                    if "8x" in self.instance_type:
+                        hub["SM_NUM_GPUS"] = json.dumps(8)
+                    elif "16x" in self.instance_type:
+                        hub["SM_NUM_GPUS"] = json.dumps(16)
+                elif "p3" in self.instance_type:
+                    hub["SM_NUM_GPUS"] = json.dumps(1)
+                    if "8x" in self.instance_type:
+                        hub["SM_NUM_GPUS"] = json.dumps(4)
+                    elif "16x" in self.instance_type:
+                        hub["SM_NUM_GPUS"] = json.dumps(8)
+                    elif "24x" in self.instance_type:
+                        hub["SM_NUM_GPUS"] = json.dumps(8)
+                elif "p4" in self.instance_type:
+                    hub["SM_NUM_GPUS"] = json.dumps(8)
+
+            if self.huggingface_model_quantize in ["bitsandbytes", "gptq"]:
+                hub["HF_MODEL_QUANTIZE"] = self.huggingface_model_quantize
+            elif self.huggingface_model_quantize is None:
                 pass
             else:
-                raise ValueError(f"huggingface_model_quantize needs to be one of bitsandbytes, gptq, not {self.huggingface_model_quantize}")
+                raise ValueError(
+                    f"huggingface_model_quantize needs to be one of bitsandbytes, gptq, not {self.huggingface_model_quantize}"
+                )
 
-        
-        
         aws_role = sagemaker.get_execution_role()
-        endpoint_name = name="hf-model-" + self.name
-        
+        endpoint_name = "hf-model-" + self.name
+
         # create Hugging Face Model Class
-        if not self.serverless and self.foundation_model and self.huggingface_model: #Basically just for large models
+        if (
+            not self.serverless and self.foundation_model and self.huggingface_model
+        ):  # Basically just for large models
             self.sagemakermodel = HuggingFaceModel(
-               image_uri=get_huggingface_llm_image_uri("huggingface"),
-               env=hub,                                                # configuration for loading model from Hub
-               role=aws_role,                                          # IAM role with permissions to create an endpoint
-               name=endpoint_name,
-               transformers_version="4.26",                             # Transformers version used
-               pytorch_version="1.13",                                  # PyTorch version used
-               py_version='py39',                                      # Python version used
+                image_uri=get_huggingface_llm_image_uri("huggingface"),
+                env=hub,  # configuration for loading model from Hub
+                role=aws_role,  # IAM role with permissions to create an endpoint
+                name=endpoint_name,
+                transformers_version="4.26",  # Transformers version used
+                pytorch_version="1.13",  # PyTorch version used
+                py_version="py39",  # Python version used
             )
         else:
             self.sagemakermodel = HuggingFaceModel(
-                env=hub,                      # configuration for loading model from Hub
-                role=aws_role,                    # iam role with permissions to create an Endpoint
+                env=hub,  # configuration for loading model from Hub
+                role=aws_role,  # iam role with permissions to create an Endpoint
                 transformers_version="4.26",  # transformers version used
-                pytorch_version="1.13",        # pytorch version used
-                py_version='py39',            # python version used
-                )
-    
+                pytorch_version="1.13",  # pytorch version used
+                py_version="py39",  # python version used
+            )
+
     def deploy_foundation_model(self):
         # Assume foundation model on Jumpstart here
 
-        
-        from sagemaker import image_uris, instance_types, model_uris, script_uris
+        from sagemaker import instance_types
+
         self.model = self.model[0]
         # print("self.model = ", self.model)
         instance_type = instance_types.retrieve_default(
-            model_id=self.model, model_version=self.foundation_model_version, scope="inference"
+            model_id=self.model,
+            model_version=self.foundation_model_version,
+            scope="inference",
         )
-        if self.instance_type == None:
+        if self.instance_type is None:
             self.instance_type = instance_type
         # self.costperhour = self.costdict[self.instance_type]
 
-        # Retrieve the inference docker container uri. 
+        # Retrieve the inference docker container uri.
         deploy_image_uri = sagemaker.image_uris.retrieve(
             region=None,
             framework=None,  # automatically inferred from model_id
             image_scope="inference",
             model_id=self.model,
             model_version=self.foundation_model_version,
             instance_type=instance_type,
         )
 
         # Retrieve the inference script uri. This includes all dependencies and scripts for model loading, inference handling etc.
         deploy_source_uri = sagemaker.script_uris.retrieve(
-            model_id=self.model, model_version=self.foundation_model_version, script_scope="inference"
+            model_id=self.model,
+            model_version=self.foundation_model_version,
+            script_scope="inference",
         )
+        print(f"deploy_source_uri: {deploy_source_uri}")
 
         # Retrieve the model uri.
         model_uri = sagemaker.model_uris.retrieve(
-            model_id=self.model, model_version=self.foundation_model_version, model_scope="inference"
+            model_id=self.model,
+            model_version=self.foundation_model_version,
+            model_scope="inference",
         )
         aws_role = sagemaker.get_execution_role()
         endpoint_name = "model-" + self.name
-        
+
         # Create the SageMaker model instance
         if self.model in _model_env_variable_map:
             # For those large models, we already repack the inference script and model
             # artifacts for you, so the `source_dir` argument to Model is not required.
-            
-            
+
             self.sagemakermodel = sagemaker.model.Model(
                 image_uri=deploy_image_uri,
                 model_data=model_uri,
                 role=aws_role,
                 predictor_cls=sagemaker.predictor.Predictor,
                 name=endpoint_name,
                 env=_model_env_variable_map[self.model],
             )
         else:
             from sagemaker.jumpstart.model import JumpStartModel
-            
-            self.sagemakermodel =  JumpStartModel(model_id = self.model,
-                                             model_version = self.foundation_model_version,
-                                             role=aws_role)
 
-            
-    def get_sagemaker_session(self,local_download_dir='src') -> sagemaker.Session:
+            self.sagemakermodel = JumpStartModel(
+                model_id=self.model,
+                model_version=self.foundation_model_version,
+                role=aws_role,
+            )
+
+    def get_sagemaker_session(self, local_download_dir="src") -> sagemaker.Session:
         """Return the SageMaker session."""
 
         sagemaker_client = boto3.client(
             service_name="sagemaker", region_name=boto3.Session().region_name
         )
 
         session_settings = sagemaker.session_settings.SessionSettings(
@@ -424,20 +458,20 @@
 
         # the unit test will ensure you do not commit this change
         session = sagemaker.session.Session(
             sagemaker_client=sagemaker_client, settings=session_settings
         )
 
         return session
-        
+
     def process_instance_type(self):
         # ------ instance checks --------
         self.instancedict = {}
-    
-        if self.instance_type == None:
+
+        if self.instance_type is None:
             # ------ load instance types dict ---------
             instancetypepath = pkg_resources.resource_filename(
                 "ezsmdeploy", "data/instancetypes.csv"
             )
             with open(instancetypepath, mode="r") as infile:
                 reader = csv.reader(infile)
                 for rows in reader:  # memGb / vcpu, cost, cost/memGb-per-vcpu
@@ -447,22 +481,21 @@
                         self.costdict[rows[0]] / float(rows[2]) / (2 * float(rows[1])),
                     )
 
             # ------ auto instance selection ---------
             self.choose_instance_type()
 
         else:
-
             if (self.instance_type in list(self.costdict.keys())) or (
                 self.instance_type in ["local", "local_gpu"]
             ):
                 if self.instance_type not in ["local", "local_gpu"]:
                     self.costperhour = self.costdict[self.instance_type]
 
-                    if self.ei != None:
+                    if self.ei is not None:
                         eicosts = {
                             "ml.eia2.medium": 0.12,
                             "ml.eia2.large": 0.24,
                             "ml.eia2.xlarge": 0.34,
                             "ml.eia.medium": 0.13,
                             "ml.eia.large": 0.26,
                             "ml.eia.xlarge": 0.52,
@@ -476,21 +509,21 @@
                     "Please choose an instance type in",
                     list(self.costdict.keys()),
                     ", or choose local for local testing.",
                 )
 
     def choose_instance_type(self):
         # TO DO : add heuristic for auto selection of instance size
-        
-        if self.prefix =='':
+
+        if self.prefix == "":
             tmppath = "ezsmdeploy/model-" + self.name + "/"
         else:
-            tmppath = self.prefix+"/ezsmdeploy/model-" + self.name + "/"
+            tmppath = self.prefix + "/ezsmdeploy/model-" + self.name + "/"
 
-        size = self.get_size(self.bucket, tmppath )
+        size = self.get_size(self.bucket, tmppath)
 
         self.instancetypespath = pkg_resources.resource_filename(
             "ezsmdeploy", "data/instancetypes.csv"
         )
 
         # Assume you need at least 4 workers, each model is deployed redundantly to every vcpu.
         # So we base this decision on memory available per vcpu. If model is being downloaded from a hub
@@ -502,64 +535,61 @@
         choseninstance = None
         mincost = 1000
 
         for instance in list(self.instancedict.keys()):
             # cost and memory per worker
             memperworker = self.instancedict[instance][0]
             cost = self.instancedict[instance][1]
-            costpermem = self.instancedict[instance][2]
+            self.instancedict[instance][2]
             #
             if self.budget == 100:
                 # even though budget is unlimited, minimize cost
                 if memperworker > size and cost < mincost:
                     mincost = cost
                     choseninstance = instance
                     # print("instance ={}, size={}, memperworker={}, choseninstance = {}, mincost = {}".format(instance, size, memperworker, choseninstance,mincost))
             else:
                 if memperworker > size and cost <= self.budget:
                     choseninstance = instance
                     break
 
-        if choseninstance == None and self.budget != 100:
+        if choseninstance is None and self.budget != 100:
             raise ValueError(
                 "Could not find an instance that satisfies your budget of "
                 + str(self.budget)
                 + " per hour and can host your models with a total size of "
                 + str(size)
                 + " Gb. Please choose a higher budget per hour."
             )
-        elif choseninstance == None and self.budget == 100:
+        elif choseninstance is None and self.budget == 100:
             raise ValueError(
                 "You may be using large models with a total size of "
                 + str(size)
                 + " Gb. Please choose a high memory GPU instance and launch without multiple models (if applicable)"
             )
 
         self.instance_type = choseninstance
 
         self.costperhour = self.costdict[self.instance_type]
 
     def add_model(self, s3path, relativepath):
         self.sagemakermodel.add_model(s3path, relativepath)
 
     def create_model(self):
-
         if not self.multimodel:
-
             self.sagemakermodel = Model(
                 name="model-" + self.name,
                 model_data=self.modelpath[0],
                 image_uri=self.image,
                 role=sagemaker.get_execution_role(),
                 # sagemaker_session=self.session,
                 predictor_cls=sagemaker.predictor.Predictor,
             )
 
         else:
-
             self.sagemakermodel = MultiDataModel(
                 name="model-" + self.name,
                 model_data_prefix="/".join(self.modelpath[0].split("/")[:-1]) + "/",
                 image_uri=self.image,
                 role=sagemaker.get_execution_role(),
                 # sagemaker_session=self.session,
                 predictor_cls=sagemaker.predictor.Predictor,
@@ -567,86 +597,85 @@
 
             for path in self.modelpath:
                 self.add_model(path, "serving/")
 
             self.ei = False
 
     def deploy_model(self):
-
         if self.monitor:
             from sagemaker.model_monitor import DataCaptureConfig
-            
-            
-            if self.prefix == '':
+
+            if self.prefix == "":
                 tmps3uri = "s3://{}/ezsmdeploy/model-{}/datacapture".format(
                     self.bucket, self.name
                 )
             else:
                 tmps3uri = "s3://{}/{}/ezsmdeploy/model-{}/datacapture".format(
                     self.bucket, self.prefix, self.name
                 )
-            
+
             data_capture_config = DataCaptureConfig(
                 enable_capture=True,
                 sampling_percentage=100,
-                destination_s3_uri=tmps3uri
+                destination_s3_uri=tmps3uri,
             )
         else:
             data_capture_config = None
-        
+
         if self.instance_type is not None:
             volume_size = None
-            if "p3" in self.instance_type or "p4" in self.instance_type or "16x" in self.instance_type or "24x" in self.instance_type or "48x" in self.instance_type or self.foundation_model:
-                volume_size = 256 
-            
+            if (
+                "p3" in self.instance_type
+                or "p4" in self.instance_type
+                or "16x" in self.instance_type
+                or "24x" in self.instance_type
+                or "48x" in self.instance_type
+                or self.foundation_model
+            ):
+                volume_size = 256
+
             if "g5" in self.instance_type:
                 volume_size = None
-                    
+
         else:
-            volume_size = None 
-            
-        
+            volume_size = None
+
         if self.foundation_model and not self.huggingface_model:
             # deploy the Model. Note that we need to pass Predictor class when we deploy model through Model class,
             # for being able to run inference through the sagemaker API.
 
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 # predictor_cls=sagemaker.predictor.Predictor, # Have to remove this since the new JumpstartModel SDK fails
                 endpoint_name="ezsm-foundation-endpoint-" + self.name,
                 volume_size=volume_size,
                 # serverless_inference_config=self.serverless_config, #ignoring serverless inference
-                wait=self.wait
+                wait=self.wait,
             )
         elif self.foundation_model and self.huggingface_model:
-            
-            
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 endpoint_name="ezsm-hf-endpoint-" + self.name,
                 volume_size=volume_size,
                 wait=self.wait,
                 container_startup_health_check_timeout=300,
             )
-            
+
         elif self.huggingface_model and not self.foundation_model:
-            
-            
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 endpoint_name="ezsm-hf-endpoint-" + self.name,
                 volume_size=volume_size,
                 serverless_inference_config=self.serverless_config,
-                wait=self.wait
+                wait=self.wait,
             )
-                
-            
+
         else:
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 accelerator_type=self.ei,
                 endpoint_name="ezsm-endpoint-" + self.name,
                 update_endpoint=False,
@@ -667,15 +696,15 @@
         for obj in my_bucket.objects.filter(Prefix=path):
             total_size = total_size + obj.size
 
         return total_size / ((1024.0) ** 3)
 
     def upload_model(self):
         i = 1
-        if self.prefix == '':
+        if self.prefix == "":
             tmppath = "ezsmdeploy/model-"
         else:
             tmppath = self.prefix + "/ezsmdeploy/model-"
         self.modelpath = []
         for name in self.model:
             self.modelpath.append(
                 self.session.upload_data(
@@ -683,38 +712,35 @@
                     bucket=self.bucket,
                     key_prefix=tmppath + self.name,
                 )
             )
             i += 1
 
     def tar_model(self):
-
         i = 1
         for name in self.model:
-
-            if "tar.gz" in name and 's3' in name:
+            if "tar.gz" in name and "s3" in name:
                 # download and uncompress
                 self.session.download_data(
                     path="./downloads/{}".format(i),
                     bucket=name.split("/")[2],
                     key_prefix="/".join(name.split("/")[3:]),
                 )
-                
+
                 with tarfile.open(
                     glob.glob("./downloads/{}/*.tar.gz".format(i))[0]
                 ) as tar:
                     tar.extractall("./extractedmodel/{}/".format(i))
 
                 name = "extractedmodel/{}/".format(i)
-                
-            elif 'tar.gz' in name and 's3' not in name:
-                
+
+            elif "tar.gz" in name and "s3" not in name:
                 self.makedir_safe("./downloads/{}/".format(i))
                 shutil.copy(name, "./downloads/{}/".format(i))
-                
+
                 with tarfile.open(
                     glob.glob("./downloads/{}/*.tar.gz".format(i))[0]
                 ) as tar:
                     tar.extractall("./extractedmodel/{}/".format(i))
 
                 name = "extractedmodel/{}/".format(i)
 
@@ -723,15 +749,14 @@
                 tar.add(name, arcname=".")
             else:
                 tar.add(name)
             tar.close()
             i += 1
 
     def makedir_safe(self, directory):
-
         try:
             shutil.rmtree(directory)
         except:
             pass
 
         try:
             if not os.path.exists(directory):
@@ -761,39 +786,37 @@
             f.close()
 
         else:
             raise ValueError(
                 "pass in a path/to/requirements.txt or a list of requirements ['scikit-learn',...,...]"
             )
 
-
-
     def build_docker(self):
         cmd = "chmod +x src/build-docker.sh  & sudo ./src/build-docker.sh {}"
-        
-        with open('src/dockeroutput.txt', 'w') as f:
-            #print("Start process")
-            p = subprocess.Popen(cmd.format(self.name), stdout=f, shell=True)
-        
-        #print("process running in background")
-        
+
+        with open("src/dockeroutput.txt", "w") as f:
+            # print("Start process")
+            _ = subprocess.Popen(cmd.format(self.name), stdout=f, shell=True)
+
+        # print("process running in background")
+
         acct = (
             os.popen("aws sts get-caller-identity --query Account --output text")
             .read()
             .split("\n")[0]
         )
         region = os.popen("aws configure get region").read().split("\n")[0]
         self.image = "{}.dkr.ecr.{}.amazonaws.com/ezsmdeploy-image-{}".format(
             acct, region, self.name
         )
 
         while not os.path.exists("src/done.txt"):
             time.sleep(3)
-        
-        self.dockeroutput = "Please see src/dockeroutput.txt" 
+
+        self.dockeroutput = "Please see src/dockeroutput.txt"
 
     def autoscale_endpoint(self):
         response = boto3.client("sagemaker").describe_endpoint(
             EndpointName=self.endpoint_name
         )
 
         in1 = response["EndpointName"]
@@ -826,29 +849,26 @@
         )
 
         self.scalingresponse = response
 
     def test(
         self, input_data, target_model=None, usercount=10, hatchrate=5, timeoutsecs=5
     ):
-
-        if self.multimodel and target_model == None:
+        if self.multimodel and target_model is None:
             raise ValueError(
                 "since this is a multimodel endpoint, please pass in a target model that you wish to test"
             )
 
         if self.deployed:
-
             path1 = pkg_resources.resource_filename("ezsmdeploy", "data/smlocust.py")
             shutil.copy(path1, "src/smlocust.py")
 
             start = datetime.datetime.now()
 
             with yaspin(Spinners.point, color="green", text="") as sp:
-
                 sp.hide()
                 sp.write(
                     str(datetime.datetime.now() - start)
                     + " | Starting test with Locust"
                 )
                 sp.show()
 
@@ -869,15 +889,15 @@
                         )
 
                 pickle.dump(input_data, open("src/testdata.p", "wb"))
 
                 cmd = "locust -f src/smlocust.py --no-web -c {} -r {} --run-time {}s --csv=src/locuststats; touch src/testdone.txt".format(
                     usercount, hatchrate, timeoutsecs
                 )
-                p = os.system(cmd)
+                os.system(cmd)
                 while not os.path.exists("src/testdone.txt"):
                     time.sleep(3)
 
                 os.remove("src/testdone.txt")
 
                 sp.hide()
                 sp.write(
@@ -890,16 +910,15 @@
             raise ValueError("Deploy model to endpoint first before testing")
 
     def deploy(self):
         # print(self.__dict__)
         start = datetime.datetime.now()
 
         with yaspin(Spinners.point, color="green", text="") as sp:
-
-            if not (self.foundation_model or self.huggingface_model) :
+            if not (self.foundation_model or self.huggingface_model):
                 try:
                     shutil.rmtree("src/")
                 except:
                     pass
 
                 # compress model files
                 self.tar_model()
@@ -928,41 +947,42 @@
                 sp.show()
 
                 #                 if self.gpu and self.image == None:
                 #                     raise ValueError("The default container image used here is based on the multi-model server which does not support GPU instances. Please provide a docker image (ECR repository link) to proceed with model build and deployment.")
 
                 # else:
                 # handle requirements
-                if self.requirements == None:
+                if self.requirements is None:
                     rtext = (
                         str(datetime.datetime.now() - start)
                         + " | no additional requirements found"
                     )
                     self.makedir_safe("src")
                 else:
                     self.handle_requirements()
                     rtext = (
-                        str(datetime.datetime.now() - start) + " | added requirements file"
+                        str(datetime.datetime.now() - start)
+                        + " | added requirements file"
                     )
                 sp.hide()
                 sp.write(rtext)
                 sp.show()
 
                 # move script to src
                 shutil.copy(self.script, "src/transformscript.py")
                 sp.hide()
                 sp.write(str(datetime.datetime.now() - start) + " | added source file")
                 sp.show()
 
                 # ------ Dockerfile checks -------
-                if self.dockerfilepath == None and self.multimodel == True:
+                if self.dockerfilepath is None and self.multimodel is True:
                     self.dockerfilepath = pkg_resources.resource_filename(
                         "ezsmdeploy", "data/Dockerfile"
                     )
-                elif self.dockerfilepath == None and self.multimodel == False:
+                elif self.dockerfilepath is None and self.multimodel is False:
                     self.dockerfilepath = pkg_resources.resource_filename(
                         "ezsmdeploy", "data/Dockerfile_flask"
                     )
 
                 # move Dockerfile to src
                 shutil.copy(self.dockerfilepath, "src/Dockerfile")
                 sp.hide()
@@ -987,33 +1007,37 @@
                     shutil.copy(path2, "src/dockerd-entrypoint.py")
                     shutil.copy(path3, "src/build-docker.sh")
 
                     self.ei = None
 
                 else:
                     # Use Flask stack
-                    path1 = pkg_resources.resource_filename("ezsmdeploy", "data/nginx.conf")
+                    path1 = pkg_resources.resource_filename(
+                        "ezsmdeploy", "data/nginx.conf"
+                    )
                     path2 = pkg_resources.resource_filename(
                         "ezsmdeploy", "data/predictor.py"
                     )
                     path3 = pkg_resources.resource_filename("ezsmdeploy", "data/serve")
                     path4 = pkg_resources.resource_filename("ezsmdeploy", "data/train")
-                    path5 = pkg_resources.resource_filename("ezsmdeploy", "data/wsgi.py")
+                    path5 = pkg_resources.resource_filename(
+                        "ezsmdeploy", "data/wsgi.py"
+                    )
                     path6 = pkg_resources.resource_filename(
                         "ezsmdeploy", "data/build-docker.sh"
                     )
 
                     shutil.copy(path1, "src/nginx.conf")
                     shutil.copy(path2, "src/predictor.py")
                     shutil.copy(path3, "src/serve")
                     shutil.copy(path4, "src/train")
                     shutil.copy(path5, "src/wsgi.py")
                     shutil.copy(path6, "src/build-docker.sh")
 
-                    if self.gpu and self.ei != None:
+                    if self.gpu and self.ei is not None:
                         self.ei = None
                         sp.hide()
                         sp.write(
                             str(datetime.datetime.now() - start)
                             + " | Setting Elastic Inference \
                         to None since you selected a GPU instance"
                         )
@@ -1031,30 +1055,33 @@
                     sp.write(
                         str(datetime.datetime.now() - start)
                         + " | building docker container"
                     )
                     self.build_docker()
                     sp.hide()
                     sp.write(
-                        str(datetime.datetime.now() - start) + " | built docker container"
+                        str(datetime.datetime.now() - start)
+                        + " | built docker container"
                     )
                     sp.show()
 
                 # create sagemaker model
                 self.create_model()
             else:
                 if self.foundation_model and not self.huggingface_model:
                     self.deploy_foundation_model()
                 elif self.huggingface_model:
                     self.deploy_huggingface_model()
                 else:
-                    raise ValueError("Did not find model artifact, or foundation/huggingface model")
-                
+                    raise ValueError(
+                        "Did not find model artifact, or foundation/huggingface model"
+                    )
+
             sp.hide()
-            
+
             if not self.serverless:
                 sp.write(
                     str(datetime.datetime.now() - start)
                     + " | created model(s). Now deploying on "
                     + self.instance_type
                 )
             else:
@@ -1116,48 +1143,49 @@
                 os.remove("downloads")
                 os.remove("extractedmodel")
                 os.remove("tmpmodel")
             except:
                 pass
 
             return self.predictor
-        
+
     def chat(self):
         # if self.foundation_model and 'chat' in self.model or 'Chat' in self.model :
         OpenChatKitShell(
             predictor=self.predictor,
-            model_name = self.model,
+            model_name=self.model,
             max_new_tokens=128,
             do_sample=True,
             temperature=0.6,
-            top_k=40
+            top_k=40,
         ).cmdloop()
-        
+
         # else:
         #     print("Sorry, you can only use the chat functionality with gpt-neoxt-chat-base-20b or the RedPajama chat models for now")
 
 
-
-MEANINGLESS_WORDS = ['<pad>', '</s>', '<|endoftext|>']
+MEANINGLESS_WORDS = ["<pad>", "</s>", "<|endoftext|>"]
 PRE_PROMPT = """\
 Current Date: {}
 Current Time: {}
 
 """
 
+
 def clean_response(response):
     for word in MEANINGLESS_WORDS:
         response = response.replace(word, "")
     response = response.strip("\n")
     return response
 
+
 class Conversation:
     def __init__(self, human_id, bot_id):
-        cur_date = time.strftime('%Y-%m-%d')
-        cur_time = time.strftime('%H:%M:%S %p %Z')
+        cur_date = time.strftime("%Y-%m-%d")
+        cur_time = time.strftime("%H:%M:%S %p %Z")
 
         self._human_id = human_id
         self._bot_id = bot_id
         self._prompt = PRE_PROMPT.format(cur_date, cur_time)
 
     def push_context_turn(self, context):
         # for now, context is represented as a human turn
@@ -1184,28 +1212,33 @@
         return turns[-1]
 
     def get_raw_prompt(self):
         return self._prompt
 
     @classmethod
     def from_raw_prompt(cls, value):
-        self._prompt = value
-
+        cls._prompt = value
 
 
 class OpenChatKitShell(cmd.Cmd):
     intro = (
         "EzSMdeploy Openchatkit shell -  Type /help or /? to "
         "list commands. For example, type /quit to exit shell.\n"
     )
     prompt = ">>> "
     human_id = "<human>"
     bot_id = "<bot>"
 
-    def __init__(self, predictor: Predictor, model_name: str, cmd_queue: Optional[List[str]] = None, **kwargs):
+    def __init__(
+        self,
+        predictor: Predictor,
+        model_name: str,
+        cmd_queue: Optional[List[str]] = None,
+        **kwargs,
+    ):
         super().__init__()
         self.predictor = predictor
         self.model = model_name
         self.payload_kwargs = kwargs
         self.payload_kwargs["stopping_criteria"] = [self.human_id]
         if cmd_queue is not None:
             self.cmdqueue = cmd_queue
@@ -1216,36 +1249,37 @@
     def precmd(self, line):
         command = line[1:] if line.startswith("/") else "say " + line
         return command
 
     def do_say(self, arg):
         self.conversation.push_human_turn(arg)
         prompt = self.conversation.get_raw_prompt()
-        if 'neoxt-chat' in self.model:
+        if "neoxt-chat" in self.model:
             # For neoxt - chatbase - 20B
             payload = {"text_inputs": prompt, **self.payload_kwargs}
             response = self.predictor.predict(payload)
             output = response[0][0]["generated_text"][len(prompt) :]
-        elif '-Chat' in self.model or 'chat' in self.model: #for RedPajama chat models, experimental for other chat models like openchat/openchat
-            
-            payload = {"inputs":prompt,
-           "parameters":{"max_new_tokens":100}}
-            
-            
-            response = self.predictor.predict(payload) 
-            last = response[0]['generated_text'].rfind("\n<human>") #returns -1 if the human token hasn't been found yet, which works
-            output = response[0]["generated_text"][len(prompt) :last]
-            
+        elif (
+            "-Chat" in self.model or "chat" in self.model
+        ):  # for RedPajama chat models, experimental for other chat models like openchat/openchat
+            payload = {"inputs": prompt, "parameters": {"max_new_tokens": 100}}
+
+            response = self.predictor.predict(payload)
+            last = response[0]["generated_text"].rfind(
+                "\n<human>"
+            )  # returns -1 if the human token hasn't been found yet, which works
+            output = response[0]["generated_text"][len(prompt) : last]
+
         else:
             output = "I don't recognize the output from this chat model"
-            
+
         self.conversation.push_model_response(output)
         print(self.conversation.get_last_turn())
 
     def do_reset(self, arg):
         self.conversation = Conversation(self.human_id, self.bot_id)
 
     def do_hyperparameters(self, arg):
         print(f"Hyperparameters: {self.payload_kwargs}\n")
 
     def do_quit(self, arg):
-        return True
+        return True
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/Dockerfile` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 LABEL com.amazonaws.sagemaker.capabilities.accept-bind-to-port=true
 
 RUN apt -y update && apt -y upgrade && \
     apt-get -y install curl && \
     curl -sL https://deb.nodesource.com/setup_18.x | bash - && \
     apt install nodejs -y && \
     npm install -g @bazel/bazelisk
-    
+
 # Install necessary dependencies for MMS and SageMaker Inference Toolkit
 
 RUN apt-get update && \
     apt-get -y install --no-install-recommends \
     build-essential \
     ca-certificates \
     openjdk-8-jdk-headless \
@@ -22,15 +22,15 @@
     python3-pip \
     python3-setuptools \
     nginx \
     ca-certificates \
     curl \
     wget \
     vim \
-    && rm -rf /var/lib/apt/lists/* 
+    && rm -rf /var/lib/apt/lists/*
 
 RUN python3 -V
 RUN update-alternatives --install /usr/bin/python python /usr/bin/python3 1
 RUN update-alternatives --install /usr/local/bin/pip pip /usr/local/bin/pip3 1
 
 RUN pip3 install --upgrade pip
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/Dockerfile_flask` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/Dockerfile_flask`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ca-certificates \
     curl \
     wget \
     vim \
     gcc \
     libpq-dev \
     python3-wheel \
-    && rm -rf /var/lib/apt/lists/* 
+    && rm -rf /var/lib/apt/lists/*
 
 RUN pip3 install --upgrade pip
 RUN python3 -V
 # Here we get all python packages.
 RUN pip3 install wheel
 
 RUN pip3 --no-cache-dir install setuptools \
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/build-docker.sh` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/build-docker.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # The name of our algorithm
 algorithm_name=ezsmdeploy-image-$1
 
 echo "Building container ${algorithm_name}"
 
-cd src 
+cd src
 
 account=$(aws sts get-caller-identity --query Account --output text)
 
 # Get the region defined in the current configuration (default to us-west-2 if none defined)
 region=$(aws configure get region)
 
 fullname="${account}.dkr.ecr.${region}.amazonaws.com/${algorithm_name}"
@@ -32,14 +32,14 @@
 
 echo "Building locally"
 docker build -q -t ${algorithm_name} .
 docker tag ${algorithm_name} ${fullname}
 
 echo "Pushing"
 docker push ${fullname}
- 
+
 echo "${fullname}"
 
 # Have to do this because pythons subprocess for calling this script does not wait for it to finish. Tried various args to Popen
 sudo touch done.txt
 
-echo "SUCCESS"
+echo "SUCCESS"
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/conversation.py` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/conversation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import re
 import time
 
-MEANINGLESS_WORDS = ['<pad>', '</s>', '<|endoftext|>']
+MEANINGLESS_WORDS = ["<pad>", "</s>", "<|endoftext|>"]
 PRE_PROMPT = """\
 Current Date: {}
 Current Time: {}
 
 """
 
+
 def clean_response(response):
     for word in MEANINGLESS_WORDS:
         response = response.replace(word, "")
     response = response.strip("\n")
     return response
 
+
 class Conversation:
     def __init__(self, human_id, bot_id):
-        cur_date = time.strftime('%Y-%m-%d')
-        cur_time = time.strftime('%H:%M:%S %p %Z')
+        cur_date = time.strftime("%Y-%m-%d")
+        cur_time = time.strftime("%H:%M:%S %p %Z")
 
         self._human_id = human_id
         self._bot_id = bot_id
         self._prompt = PRE_PROMPT.format(cur_date, cur_time)
 
     def push_context_turn(self, context):
         # for now, context is represented as a human turn
@@ -48,8 +50,8 @@
         return turns[-1]
 
     def get_raw_prompt(self):
         return self._prompt
 
     @classmethod
     def from_raw_prompt(cls, value):
-        self._prompt = value
+        cls._prompt = value
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/cost.csv` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/cost.csv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 ml.g5.xlarge,1.408
 ml.g5.2xlarge,1.515
 ml.g5.4xlarge,2.03
 ml.g5.8xlarge,3.06
 ml.g5.12xlarge,7.09
 ml.g5.16xlarge,5.12
 ml.g5.24xlarge,10.18
-ml.g5.48xlarge,20.36
+ml.g5.48xlarge,20.36
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/dockerd-entrypoint.py` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/dockerd-entrypoint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+import os
+import shlex
 import subprocess
 import sys
-import shlex
-import os
-from retrying import retry
 from subprocess import CalledProcessError
+
+from retrying import retry
 from sagemaker_inference import model_server
 
 
 def _retry_if_error(exception):
     return isinstance(exception, CalledProcessError or OSError)
 
 
 @retry(stop_max_delay=1000 * 50, retry_on_exception=_retry_if_error)
 def _start_mms():
     # by default the number of workers per model is 1, but we can configure it through the
     # environment variable below if desired.
-    os.environ['SAGEMAKER_MODEL_SERVER_WORKERS'] = '2'
+    os.environ["SAGEMAKER_MODEL_SERVER_WORKERS"] = "2"
     model_server.start_model_server(
         handler_service="/home/model-server/model_handler.py:handle"
     )
 
 
 def main():
     if sys.argv[1] == "serve":
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/instancetypes.csv` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/instancetypes.csv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 ml.c5.18xlarge,72,144,2
 ml.m4.10xlarge,40,160,4
 ml.m5.12xlarge,48,192,4
 ml.m5d.12xlarge,48,192,4
 ml.m4.16xlarge,64,256,4
 ml.m5d.24xlarge,96,384,4
 ml.r5d.12xlarge,48,384,8
-ml.r5d.24xlarge,96,768,8
+ml.r5d.24xlarge,96,768,8
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/model_handler.py` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/model_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 """
 ModelHandler defines an example model handler for load and inference requests
 """
-from collections import namedtuple
-import glob
-import json
-import logging
-import os
-import re
-from transformscript import *
+
+from transformscript import load_model, predict
 
 
 class ModelHandler(object):
     """
     A sample Model handler implementation.
     """
 
@@ -25,15 +20,15 @@
         :param context: Initial context contains model server system properties.
         :return:
         """
         self.initialized = True
         properties = context.system_properties
         # Contains the url parameter passed to the load request
         model_dir = properties.get("model_dir")
-        gpu_id = properties.get("gpu_id")
+        properties.get("gpu_id")
 
         try:
             # Load model
             self.model = load_model(model_dir)
             print("loaded model!")
         except:
             print("could not load model!")
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/nginx.conf` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/nginx.conf`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   # defaults
 }
 
 http {
   include /etc/nginx/mime.types;
   default_type application/octet-stream;
   access_log /var/log/nginx/access.log combined;
-  
+
   upstream gunicorn {
     server unix:/tmp/gunicorn.sock;
   }
 
   server {
     listen 8080 deferred;
     client_max_body_size 25m;
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/predictor.py` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/predictor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 # This is the file that implements a flask server to do inferences. It's the file that you will modify to
 # implement the scoring for your own algorithm.
 
 import os
-import json
-import pickle
-from io import StringIO
-import sys
-import signal
-import traceback
 
 import flask
-
-from transformscript import *
+from transformscript import load_model, predict
 
 prefix = "/opt/ml/"
 model_path = os.path.join(prefix, "model")
 
 # A singleton for holding the model. This simply loads the model and holds it.
 # It has a predict function that does a prediction based on the model and the input data.
 
 
 class ScoringService(object):
     model = None  # Where we keep the model when it's loaded
 
     @classmethod
     def get_model(cls):
         """Get the model object for this instance, loading it if it's not already loaded."""
-        if cls.model == None:
+        if cls.model is None:
             cls.model = load_model(model_path)
         return cls.model
 
     @classmethod
     def predict(cls, input):
         """For the input, do the predictions and return them.
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/serve` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/serve`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/smlocust.py` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/data/smlocust.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from locust import Locust, between, TaskSet, events, task
-import os
-import sagemaker
-import time
 import json
 import pickle
 import sys
+import time
+
+import sagemaker
+from locust import Locust, TaskSet, between, events, task
 
 with open("src/locustdata.txt") as json_file:
     locustdata = json.load(json_file)
 
 endpoint_name = locustdata["endpoint_name"]
 p = sagemaker.predictor.RealTimePredictor(endpoint_name)
 target_model = locustdata["target_model"]
 input_data = pickle.load(open("src/testdata.p", "rb"))
 
-from locust import Locust, TaskSet, task, between
-
 
 class MyTaskSet(TaskSet):
     @task
     def my_task(self):
         start_time = time.time()
         try:
             if target_model == "":
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploy/modelscript_sklearn.py` & `ezsmdeploydev-1.99.dev0/ezsmdeploy/modelscript_sklearn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-import sklearn
-from joblib import load
-import numpy as np
 import os
 
-#Return loaded model
+import numpy as np
+from joblib import load
+
+
+# Return loaded model
 def load_model(modelpath):
     print(modelpath)
-    clf = load(os.path.join(modelpath,'model.joblib'))
+    clf = load(os.path.join(modelpath, "model.joblib"))
     print("loaded")
     return clf
 
+
 # return prediction based on loaded model (from the step above) and an input payload
 def predict(model, payload):
     print(type(payload))
     try:
         print(np.frombuffer(payload))
-        print(np.frombuffer(payload).reshape((1,64)))
-        print( model.predict(np.frombuffer(payload).reshape((1,64))) )
-        
-        out = model.predict(np.frombuffer(payload).reshape((1,64)))
-        
+        print(np.frombuffer(payload).reshape((1, 64)))
+        print(model.predict(np.frombuffer(payload).reshape((1, 64))))
+
+        out = model.predict(np.frombuffer(payload).reshape((1, 64)))
+
     except Exception as e:
-        out = [type(payload),str(e)] #useful for debugging!
-    
+        out = [type(payload), str(e)]  # useful for debugging!
+
     return out
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/PKG-INFO` & `ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploydev
-Version: 1.98.dev0
+Version: 1.99.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -32,16 +32,16 @@
 .. image:: https://img.shields.io/badge/Made%20With-Love-orange.svg
    :target: https://pypi.python.org/pypi/ezsmdeploy
    :alt: Made With Love
 
 .. image:: https://img.shields.io/badge/Gen-AI-8A2BE2
    :target: https://pypi.python.org/pypi/ezsmdeploy
    :alt: GenAI
-   
-   
+
+
 
 **Ezsmdeploy** python SDK helps you easily deploy Machine learning models on SageMaker. It provides a rich set of features such as deploying models from hubs (like Huggingface or SageMaker Jumpstart), passing one or more model files (even with multi-model deployments), automatically choosing an instance based on model size or based on a budget, and load testing endpoints using an intuitive API. **Ezsmdeploy** uses the SageMaker Python SDK, which is an open source library for training and deploying machine learning models on Amazon SageMaker. This SDK however focuses on further simplifying deployment from existing models, and as such, this is for you if:
 
 1.  you want to quickly deploy and try out foundational language models as an API powered by SageMaker (**New in v 2.0**)
 2.  you have a serialized model (a pickle / joblib/ json/ TF saved model/ Pytorch .pth/ etc) file and you want to deploy and test your model as an API endpoint
 3. you have a model or multiple models stored as local files, in local folders, or in S3 as tar files (model.tar.gz)
 4. you don't want to create a custom docker container for deployment and/or don't want to deal with docker
@@ -66,16 +66,16 @@
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
     - facebook/galactica-6.7b, ml.g5.16xlarge
     - CalderaAI/30B-Lazarus, ml.g5.16xlarge
     - huggyllama/llama-65b, ml.g5.16xlarge
     - ausboss/llama-30b-supercot, ml.g4dn.4xlarge
     - MetaIX/GPT4-X-Alpasta-30b, ml.g4dn.4xlarge
-    - 
-    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50) 
+    -
+    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50)
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -109,34 +109,34 @@
 
 Cleanest way to install this package is within a virtualenv:
 
 
 ::
 
     python -m venv env
-    
+
     source env/bin/activate
 
     pip install ezsmdeploy[locust]
 
 
 In some cases, installs fail due to an existing package installed called "greenlet". This is not a direct dependency of ezsmdeploy but interferes with the installation. To fix this, either install in a virtualenv as seen above, or do:
 
 ::
 
     pip install ezsmdeploy[locust] --ignore-installed greenlet
-    
-    
+
+
 If you have another way to test the endpoint, or want to manage locust on your own, just do:
 
 ::
 
     pip install ezsmdeploy
-    
-   
+
+
 
 Key Features
 ~~~~~~~~~~~~
 
 At minimum, **ezsmdeploy** requires you to provide:
 
 1. one or more model files
@@ -154,19 +154,19 @@
 
 You can also load multiple models ...
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = ['model1.pth','model2.pth'],
                   script = 'modelscript_pytorch.py',
-                  requirements = ['numpy','torch','joblib'])    
+                  requirements = ['numpy','torch','joblib'])
 
 ...  or download tar.gz models from S3
-:: 
-    
+::
+
     ezonsm = ezsmdeploy.Deploy(model = ['s3://ezsmdeploy/pytorchmnist/model.tar.gz'],
                   script = 'modelscript_pytorch.py',
                   requirements = 'path/to/requirements.txt')
 
 
 Other Features
 ~~~~~~~~~~~~~~~
@@ -198,30 +198,30 @@
     ):
 
 
 Let's take a look at each of these parameters and what they do:
 
 * You can skip passing in requirements through a file or a list if you choose a **"framework"** in ["tensorflow", "pytorch", "mxnet", "sklearn"]. If you do, these libraries are installed automatically. However it is expected that most people will not use this, given the limited installs, and will usually pass in a custom set of requirements.
 
- :: 
+ ::
 
     ezonsm = ezsmdeploy.Deploy(model = ... ,
                   script = ... ,
                   framework = 'sklearn')
 
 * Pass in a **"name"** if you want to override the random name generated by ezsmdeploy that is used to name your custom ECR image and the endpoint.
 
- :: 
+ ::
 
     ezonsm = ezsmdeploy.Deploy(model = ... ,
                   script = ... ,
                   framework = 'sklearn',
                   name = 'randomname')
-                      
-                      
+
+
 * Set **"autoscale"** to True if required to switch on autoscaling for your endpoint. By default, this sets up endpoint autoscaling with the metric *SageMakerVariantInvocationsPerInstance* and a target value of 1000. You can override this value by also passing in a value for autoscaletarget
 
 |
 
 * **"wait**" is set to True by default and can be set to False if you don't want to wait for the endpoint to deploy.
 
 |
@@ -230,19 +230,19 @@
 
 |
 
 * Pass in a sagemaker **"session"** to override the default session; for most cases this is not necessary. Also, this may interfere with local deployments as the same session cannot be used for tasks such as downloading and uploading files, and for local and remote deployments.
 
 |
 
-* If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in. 
+* If you already have a prebuild docker image, use the **"image"** argument or pass in a **"dockerfilepath"** if you want ezsmdeploy to use this image. Note that ezsmdeploy will automatically build a custom image with your requirements and the right deployment stack (flask-nginx or MMS) based on the arguments passed in.
 
 |
 
-* If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe. 
+* If you do not pass in an **"instance_type"**, ezsmdeploy will choose an instance based on the total size of the model (or multiple models passed in), take into account the multiple workers per endpoint, and also optionally a **"budget"** that will choose instance_type based on a maximum acceptible cost per hour. You can of course, choose an instance as well. We assume you need at least 4 workers and each model is deployed redundantly to every vcpu  available on the selected instance; this eliminates instance tupes with lower number of available vcpus to choose from. If model is being downloaded from a hub (like TF hub or Torch hub or NGC) one should ideally pass in an instance since we don't know the size of model. For all instances that have the same memory per vcpu, what is done to tie break is min (cost/total vpcus). Also 'd' instances are preferred to others for faster load times at the same cost since they have NvMe.
 
 |
 
 * Passing in an **"instance_count"** > 1 will change the initial number of instances that the model(s) is(are) deployed on.
 
 |
 
@@ -251,43 +251,43 @@
 |
 
 * Set **"monitor"** to True if you would like to turn on Datacapture for this endpoint. Currently, a sampling_percentage of 100 is used. Read more about Model monitor here - https://docs.aws.amazon.com/sagemaker/latest/dg/model-monitor.html
 
 |
 
 * You should see an output as follows for a typical deployment:
-    
+
  ::
 
    0:00:00.143132 | compressed model(s)
    0:00:00.403894 | uploaded model tarball(s) ; check returned modelpath
    0:00:00.404948 | added requirements file
    0:00:00.406745 | added source file
    0:00:00.408180 | added Dockerfile
    0:00:00.409959 | added model_handler and docker utils
    0:00:00.410072 | building docker container
    0:01:59.298091 | built docker container
    0:01:59.647986 | created model(s). Now deploying on ml.m5.xlarge
    0:09:31.904897 | deployed model
    0:09:31.905450 | estimated cost is $0.3 per hour
-   0:09:31.905805 | Done! ✔ 
+   0:09:31.905805 | Done! ✔
 
 
 * Once your model is deployed, you can use locust.io to load test your endpoint. The test reports the number of requests, number of failures, average, min, max response time in milliseconds and requests per second reached based on the number of parallel users and hatch rate entered. To load test your model (make sure you have deployed it remotely first), try:
- 
+
  ::
 
      ezonsm.test(input_data, target_model='model1.tar.gz')
- 
- or 
+
+ or
 
  ::
 
      ezonsm.test(input_data, target_model='model1.tar.gz',usercount=20,hatchrate=10,timeoutsecs=10)
-     
+
  ... to override default arguments. Read more about locust.io here https://docs.locust.io/en/stable/
 
 
 Model Script requirements
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Make sure your model script has a load_model() and predict() function. While you can still use sagemaker's serializers and deserializers, assume that you will get a payload in bytes, and that you have to return a prediction in bytes. What you do in between is up to you. For example, your model script may look like:
@@ -300,15 +300,15 @@
 
     def predict(model, payload):
         try:
             # in remote / container based deployment, payload comes in as a stream of bytes
             out = [str(model.predict(np.frombuffer(payload[0]['body']).reshape((1,64))))]
         except Exception as e:
            out = [type(payload),str(e)] #useful for debugging!
-    
+
     return out
 
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
 Large Language models
@@ -325,30 +325,30 @@
 
 To deploy models using Jumpstart:
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
                                foundation_model=True)
-                               
-Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker                               
+
+Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker
 
 
 
 To deploy a huggingface LLM model (this uses the huggingface llm container):
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "tiiuae/falcon-40b-instruct",
                                foundation_model=True,
                                huggingface_model=True,
                                huggingface_model_task='text-generation',
                                instance_type="ml.g4dn.12xlarge"
                                )
-                               
+
 (See release notes for models we have tested so far with instances that worked)
 
 Note that at the time of writing this, officially supported model architectures for LLMs on Huggingface are currently:
 
     - BLOOM / BLOOMZ
     - MT0-XXL
     - Galactica
@@ -396,15 +396,15 @@
 You can read more about which permissions are necessary in the `AWS Documentation <https://docs.aws.amazon.com/sagemaker/latest/dg/sagemaker-roles.html>`__.
 
 The SageMaker Python SDK should not require any additional permissions aside from what is required for using SageMaker.
 However, if you are using an IAM role with a path in it, you should grant permission for ``iam:GetRole``.
 
 Licensing
 ~~~~~~~~~
-Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/ 
+Ezsmdeploy is licensed under the MIT license and uses the SageMaker Python SDK. SageMaker Python SDK is licensed under the Apache 2.0 License. It is copyright 2018 Amazon.com, Inc. or its affiliates. All Rights Reserved. The license is available at: http://aws.amazon.com/apache2.0/
 
 Sample Notebooks
 ~~~~~~~~~~~~~~~~~
 https://github.com/aws-samples/easy-amazon-sagemaker-deployments/tree/master/notebooks
 
 Known Gotchas
 ~~~~~~~~~~~~~~~~~~
@@ -420,15 +420,15 @@
 
 |
 
 * Ezsmdeploy uses Locust to do endpoint testing - any restrictions of the locustio package are also expected to be seen here.
 
 |
 
-* Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU). 
+* Ezsmdeploy has been tested from Sagemaker notebook instances (both GPU and non-GPU).
 
 |
 
 * The payload comes in as bytes; you can also use Sagemaker's serializer and deserializers to send in other formats of input data
 
 |
 
@@ -448,15 +448,15 @@
 
     docker system prune -a
 
 * If you encounter an "image does not exist" error, try running this script that exists after an unsuccessful run, but manually. For this, do:
 
 ::
 
-   ./src/build-docker.sh 
+   ./src/build-docker.sh
 
 * Locust load testing on local endpoint has not been tested (and may not make much sense). Please use the .test() for remote deployment
 
 |
 
 * Use instance_type "local" if you would like to test locally (this lets you test using the MMS stack). If you intend to finally deploy your model to a GPU instance, use "local_gpu" - this launches the flask-nginx stack locally and the same stack when you deploy to a GPU.
 
@@ -465,10 +465,7 @@
 * At the time of writing this guide, launching a multi-model server from sagemaker does not support GPUs (but the open source MMS repository has no such restrictions). Ezsmdeploy checks the number of models passed in, the instance type and other parameters to decide which stack to build for your endpoint.
 
 
 CONTRIBUTING
 ------------
 
 Please submit a pull request to the packages git repo
-
-
-
```

### Comparing `ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/SOURCES.txt` & `ezsmdeploydev-1.99.dev0/ezsmdeploydev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

