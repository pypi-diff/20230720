# Comparing `tmp/faraday_agent_dispatcher-2.6.0.tar.gz` & `tmp/faraday_agent_dispatcher-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faraday_agent_dispatcher-2.6.0.tar", last modified: Fri Jul  7 20:12:50 2023, max compression
+gzip compressed data, was "faraday_agent_dispatcher-2.6.1.tar", last modified: Thu Jul 20 15:15:19 2023, max compression
```

## Comparing `faraday_agent_dispatcher-2.6.0.tar` & `faraday_agent_dispatcher-2.6.1.tar`

### file list

```diff
@@ -1,345 +1,348 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.816641 faraday_agent_dispatcher-2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     2366 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.758642 faraday_agent_dispatcher-2.6.0/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.768642 faraday_agent_dispatcher-2.6.0/.gitlab/ci/
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/.pre-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/.rules-conditions.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.768642 faraday_agent_dispatcher-2.6.0/.gitlab/ci/build_ci/
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/build_ci/.build-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/fetch-secrets.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.768642 faraday_agent_dispatcher-2.6.0/.gitlab/ci/plugins-integration/
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.768642 faraday_agent_dispatcher-2.6.0/.gitlab/ci/publish/
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/publish/.pypi-gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.769642 faraday_agent_dispatcher-2.6.0/.gitlab/ci/testing/
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/testing/.post-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     2762 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab/ci/testing/.testing-gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/.pre-push-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/AUTHORS.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.769642 faraday_agent_dispatcher-2.6.0/CHANGELOG/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.770642 faraday_agent_dispatcher-2.6.0/CHANGELOG/0.1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/0.1/01.first version.md
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/0.1/02.minimal structure.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/0.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/0.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.771642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.0/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.0/01.env_var.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.0/02.executor.md
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.0/03.params.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.772642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/01.run.md
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/02.wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/03.01.manage_execution_id.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/03.02.change_ws_route.md
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/04.error_management.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/05.invalid token.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/06.ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.774642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/01.package_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/02.signal.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/03.close_connection.md
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/04.sslcert.md
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/05.config_folder.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.776642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/01.check_command_before_run.md
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/02.connect_checks_timeout.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/03.connect_checks_not_responding.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/04.connect_checks_ssl_verify_fails.md
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/05.executor_with_comma.md
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/06.ssl_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/07.doc.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/E01.nmap_multi_target.md
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/E02.w3af_use_python2.md
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/E03.escape.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.2.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.778642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/1.multi_workspace.md
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/2.migrate_in_run.md
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/3.fix_close_agent.md
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/4.page-size.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/E00.md
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/E01.fix_arachni.md
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/E02.fix_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.779642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.1/1.proxy_setup.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.1/E01.fix_nessus.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.3.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.780642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/1.base_route.md
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/2.duration.md
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/E00.md
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/E01_flags_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/E02_env_python.md
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/E03_scheme_http_s_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.781642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.1/1.general_changes.md
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.1/E1.wpscan_not_use_docker.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.1/E2.fix_nuclei.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.781642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.2/1.plugins.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.2/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.4.2/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.783642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/1.change_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/2.v3.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/3.connectivity_endpoint.md
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/4.token.md
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/5.update_host_input.md
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/E1.update_openvas.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.783642 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.1/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.1/1.fix_burp_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/1.5.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.784642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.0.0/1.typing.md
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.0.0/2.add_manifests_versioning.md
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.0.0/3.FIX_typo_in_wizard.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.0.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.0.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.786642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.0/1.add_reminder_for_token.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.0/2.fix_dates.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.0/3.manage_402.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.0/E1.add_insightvm_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.0/E2.update_burp.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.0/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.786642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.1/1.add_option_ignore_ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.1/2.redo_defaults_ports_after_ssl.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.1/faraday_version.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.787642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.2/add_script_to_nmap.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.2/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.787642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.3/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.3/add_commands_to_wpscan.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.3/date.md
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.1.3/move_shodan_to_official.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.789642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/Add_timeout_parameter_to_arachni.md
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/add w3af.md
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/add_ignore_info_and_hostname_resolution.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/fix_exectuors.md
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/fix_logs.md
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/remove_ws.md
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.2.0/send_parameters_at_connection_time.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.790642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.3.0/add_scan_functionality_to_insightvm.md
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.3.0/add_tags_for_plugins.md
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.3.0/add_vulners.md
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.3.0/change_api_key.md
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.3.0/change_venvs.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.3.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.3.0/update_docs.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.790642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.4.0/Add_qualys.md
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.4.0/change_pgrep_for_psutil.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.4.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.791642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.0/
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.0/add_sonar_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.0/add_tenableio_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.0/date.md
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.0/fix_gvm_executor.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.0/transform_to_str.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.792642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.1/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.1/allow_ip_target_for_nuclei.md
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.1/date.md
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.5.1/fixes_for_bandit.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.792642 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.6.0/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.6.0/186.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/2.6.0/date.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.792642 faraday_agent_dispatcher-2.6.0/CHANGELOG/current/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/current/.keep
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CHANGELOG/footer.md
--rw-rw-rw-   0 root         (0) root         (0)     3711 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    15306 2023-07-07 20:12:50.816641 faraday_agent_dispatcher-2.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6247 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8129 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/RELEASE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.761642 faraday_agent_dispatcher-2.6.0/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.793642 faraday_agent_dispatcher-2.6.0/docker/plugins-docker/
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docker/plugins-docker/Dockerfile
--rwxrwxrwx   0 root         (0) root         (0)      802 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docker/plugins-docker/docker.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.793642 faraday_agent_dispatcher-2.6.0/docker/publish/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docker/publish/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docker/publish/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.794642 faraday_agent_dispatcher-2.6.0/docker/publish/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docker/publish/templates/template_dispatcher.ini
--rw-rw-rw-   0 root         (0) root         (0)     4473 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docker/publish/templates/template_dispatcher.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docker/publish/templates/template_dispatcher_with_report.ini
--rw-rw-rw-   0 root         (0) root         (0)     4830 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docker/publish/templates/template_dispatcher_with_report.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.794642 faraday_agent_dispatcher-2.6.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.795642 faraday_agent_dispatcher-2.6.0/docs/docs/
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/418.md
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/CNAME
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.795642 faraday_agent_dispatcher-2.6.0/docs/docs/css/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/css/faraday_doc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.795642 faraday_agent_dispatcher-2.6.0/docs/docs/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/examples/new-custom-executor.md
--rw-rw-rw-   0 root         (0) root         (0)     9813 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/getting-started.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.797642 faraday_agent_dispatcher-2.6.0/docs/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)    31633 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/agent_example.png
--rw-rw-rw-   0 root         (0) root         (0)    44658 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/arch.png
--rw-rw-rw-   0 root         (0) root         (0)    20584 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/arch_dispatcher.png
--rw-rw-rw-   0 root         (0) root         (0)    26625 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/arch_executors.png
--rw-rw-rw-   0 root         (0) root         (0)    21253 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/executor_example.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.762642 faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.798642 faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/qualys/
--rw-rw-rw-   0 root         (0) root         (0)    54521 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/qualys/check_profile.png
--rw-rw-rw-   0 root         (0) root         (0)   280745 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/qualys/new_profile.png
--rw-rw-rw-   0 root         (0) root         (0)   194186 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/qualys/profileid.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.798642 faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/sonarqube/
--rw-rw-rw-   0 root         (0) root         (0)    34458 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/sonarqube/generate_token.png
--rw-rw-rw-   0 root         (0) root         (0)    10160 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/sonarqube/profile_icon.png
--rw-rw-rw-   0 root         (0) root         (0)     3175 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/favicon.png
--rw-rw-rw-   0 root         (0) root         (0)      581 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    20392 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/images/token.png
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.798642 faraday_agent_dispatcher-2.6.0/docs/docs/js/
--rw-rw-rw-   0 root         (0) root         (0)     2051 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/js/details.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.800642 faraday_agent_dispatcher-2.6.0/docs/docs/misc/
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/appscan.md
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/docker.md
--rw-rw-rw-   0 root         (0) root         (0)     1545 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/qualys.md
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/sonarqube.md
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/template_dispatcher.ini
--rw-rw-rw-   0 root         (0) root         (0)     4473 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/template_dispatcher.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/template_dispatcher_with_report.ini
--rw-rw-rw-   0 root         (0) root         (0)     4830 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/template_dispatcher_with_report.yaml
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/misc/tenableio.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.800642 faraday_agent_dispatcher-2.6.0/docs/docs/technical/
--rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/technical/agents.md
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/docs/technical/arch.md
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.802641 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.803642 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4981 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.804642 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/general_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/general_prompts.py
--rw-rw-rw-   0 root         (0) root         (0)    12031 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/model_load.py
--rw-rw-rw-   0 root         (0) root         (0)     9860 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    14016 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)    27417 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/example_config.ini
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/example_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2537 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6288 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/executor_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.763642 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.763642 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.808642 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/
--rw-rw-rw-   0 root         (0) root         (0)     9484 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/appscan.py
--rw-rw-rw-   0 root         (0) root         (0)     3269 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/arachni.py
--rw-rw-rw-   0 root         (0) root         (0)     8406 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/burp.py
--rw-rw-rw-   0 root         (0) root         (0)     3808 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/crackmapexec.py
--rw-rw-rw-   0 root         (0) root         (0)     6135 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py
--rw-rw-rw-   0 root         (0) root         (0)     6447 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/insightvm.py
--rwxrwxrwx   0 root         (0) root         (0)     9563 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/nessus.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/nikto2.py
--rwxrwxrwx   0 root         (0) root         (0)     3551 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/nmap.py
--rwxrwxrwx   0 root         (0) root         (0)     3155 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/nuclei.py
--rw-rw-rw-   0 root         (0) root         (0)     4424 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     6205 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/qualys.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/report_processor.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/shodan2.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/sonarqube.py
--rwxrwxrwx   0 root         (0) root         (0)      887 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/sublist3r.sh
--rw-rw-rw-   0 root         (0) root         (0)     3416 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/tenableio.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/w3af.py
--rw-rw-rw-   0 root         (0) root         (0)     2521 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/wpscan.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/zap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.809641 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3861 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/control_values_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2217 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/text_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.803642 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15306 2023-07-07 20:12:50.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10132 2023-07-07 20:12:50.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 20:12:50.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-07 20:12:50.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 20:12:50.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-07 20:12:50.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-07 20:12:50.000000 faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-07 20:12:50.816641 faraday_agent_dispatcher-2.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3100 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.810641 faraday_agent_dispatcher-2.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.811642 faraday_agent_dispatcher-2.6.0/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/basic_executor.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/mock.pub
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/ok.crt
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/ok.key
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.812641 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/0.1.ini
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/0.1_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.0.ini
--rw-rw-rw-   0 root         (0) root         (0)      359 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.0_error0.ini
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.0_error1.ini
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.0_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.2.ini
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.2_with_agent_token.ini
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.5.ini
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/test_config.ini
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/data/wrong.crt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.813641 faraday_agent_dispatcher-2.6.0/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.813641 faraday_agent_dispatcher-2.6.0/tests/integration/faraday/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/integration/faraday/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7314 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/integration/faraday/test_execution.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.813641 faraday_agent_dispatcher-2.6.0/tests/plugins-docker/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/plugins-docker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/plugins-docker/test_executors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.814641 faraday_agent_dispatcher-2.6.0/tests/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.815641 faraday_agent_dispatcher-2.6.0/tests/unittests/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    46373 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/config/agent_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    37399 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/config/wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12777 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/test_agent_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     5088 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/test_config_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/test_import_official_executors.py
--rw-rw-rw-   0 root         (0) root         (0)     7983 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/unittests/wizard_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 20:12:50.816641 faraday_agent_dispatcher-2.6.0/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9651 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/utils/testing_faraday_server.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tests/utils/text_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-07-07 20:12:22.000000 faraday_agent_dispatcher-2.6.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.603035 faraday_agent_dispatcher-2.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.556034 faraday_agent_dispatcher-2.6.1/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.564034 faraday_agent_dispatcher-2.6.1/.gitlab/ci/
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/.pre-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/.rules-conditions.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.564034 faraday_agent_dispatcher-2.6.1/.gitlab/ci/build_ci/
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/build_ci/.build-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/fetch-secrets.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.564034 faraday_agent_dispatcher-2.6.1/.gitlab/ci/plugins-integration/
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.564034 faraday_agent_dispatcher-2.6.1/.gitlab/ci/publish/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/publish/.pypi-gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.565034 faraday_agent_dispatcher-2.6.1/.gitlab/ci/testing/
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/testing/.post-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2762 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab/ci/testing/.testing-gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/.pre-push-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/AUTHORS.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.565034 faraday_agent_dispatcher-2.6.1/CHANGELOG/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.565034 faraday_agent_dispatcher-2.6.1/CHANGELOG/0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/0.1/01.first version.md
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/0.1/02.minimal structure.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/0.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/0.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.566034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.0/01.env_var.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.0/02.executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.0/03.params.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.567034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/01.run.md
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/02.wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/03.01.manage_execution_id.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/03.02.change_ws_route.md
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/04.error_management.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/05.invalid token.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/06.ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.568034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/01.package_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/02.signal.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/03.close_connection.md
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/04.sslcert.md
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/05.config_folder.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.570034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/01.check_command_before_run.md
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/02.connect_checks_timeout.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/03.connect_checks_not_responding.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/04.connect_checks_ssl_verify_fails.md
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/05.executor_with_comma.md
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/06.ssl_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/07.doc.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/E01.nmap_multi_target.md
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/E02.w3af_use_python2.md
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/E03.escape.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.2.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.571034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/1.multi_workspace.md
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/2.migrate_in_run.md
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/3.fix_close_agent.md
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/4.page-size.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/E01.fix_arachni.md
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/E02.fix_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.572034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.1/1.proxy_setup.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.1/E01.fix_nessus.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.3.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.573034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/1.base_route.md
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/2.duration.md
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/E00.md
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/E01_flags_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/E02_env_python.md
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/E03_scheme_http_s_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.574034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.1/1.general_changes.md
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.1/E1.wpscan_not_use_docker.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.1/E2.fix_nuclei.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.574034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.2/1.plugins.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.2/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.4.2/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.575034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/1.change_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/2.v3.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/3.connectivity_endpoint.md
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/4.token.md
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/5.update_host_input.md
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/E1.update_openvas.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.576034 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.1/1.fix_burp_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/1.5.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.576034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.0.0/1.typing.md
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.0.0/2.add_manifests_versioning.md
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.0.0/3.FIX_typo_in_wizard.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.0.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.0.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.577034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.0/1.add_reminder_for_token.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.0/2.fix_dates.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.0/3.manage_402.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.0/E1.add_insightvm_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.0/E2.update_burp.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.0/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.578034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.1/1.add_option_ignore_ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.1/2.redo_defaults_ports_after_ssl.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.1/faraday_version.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.578034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.2/add_script_to_nmap.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.2/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.579034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.3/add_commands_to_wpscan.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.3/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.1.3/move_shodan_to_official.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.580034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/Add_timeout_parameter_to_arachni.md
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/add w3af.md
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/add_ignore_info_and_hostname_resolution.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/fix_exectuors.md
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/fix_logs.md
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/remove_ws.md
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.2.0/send_parameters_at_connection_time.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.581035 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.3.0/add_scan_functionality_to_insightvm.md
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.3.0/add_tags_for_plugins.md
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.3.0/add_vulners.md
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.3.0/change_api_key.md
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.3.0/change_venvs.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.3.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.3.0/update_docs.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.581035 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.4.0/Add_qualys.md
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.4.0/change_pgrep_for_psutil.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.4.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.582034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.0/add_sonar_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.0/add_tenableio_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.0/date.md
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.0/fix_gvm_executor.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.0/transform_to_str.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.583034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.1/allow_ip_target_for_nuclei.md
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.1/date.md
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.5.1/fixes_for_bandit.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.583034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.6.0/186.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.6.0/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.583034 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.6.1/187.md
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/2.6.1/date.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.583034 faraday_agent_dispatcher-2.6.1/CHANGELOG/current/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/current/.keep
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CHANGELOG/footer.md
+-rw-rw-rw-   0 root         (0) root         (0)     3711 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)    15393 2023-07-20 15:15:19.603035 faraday_agent_dispatcher-2.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6247 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8216 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/RELEASE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.559034 faraday_agent_dispatcher-2.6.1/docker/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.584035 faraday_agent_dispatcher-2.6.1/docker/plugins-docker/
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docker/plugins-docker/Dockerfile
+-rwxrwxrwx   0 root         (0) root         (0)      802 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docker/plugins-docker/docker.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.584035 faraday_agent_dispatcher-2.6.1/docker/publish/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docker/publish/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docker/publish/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.584035 faraday_agent_dispatcher-2.6.1/docker/publish/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docker/publish/templates/template_dispatcher.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4473 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docker/publish/templates/template_dispatcher.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docker/publish/templates/template_dispatcher_with_report.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docker/publish/templates/template_dispatcher_with_report.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.585034 faraday_agent_dispatcher-2.6.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.585034 faraday_agent_dispatcher-2.6.1/docs/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/418.md
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/CNAME
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.585034 faraday_agent_dispatcher-2.6.1/docs/docs/css/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/css/faraday_doc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.586034 faraday_agent_dispatcher-2.6.1/docs/docs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/examples/new-custom-executor.md
+-rw-rw-rw-   0 root         (0) root         (0)     9813 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/getting-started.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.587035 faraday_agent_dispatcher-2.6.1/docs/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)    31633 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/agent_example.png
+-rw-rw-rw-   0 root         (0) root         (0)    44658 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/arch.png
+-rw-rw-rw-   0 root         (0) root         (0)    20584 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/arch_dispatcher.png
+-rw-rw-rw-   0 root         (0) root         (0)    26625 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/arch_executors.png
+-rw-rw-rw-   0 root         (0) root         (0)    21253 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/executor_example.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.559034 faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.588034 faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/qualys/
+-rw-rw-rw-   0 root         (0) root         (0)    54521 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/qualys/check_profile.png
+-rw-rw-rw-   0 root         (0) root         (0)   280745 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/qualys/new_profile.png
+-rw-rw-rw-   0 root         (0) root         (0)   194186 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/qualys/profileid.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.588034 faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/sonarqube/
+-rw-rw-rw-   0 root         (0) root         (0)    34458 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/sonarqube/generate_token.png
+-rw-rw-rw-   0 root         (0) root         (0)    10160 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/sonarqube/profile_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     3175 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/favicon.png
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    20392 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/images/token.png
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.589035 faraday_agent_dispatcher-2.6.1/docs/docs/js/
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/js/details.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.590035 faraday_agent_dispatcher-2.6.1/docs/docs/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/appscan.md
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/docker.md
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/qualys.md
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/sonarqube.md
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/template_dispatcher.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4473 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/template_dispatcher.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/template_dispatcher_with_report.ini
+-rw-rw-rw-   0 root         (0) root         (0)     4830 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/template_dispatcher_with_report.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/misc/tenableio.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.590035 faraday_agent_dispatcher-2.6.1/docs/docs/technical/
+-rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/technical/agents.md
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/docs/technical/arch.md
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.591035 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.593035 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4981 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.594035 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/general_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/general_prompts.py
+-rw-rw-rw-   0 root         (0) root         (0)    12031 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/model_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     9860 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    14016 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    27417 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/example_config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/example_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6288 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/executor_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.560034 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.560034 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.597035 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/
+-rw-rw-rw-   0 root         (0) root         (0)     9484 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/appscan.py
+-rw-rw-rw-   0 root         (0) root         (0)     3269 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/arachni.py
+-rw-rw-rw-   0 root         (0) root         (0)     8406 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/burp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3808 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/crackmapexec.py
+-rw-rw-rw-   0 root         (0) root         (0)     6135 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     6447 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/insightvm.py
+-rwxrwxrwx   0 root         (0) root         (0)     9563 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/nessus.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/nikto2.py
+-rwxrwxrwx   0 root         (0) root         (0)     3551 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/nmap.py
+-rwxrwxrwx   0 root         (0) root         (0)     3152 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/nuclei.py
+-rw-rw-rw-   0 root         (0) root         (0)     4424 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6205 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/qualys.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/report_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/shodan2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/sonarqube.py
+-rwxrwxrwx   0 root         (0) root         (0)      887 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/sublist3r.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3416 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/tenableio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/w3af.py
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/wpscan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/zap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.597035 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/control_values_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2217 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/text_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.592035 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15393 2023-07-20 15:15:19.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10179 2023-07-20 15:15:19.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 15:15:19.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-20 15:15:19.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 15:15:19.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-20 15:15:19.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-20 15:15:19.000000 faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-20 15:15:19.603035 faraday_agent_dispatcher-2.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3100 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.598035 faraday_agent_dispatcher-2.6.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.599035 faraday_agent_dispatcher-2.6.1/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/basic_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/mock.pub
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/ok.crt
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/ok.key
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.600035 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/0.1.ini
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/0.1_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.0.ini
+-rw-rw-rw-   0 root         (0) root         (0)      359 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.0_error0.ini
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.0_error1.ini
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.0_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.2.ini
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.2_with_agent_token.ini
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.5.ini
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/test_config.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/data/wrong.crt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.600035 faraday_agent_dispatcher-2.6.1/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.600035 faraday_agent_dispatcher-2.6.1/tests/integration/faraday/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/integration/faraday/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7314 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/integration/faraday/test_execution.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.601035 faraday_agent_dispatcher-2.6.1/tests/plugins-docker/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/plugins-docker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/plugins-docker/test_executors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.601035 faraday_agent_dispatcher-2.6.1/tests/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.602035 faraday_agent_dispatcher-2.6.1/tests/unittests/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46373 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/config/agent_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    37399 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/config/wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12777 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/test_agent_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     5088 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/test_config_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/test_import_official_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7983 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/unittests/wizard_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 15:15:19.602035 faraday_agent_dispatcher-2.6.1/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9651 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/utils/testing_faraday_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tests/utils/text_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-07-20 15:14:47.000000 faraday_agent_dispatcher-2.6.1/tox.ini
```

### Comparing `faraday_agent_dispatcher-2.6.0/.gitignore` & `faraday_agent_dispatcher-2.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.gitlab/ci/.pre-gitlab-ci.yml` & `faraday_agent_dispatcher-2.6.1/.gitlab/ci/.pre-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.gitlab/ci/build_ci/.build-gitlab-ci.yml` & `faraday_agent_dispatcher-2.6.1/.gitlab/ci/build_ci/.build-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.gitlab/ci/fetch-secrets.yml` & `faraday_agent_dispatcher-2.6.1/.gitlab/ci/fetch-secrets.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml` & `faraday_agent_dispatcher-2.6.1/.gitlab/ci/plugins-integration/.build-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml` & `faraday_agent_dispatcher-2.6.1/.gitlab/ci/plugins-integration/.testing-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml` & `faraday_agent_dispatcher-2.6.1/.gitlab/ci/publish/.publish-dockerhub-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.gitlab/ci/testing/.testing-gitlab-ci.yml` & `faraday_agent_dispatcher-2.6.1/.gitlab/ci/testing/.testing-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.gitlab-ci.yml` & `faraday_agent_dispatcher-2.6.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/.pre-commit-config.yaml` & `faraday_agent_dispatcher-2.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/CONTRIBUTING.rst` & `faraday_agent_dispatcher-2.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/COPYING` & `faraday_agent_dispatcher-2.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/Makefile` & `faraday_agent_dispatcher-2.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/PKG-INFO` & `faraday_agent_dispatcher-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday_agent_dispatcher
-Version: 2.6.0
+Version: 2.6.1
 Summary: Faraday agent dispatcher to communicate an agent to faraday
 Home-page: https://github.com/infobyte/faraday_agent_dispatcher
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday integration
 Classifier: Development Status :: 5 - Production/Stable
@@ -184,24 +184,28 @@
 
 For more info you can check our [documentation][doc]
 
 [doc]: https://docs.agents.faradaysec.com
 [API]: https://api.faradaysec.com/
 
 
+2.6.1 [July 20th, 2023]:
+---
+ * [FIX] Now nuclei executor use -j flag instead of -json. #187
+
 2.6.0 [July 7th, 2023]:
 ---
- * [ADD] Add HCL Appscan executor. #186
+ * [ADD] Add HCL Appscan executer #186
 
 2.5.1 [Jan 3rd, 2023]:
 ---
  * [DEL] Now nuclei doesn't check if the target is an ip
  * [MOD] Add a fixes for bandit vuln:
-      - Replace assert return code with a if
-      - Remove default x_token in nessus executor
+   - Replace assert return code with a if
+   - Remove default x_token in nessus executor
 
 2.5.0 [Nov 30th, 2022]:
 ---
  * [ADD] Add new Sonar Qube executor
  * [ADD] Add tenableio executor
  * [FIX] Make gvm executor compatible with new version of python-gvm
  * [FIX] Now if a venv is int or float it will convert to string
```

### Comparing `faraday_agent_dispatcher-2.6.0/README.md` & `faraday_agent_dispatcher-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/RELEASE.md` & `faraday_agent_dispatcher-2.6.1/RELEASE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+2.6.1 [July 20th, 2023]:
+---
+ * [FIX] Now nuclei executor use -j flag instead of -json. #187
+
 2.6.0 [July 7th, 2023]:
 ---
- * [ADD] Add HCL Appscan executor. #186
+ * [ADD] Add HCL Appscan executer #186
 
 2.5.1 [Jan 3rd, 2023]:
 ---
  * [DEL] Now nuclei doesn't check if the target is an ip
  * [MOD] Add a fixes for bandit vuln:
-      - Replace assert return code with a if
-      - Remove default x_token in nessus executor
+   - Replace assert return code with a if
+   - Remove default x_token in nessus executor
 
 2.5.0 [Nov 30th, 2022]:
 ---
  * [ADD] Add new Sonar Qube executor
  * [ADD] Add tenableio executor
  * [FIX] Make gvm executor compatible with new version of python-gvm
  * [FIX] Now if a venv is int or float it will convert to string
```

### Comparing `faraday_agent_dispatcher-2.6.0/docker/plugins-docker/Dockerfile` & `faraday_agent_dispatcher-2.6.1/docker/plugins-docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docker/plugins-docker/docker.sh` & `faraday_agent_dispatcher-2.6.1/docker/plugins-docker/docker.sh`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docker/publish/Dockerfile` & `faraday_agent_dispatcher-2.6.1/docker/publish/Dockerfile`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docker/publish/templates/template_dispatcher.ini` & `faraday_agent_dispatcher-2.6.1/docker/publish/templates/template_dispatcher.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docker/publish/templates/template_dispatcher.yaml` & `faraday_agent_dispatcher-2.6.1/docker/publish/templates/template_dispatcher.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docker/publish/templates/template_dispatcher_with_report.ini` & `faraday_agent_dispatcher-2.6.1/docker/publish/templates/template_dispatcher_with_report.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docker/publish/templates/template_dispatcher_with_report.yaml` & `faraday_agent_dispatcher-2.6.1/docker/publish/templates/template_dispatcher_with_report.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/.gitlab-ci.yml` & `faraday_agent_dispatcher-2.6.1/docs/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/getting-started.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/agent_example.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/agent_example.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/arch.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/arch.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/arch_dispatcher.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/arch_dispatcher.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/arch_executors.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/arch_executors.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/executor_example.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/executor_example.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/qualys/check_profile.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/qualys/check_profile.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/qualys/new_profile.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/qualys/new_profile.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/qualys/profileid.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/qualys/profileid.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/sonarqube/generate_token.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/sonarqube/generate_token.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/executors/sonarqube/profile_icon.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/executors/sonarqube/profile_icon.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/favicon.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/logo.svg` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/images/token.png` & `faraday_agent_dispatcher-2.6.1/docs/docs/images/token.png`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/index.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/js/details.js` & `faraday_agent_dispatcher-2.6.1/docs/docs/js/details.js`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/appscan.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/appscan.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/docker.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/docker.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/qualys.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/qualys.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/sonarqube.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/sonarqube.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/template_dispatcher.ini` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/template_dispatcher.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/template_dispatcher.yaml` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/template_dispatcher.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/template_dispatcher_with_report.ini` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/template_dispatcher_with_report.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/template_dispatcher_with_report.yaml` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/template_dispatcher_with_report.yaml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/misc/tenableio.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/misc/tenableio.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/technical/agents.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/technical/agents.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/docs/technical/arch.md` & `faraday_agent_dispatcher-2.6.1/docs/docs/technical/arch.md`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/docs/mkdocs.yml` & `faraday_agent_dispatcher-2.6.1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/__init__.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """Top-level package for faraday_agent_dispatcher."""
 
 __author__ = """Faraday Development Team"""
 __email__ = "devel@infobytesec.com"
-__version__ = "2.6.0"
+__version__ = "2.6.1"
```

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/main.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/main.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/general_inputs.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/general_inputs.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/general_prompts.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/general_prompts.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/utils/model_load.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/utils/model_load.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/cli/wizard.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/cli/wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/config.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/config.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/dispatcher.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/example_config.ini` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/example_config.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/executor.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/executor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/executor_helper.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/executor_helper.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/logger.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/logger.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/appscan.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/appscan.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/arachni.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/arachni.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/burp.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/burp.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/crackmapexec.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/crackmapexec.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/gvm_openvas.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/insightvm.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/insightvm.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/nessus.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/nessus.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/nikto2.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/nikto2.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/nmap.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/nmap.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/nuclei.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/nuclei.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             ]
 
         if NUCLEI_EXCLUDE:
             exclude_list = NUCLEI_EXCLUDE.split(",")
             for exclude in exclude_list:
                 cmd += ["-exclude", str(Path(NUCLEI_TEMPLATES) / exclude)]
 
-        cmd += ["-json", "-o", name_output]
+        cmd += ["-j", "-o", name_output]
         nuclei_process = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
         if len(nuclei_process.stdout) > 0:
             print(
                 f"Nuclei stdout: {nuclei_process.stdout.decode('utf-8')}",
                 file=sys.stderr,
             )
```

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/openvas_legacy.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/qualys.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/qualys.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/report_processor.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/report_processor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/shodan2.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/shodan2.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/sonarqube.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/sonarqube.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/sublist3r.sh` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/sublist3r.sh`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/tenableio.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/tenableio.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/w3af.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/w3af.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/wpscan.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/wpscan.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/wpscan_legacy.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/static/executors/official/zap.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/static/executors/official/zap.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/control_values_utils.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/control_values_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/metadata_utils.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher/utils/url_utils.py` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher/utils/url_utils.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/PKG-INFO` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faraday-agent-dispatcher
-Version: 2.6.0
+Version: 2.6.1
 Summary: Faraday agent dispatcher to communicate an agent to faraday
 Home-page: https://github.com/infobyte/faraday_agent_dispatcher
 Author: Faraday Development Team
 Author-email: devel@infobytesec.com
 License: GNU General Public License v3
 Keywords: faraday integration
 Classifier: Development Status :: 5 - Production/Stable
@@ -184,24 +184,28 @@
 
 For more info you can check our [documentation][doc]
 
 [doc]: https://docs.agents.faradaysec.com
 [API]: https://api.faradaysec.com/
 
 
+2.6.1 [July 20th, 2023]:
+---
+ * [FIX] Now nuclei executor use -j flag instead of -json. #187
+
 2.6.0 [July 7th, 2023]:
 ---
- * [ADD] Add HCL Appscan executor. #186
+ * [ADD] Add HCL Appscan executer #186
 
 2.5.1 [Jan 3rd, 2023]:
 ---
  * [DEL] Now nuclei doesn't check if the target is an ip
  * [MOD] Add a fixes for bandit vuln:
-      - Replace assert return code with a if
-      - Remove default x_token in nessus executor
+   - Replace assert return code with a if
+   - Remove default x_token in nessus executor
 
 2.5.0 [Nov 30th, 2022]:
 ---
  * [ADD] Add new Sonar Qube executor
  * [ADD] Add tenableio executor
  * [FIX] Make gvm executor compatible with new version of python-gvm
  * [FIX] Now if a venv is int or float it will convert to string
```

### Comparing `faraday_agent_dispatcher-2.6.0/faraday_agent_dispatcher.egg-info/SOURCES.txt` & `faraday_agent_dispatcher-2.6.1/faraday_agent_dispatcher.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,16 @@
 CHANGELOG/2.5.0/fix_gvm_executor.md
 CHANGELOG/2.5.0/transform_to_str.md
 CHANGELOG/2.5.1/allow_ip_target_for_nuclei.md
 CHANGELOG/2.5.1/date.md
 CHANGELOG/2.5.1/fixes_for_bandit.md
 CHANGELOG/2.6.0/186.md
 CHANGELOG/2.6.0/date.md
+CHANGELOG/2.6.1/187.md
+CHANGELOG/2.6.1/date.md
 CHANGELOG/current/.keep
 docker/plugins-docker/Dockerfile
 docker/plugins-docker/docker.sh
 docker/publish/.dockerignore
 docker/publish/Dockerfile
 docker/publish/templates/template_dispatcher.ini
 docker/publish/templates/template_dispatcher.yaml
```

### Comparing `faraday_agent_dispatcher-2.6.0/setup.py` & `faraday_agent_dispatcher-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/basic_executor.py` & `faraday_agent_dispatcher-2.6.1/tests/data/basic_executor.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/ok.crt` & `faraday_agent_dispatcher-2.6.1/tests/data/ok.crt`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/ok.key` & `faraday_agent_dispatcher-2.6.1/tests/data/ok.key`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.0_with_agent_token.ini` & `faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.0_with_agent_token.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.2.ini` & `faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.2.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.2_with_agent_token.ini` & `faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.2_with_agent_token.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/old_version_inis/1.5.ini` & `faraday_agent_dispatcher-2.6.1/tests/data/old_version_inis/1.5.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/test_config.ini` & `faraday_agent_dispatcher-2.6.1/tests/data/test_config.ini`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/data/wrong.crt` & `faraday_agent_dispatcher-2.6.1/tests/data/wrong.crt`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/integration/faraday/test_execution.py` & `faraday_agent_dispatcher-2.6.1/tests/integration/faraday/test_execution.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/plugins-docker/test_executors.py` & `faraday_agent_dispatcher-2.6.1/tests/plugins-docker/test_executors.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/unittests/config/agent_dispatcher.py` & `faraday_agent_dispatcher-2.6.1/tests/unittests/config/agent_dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/unittests/config/wizard.py` & `faraday_agent_dispatcher-2.6.1/tests/unittests/config/wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/unittests/test_agent_dispatcher.py` & `faraday_agent_dispatcher-2.6.1/tests/unittests/test_agent_dispatcher.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/unittests/test_config_wizard.py` & `faraday_agent_dispatcher-2.6.1/tests/unittests/test_config_wizard.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/unittests/test_import_official_executors.py` & `faraday_agent_dispatcher-2.6.1/tests/unittests/test_import_official_executors.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/unittests/wizard_input.py` & `faraday_agent_dispatcher-2.6.1/tests/unittests/wizard_input.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tests/utils/testing_faraday_server.py` & `faraday_agent_dispatcher-2.6.1/tests/utils/testing_faraday_server.py`

 * *Files identical despite different names*

### Comparing `faraday_agent_dispatcher-2.6.0/tox.ini` & `faraday_agent_dispatcher-2.6.1/tox.ini`

 * *Files identical despite different names*

