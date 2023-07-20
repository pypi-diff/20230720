# Comparing `tmp/abin_sim-1.1.4.tar.gz` & `tmp/abin_sim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abin_sim-1.1.4.tar", max compression
+gzip compressed data, was "abin_sim-1.2.0.tar", max compression
```

## Comparing `abin_sim-1.1.4.tar` & `abin_sim-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 2023-07-14 14:26:11.781594 abin_sim-1.1.4/LICENSE
--rw-r--r--   0        0        0     8594 2023-07-14 14:26:11.781594 abin_sim-1.1.4/README.md
--rw-r--r--   0        0        0       21 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/__init__.py
--rw-r--r--   0        0        0     8435 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/cli.py
--rw-r--r--   0        0        0      194 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/config.py
--rw-r--r--   0        0        0     1174 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/core/file_manager.py
--rw-r--r--   0        0        0     5836 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/core/functions.py
--rw-r--r--   0        0        0     1190 2023-07-14 14:26:11.781594 abin_sim-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-07-20 21:06:42.333963 abin_sim-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8594 2023-07-20 21:06:42.333963 abin_sim-1.2.0/README.md
+-rw-r--r--   0        0        0       21 2023-07-20 21:06:42.333963 abin_sim-1.2.0/abin_sim/__init__.py
+-rw-r--r--   0        0        0     9288 2023-07-20 21:06:42.333963 abin_sim-1.2.0/abin_sim/cli.py
+-rw-r--r--   0        0        0      194 2023-07-20 21:06:42.337963 abin_sim-1.2.0/abin_sim/config.py
+-rw-r--r--   0        0        0     2063 2023-07-20 21:06:42.337963 abin_sim-1.2.0/abin_sim/core/file_manager.py
+-rw-r--r--   0        0        0     6603 2023-07-20 21:06:42.337963 abin_sim-1.2.0/abin_sim/core/functions.py
+-rw-r--r--   0        0        0     1190 2023-07-20 21:06:42.337963 abin_sim-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.2.0/PKG-INFO
```

### Comparing `abin_sim-1.1.4/README.md` & `abin_sim-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.4/abin_sim/cli.py` & `abin_sim-1.2.0/abin_sim/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from rich.table import Table
 from rich.tree import Tree
 from typer import Context, Exit, Option, Typer
 
 from abin_sim import __version__
 
 from .config import settings
-from .core.file_manager import make_return
+from .core.file_manager import make_envjs, make_return
 from .core.functions import (
     convert_to_json,
     get_environment,
     get_metadata,
     get_secret,
     make_conf,
+    query_yes_no,
     update_secret,
 )
 
 console = Console()
 app = Typer()
 
 
@@ -88,23 +89,23 @@
 def get(
     app: str = Option(
         ...,
         help='Nome da aplicação que deseja recuperar os secrets.',
     ),
     env: str = Option(
         ...,
-        help='Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main).'
+        help='Ambiente da aplicação que deseja recuperar (Envs: local, dev, qa, main).'
     ),
     proj: str = Option(
         ...,
-        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua)'
+        help='Projeto que deseja conectar para recuperar os secrets (Projs: sim, charrua)'
     ),
     file: bool = Option(
         True,
-        help='Cria um arquivo .env para armazenar os secrets.',
+        help='Grava em arquivo os secrets do Vault.',
     ),
 ):
     vault_token = settings.params.vault_token
     vault_url = settings.params.vault_url
     metadata = get_metadata(app, env, proj, vault_token, vault_url)
     if not 'Erro' in metadata:
         if file == None or file == False:
@@ -112,55 +113,70 @@
                 secret = get_secret(app, env, proj, conf, vault_token, vault_url)
                 console.print(f'--- {conf} ---')
                 console.print(secret)
                 console.print('\n')
         else:
             for conf in metadata:
                 secret = get_secret(app, env, proj, conf, vault_token, vault_url)
+                if conf == 'env' and 'front' in app: conf_envjs = secret
                 if 'Erro' not in secret:
                     conf_file = make_return(env, secret, settings.params.path, conf)
-            # if conf_file['LocalEnvJS']:
+            if 'front' in app:
+                location_envjs = query_yes_no(f'Será gerado o arquivo env.js em {settings.params.path}src/assets. Local existe?', 'yes')
+                if location_envjs:
+                    envjs = make_envjs(conf_envjs, settings.params.path)
+                else:
+                    console.print('Crie a pasta e rode novamente o métdo GET para gerar o env.js.')
             if conf_file['Status']:
+                if 'front' in app and location_envjs:
+                    if envjs['Status']:
+                        console.print(f'Arquivo env.js salvo em:\n {"-> " + settings.params.path+"src/assets/"}')
                 console.print(f'{app} secrets salvos em:\n {"-> " + settings.params.path if conf_file["ConfFiles"] else ""} {"-> " + settings.params.path+"src/assets/" if conf_file["EnvJS"] else ""}')
             else:
                 console.print(conf_file['Message'])
     else:
         console.print(f'Erro ao buscar metadata -> {metadata}')
 
 @app.command('update')
 def update(
     app: str = Option(
         ...,
         help='Nome da aplicação que deseja recuperar os secrets.',
     ),
     env: str = Option(
         ...,
-        help='Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main).'
+        help='Ambiente da aplicação que deseja recuperar (Envs: local, dev, qa, main).'
     ),
     proj: str = Option(
         ...,
-        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua)'
+        help='Projeto que deseja conectar para recuperar os secrets (Projs: sim, charrua)'
     ),
     secret: str = Option(
         default='env',
         help='Secret que será atualizada no Vault (Ex.: env, gcp.json, config.yaml ...)',
     ),
     file: str = Option(
         ...,
-        help='Arquivo com variárias de ambiente',
+        help='Arquivo que será enviado ao Vault',
     ),
 ):
     vault_token = settings.params.vault_token
     vault_url = settings.params.vault_url
     if secret == 'env':
         payload = convert_to_json(file)
     else:
         payload = file
-    ret = update_secret(app, env, proj, secret, vault_token, vault_url, payload)
-    console.print(ret)
+
+    confirm = query_yes_no(f'Gostaria de atualizar a secret "{secret}" para o app {app}, no projeto {env.upper()}-{proj.upper()} ?', 'no')
+    if confirm:
+        ret = update_secret(app, env, proj, secret, vault_token, vault_url, payload)
+        console.print(ret)
+    else:
+        console.print({'Status': 'Canceled'})
+    
 
 @app.command('list')
 def list():
     vault_environment = get_environment(settings.params.vault_token, settings.params.vault_url)
     console.print('''
 ╭─ [i]Referência[/i] ──────────────────────╮
 
@@ -178,23 +194,23 @@
     
     console.print(tree)
 
 @app.command('compare')
 def compare(
     app: str = Option(
         ...,
-        help='Nome da aplicação que deseja recuperar os secrets.',
+        help='Nome da aplicação que deseja comparar os secrets.',
     ),
     env: str = Option(
         ...,
-        help='Ambiente da aplicação que deseja recuperar (Envs possíveis: dev, qa, main).'
+        help='Dois ambientes, separados por vírgula, que deseja comparar (Envs: local, dev, qa, main).'
     ),
     proj: str = Option(
         ...,
-        help='Projeto que deseja conectar para recuperar os secrets (Projs possíveis: sim, charrua)'
+        help='Projeto que deseja conectar para comparar os secrets (Projs: sim, charrua)'
     ),
 ):
     # envs = []
     envs_a = []
     envs_b = []
     envs = env.split(',')
     if len(envs) == 2:
@@ -236,8 +252,8 @@
     counter = len(envs_a_diff) if len(envs_a_diff) > len(envs_b_diff) else len(envs_b_diff)
     for num in range(0, counter):
         if 0 <= num < len(envs_a_diff): value_a = str(envs_a_diff[num])
         else: value_a = ''
         if 0 <= num < len(envs_b_diff): value_b = str(envs_b_diff[num])
         else: value_b = ''
         tbl_diferences.add_row(value_a, value_b, style='red')
-    console.print(tbl_envs, tbl_diferences)
+    console.print(tbl_envs, tbl_diferences)
```

### Comparing `abin_sim-1.1.4/abin_sim/core/functions.py` & `abin_sim-1.2.0/abin_sim/core/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 from os import environ
+from sys import stdout
 
 import requests
 from pathlib3x import Path
 
 # def qualquer(valor: str) -> str:
 #     if valor == 'a':
 #         dado = 'VOCE PASSOU A'
@@ -67,15 +68,15 @@
 
     contentList = [x.strip().split('^#')[0].split('=', 1) for x in content if '=' in x.split('^#')[0]]
     contentDict = dict(contentList)
     for k, v in contentList:
         # for i, x in enumerate(v.split('$')[1:]):
         #     key = re.findall(r'\w+', x)[0]
         #     v = v.replace('$' + key, contentDict[key])
-        if '=' in v:
+        if '=' in v or '$' in v and not "'" in v:
             contentDict[k] = f"'{v.strip()}'"
         else:
             contentDict[k] = v.strip()
 
     return json.dumps(contentDict)
 
 def replace_string(secret, search, replace):
@@ -183,8 +184,32 @@
             if paths_response.status_code == 200:
                 paths_metadata[path] = paths_response.json()['data']['keys']
             
         retorno = paths_metadata
     else:
         retorno = {'Status': f'Erro: {mounts.text}'}
     
-    return retorno
+    return retorno
+
+def query_yes_no(
+    question: str, 
+    default: str
+) -> str:
+    valid = {"yes": True, "y": True, "ye": True, "no": False, "n": False}
+    if default is None:
+        prompt = " [y/n] "
+    elif default == "yes":
+        prompt = " [Y/n] "
+    elif default == "no":
+        prompt = " [y/N] "
+    else:
+        raise ValueError("invalid default answer: '%s'" % default)
+
+    while True:
+        stdout.write(f'{question} {prompt}')
+        choice = input().lower()
+        if default is not None and choice == "":
+            return valid[default]
+        elif choice in valid:
+            return valid[choice]
+        else:
+            stdout.write("Please respond with 'yes' or 'no' " "(or 'y' or 'n').\n")
```

### Comparing `abin_sim-1.1.4/pyproject.toml` & `abin_sim-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abin-sim"
-version = "1.1.4"
+version = "1.2.0"
 description = "ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech"
 license = "BeerWare"
 authors = ["Bonatto <andrebonatto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "abin_sim"}]
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `abin_sim-1.1.4/PKG-INFO` & `abin_sim-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abin-sim
-Version: 1.1.4
+Version: 1.2.0
 Summary: ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech
 License: Beerware
 Author: Bonatto
 Author-email: andrebonatto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

