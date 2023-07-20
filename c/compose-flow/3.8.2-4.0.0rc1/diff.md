# Comparing `tmp/compose-flow-3.8.2.tar.gz` & `tmp/compose-flow-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/compose-flow-3.8.2.tar", last modified: Thu May  6 22:08:32 2021, max compression
+gzip compressed data, was "compose-flow-4.0.0rc1.tar", last modified: Thu Jul 20 18:57:44 2023, max compression
```

## Comparing `compose-flow-3.8.2.tar` & `compose-flow-4.0.0rc1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/
--rw-r--r--   0 root         (0) swarmclient  (1000)       83 2021-05-06 22:08:32.000000 compose-flow-3.8.2/setup.cfg
--rw-r--r--   0 root         (0) swarmclient  (1000)       49 2021-05-06 22:06:32.000000 compose-flow-3.8.2/.dockerignore
--rw-r--r--   0 root         (0) swarmclient  (1000)      105 2021-05-06 22:06:32.000000 compose-flow-3.8.2/.gitignore
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/files/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/files/home/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/files/home/swarmclient/
--rw-r--r--   0 root         (0) swarmclient  (1000)      142 2021-05-06 22:06:32.000000 compose-flow-3.8.2/files/home/swarmclient/.pypirc
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/files/usr/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/files/usr/local/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/files/usr/local/bin/
--rw-r--r--   0 root         (0) swarmclient  (1000)      210 2021-05-06 22:06:32.000000 compose-flow-3.8.2/files/usr/local/bin/entrypoint.sh
--rw-r--r--   0 root         (0) swarmclient  (1000)     1691 2021-05-06 22:06:32.000000 compose-flow-3.8.2/README.md
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/compose/
--rw-r--r--   0 root         (0) swarmclient  (1000)       73 2021-05-06 22:06:32.000000 compose-flow-3.8.2/compose/docker-compose.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)      157 2021-05-06 22:06:32.000000 compose-flow-3.8.2/compose/docker-compose.results.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)       54 2021-05-06 22:06:32.000000 compose-flow-3.8.2/compose/docker-compose.mount.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)     1303 2021-05-06 22:06:32.000000 compose-flow-3.8.2/compose/compose-flow.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)       78 2021-05-06 22:06:32.000000 compose-flow-3.8.2/compose/docker-compose.publish.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)      381 2021-05-06 22:06:32.000000 compose-flow-3.8.2/Pipfile
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/scripts/
--rw-r--r--   0 root         (0) swarmclient  (1000)      119 2021-05-06 22:06:32.000000 compose-flow-3.8.2/scripts/watch-tests.sh
--rw-r--r--   0 root         (0) swarmclient  (1000)      304 2021-05-06 22:06:32.000000 compose-flow-3.8.2/scripts/publish.sh
--rw-r--r--   0 root         (0) swarmclient  (1000)      101 2021-05-06 22:06:32.000000 compose-flow-3.8.2/scripts/tag_and_publish.sh
--rw-r--r--   0 root         (0) swarmclient  (1000)      715 2021-05-06 22:06:32.000000 compose-flow-3.8.2/scripts/dump_swarm_config.py
--rwxr-xr-x   0 root         (0) swarmclient  (1000)      245 2021-05-06 22:06:32.000000 compose-flow-3.8.2/scripts/lock.sh
--rw-r--r--   0 root         (0) swarmclient  (1000)       71 2021-05-06 22:06:32.000000 compose-flow-3.8.2/scripts/black.sh
--rw-r--r--   0 root         (0) swarmclient  (1000)    51950 2021-05-06 22:06:32.000000 compose-flow-3.8.2/Pipfile.lock
--rw-r--r--   0 root         (0) swarmclient  (1000)     2611 2021-05-06 22:08:32.000000 compose-flow-3.8.2/PKG-INFO
--rw-r--r--   0 root         (0) swarmclient  (1000)     2131 2021-05-06 22:08:32.000000 compose-flow-3.8.2/setup.py
--rw-r--r--   0 root         (0) swarmclient  (1000)    11357 2021-05-06 22:06:32.000000 compose-flow-3.8.2/LICENSE
--rw-r--r--   0 root         (0) swarmclient  (1000)     2587 2021-05-06 22:06:32.000000 compose-flow-3.8.2/Dockerfile
--rw-r--r--   0 root         (0) swarmclient  (1000)       34 2021-05-06 22:06:32.000000 compose-flow-3.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) swarmclient  (1000)      508 2021-05-06 22:06:32.000000 compose-flow-3.8.2/Jenkinsfile
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/tests/
--rw-r--r--   0 root         (0) swarmclient  (1000)     1454 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_remote.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     6266 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_workflow.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3813 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_pod.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      941 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_utils.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     5287 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_publish.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      719 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_passthrough.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      408 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/utils.py
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/tests/files/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/tests/files/manifests/
--rw-r--r--   0 root         (0) swarmclient  (1000)      211 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/invalid-ingress-multidoc.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)       97 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/external-zalando-ingress.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)      272 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/no-resources-job.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)       24 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/invalid-zalando-ingress.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)       78 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/nginx-ingress.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)     1452 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/good-init-deployment.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)      919 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/good-job.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)       90 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/internal-zalando-ingress.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)     2233 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/no-limits-deployment.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)     2115 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/manifests/good-cronjob.yaml
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/tests/files/values/
--rw-r--r--   0 root         (0) swarmclient  (1000)       93 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/values/good-resources-values.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)       69 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/values/multidoc-values.yaml
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/tests/files/answers/
--rw-r--r--   0 root         (0) swarmclient  (1000)       86 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/answers/no-requests-answers.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)       90 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/answers/no-limits-answers.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)       47 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/answers/multidoc-answers.yaml
--rw-r--r--   0 root         (0) swarmclient  (1000)      137 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/answers/good-resources-answers.yaml
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/tests/files/profiles/
--rw-r--r--   0 root         (0) swarmclient  (1000)      105 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/profiles/limit_no_reservation.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)      111 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/profiles/reservation_no_limit.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)      205 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/profiles/limit_and_reservation.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)      119 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/profiles/with_node_constraints.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)       37 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/profiles/no_constraints.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)       68 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/profiles/global_no_constraints.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)       66 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/profiles/resources_nothing_set.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)      143 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/files/profiles/no_node_constraints.yml
--rw-r--r--   0 root         (0) swarmclient  (1000)      903 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_service.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      468 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_shell.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3203 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_backends.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     5524 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_docker_image.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     7664 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_deploy.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      695 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_base.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      813 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_docker.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      976 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_task.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     6254 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_kube_checks.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     8457 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_profile.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      487 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/__init__.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      615 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_kube_mixins.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     6435 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/tests/test_env.py
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow/commands/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/
--rw-r--r--   0 root         (0) swarmclient  (1000)      490 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/rancher.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      435 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/help.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     2501 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/swarm.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     5042 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/base.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      272 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/docker.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     2722 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/publish.py
--rw-r--r--   0 root         (0) swarmclient  (1000)    14788 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/env.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3250 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/deploy.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     1477 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/compose.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      509 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/workflow_config.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     6633 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/remote.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     6271 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/service.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3673 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/pod.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     2608 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/task.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      212 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/build.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     1600 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/passthrough_base.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     1230 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/kompose.py
--rw-r--r--   0 root         (0) swarmclient  (1000)    14763 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/profile.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     1770 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/remote_config.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3141 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/__init__.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      496 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/helm.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      503 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/subcommands/kubectl.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     9950 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/workflow.py
--rw-r--r--   0 root         (0) swarmclient  (1000)       31 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/commands/__init__.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      708 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/settings.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     2789 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/errors.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      895 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/shell.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3467 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/docker.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3543 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/config.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     6180 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/utils.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     2315 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/compose.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      641 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/entrypoints.py
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow/kube/
--rw-r--r--   0 root         (0) swarmclient  (1000)     8131 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/kube/checks.py
--rw-r--r--   0 root         (0) swarmclient  (1000)    23545 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/kube/mixins.py
--rw-r--r--   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/kube/__init__.py
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow/environment/
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow/environment/backends/
--rw-r--r--   0 root         (0) swarmclient  (1000)     1227 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/environment/backends/kube_backend.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     1467 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/environment/backends/local_backend.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     1078 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/environment/backends/base_backend.py
--rw-r--r--   0 root         (0) swarmclient  (1000)      381 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/environment/backends/__init__.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     1218 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/environment/backends/rancher_backend.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3759 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/environment/backends/swarm_backend.py
--rw-r--r--   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/environment/__init__.py
--rw-r--r--   0 root         (0) swarmclient  (1000)     3688 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/docker_image.py
--rw-r--r--   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:06:32.000000 compose-flow-3.8.2/src/compose_flow/__init__.py
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow.egg-info/
--rw-r--r--   0 root         (0) swarmclient  (1000)       72 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) swarmclient  (1000)       99 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow.egg-info/requires.txt
--rw-r--r--   0 root         (0) swarmclient  (1000)     4345 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) swarmclient  (1000)     2611 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) swarmclient  (1000)        1 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) swarmclient  (1000)       19 2021-05-06 22:08:32.000000 compose-flow-3.8.2/src/compose_flow.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0) swarmclient  (1000)        0 2021-05-06 22:08:32.000000 compose-flow-3.8.2/docs/
--rw-r--r--   0 root         (0) swarmclient  (1000)     9328 2021-05-06 22:06:32.000000 compose-flow-3.8.2/docs/k8s.md
--rw-r--r--   0 root         (0) swarmclient  (1000)     9824 2021-05-06 22:06:32.000000 compose-flow-3.8.2/docs/advanced.md
--rw-r--r--   0 root         (0) swarmclient  (1000)      132 2021-05-06 22:06:32.000000 compose-flow-3.8.2/pylama.ini
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/
+-rw-r--r--   0 root         (0) docker     (999)       49 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/.dockerignore
+-rw-r--r--   0 root         (0) docker     (999)      105 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/.gitignore
+-rw-r--r--   0 root         (0) docker     (999)     2642 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/Dockerfile
+-rw-r--r--   0 root         (0) docker     (999)      508 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/Jenkinsfile
+-rw-r--r--   0 root         (0) docker     (999)    11357 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) docker     (999)       34 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) docker     (999)     1964 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) docker     (999)      339 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/Pipfile
+-rw-r--r--   0 root         (0) docker     (999)    73192 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/Pipfile.lock
+-rw-r--r--   0 root         (0) docker     (999)     1691 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/README.md
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/compose/
+-rw-r--r--   0 root         (0) docker     (999)     1171 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/compose-flow.yml
+-rw-r--r--   0 root         (0) docker     (999)       54 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/docker-compose.mount.yml
+-rw-r--r--   0 root         (0) docker     (999)       78 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/docker-compose.publish.yml
+-rw-r--r--   0 root         (0) docker     (999)      157 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/docker-compose.results.yml
+-rw-r--r--   0 root         (0) docker     (999)       73 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/compose/docker-compose.yml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/docs/
+-rw-r--r--   0 root         (0) docker     (999)     9824 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/docs/advanced.md
+-rw-r--r--   0 root         (0) docker     (999)     9328 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/docs/k8s.md
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/files/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/files/home/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/files/home/swarmclient/
+-rw-r--r--   0 root         (0) docker     (999)      142 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/files/home/swarmclient/.pypirc
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/files/usr/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/files/usr/local/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/files/usr/local/bin/
+-rw-r--r--   0 root         (0) docker     (999)      210 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/files/usr/local/bin/entrypoint.sh
+-rw-r--r--   0 root         (0) docker     (999)      132 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/pylama.ini
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.858718 compose-flow-4.0.0rc1/scripts/
+-rw-r--r--   0 root         (0) docker     (999)       71 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/black.sh
+-rw-r--r--   0 root         (0) docker     (999)      715 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/dump_swarm_config.py
+-rwxr-xr-x   0 root         (0) docker     (999)      245 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/lock.sh
+-rw-r--r--   0 root         (0) docker     (999)      304 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/publish.sh
+-rw-r--r--   0 root         (0) docker     (999)      101 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/tag_and_publish.sh
+-rw-r--r--   0 root         (0) docker     (999)      119 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/scripts/watch-tests.sh
+-rw-r--r--   0 root         (0) docker     (999)       83 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) docker     (999)     2131 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/src/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.862718 compose-flow-4.0.0rc1/src/compose_flow/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.862718 compose-flow-4.0.0rc1/src/compose_flow/commands/
+-rw-r--r--   0 root         (0) docker     (999)       31 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.866718 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/
+-rw-r--r--   0 root         (0) docker     (999)     3141 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     5042 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/base.py
+-rw-r--r--   0 root         (0) docker     (999)      212 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/build.py
+-rw-r--r--   0 root         (0) docker     (999)     1477 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/compose.py
+-rw-r--r--   0 root         (0) docker     (999)     3250 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/deploy.py
+-rw-r--r--   0 root         (0) docker     (999)      272 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/docker.py
+-rw-r--r--   0 root         (0) docker     (999)    14787 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/env.py
+-rw-r--r--   0 root         (0) docker     (999)      496 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/helm.py
+-rw-r--r--   0 root         (0) docker     (999)      435 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/help.py
+-rw-r--r--   0 root         (0) docker     (999)     1230 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/kompose.py
+-rw-r--r--   0 root         (0) docker     (999)      503 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/kubectl.py
+-rw-r--r--   0 root         (0) docker     (999)     1600 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/passthrough_base.py
+-rw-r--r--   0 root         (0) docker     (999)     3672 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/pod.py
+-rw-r--r--   0 root         (0) docker     (999)    14763 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/profile.py
+-rw-r--r--   0 root         (0) docker     (999)     2722 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/publish.py
+-rw-r--r--   0 root         (0) docker     (999)      490 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/rancher.py
+-rw-r--r--   0 root         (0) docker     (999)     6633 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/remote.py
+-rw-r--r--   0 root         (0) docker     (999)     1770 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/remote_config.py
+-rw-r--r--   0 root         (0) docker     (999)     6271 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/service.py
+-rw-r--r--   0 root         (0) docker     (999)     2501 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/swarm.py
+-rw-r--r--   0 root         (0) docker     (999)     2608 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/task.py
+-rw-r--r--   0 root         (0) docker     (999)      509 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/workflow_config.py
+-rw-r--r--   0 root         (0) docker     (999)     9950 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/commands/workflow.py
+-rw-r--r--   0 root         (0) docker     (999)     2315 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/compose.py
+-rw-r--r--   0 root         (0) docker     (999)     3539 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/config.py
+-rw-r--r--   0 root         (0) docker     (999)     3467 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/docker.py
+-rw-r--r--   0 root         (0) docker     (999)     3688 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/docker_image.py
+-rw-r--r--   0 root         (0) docker     (999)      641 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/entrypoints.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.866718 compose-flow-4.0.0rc1/src/compose_flow/environment/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.866718 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/
+-rw-r--r--   0 root         (0) docker     (999)      381 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     1078 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/base_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1227 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/kube_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1467 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/local_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     1218 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/rancher_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     3759 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/environment/backends/swarm_backend.py
+-rw-r--r--   0 root         (0) docker     (999)     2789 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/errors.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.866718 compose-flow-4.0.0rc1/src/compose_flow/kube/
+-rw-r--r--   0 root         (0) docker     (999)        0 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/kube/__init__.py
+-rw-r--r--   0 root         (0) docker     (999)     8131 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/kube/checks.py
+-rw-r--r--   0 root         (0) docker     (999)    23597 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/kube/mixins.py
+-rw-r--r--   0 root         (0) docker     (999)      708 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/settings.py
+-rw-r--r--   0 root         (0) docker     (999)      895 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/shell.py
+-rw-r--r--   0 root         (0) docker     (999)     6180 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/compose_flow/utils.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.862718 compose-flow-4.0.0rc1/src/compose_flow.egg-info/
+-rw-r--r--   0 root         (0) docker     (999)     1964 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) docker     (999)     4345 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) docker     (999)        1 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) docker     (999)       71 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) docker     (999)       68 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) docker     (999)       19 2023-07-20 18:57:44.000000 compose-flow-4.0.0rc1/src/compose_flow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.870718 compose-flow-4.0.0rc1/src/tests/
+-rw-r--r--   0 root         (0) docker     (999)      487 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/__init__.py
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.854718 compose-flow-4.0.0rc1/src/tests/files/
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.870718 compose-flow-4.0.0rc1/src/tests/files/answers/
+-rw-r--r--   0 root         (0) docker     (999)      137 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/answers/good-resources-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       47 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/answers/multidoc-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       90 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/answers/no-limits-answers.yaml
+-rw-r--r--   0 root         (0) docker     (999)       86 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/answers/no-requests-answers.yaml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.870718 compose-flow-4.0.0rc1/src/tests/files/manifests/
+-rw-r--r--   0 root         (0) docker     (999)       97 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/external-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)     2115 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/good-cronjob.yaml
+-rw-r--r--   0 root         (0) docker     (999)     1452 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/good-init-deployment.yaml
+-rw-r--r--   0 root         (0) docker     (999)      919 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/good-job.yaml
+-rw-r--r--   0 root         (0) docker     (999)       90 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/internal-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)      211 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/invalid-ingress-multidoc.yaml
+-rw-r--r--   0 root         (0) docker     (999)       24 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/invalid-zalando-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)       78 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/nginx-ingress.yaml
+-rw-r--r--   0 root         (0) docker     (999)     2233 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/no-limits-deployment.yaml
+-rw-r--r--   0 root         (0) docker     (999)      272 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/manifests/no-resources-job.yaml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/src/tests/files/profiles/
+-rw-r--r--   0 root         (0) docker     (999)       68 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/global_no_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      205 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/limit_and_reservation.yml
+-rw-r--r--   0 root         (0) docker     (999)      105 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/limit_no_reservation.yml
+-rw-r--r--   0 root         (0) docker     (999)       37 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/no_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      143 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/no_node_constraints.yml
+-rw-r--r--   0 root         (0) docker     (999)      111 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/reservation_no_limit.yml
+-rw-r--r--   0 root         (0) docker     (999)       66 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/resources_nothing_set.yml
+-rw-r--r--   0 root         (0) docker     (999)      119 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/profiles/with_node_constraints.yml
+drwxr-xr-x   0 root         (0) docker     (999)        0 2023-07-20 18:57:44.874718 compose-flow-4.0.0rc1/src/tests/files/values/
+-rw-r--r--   0 root         (0) docker     (999)       93 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/values/good-resources-values.yaml
+-rw-r--r--   0 root         (0) docker     (999)       69 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/files/values/multidoc-values.yaml
+-rw-r--r--   0 root         (0) docker     (999)     3203 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_backends.py
+-rw-r--r--   0 root         (0) docker     (999)      695 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_base.py
+-rw-r--r--   0 root         (0) docker     (999)     7664 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_deploy.py
+-rw-r--r--   0 root         (0) docker     (999)      813 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_docker.py
+-rw-r--r--   0 root         (0) docker     (999)     5524 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_docker_image.py
+-rw-r--r--   0 root         (0) docker     (999)     6417 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_env.py
+-rw-r--r--   0 root         (0) docker     (999)     6254 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_kube_checks.py
+-rw-r--r--   0 root         (0) docker     (999)      606 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_kube_mixins.py
+-rw-r--r--   0 root         (0) docker     (999)      719 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_passthrough.py
+-rw-r--r--   0 root         (0) docker     (999)     3813 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_pod.py
+-rw-r--r--   0 root         (0) docker     (999)     8457 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_profile.py
+-rw-r--r--   0 root         (0) docker     (999)     5287 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_publish.py
+-rw-r--r--   0 root         (0) docker     (999)     1454 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_remote.py
+-rw-r--r--   0 root         (0) docker     (999)      903 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_service.py
+-rw-r--r--   0 root         (0) docker     (999)      468 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_shell.py
+-rw-r--r--   0 root         (0) docker     (999)      976 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_task.py
+-rw-r--r--   0 root         (0) docker     (999)      923 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_utils.py
+-rw-r--r--   0 root         (0) docker     (999)     6266 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/test_workflow.py
+-rw-r--r--   0 root         (0) docker     (999)      408 2023-07-20 18:56:34.000000 compose-flow-4.0.0rc1/src/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `compose-flow-3.8.2/README.md` & `compose-flow-4.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/compose/compose-flow.yml` & `compose-flow-4.0.0rc1/compose/compose-flow.yml`

 * *Files 23% similar despite different names*

```diff
@@ -23,26 +23,26 @@
   dev:
     backend: rancher
   prod:
     backend: rancher
 
 tasks:
   blacken:
-    command: compose-flow compose run --rm app black --target-version py36 --target-version py37 --target-version py38 .
+    command: compose-flow compose run --rm app black --target-version py39 .
 
   blacken-check:
-    command: compose-flow compose run --rm app black --target-version py36 --target-version py37 --target-version py38 --check .
+    command: compose-flow compose run --rm app black --target-version py39 --check .
 
   publish:
     command: compose-flow compose run -u root:docker --rm app /bin/bash ./scripts/publish.sh
 
   test:
     command: compose-flow compose run --rm app nosetests -v ./src
 
   lint:
     command: compose-flow compose run --rm app /bin/bash -c 'pylama ./src'
 
   jenkinslint:
-    command: compose-flow compose run -u root:docker --rm app /bin/bash -c 'black --target-version py36 --target-version py37 --target-version py38 --check . && (pylama -r results/pylama.log -f pylint setup.py ./scripts ./src || /bin/true)'
+    command: compose-flow compose run -u root:docker --rm app /bin/bash -c 'black --target-version py39 --check . && (pylama -r results/pylama.log -f pylint setup.py ./scripts ./src || /bin/true)'
 
   jenkinstest:
     command: compose-flow compose run -u root:docker --rm app /bin/bash -c 'nosetests -v ./src --with-xunit --xunit-file=results/report.xml || /bin/true'
```

### Comparing `compose-flow-3.8.2/scripts/dump_swarm_config.py` & `compose-flow-4.0.0rc1/scripts/dump_swarm_config.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/PKG-INFO` & `compose-flow-4.0.0rc1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,88 @@
 Metadata-Version: 2.1
 Name: compose-flow
-Version: 3.8.2
+Version: 4.0.0rc1
 Summary: codified workflows for docker compose
 Home-page: https://github.com/openslate/compose-flow
 Author: OpenSlate
 Author-email: code@openslate.com
-License: UNKNOWN
-Description: # Compose Flow
-        
-        This utility is built on top of [Docker Compose](https://docs.docker.com/compose/) and [Swarm Mode](https://docs.docker.com/engine/swarm/).  It establishes workflow conventions that are easily shared between team members -- and butlers -- who need to manage and deploy services, including:
-        
-        - managing [Stacks](https://docs.docker.com/get-started/part5/#prerequisites) across multiple Swarms (e.g. separate dev and prod Swarms)
-        - connecting to and working with service containers
-        - building and publishing images
-        - sharing service configuration between team members
-        
-        
-        ## Installation
-        
-        ```
-        pip install compose-flow
-        ```
-        
-        
-        ## Compose-Flow configuration
-        
-        Create the file `~/.compose/config.yml` with the following sections.
-        
-        ### Build
-        
-        ```yaml
-        build:
-          # the image prefix can be your Docker Hub username or a private registry address
-          image_prefix: myprivateregistry.com
-        ```
-        
-        ### Remotes
-        
-        ```yaml
-        remotes:
-          local:
-            backend: swarm
-          test:
-            backend: rancher
-            rancher:
-              project: Ops
-              cluster: prod
-          dev:
-            backend: rancher
-          prod:
-            backend: rancher
-        ```
-        
-        With this in place you're ready to go onto your project setup.
-        
-        
-        # A basic example
-        
-        This is the most basic file to get started.
-        
-        Place this at `compose/compose-flow.yml` in your project directory:
-        
-        ```
-        profiles:
-          local:
-            - docker-compose.yml
-        ```
-        
-        Alongside it, place the file `compose/docker-compose.yml`:
-        
-        ```
-        version: '3.7'
-        services:
-          app:
-            build: ..
-            image: ${DOCKER_IMAGE}
-        ```
-        
-        For building, run: `compose-flow build`.
-        
-        For publishing: `compose-flow publish`.
-        
-        For deploying as configured above: `compose-flow -e local deploy`.
-        
-        More information at [docs/advanced.md](docs/advanced.md)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Compose Flow
+
+This utility is built on top of [Docker Compose](https://docs.docker.com/compose/) and [Swarm Mode](https://docs.docker.com/engine/swarm/).  It establishes workflow conventions that are easily shared between team members -- and butlers -- who need to manage and deploy services, including:
+
+- managing [Stacks](https://docs.docker.com/get-started/part5/#prerequisites) across multiple Swarms (e.g. separate dev and prod Swarms)
+- connecting to and working with service containers
+- building and publishing images
+- sharing service configuration between team members
+
+
+## Installation
+
+```
+pip install compose-flow
+```
+
+
+## Compose-Flow configuration
+
+Create the file `~/.compose/config.yml` with the following sections.
+
+### Build
+
+```yaml
+build:
+  # the image prefix can be your Docker Hub username or a private registry address
+  image_prefix: myprivateregistry.com
+```
+
+### Remotes
+
+```yaml
+remotes:
+  local:
+    backend: swarm
+  test:
+    backend: rancher
+    rancher:
+      project: Ops
+      cluster: prod
+  dev:
+    backend: rancher
+  prod:
+    backend: rancher
+```
+
+With this in place you're ready to go onto your project setup.
+
+
+# A basic example
+
+This is the most basic file to get started.
+
+Place this at `compose/compose-flow.yml` in your project directory:
+
+```
+profiles:
+  local:
+    - docker-compose.yml
+```
+
+Alongside it, place the file `compose/docker-compose.yml`:
+
+```
+version: '3.7'
+services:
+  app:
+    build: ..
+    image: ${DOCKER_IMAGE}
+```
+
+For building, run: `compose-flow build`.
+
+For publishing: `compose-flow publish`.
+
+For deploying as configured above: `compose-flow -e local deploy`.
+
+More information at [docs/advanced.md](docs/advanced.md)
```

### Comparing `compose-flow-3.8.2/setup.py` & `compose-flow-4.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/LICENSE` & `compose-flow-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/Dockerfile` & `compose-flow-4.0.0rc1/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-FROM python:3.6-stretch
-MAINTAINER osslabs <code@openslatedata.com>
+FROM python:3.9-bullseye
+LABEL maintainer="code@doubleverify.com"
 
 ARG user=swarmclient
 ARG group=swarmclient
 ARG uid=1000
 ARG gid=1000
 
 ENV HOME /home/${user}
@@ -71,8 +71,10 @@
 
 RUN python setup.py install
 
 RUN chown -R ${user}:${group} ${HOME} ${SRC_DIR}
 
 USER ${user}
 
+RUN git config --global --add safe.directory ${SRC_DIR}
+
 ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
```

### Comparing `compose-flow-3.8.2/src/tests/test_remote.py` & `compose-flow-4.0.0rc1/src/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_workflow.py` & `compose-flow-4.0.0rc1/src/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_pod.py` & `compose-flow-4.0.0rc1/src/tests/test_pod.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_utils.py` & `compose-flow-4.0.0rc1/src/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,19 +14,17 @@
         rendered = utils.render(content, env=env)
 
         expected = f'      - /tmp/jenkins/{env["JOB_NAME"]}/{env["BUILD_NUMBER"]}:/usr/local/src/results'
 
         self.assertEqual(expected, rendered)
 
     def test_get_kv(self, *mocks):
-        """Ensure a single item is parsed
-        """
+        """Ensure a single item is parsed"""
         data = utils.get_kv("FOO=one")
 
         self.assertEqual(("FOO", "one"), data)
 
     def test_get_kv_multiple(self, *mocks):
-        """Ensure multiple items are parsed
-        """
+        """Ensure multiple items are parsed"""
         data = utils.get_kv("FOO=one\nBAR=two", multiple=True)
 
         self.assertEqual([("FOO", "one"), ("BAR", "two")], data)
```

### Comparing `compose-flow-3.8.2/src/tests/test_publish.py` & `compose-flow-4.0.0rc1/src/tests/test_publish.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_passthrough.py` & `compose-flow-4.0.0rc1/src/tests/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/files/manifests/good-init-deployment.yaml` & `compose-flow-4.0.0rc1/src/tests/files/manifests/good-init-deployment.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/files/manifests/good-job.yaml` & `compose-flow-4.0.0rc1/src/tests/files/manifests/good-job.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/files/manifests/no-limits-deployment.yaml` & `compose-flow-4.0.0rc1/src/tests/files/manifests/no-limits-deployment.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/files/manifests/good-cronjob.yaml` & `compose-flow-4.0.0rc1/src/tests/files/manifests/good-cronjob.yaml`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_service.py` & `compose-flow-4.0.0rc1/src/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_backends.py` & `compose-flow-4.0.0rc1/src/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_docker_image.py` & `compose-flow-4.0.0rc1/src/tests/test_docker_image.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_deploy.py` & `compose-flow-4.0.0rc1/src/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_base.py` & `compose-flow-4.0.0rc1/src/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_docker.py` & `compose-flow-4.0.0rc1/src/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_task.py` & `compose-flow-4.0.0rc1/src/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_kube_checks.py` & `compose-flow-4.0.0rc1/src/tests/test_kube_checks.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_profile.py` & `compose-flow-4.0.0rc1/src/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/tests/test_kube_mixins.py` & `compose-flow-4.0.0rc1/src/tests/test_kube_mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from unittest import TestCase, mock
 
 from compose_flow.kube.mixins import KubeMixIn
 
 
 class KubeMixInTestCase(TestCase):
     def test_get_secret_name_param(self, *mocks):
-        """Ensure the name param is used when getting a secret
-        """
+        """Ensure the name param is used when getting a secret"""
         mixin = KubeMixIn()
         mixin.workflow = mock.Mock(config_name="BAD")
         mixin.namespace = "something"
         mixin.execute = mock.Mock()
 
         secret_name = "GOODNAME"
         mixin._get_secret(secret_name)
```

### Comparing `compose-flow-3.8.2/src/tests/test_env.py` & `compose-flow-4.0.0rc1/src/tests/test_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,15 @@
         flow = Workflow(argv=command)
         env = Env(flow)
 
         self.assertEqual(flow.config_name, "dev-testdirname")
 
     @mock.patch("compose_flow.commands.subcommands.env.get_backend")
     def test_empty_env_value(self, *mocks):
-        """Ensure that a value can be empty if the line ends with an equals
-        """
+        """Ensure that a value can be empty if the line ends with an equals"""
         get_backend_mock = mocks[0]
         get_backend_mock.return_value.read.return_value = "FOO="
 
         command = shlex.split("-e dev env cat")
         flow = Workflow(argv=command)
 
         self.assertEquals("", flow.environment.data["FOO"])
@@ -182,16 +181,15 @@
         assert os.environ.get("FOO") is None
         with self.assertRaises(errors.RuntimeEnvError):
             # noinspection PyStatementEffect
             flow.profile.data["services"]
 
     @mock.patch("compose_flow.commands.subcommands.env.get_backend")
     def test_rendered_extends(self, *mocks):
-        """Ensure the rendered config includes extended variables
-        """
+        """Ensure the rendered config includes extended variables"""
 
         def backend_read(config_name):
             data = "CF_ENV_EXTENDS_BASENAME=foo"
             if "foo" in config_name:
                 data = "FOO=true"
 
             return data
```

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/swarm.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/swarm.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/base.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/publish.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/publish.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/env.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
         # the original values for config items whose values have been rendered
         # for example, the value for `FOO=runtime://` will be whatever $FOO is at runtime
         # similarly, the value for `FOO=runtime://BAR` will be whatever $BAR is at runtime
         self._rendered_config = {}
 
     def _get_default_backend(self, remote):
-
         app_config = self.workflow.app_config
 
         remote_section = app_config.get("remotes", {}).get(remote, {})
 
         if "environment" in remote_section.keys():
             warning_msg = (
                 "The environment subsection of .compose/config.yml has been deprecated! "
```

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/deploy.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/deploy.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/compose.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/compose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/remote.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/remote.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/service.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/pod.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/pod.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 from compose_flow.kube.mixins import KubeMixIn
 from .base import BaseSubcommand
 from compose_flow import errors, shell
 
 
 class Pod(BaseSubcommand, KubeMixIn):
-
     command_name = "pod"
 
     setup_environment = True
 
     setup_profile = False
 
     @property
```

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/task.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/task.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/passthrough_base.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/passthrough_base.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/kompose.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/kompose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/profile.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/profile.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/remote_config.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/remote_config.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/subcommands/__init__.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/commands/workflow.py` & `compose-flow-4.0.0rc1/src/compose_flow/commands/workflow.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/settings.py` & `compose-flow-4.0.0rc1/src/compose_flow/settings.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/errors.py` & `compose-flow-4.0.0rc1/src/compose_flow/errors.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/shell.py` & `compose-flow-4.0.0rc1/src/compose_flow/shell.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/docker.py` & `compose-flow-4.0.0rc1/src/compose_flow/docker.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/config.py` & `compose-flow-4.0.0rc1/src/compose_flow/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+import logging
 import os
 import pathlib
 import typing
 
 from functools import lru_cache
 
-from influxstats.logging import get_logger
-
 from compose_flow.utils import remerge, yaml_dump, yaml_load
 
 if typing.TYPE_CHECKING:
     from .commands.workflow import Workflow
 
 DictNone = typing.Union[dict, None]
 
@@ -51,15 +50,15 @@
 
 def get_base_config_name(workflow: "Workflow") -> str:
     """Returns the config name without the environment prefix
 
     Args:
         workflow: The running workflow
     """
-    logger = get_logger()
+    logger = logging.getLogger(__name__)
 
     base_config_name = workflow.config_name
 
     # NOTE: use environment_name instead of environment because
     # using the latter may cause a recursive loop
     environment_prefix = f"{workflow.environment_name}-"
 
@@ -87,19 +86,18 @@
 
     data = check_config(workflow, data)
 
     return data
 
 
 def read_project_config(workflow: "Workflow") -> dict:
-    """Reads the project config from the filesystem
-    """
+    """Reads the project config from the filesystem"""
     data = {}
 
-    logger = get_logger()
+    logger = logging.getLogger(__name__)
 
     compose_flow_filename = workflow.args.compose_flow_filename
 
     if compose_flow_filename:
         paths = [compose_flow_filename]
     else:
         config_name_config_file = f"compose-flow.{workflow.config_basename}.yml"
```

### Comparing `compose-flow-3.8.2/src/compose_flow/utils.py` & `compose-flow-4.0.0rc1/src/compose_flow/utils.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/compose.py` & `compose-flow-4.0.0rc1/src/compose_flow/compose.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/entrypoints.py` & `compose-flow-4.0.0rc1/src/compose_flow/entrypoints.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/kube/checks.py` & `compose-flow-4.0.0rc1/src/compose_flow/kube/checks.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/kube/mixins.py` & `compose-flow-4.0.0rc1/src/compose_flow/kube/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=E1101  # disable no-member error
+
 """
 Compose subcommand
 """
 import base64
 from functools import lru_cache
 import os
 import pathlib
```

### Comparing `compose-flow-3.8.2/src/compose_flow/environment/backends/kube_backend.py` & `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/kube_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/environment/backends/local_backend.py` & `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/environment/backends/base_backend.py` & `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/base_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/environment/backends/rancher_backend.py` & `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/rancher_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/environment/backends/swarm_backend.py` & `compose-flow-4.0.0rc1/src/compose_flow/environment/backends/swarm_backend.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow/docker_image.py` & `compose-flow-4.0.0rc1/src/compose_flow/docker_image.py`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow.egg-info/SOURCES.txt` & `compose-flow-4.0.0rc1/src/compose_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/src/compose_flow.egg-info/PKG-INFO` & `compose-flow-4.0.0rc1/src/compose_flow.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,88 @@
 Metadata-Version: 2.1
 Name: compose-flow
-Version: 3.8.2
+Version: 4.0.0rc1
 Summary: codified workflows for docker compose
 Home-page: https://github.com/openslate/compose-flow
 Author: OpenSlate
 Author-email: code@openslate.com
-License: UNKNOWN
-Description: # Compose Flow
-        
-        This utility is built on top of [Docker Compose](https://docs.docker.com/compose/) and [Swarm Mode](https://docs.docker.com/engine/swarm/).  It establishes workflow conventions that are easily shared between team members -- and butlers -- who need to manage and deploy services, including:
-        
-        - managing [Stacks](https://docs.docker.com/get-started/part5/#prerequisites) across multiple Swarms (e.g. separate dev and prod Swarms)
-        - connecting to and working with service containers
-        - building and publishing images
-        - sharing service configuration between team members
-        
-        
-        ## Installation
-        
-        ```
-        pip install compose-flow
-        ```
-        
-        
-        ## Compose-Flow configuration
-        
-        Create the file `~/.compose/config.yml` with the following sections.
-        
-        ### Build
-        
-        ```yaml
-        build:
-          # the image prefix can be your Docker Hub username or a private registry address
-          image_prefix: myprivateregistry.com
-        ```
-        
-        ### Remotes
-        
-        ```yaml
-        remotes:
-          local:
-            backend: swarm
-          test:
-            backend: rancher
-            rancher:
-              project: Ops
-              cluster: prod
-          dev:
-            backend: rancher
-          prod:
-            backend: rancher
-        ```
-        
-        With this in place you're ready to go onto your project setup.
-        
-        
-        # A basic example
-        
-        This is the most basic file to get started.
-        
-        Place this at `compose/compose-flow.yml` in your project directory:
-        
-        ```
-        profiles:
-          local:
-            - docker-compose.yml
-        ```
-        
-        Alongside it, place the file `compose/docker-compose.yml`:
-        
-        ```
-        version: '3.7'
-        services:
-          app:
-            build: ..
-            image: ${DOCKER_IMAGE}
-        ```
-        
-        For building, run: `compose-flow build`.
-        
-        For publishing: `compose-flow publish`.
-        
-        For deploying as configured above: `compose-flow -e local deploy`.
-        
-        More information at [docs/advanced.md](docs/advanced.md)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Compose Flow
+
+This utility is built on top of [Docker Compose](https://docs.docker.com/compose/) and [Swarm Mode](https://docs.docker.com/engine/swarm/).  It establishes workflow conventions that are easily shared between team members -- and butlers -- who need to manage and deploy services, including:
+
+- managing [Stacks](https://docs.docker.com/get-started/part5/#prerequisites) across multiple Swarms (e.g. separate dev and prod Swarms)
+- connecting to and working with service containers
+- building and publishing images
+- sharing service configuration between team members
+
+
+## Installation
+
+```
+pip install compose-flow
+```
+
+
+## Compose-Flow configuration
+
+Create the file `~/.compose/config.yml` with the following sections.
+
+### Build
+
+```yaml
+build:
+  # the image prefix can be your Docker Hub username or a private registry address
+  image_prefix: myprivateregistry.com
+```
+
+### Remotes
+
+```yaml
+remotes:
+  local:
+    backend: swarm
+  test:
+    backend: rancher
+    rancher:
+      project: Ops
+      cluster: prod
+  dev:
+    backend: rancher
+  prod:
+    backend: rancher
+```
+
+With this in place you're ready to go onto your project setup.
+
+
+# A basic example
+
+This is the most basic file to get started.
+
+Place this at `compose/compose-flow.yml` in your project directory:
+
+```
+profiles:
+  local:
+    - docker-compose.yml
+```
+
+Alongside it, place the file `compose/docker-compose.yml`:
+
+```
+version: '3.7'
+services:
+  app:
+    build: ..
+    image: ${DOCKER_IMAGE}
+```
+
+For building, run: `compose-flow build`.
+
+For publishing: `compose-flow publish`.
+
+For deploying as configured above: `compose-flow -e local deploy`.
+
+More information at [docs/advanced.md](docs/advanced.md)
```

### Comparing `compose-flow-3.8.2/docs/k8s.md` & `compose-flow-4.0.0rc1/docs/k8s.md`

 * *Files identical despite different names*

### Comparing `compose-flow-3.8.2/docs/advanced.md` & `compose-flow-4.0.0rc1/docs/advanced.md`

 * *Files identical despite different names*

