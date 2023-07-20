# Comparing `tmp/clearml_session-0.6.0-py3-none-any.whl.zip` & `tmp/clearml_session-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 40551 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-05 05:49 clearml_session/__init__.py
--rw-r--r--  2.0 unx    52386 b- defN 23-Jul-05 05:49 clearml_session/__main__.py
--rw-r--r--  2.0 unx    37840 b- defN 23-Jul-05 05:49 clearml_session/interactive_session_task.py
--rw-r--r--  2.0 unx     4781 b- defN 23-Jul-05 05:49 clearml_session/single_thread_proxy.py
--rw-r--r--  2.0 unx    15948 b- defN 23-Jul-05 05:49 clearml_session/tcp_proxy.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-05 05:49 clearml_session/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    18143 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/RECORD
-12 files, 141712 bytes uncompressed, 38745 bytes compressed:  72.7%
+Zip file size: 40930 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 09:12 clearml_session/__init__.py
+-rw-r--r--  2.0 unx    53262 b- defN 23-Jul-20 09:12 clearml_session/__main__.py
+-rw-r--r--  2.0 unx    39023 b- defN 23-Jul-20 09:12 clearml_session/interactive_session_task.py
+-rw-r--r--  2.0 unx     4781 b- defN 23-Jul-20 09:12 clearml_session/single_thread_proxy.py
+-rw-r--r--  2.0 unx    15948 b- defN 23-Jul-20 09:12 clearml_session/tcp_proxy.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-20 09:12 clearml_session/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-20 09:12 clearml_session-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18517 b- defN 23-Jul-20 09:12 clearml_session-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 09:12 clearml_session-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 23-Jul-20 09:12 clearml_session-0.7.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-20 09:12 clearml_session-0.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-20 09:12 clearml_session-0.7.0.dist-info/RECORD
+12 files, 144145 bytes uncompressed, 39124 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: clearml_session/tcp_proxy.py
 Comment: 
 
 Filename: clearml_session/version.py
 Comment: 
 
-Filename: clearml_session-0.6.0.dist-info/LICENSE
+Filename: clearml_session-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: clearml_session-0.6.0.dist-info/METADATA
+Filename: clearml_session-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: clearml_session-0.6.0.dist-info/WHEEL
+Filename: clearml_session-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: clearml_session-0.6.0.dist-info/entry_points.txt
+Filename: clearml_session-0.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: clearml_session-0.6.0.dist-info/top_level.txt
+Filename: clearml_session-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: clearml_session-0.6.0.dist-info/RECORD
+Filename: clearml_session-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clearml_session/__main__.py

```diff
@@ -533,14 +533,16 @@
             task_params['properties/external_ssh_port'] = remote_gateway_parts[1]
     task_params['{}/ssh_server'.format(section)] = str(True)
     task_params["{}/jupyterlab".format(section)] = bool(state.get('jupyter_lab'))
     task_params["{}/vscode_server".format(section)] = bool(state.get('vscode_server'))
     task_params["{}/public_ip".format(section)] = bool(state.get('public_ip'))
     task_params["{}/ssh_ports".format(section)] = state.get('remote_ssh_port') or ''
     task_params["{}/vscode_version".format(section)] = state.get('vscode_version') or ''
+    task_params["{}/vscode_extensions".format(section)] = state.get('vscode_extensions') or ''
+    task_params["{}/force_dropbear".format(section)] = bool(state.get('force_dropbear'))
     if state.get('user_folder'):
         task_params['{}/user_base_directory'.format(section)] = state.get('user_folder')
     docker = state.get('docker') or task.get_base_docker()
     if not state.get('skip_docker_network') and not docker:
         docker = default_docker_image
     if docker:
         task_params['{}/default_docker'.format(section)] = docker.replace('--network host', '').strip()
@@ -692,15 +694,15 @@
 
     return task
 
 
 def start_ssh_tunnel(username, remote_address, ssh_port, ssh_password, local_remote_pair_list, debug=False):
     print('Starting SSH tunnel to {}@{}, port {}'.format(username, remote_address, ssh_port))
     child = None
-    args = ['-N', '-C',
+    args = ['-C',
             '{}@{}'.format(username, remote_address), '-p', '{}'.format(ssh_port),
             '-o', 'UserKnownHostsFile=/dev/null',
             '-o', 'Compression=yes',
             '-o', 'StrictHostKeyChecking=no',
             '-o', 'ServerAliveInterval=10',
             '-o', 'ServerAliveCountMax=10', ]
 
@@ -713,15 +715,16 @@
     # noinspection PyBroadException
     try:
         child = pexpect.spawn(
             command=_check_ssh_executable(),
             args=args,
             logfile=fd, timeout=20, encoding='utf-8')
 
-        i = child.expect([r'(?i)password:', r'\(yes\/no\)', r'.*[$#] ', pexpect.EOF])
+        # Match only "(yes/no" in order to handle both (yes/no) and (yes/no/[fingerprint])
+        i = child.expect([r'(?i)password:', r'\(yes\/no', r'.*[$#] ', pexpect.EOF])
         if i == 0:
             child.sendline(ssh_password)
             try:
                 child.expect([r'(?i)password:'], timeout=5)
                 print('{}Error: incorrect password'.format(fd.read() + '\n' if debug else ''))
                 ssh_password = input('Please enter password manually: ')
                 child.sendline(ssh_password)
@@ -941,14 +944,18 @@
                         help='Set the remote ssh server port, running on the agent`s machine. (default: 10022)')
     parser.add_argument('--vscode-server', default=True, nargs='?', const='true', metavar='true/false',
                         type=lambda x: (str(x).strip().lower() in ('true', 'yes')),
                         help='Install vscode server (code-server) on interactive session (default: true)')
     parser.add_argument('--vscode-version', type=str, default=None,
                         help='Set vscode server (code-server) version, as well as vscode python extension version '
                              '<vscode:python-ext> (example: "3.7.4:2020.10.332292344")')
+    parser.add_argument('--vscode-extensions', type=str, default=None,
+                        help='Install additional vscode extensions, as well as vscode python extension '
+                             '(example: "ms-python.python,ms-python.black-formatter,'
+                             'ms-python.pylint,ms-python.flake8")')
     parser.add_argument('--jupyter-lab', default=True, nargs='?', const='true', metavar='true/false',
                         type=lambda x: (str(x).strip().lower() in ('true', 'yes')),
                         help='Install Jupyter-Lab on interactive session (default: true)')
     parser.add_argument('--git-credentials', default=False, nargs='?', const='true', metavar='true/false',
                         type=lambda x: (str(x).strip().lower() in ('true', 'yes')),
                         help='If true, local .git-credentials file is sent to the interactive session. '
                              '(default: false)')
@@ -990,21 +997,24 @@
                              '(assumes k8s network ingestion) (default: false)')
     parser.add_argument('--password', type=str, default=None,
                         help='Advanced: Select ssh password for the interactive session '
                              '(default: `randomly-generated` or previously used one)')
     parser.add_argument('--username', type=str, default=None,
                         help='Advanced: Select ssh username for the interactive session '
                              '(default: `root` or previously used one)')
+    parser.add_argument('--force_dropbear', default=None, nargs='?', const='true', metavar='true/false',
+                        type=lambda x: (str(x).strip().lower() in ('true', 'yes')),
+                        help='Force using `dropbear` instead of SSHd')
     parser.add_argument('--verbose', action='store_true', default=None,
                         help='Advanced: If set, print verbose progress information, '
                              'e.g. the remote machine setup process log')
-    parser.add_argument("--yes", "-y",
-                        action="store_true", default=False,
-                        help="Automatic yes to prompts; assume \"yes\" as answer "
-                             "to all prompts and run non-interactively",)
+    parser.add_argument('--yes', '-y',
+                        action='store_true', default=False,
+                        help='Automatic yes to prompts; assume \"yes\" as answer '
+                             'to all prompts and run non-interactively',)
 
 
 def get_version():
     from .version import __version__
     return __version__
 
 
@@ -1137,19 +1147,19 @@
     # a single running session
     if len(running_task_ids_created) == 1:
         task_id = running_task_ids_created[0][0]
         if assume_yes:
             print("{} active session {}".format(verb, task_id))
         else:
             choice = input("{} active session id={} [Y]/n? ".format(question_verb, task_id))
-            if str(choice).strip().lower() in ("y", "yes"):
+            if str(choice).strip().lower() in ("", "y", "yes"):
                 return Task.get_task(task_id=task_id)
 
     # multiple sessions running
-    print('Active sessions:')
+    print("{} active session:".format(verb))
     try:
         prev_task_id = state.get('task_id')
         default_i = next(i for i, (tid, _, _) in enumerate(running_task_ids_created) if prev_task_id == tid)
     except StopIteration:
         default_i = None
 
     session_list = "\n".join(
```

## clearml_session/interactive_session_task.py

```diff
@@ -245,16 +245,16 @@
 
 def start_vscode_server(hostname, hostnames, param, task, env):
     if not param.get("vscode_server"):
         return
 
     # get vscode version and python extension version
     # they are extremely flaky, this combination works, most do not.
-    vscode_version = '3.12.0'
-    python_ext_version = '2021.10.1365161279'
+    vscode_version = '4.14.1'
+    python_ext_version = '2023.12.0'
     if param.get("vscode_version"):
         vscode_version_parts = param.get("vscode_version").split(':')
         vscode_version = vscode_version_parts[0]
         if len(vscode_version_parts) > 1:
             python_ext_version = vscode_version_parts[1]
 
     # make a copy of env and remove the pythonpath from it.
@@ -262,15 +262,15 @@
     env.pop('PYTHONPATH', None)
 
     python_ext_download_link = \
         os.environ.get("CLEARML_SESSION_VSCODE_PY_EXT") or \
         'https://github.com/microsoft/vscode-python/releases/download/{}/ms-python-release.vsix'
     code_server_deb_download_link = \
         os.environ.get("CLEARML_SESSION_VSCODE_SERVER_DEB") or \
-        'https://github.com/cdr/code-server/releases/download/v{version}/code-server_{version}_amd64.deb'
+        'https://github.com/coder/code-server/releases/download/v{version}/code-server_{version}_amd64.deb'
 
     pre_installed = False
     python_ext = None
 
     # find a free tcp port
     port = get_free_port(9000, 9100)
 
@@ -334,26 +334,48 @@
             user_folder = os.path.expanduser("~/.local/share/code-server/")
             if not os.path.isdir(user_folder):
                 user_folder = None
                 exts_folder = None
             else:
                 exts_folder = os.path.expanduser("~/.local/share/code-server/extensions/")
         else:
+            vscode_extensions = param.get("vscode_extensions") or ""
+            vscode_extensions_cmd = []
+            jupyter_ext_version = True
+            for ext in vscode_extensions.split(","):
+                ext = ext.strip()
+                if not ext:
+                    continue
+
+                if ext.startswith("ms-python.python"):
+                    python_ext_version = python_ext = None
+                elif ext.startswith("ms-toolsai.jupyter"):
+                    jupyter_ext_version = None
+
+                vscode_extensions_cmd += ["--install-extension", ext]
+
+            if python_ext:
+                vscode_extensions_cmd += ["--install-extension", "{}".format(python_ext)]
+            elif python_ext_version:
+                vscode_extensions_cmd += ["--install-extension", "ms-python.python@{}".format(python_ext_version)]
+
+            if jupyter_ext_version:
+                vscode_extensions_cmd += ["--install-extension", "ms-toolsai.jupyter"]
+
+            print("VScode extensions: {}".format(vscode_extensions_cmd))
             subprocess.Popen(
                 [
                     vscode_path,
                     "--auth",
                     "none",
                     "--bind-addr",
                     "127.0.0.1:{}".format(port),
                     "--user-data-dir", user_folder,
                     "--extensions-dir", exts_folder,
-                    "--install-extension", "ms-toolsai.jupyter",
-                    # "--install-extension", "donjayamanne.python-extension-pack"
-                ] + ["--install-extension", "ms-python.python@{}".format(python_ext_version)] if python_ext else [],
+                ] + vscode_extensions_cmd,
                 env=env,
                 stdout=fd,
                 stderr=fd,
             )
 
         if user_folder:
             settings = Path(os.path.expanduser(os.path.join(user_folder, 'User/settings.json')))
@@ -393,14 +415,15 @@
             error_code = proc.wait(timeout=1)
             raise ValueError("code-server failed starting, return code {}".format(error_code))
         except subprocess.TimeoutExpired:
             pass
 
     except Exception as ex:
         print('Failed running vscode server: {}'.format(ex))
+        task.set_parameter(name='properties/vscode_port', value=str(-1))
         return
 
     task.set_parameter(name='properties/vscode_port', value=str(port))
 
 
 def start_jupyter_server(hostname, hostnames, param, task, env):
     if not param.get('jupyterlab', True):
@@ -471,18 +494,18 @@
     # noinspection PyBroadException
     try:
         ssh_port = param.get("ssh_ports") or "10022:15000"
         min_port = int(ssh_port.split(":")[0])
         max_port = max(min_port+32, int(ssh_port.split(":")[-1]))
         port = get_free_port(min_port, max_port)
         proxy_port = get_free_port(min_port, max_port)
-        use_dropbear = False
+        use_dropbear = bool(param.get("force_dropbear", False))
 
         # if we are root, install open-ssh
-        if os.geteuid() == 0:
+        if not use_dropbear and os.geteuid() == 0:
             # noinspection SpellCheckingInspection
             os.system(
                 "export PYTHONPATH=\"\" && "
                 "([ ! -z $(which sshd) ] || (apt-get update ; apt-get install -y openssh-server)) && "
                 "mkdir -p /var/run/sshd && "
                 "echo 'root:{password}' | chpasswd && "
                 "echo 'PermitRootLogin yes' >> /etc/ssh/sshd_config && "
@@ -531,15 +554,15 @@
                         'https://github.com/allegroai/dropbear/releases/download/DROPBEAR_CLEARML_2023.02/dropbearmulti'
                     dropbear = StorageManager.get_local_copy(dropbear_download_link, extract_archive=False)
                     os.chmod(dropbear, 0o744)
                     sshd_path = dropbear
                     use_dropbear = True
 
                 except Exception:
-                    print('Error: failed locating SSHd and dailed fetching `dropbear`, leaving!')
+                    print('Error: failed locating SSHd and failed fetching `dropbear`, leaving!')
                     return
 
             # noinspection PyBroadException
             try:
                 ssh_config_path = os.path.join(os.getcwd(), '.clearml_session_sshd')
                 # noinspection PyBroadException
                 try:
@@ -584,35 +607,36 @@
             except Exception:  # noqa
                 pass
             if v:
                 with open(filename, 'wt') as f:
                     f.write(v + (' {}@{}'.format(
                         getpass.getuser() or "root", hostname) if filename.endswith('.pub') else ''))
                 os.chmod(filename, 0o600 if filename.endswith('.pub') else 0o600)
-            keys_filename[k] = filename
+                keys_filename[k] = filename
 
         # run server in foreground so it gets killed with us
         if use_dropbear:
             # convert key files
             dropbear_key_files = []
             for k, ssh_key_file in keys_filename.items():
                 # skip over the public keys, there is no need for them
-                if ssh_key_file.endswith(".pub"):
+                if not ssh_key_file or ssh_key_file.endswith(".pub"):
                     continue
                 drop_key_file = ssh_key_file + ".dropbear"
                 try:
                     os.system("{} dropbearconvert openssh dropbear {} {}".format(
                         sshd_path, ssh_key_file, drop_key_file))
                     if Path(drop_key_file).is_file():
                         dropbear_key_files += ["-r", drop_key_file]
                 except Exception:
                     pass
             proc_args = [sshd_path, "dropbear", "-e", "-K", "30", "-I", "0", "-F", "-p", str(port)] + dropbear_key_files
-            # this is a copy oof `env` so there is nothing to worry about
-            env["DROPBEAR_CLEARML_FIXED_PASSWORD"] = ssh_password
+            # this is a copy of `env` so there is nothing to worry about
+            if ssh_password:
+                env["DROPBEAR_CLEARML_FIXED_PASSWORD"] = ssh_password
         else:
             proc_args = [sshd_path, "-D", "-p", str(port)] + (["-f", custom_ssh_conf] if custom_ssh_conf else [])
 
         proc = subprocess.Popen(args=proc_args, env=env)
         # noinspection PyBroadException
         try:
             result = proc.wait(timeout=1)
@@ -704,16 +728,18 @@
 
     # create symbolic link to the venv
     environment = os.path.expanduser('~/environment')
     # noinspection PyBroadException
     try:
         os.symlink(os.path.abspath(os.path.join(os.path.abspath(sys.executable), '..', '..')), environment)
         print('Virtual environment are available at {}'.format(environment))
-    except Exception:
-        pass
+    except Exception as e:
+        print("Error: Exception while trying to create symlink. The Application will continue...")
+        print(e)
+
     # set default user credentials
     if param.get("user_key") and param.get("user_secret"):
         os.system("echo 'export CLEARML_API_ACCESS_KEY=\"{}\"' >> ~/.bashrc".format(
             param.get("user_key", "").replace('$', '\\$')))
         os.system("echo 'export CLEARML_API_SECRET_KEY=\"{}\"' >> ~/.bashrc".format(
             param.get("user_secret", "").replace('$', '\\$')))
         os.system("echo 'export CLEARML_DOCKER_IMAGE=\"{}\"' >> ~/.bashrc".format(
@@ -883,17 +909,19 @@
         "ssh_server": True,
         "ssh_password": "training",
         "default_docker": "nvidia/cuda",
         "user_key": None,
         "user_secret": None,
         "vscode_server": True,
         "vscode_version": '',
+        "vscode_extensions": '',
         "jupyterlab": True,
         "public_ip": False,
         "ssh_ports": None,
+        "force_dropbear": False,
     }
     task = init_task(param, default_ssh_fingerprint)
 
     run_user_init_script(task)
 
     hostname, hostnames = get_host_name(task, param)
```

## clearml_session/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.6.0'
+__version__ = '0.7.0'
```

## Comparing `clearml_session-0.6.0.dist-info/LICENSE` & `clearml_session-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clearml_session-0.6.0.dist-info/METADATA` & `clearml_session-0.7.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearml-session
-Version: 0.6.0
+Version: 0.7.0
 Summary: clearml-session - CLI for launching JupyterLab / VSCode on a remote machine
 Home-page: https://github.com/allegroai/clearml-session
 Author: Allegroai
 Author-email: clearml@allegro.ai
 License: Apache License 2.0
 Keywords: clearml mlops devops trains development machine deep learning version control machine-learning machinelearning deeplearning deep-learning experiment-manager jupyter vscode
 Platform: UNKNOWN
@@ -198,17 +198,15 @@
 ### Shutting down a remote session
 
 On the `clearml-session` CLI terminal, enter 'shutdown' (case-insensitive)
 It will shut down the remote session, free the resource and close the CLI
 
 ``` console
 Enter "r" (or "reconnect") to reconnect the session (for example after suspend)
-Ctrl-C (or "quit") to abort (remote session rema
-Yes of course, current SSO supports Google/GitHub/BitBucket/... + SAML/LDAP (Usually with user permissions fully integrated to the LDAP)
-ins active)
+Ctrl-C (or "quit") to abort (remote session remains active)
 or "Shutdown" to shutdown remote interactive session
 
 shutdown
 
 Shutting down interactive session
 Interactive session ended
 Leaving interactive session
@@ -254,28 +252,30 @@
                        [--shutdown [SHUTDOWN]]
                        [--debugging-session DEBUGGING_SESSION] [--queue QUEUE]
                        [--docker DOCKER] [--docker-args DOCKER_ARGS]
                        [--public-ip [true/false]]
                        [--remote-ssh-port REMOTE_SSH_PORT]
                        [--vscode-server [true/false]]
                        [--vscode-version VSCODE_VERSION]
+                       [--vscode-extensions VSCODE_EXTENSIONS]
                        [--jupyter-lab [true/false]]
                        [--git-credentials [true/false]]
                        [--user-folder USER_FOLDER]
                        [--packages [PACKAGES [PACKAGES ...]]]
                        [--requirements REQUIREMENTS]
                        [--init-script [INIT_SCRIPT]]
                        [--config-file CONFIG_FILE]
                        [--remote-gateway [REMOTE_GATEWAY]]
                        [--base-task-id BASE_TASK_ID] [--project PROJECT]
                        [--keepalive [true/false]]
                        [--queue-excluded-tag [QUEUE_EXCLUDED_TAG [QUEUE_EXCLUDED_TAG ...]]]
                        [--queue-include-tag [QUEUE_INCLUDE_TAG [QUEUE_INCLUDE_TAG ...]]]
                        [--skip-docker-network] [--password PASSWORD]
-                       [--username USERNAME] [--verbose] [--yes]
+                       [--username USERNAME] [--force_dropbear [true/false]]
+                       [--verbose] [--yes]
 
 clearml-session - CLI for launching JupyterLab / VSCode on a remote machine
 
 optional arguments:
   -h, --help            show this help message and exit
   --version             Display the clearml-session utility version
   --attach [ATTACH]     Attach to running interactive session (default:
@@ -307,14 +307,19 @@
   --vscode-server [true/false]
                         Install vscode server (code-server) on interactive
                         session (default: true)
   --vscode-version VSCODE_VERSION
                         Set vscode server (code-server) version, as well as
                         vscode python extension version <vscode:python-ext>
                         (example: "3.7.4:2020.10.332292344")
+  --vscode-extensions VSCODE_EXTENSIONS
+                        Install additional vscode extensions, as well as
+                        vscode python extension (example: "ms-
+                        python.python,ms-python.black-formatter,ms-
+                        python.pylint,ms-python.flake8")
   --jupyter-lab [true/false]
                         Install Jupyter-Lab on interactive session (default:
                         true)
   --git-credentials [true/false]
                         If true, local .git-credentials file is sent to the
                         interactive session. (default: false)
   --user-folder USER_FOLDER
@@ -361,14 +366,16 @@
                         to docker (assumes k8s network ingestion) (default:
                         false)
   --password PASSWORD   Advanced: Select ssh password for the interactive
                         session (default: `randomly-generated` or previously
                         used one)
   --username USERNAME   Advanced: Select ssh username for the interactive
                         session (default: `root` or previously used one)
+  --force_dropbear [true/false]
+                        Force using `dropbear` instead of SSHd
   --verbose             Advanced: If set, print verbose progress information,
                         e.g. the remote machine setup process log
   --yes, -y             Automatic yes to prompts; assume "yes" as answer to
                         all prompts and run non-interactively
 
 Notice! all arguments are stored as new defaults for the next session
 ```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clearml-session Version: 0.6.0 Summary: clearml-
+Metadata-Version: 2.1 Name: clearml-session Version: 0.7.0 Summary: clearml-
 session - CLI for launching JupyterLab / VSCode on a remote machine Home-page:
 https://github.com/allegroai/clearml-session Author: Allegroai Author-email:
 clearml@allegro.ai License: Apache License 2.0 Keywords: clearml mlops devops
 trains development machine deep learning version control machine-learning
 machinelearning deeplearning deep-learning experiment-manager jupyter vscode
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
@@ -118,94 +118,96 @@
 ``` bash clearml-session ``` Then press "Y" (or enter) to reconnect to the
 already running session ``` console clearml-session - launch interactive
 session Checking previous session Connect to active session
 id=3d38e738c5ff458a9ec465e77e19da23 [Y]/n? ``` ### Shutting down a remote
 session On the `clearml-session` CLI terminal, enter 'shutdown' (case-
 insensitive) It will shut down the remote session, free the resource and close
 the CLI ``` console Enter "r" (or "reconnect") to reconnect the session (for
-example after suspend) Ctrl-C (or "quit") to abort (remote session rema Yes of
-course, current SSO supports Google/GitHub/BitBucket/... + SAML/LDAP (Usually
-with userÂ permissionsÂ fully integrated to the LDAP) ins active) or "Shutdown"
-to shutdown remote interactive session shutdown Shutting down interactive
-session Interactive session ended Leaving interactive session ``` ###
-Connecting to a running interactive session from a different machine Continue
-working on an interactive session from **any** machine. In the `clearml` web
-UI, go to DevOps project, and find your interactive session. Click on the ID
-button next to the Task name, and copy the unique ID. ``` bash clearml-session
---attach  ``` Click on the JupyterLab/VSCode link, or connect directly to the
-SSH session ### Debug a previously executed experiment If you have a previously
-executed experiment in the system, you can create an exact copy of the
-experiment and debug it on the remote interactive session. `clearml-session`
-will replicate the exact remote environment, add JupyterLab/VSCode/SSH and
-allow you interactively execute and debug the experiment, on the allocated
-remote machine. In the `clearml` web UI, find the experiment (Task) you wish to
-debug. Click on the ID button next to the Task name, and copy the unique ID.
-``` bash clearml-session --debugging-session  ``` Click on the JupyterLab/
-VSCode link, or connect directly to the SSH session ## CLI options ``` bash
-clearml-session --help ``` ``` console clearml-session - CLI for launching
-JupyterLab / VSCode on a remote machine usage: clearml-session [-h] [--version]
-[--attach [ATTACH]] [--shutdown [SHUTDOWN]] [--debugging-session
+example after suspend) Ctrl-C (or "quit") to abort (remote session remains
+active) or "Shutdown" to shutdown remote interactive session shutdown Shutting
+down interactive session Interactive session ended Leaving interactive session
+``` ### Connecting to a running interactive session from a different machine
+Continue working on an interactive session from **any** machine. In the
+`clearml` web UI, go to DevOps project, and find your interactive session.
+Click on the ID button next to the Task name, and copy the unique ID. ``` bash
+clearml-session --attach  ``` Click on the JupyterLab/VSCode link, or connect
+directly to the SSH session ### Debug a previously executed experiment If you
+have a previously executed experiment in the system, you can create an exact
+copy of the experiment and debug it on the remote interactive session.
+`clearml-session` will replicate the exact remote environment, add JupyterLab/
+VSCode/SSH and allow you interactively execute and debug the experiment, on the
+allocated remote machine. In the `clearml` web UI, find the experiment (Task)
+you wish to debug. Click on the ID button next to the Task name, and copy the
+unique ID. ``` bash clearml-session --debugging-session  ``` Click on the
+JupyterLab/VSCode link, or connect directly to the SSH session ## CLI options
+``` bash clearml-session --help ``` ``` console clearml-session - CLI for
+launching JupyterLab / VSCode on a remote machine usage: clearml-session [-h]
+[--version] [--attach [ATTACH]] [--shutdown [SHUTDOWN]] [--debugging-session
 DEBUGGING_SESSION] [--queue QUEUE] [--docker DOCKER] [--docker-args
 DOCKER_ARGS] [--public-ip [true/false]] [--remote-ssh-port REMOTE_SSH_PORT] [--
-vscode-server [true/false]] [--vscode-version VSCODE_VERSION] [--jupyter-lab
-[true/false]] [--git-credentials [true/false]] [--user-folder USER_FOLDER] [--
-packages [PACKAGES [PACKAGES ...]]] [--requirements REQUIREMENTS] [--init-
-script [INIT_SCRIPT]] [--config-file CONFIG_FILE] [--remote-gateway
-[REMOTE_GATEWAY]] [--base-task-id BASE_TASK_ID] [--project PROJECT] [--
-keepalive [true/false]] [--queue-excluded-tag [QUEUE_EXCLUDED_TAG
-[QUEUE_EXCLUDED_TAG ...]]] [--queue-include-tag [QUEUE_INCLUDE_TAG
-[QUEUE_INCLUDE_TAG ...]]] [--skip-docker-network] [--password PASSWORD] [--
-username USERNAME] [--verbose] [--yes] clearml-session - CLI for launching
-JupyterLab / VSCode on a remote machine optional arguments: -h, --help show
-this help message and exit --version Display the clearml-session utility
-version --attach [ATTACH] Attach to running interactive session (default:
-previous session) --shutdown [SHUTDOWN], -S [SHUTDOWN] Shut down an active
-session (default: previous session) --debugging-session DEBUGGING_SESSION Pass
-existing Task id (experiment), create a copy of the experiment on a remote
-machine, and launch jupyter/ssh for interactive access. Example --debugging-
-session  --queue QUEUE Select the queue to launch the interactive session on
-(default: previously used queue) --docker DOCKER Select the docker image to use
-in the interactive session on (default: previously used docker image or
-`nvidia/cuda:10.1-runtime-ubuntu18.04`) --docker-args DOCKER_ARGS Add
-additional arguments for the docker image to use in the interactive session on
-(default: previously used docker-args) --public-ip [true/false] If True
-register the public IP of the remote machine. Set if running on the cloud.
-Default: false (use for local / on-premises) --remote-ssh-port REMOTE_SSH_PORT
-Set the remote ssh server port, running on the agent`s machine. (default:
-10022) --vscode-server [true/false] Install vscode server (code-server) on
-interactive session (default: true) --vscode-version VSCODE_VERSION Set vscode
-server (code-server) version, as well as vscode python extension version
-(example: "3.7.4:2020.10.332292344") --jupyter-lab [true/false] Install
-Jupyter-Lab on interactive session (default: true) --git-credentials [true/
-false] If true, local .git-credentials file is sent to the interactive session.
-(default: false) --user-folder USER_FOLDER Advanced: Set the remote base folder
-(default: ~/) --packages [PACKAGES [PACKAGES ...]] Additional packages to add,
-supports version numbers (default: previously added packages). examples: --
-packages torch==1.7 tqdm --requirements REQUIREMENTS Specify requirements.txt
-file to install when setting the interactive session. Requirements file is read
-and stored in `packages` section as default for the next sessions. Can be
-overridden by calling `--packages` --init-script [INIT_SCRIPT] Specify BASH
-init script file to be executed when setting the interactive session. Script
-content is read and stored as default script for the next sessions. To clear
-the init-script do not pass a file --config-file CONFIG_FILE Advanced: Change
-the configuration file used to store the previous state (default:
-~/.clearml_session.json) --remote-gateway [REMOTE_GATEWAY] Advanced: Specify
-gateway ip/address:port to be passed to interactive session (for use with k8s
-ingestion / ELB) --base-task-id BASE_TASK_ID Advanced: Set the base task ID for
-the interactive session. (default: previously used Task). Use `none` for the
-default interactive session --project PROJECT Advanced: Set the project name
-for the interactive session Task --keepalive [true/false] Advanced: If set,
-enables the transparent proxy always keeping the sockets alive. Default: False,
-do not use transparent socket for mitigating connection drops. --queue-
-excluded-tag [QUEUE_EXCLUDED_TAG [QUEUE_EXCLUDED_TAG ...]] Advanced: Excluded
-queues with this specific tag from the selection --queue-include-tag
-[QUEUE_INCLUDE_TAG [QUEUE_INCLUDE_TAG ...]] Advanced: Only include queues with
-this specific tag from the selection --skip-docker-network Advanced: If set, `-
--network host` is **not** passed to docker (assumes k8s network ingestion)
-(default: false) --password PASSWORD Advanced: Select ssh password for the
-interactive session (default: `randomly-generated` or previously used one) --
-username USERNAME Advanced: Select ssh username for the interactive session
-(default: `root` or previously used one) --verbose Advanced: If set, print
-verbose progress information, e.g. the remote machine setup process log --yes,
--y Automatic yes to prompts; assume "yes" as answer to all prompts and run non-
-interactively Notice! all arguments are stored as new defaults for the next
-session ```
+vscode-server [true/false]] [--vscode-version VSCODE_VERSION] [--vscode-
+extensions VSCODE_EXTENSIONS] [--jupyter-lab [true/false]] [--git-credentials
+[true/false]] [--user-folder USER_FOLDER] [--packages [PACKAGES [PACKAGES
+...]]] [--requirements REQUIREMENTS] [--init-script [INIT_SCRIPT]] [--config-
+file CONFIG_FILE] [--remote-gateway [REMOTE_GATEWAY]] [--base-task-id
+BASE_TASK_ID] [--project PROJECT] [--keepalive [true/false]] [--queue-excluded-
+tag [QUEUE_EXCLUDED_TAG [QUEUE_EXCLUDED_TAG ...]]] [--queue-include-tag
+[QUEUE_INCLUDE_TAG [QUEUE_INCLUDE_TAG ...]]] [--skip-docker-network] [--
+password PASSWORD] [--username USERNAME] [--force_dropbear [true/false]] [--
+verbose] [--yes] clearml-session - CLI for launching JupyterLab / VSCode on a
+remote machine optional arguments: -h, --help show this help message and exit -
+-version Display the clearml-session utility version --attach [ATTACH] Attach
+to running interactive session (default: previous session) --shutdown
+[SHUTDOWN], -S [SHUTDOWN] Shut down an active session (default: previous
+session) --debugging-session DEBUGGING_SESSION Pass existing Task id
+(experiment), create a copy of the experiment on a remote machine, and launch
+jupyter/ssh for interactive access. Example --debugging-session  --queue QUEUE
+Select the queue to launch the interactive session on (default: previously used
+queue) --docker DOCKER Select the docker image to use in the interactive
+session on (default: previously used docker image or `nvidia/cuda:10.1-runtime-
+ubuntu18.04`) --docker-args DOCKER_ARGS Add additional arguments for the docker
+image to use in the interactive session on (default: previously used docker-
+args) --public-ip [true/false] If True register the public IP of the remote
+machine. Set if running on the cloud. Default: false (use for local / on-
+premises) --remote-ssh-port REMOTE_SSH_PORT Set the remote ssh server port,
+running on the agent`s machine. (default: 10022) --vscode-server [true/false]
+Install vscode server (code-server) on interactive session (default: true) --
+vscode-version VSCODE_VERSION Set vscode server (code-server) version, as well
+as vscode python extension version  (example: "3.7.4:2020.10.332292344") --
+vscode-extensions VSCODE_EXTENSIONS Install additional vscode extensions, as
+well as vscode python extension (example: "ms- python.python,ms-python.black-
+formatter,ms- python.pylint,ms-python.flake8") --jupyter-lab [true/false]
+Install Jupyter-Lab on interactive session (default: true) --git-credentials
+[true/false] If true, local .git-credentials file is sent to the interactive
+session. (default: false) --user-folder USER_FOLDER Advanced: Set the remote
+base folder (default: ~/) --packages [PACKAGES [PACKAGES ...]] Additional
+packages to add, supports version numbers (default: previously added packages).
+examples: --packages torch==1.7 tqdm --requirements REQUIREMENTS Specify
+requirements.txt file to install when setting the interactive session.
+Requirements file is read and stored in `packages` section as default for the
+next sessions. Can be overridden by calling `--packages` --init-script
+[INIT_SCRIPT] Specify BASH init script file to be executed when setting the
+interactive session. Script content is read and stored as default script for
+the next sessions. To clear the init-script do not pass a file --config-file
+CONFIG_FILE Advanced: Change the configuration file used to store the previous
+state (default: ~/.clearml_session.json) --remote-gateway [REMOTE_GATEWAY]
+Advanced: Specify gateway ip/address:port to be passed to interactive session
+(for use with k8s ingestion / ELB) --base-task-id BASE_TASK_ID Advanced: Set
+the base task ID for the interactive session. (default: previously used Task).
+Use `none` for the default interactive session --project PROJECT Advanced: Set
+the project name for the interactive session Task --keepalive [true/false]
+Advanced: If set, enables the transparent proxy always keeping the sockets
+alive. Default: False, do not use transparent socket for mitigating connection
+drops. --queue-excluded-tag [QUEUE_EXCLUDED_TAG [QUEUE_EXCLUDED_TAG ...]]
+Advanced: Excluded queues with this specific tag from the selection --queue-
+include-tag [QUEUE_INCLUDE_TAG [QUEUE_INCLUDE_TAG ...]] Advanced: Only include
+queues with this specific tag from the selection --skip-docker-network
+Advanced: If set, `--network host` is **not** passed to docker (assumes k8s
+network ingestion) (default: false) --password PASSWORD Advanced: Select ssh
+password for the interactive session (default: `randomly-generated` or
+previously used one) --username USERNAME Advanced: Select ssh username for the
+interactive session (default: `root` or previously used one) --force_dropbear
+[true/false] Force using `dropbear` instead of SSHd --verbose Advanced: If set,
+print verbose progress information, e.g. the remote machine setup process log -
+-yes, -y Automatic yes to prompts; assume "yes" as answer to all prompts and
+run non-interactively Notice! all arguments are stored as new defaults for the
+next session ```
```

