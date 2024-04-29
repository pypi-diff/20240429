# Comparing `tmp/paka-0.1.5.tar.gz` & `tmp/paka-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.5.tar", max compression
+gzip compressed data, was "paka-0.1.6.tar", max compression
```

## Comparing `paka-0.1.5.tar` & `paka-0.1.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1072 2024-04-25 22:57:30.021339 paka-0.1.5/LICENSE
--rw-r--r--   0        0        0     4570 2024-04-25 22:57:30.021339 paka-0.1.5/README.md
--rw-r--r--   0        0        0      153 2024-04-25 22:57:30.025339 paka-0.1.5/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/__init__.py
--rw-r--r--   0        0        0     1608 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/__main__.py
--rw-r--r--   0        0        0     1141 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/build.py
--rw-r--r--   0        0        0     3891 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/cluster.py
--rw-r--r--   0        0        0     6726 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/function.py
--rw-r--r--   0        0        0     5910 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/job.py
--rw-r--r--   0        0        0      427 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     1943 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/model_group.py
--rw-r--r--   0        0        0     3188 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/run.py
--rw-r--r--   0        0        0     8815 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3113 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      722 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2521 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    12154 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1468 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      725 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     4078 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1932 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     4643 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1228 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/keda.py
--rw-r--r--   0        0        0     4956 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/knative.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     2686 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      879 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/namespace.py
--rw-r--r--   0        0        0     3414 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/nvidia_device_plugin.py
--rw-r--r--   0        0        0     4273 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     4000 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2325 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/redis.py
--rw-r--r--   0        0        0      935 2024-04-25 22:57:30.025339 paka-0.1.5/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    16434 2024-04-25 22:57:30.025339 paka-0.1.5/paka/config.py
--rw-r--r--   0        0        0      115 2024-04-25 22:57:30.025339 paka-0.1.5/paka/constants.py
--rw-r--r--   0        0        0     3015 2024-04-25 22:57:30.025339 paka-0.1.5/paka/container/ecr.py
--rw-r--r--   0        0        0     2374 2024-04-25 22:57:30.025339 paka-0.1.5/paka/container/pack.py
--rw-r--r--   0        0        0    19188 2024-04-25 22:57:30.025339 paka-0.1.5/paka/k8s.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/function/__init__.py
--rw-r--r--   0        0        0     5742 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/function/service.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/job/__init__.py
--rw-r--r--   0        0        0     2342 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/job/autoscaler.py
--rw-r--r--   0        0        0     4142 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/job/worker.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/model_group/__init__.py
--rw-r--r--   0        0        0     1358 2024-04-25 22:57:30.025339 paka-0.1.5/paka/kube_resources/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-04-25 22:57:30.029339 paka-0.1.5/paka/kube_resources/model_group/manifest.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.029339 paka-0.1.5/paka/kube_resources/model_group/runtime/__init__.py
--rw-r--r--   0        0        0     4306 2024-04-25 22:57:30.029339 paka-0.1.5/paka/kube_resources/model_group/runtime/llama_cpp.py
--rw-r--r--   0        0        0    17973 2024-04-25 22:57:30.029339 paka-0.1.5/paka/kube_resources/model_group/service.py
--rw-r--r--   0        0        0      761 2024-04-25 22:57:30.029339 paka-0.1.5/paka/logger.py
--rw-r--r--   0        0        0        0 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/__init__.py
--rw-r--r--   0        0        0     2946 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/base_model.py
--rw-r--r--   0        0        0     2352 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/hf_model.py
--rw-r--r--   0        0        0     1378 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/http_model.py
--rw-r--r--   0        0        0     1444 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/manifest.py
--rw-r--r--   0        0        0     2565 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/progress_bar.py
--rw-r--r--   0        0        0     7621 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/registry.py
--rw-r--r--   0        0        0     2086 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/settings.py
--rw-r--r--   0        0        0    10074 2024-04-25 22:57:30.029339 paka-0.1.5/paka/model/store.py
--rw-r--r--   0        0        0     9786 2024-04-25 22:57:30.029339 paka-0.1.5/paka/utils.py
--rw-r--r--   0        0        0     1379 2024-04-25 22:57:30.029339 paka-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5816 1970-01-01 00:00:00.000000 paka-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-29 21:50:17.981877 paka-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4467 2024-04-29 21:50:17.981877 paka-0.1.6/README.md
+-rw-r--r--   0        0        0      153 2024-04-29 21:50:17.985877 paka-0.1.6/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/__main__.py
+-rw-r--r--   0        0        0     1141 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/build.py
+-rw-r--r--   0        0        0     3845 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/cluster.py
+-rw-r--r--   0        0        0     6721 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/function.py
+-rw-r--r--   0        0        0     5905 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/job.py
+-rw-r--r--   0        0        0      433 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     1938 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3194 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/run.py
+-rw-r--r--   0        0        0     8974 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3113 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      722 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2521 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    12154 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1468 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      725 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     4078 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     1932 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     4643 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1228 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4956 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/knative.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     2609 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      879 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     3414 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/nvidia_device_plugin.py
+-rw-r--r--   0        0        0     4273 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     3702 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/pulumi.py
+-rw-r--r--   0        0        0     4000 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2325 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/redis.py
+-rw-r--r--   0        0        0      935 2024-04-29 21:50:17.985877 paka-0.1.6/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    16434 2024-04-29 21:50:17.985877 paka-0.1.6/paka/config.py
+-rw-r--r--   0        0        0      416 2024-04-29 21:50:17.985877 paka-0.1.6/paka/constants.py
+-rw-r--r--   0        0        0     3623 2024-04-29 21:50:17.985877 paka-0.1.6/paka/container/ecr.py
+-rw-r--r--   0        0        0     2886 2024-04-29 21:50:17.985877 paka-0.1.6/paka/container/pack.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/function/__init__.py
+-rw-r--r--   0        0        0     5748 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/function/service.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/job/__init__.py
+-rw-r--r--   0        0        0     2365 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/job/autoscaler.py
+-rw-r--r--   0        0        0     4137 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/job/worker.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.985877 paka-0.1.6/paka/k8s/model_group/__init__.py
+-rw-r--r--   0        0        0     1364 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/manifest.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/runtime/__init__.py
+-rw-r--r--   0        0        0     4596 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/runtime/llama_cpp.py
+-rw-r--r--   0        0        0    21055 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/model_group/service.py
+-rw-r--r--   0        0        0    19377 2024-04-29 21:50:17.989877 paka-0.1.6/paka/k8s/utils.py
+-rw-r--r--   0        0        0      761 2024-04-29 21:50:17.989877 paka-0.1.6/paka/logger.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/__init__.py
+-rw-r--r--   0        0        0     3031 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/base_model.py
+-rw-r--r--   0        0        0     2352 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/hf_model.py
+-rw-r--r--   0        0        0     1378 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/http_model.py
+-rw-r--r--   0        0        0     1444 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/manifest.py
+-rw-r--r--   0        0        0     2565 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/progress_bar.py
+-rw-r--r--   0        0        0     2086 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/settings.py
+-rw-r--r--   0        0        0    10057 2024-04-29 21:50:17.989877 paka-0.1.6/paka/model/store.py
+-rw-r--r--   0        0        0    10896 2024-04-29 21:50:17.989877 paka-0.1.6/paka/utils.py
+-rw-r--r--   0        0        0     1410 2024-04-29 21:50:17.989877 paka-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 paka-0.1.6/PKG-INFO
```

### Comparing `paka-0.1.5/LICENSE` & `paka-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/README.md` & `paka-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Welcome to Paka
 
-<img src="docs/img/paka.svg" alt="paka.svg" width="200" height="200">
+<img src="https://raw.githubusercontent.com/jjleng/paka/main/docs/img/paka.svg" alt="paka.svg" width="200" height="200">
 
 **paka** is a versatile LLMOps tool that simplifies the deployment and management of large language model (LLM) apps with a single command.
 
 ## Paka Highlights
 
 - **Cloud-Agnostic Resource Provisioning**: paka starts by breaking down the barriers of cloud vendor lock-in, currently supporting EKS with plans to expand to more cloud services.
 - **Optimized Model Execution**: Designed for efficiency, paka runs LLM models on CPUs and Nvidia GPUs, ensuring optimal performance. Auto-scaling of model replicas based on CPU usage, request rate, and latency.
@@ -95,24 +95,18 @@
 
 ### Destroy a cluster
 ```bash
 paka cluster down -f cluster.yaml
 ```
 
 ## Contributing
+- code changes
+- `make check-all`
 - Open a PR
-- Format and lint code with `make lint`
-- Run tests with `make test`
 
 ## Dependencies
-- docker daemon
-- pack cli (https://buildpacks.io/docs/for-platform-operators/how-to/integrate-ci/pack/)
-- pulumi cli (https://www.pulumi.com/docs/install/)
-- aws cli and credentials for the AWS deployment
+- docker daemon and CLI
+- credentials for the AWS cloud
 ```bash
-# Make sure aws credentials and cli are set up. Your aws credentials should have access to the following services:
-# - S3
-# - ECR
-# - EKS
-# - EC2
-aws configure
+# Ensure your AWS credentials are correctly configured. Execute the command below and verify that the keys `aws_access_key_id` and `aws_secret_access_key` are present.
+cat ~/.aws/credentials
 ```
```

### Comparing `paka-0.1.5/paka/cli/__main__.py` & `paka-0.1.6/paka/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cli/build.py` & `paka-0.1.6/paka/cli/build.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cli/cluster.py` & `paka-0.1.6/paka/cli/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import List
 
 import click
 import typer
 
 from paka.cli.utils import load_cluster_manager
-from paka.k8s import remove_crd_finalizers
-from paka.k8s import update_kubeconfig as merge_update_kubeconfig
+from paka.k8s.utils import remove_crd_finalizers
+from paka.k8s.utils import update_kubeconfig as merge_update_kubeconfig
 from paka.logger import logger
 
 cluster_app = typer.Typer()
 
 
 @cluster_app.command()
 def up(
@@ -63,29 +63,28 @@
     Tears down the Kubernetes cluster, removing all associated resources and data.
     """
     if yes or click.confirm(
         f"Are you sure you want to proceed with the operation? Please note that "
         "all resources and data will be permanently deleted.",
         default=False,
     ):
-        try:
-            # Sometime finalizers might block CRD deletion, so we need to force delete those.
-            # This is best effort and might not work in all cases.
-            # TODO: better way to handle this
-            remove_crd_finalizers(
-                "scaledobjects.keda.sh",
-            )
-            remove_crd_finalizers(
-                "routes.serving.knative.dev",
-            )
-            remove_crd_finalizers(
-                "ingresses.networking.internal.knative.dev",
-            )
-        except Exception:
-            pass
+        # Sometime finalizers might block CRD deletion, so we need to force delete those.
+        # This is best effort and might not work in all cases.
+        # TODO: better way to handle this
+        crds = [
+            "scaledobjects.keda.sh",
+            "routes.serving.knative.dev",
+            "ingresses.networking.internal.knative.dev",
+        ]
+
+        for crd in crds:
+            try:
+                remove_crd_finalizers(crd)
+            except Exception as e:
+                pass
 
         cluster_manager = load_cluster_manager(cluster_config)
         cluster_manager.destroy()
 
 
 @cluster_app.command()
 def preview(
```

### Comparing `paka-0.1.5/paka/cli/function.py` & `paka-0.1.6/paka/cli/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 import click
 import typer
 from kubernetes.dynamic.exceptions import NotFoundError
 from tabulate import tabulate
 
 from paka.cli.utils import resolve_image
-from paka.k8s import try_load_kubeconfig
-from paka.kube_resources.function.service import (
+from paka.k8s.function.service import (
     create_knative_service,
     delete_knative_service,
     list_knative_services,
 )
+from paka.k8s.utils import try_load_kubeconfig
 from paka.logger import logger
 from paka.utils import kubify_name, read_current_cluster_data
 
 try_load_kubeconfig()
 
 function_app = typer.Typer()
```

### Comparing `paka-0.1.5/paka/cli/job.py` & `paka-0.1.6/paka/cli/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Optional
 
 import click
 import typer
 from kubernetes import client
 
 from paka.cli.utils import resolve_image
-from paka.k8s import try_load_kubeconfig
-from paka.kube_resources.job.worker import create_workers, delete_workers
+from paka.k8s.job.worker import create_workers, delete_workers
+from paka.k8s.utils import try_load_kubeconfig
 from paka.logger import logger
 from paka.utils import kubify_name, read_current_cluster_data
 
 try_load_kubeconfig()
 
 job_app = typer.Typer()
```

### Comparing `paka-0.1.5/paka/cli/model_group.py` & `paka-0.1.6/paka/cli/model_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Set
 
 import boto3
 import typer
 from kubernetes import client
 from tabulate import tabulate
 
-from paka.k8s import try_load_kubeconfig
-from paka.kube_resources.model_group.service import MODEL_PATH_PREFIX, filter_services
+from paka.k8s.model_group.service import MODEL_PATH_PREFIX, filter_services
+from paka.k8s.utils import try_load_kubeconfig
 from paka.logger import logger
 from paka.utils import read_current_cluster_data
 
 try_load_kubeconfig()
 
 model_group_app = typer.Typer()
```

### Comparing `paka-0.1.5/paka/cli/run.py` & `paka-0.1.6/paka/cli/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shlex
 from typing import Optional
 
 import typer
 from kubernetes import client
 
 from paka.cli.utils import resolve_image
-from paka.k8s import tail_logs, try_load_kubeconfig
+from paka.k8s.utils import tail_logs, try_load_kubeconfig
 from paka.logger import logger
 from paka.utils import kubify_name, random_str, read_current_cluster_data
 
 CLEANUP_TIMEOUT = 600  # 10 minutes
 
 run_app = typer.Typer()
```

### Comparing `paka-0.1.5/paka/cli/utils.py` & `paka-0.1.6/paka/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typer
 
 from paka.cluster.manager.aws import AWSClusterManager
 from paka.cluster.manager.base import ClusterManager
 from paka.config import parse_yaml
 from paka.constants import BP_BUILDER_ENV_VAR
 from paka.container.ecr import push_to_ecr
-from paka.container.pack import install_pack
+from paka.container.pack import ensure_pack
 from paka.logger import logger
 from paka.utils import get_pulumi_root, read_current_cluster_data
 
 
 def build(
     source_dir: str,
     image_name: str,
@@ -31,15 +31,15 @@
     Args:
         source_dir (str): The directory containing the source code of the application.
         image_name (str): The name of the Docker image to build. If not provided, the name of the source directory is used.
 
     Returns:
         str: The image tag of the built Docker image.
     """
-    install_pack()
+    pack_bin = ensure_pack()
 
     source_dir = os.path.abspath(os.path.expanduser(source_dir))
 
     if not os.path.exists(os.path.join(source_dir, ".cnignore")):
         logger.error(".cnignore file does not exist in the source directory.")
         raise typer.Exit(1)
 
@@ -70,15 +70,15 @@
 
     try:
         subprocess.run(["cd", source_dir], check=True)
 
         builder = os.environ.get(BP_BUILDER_ENV_VAR, "paketobuildpacks/builder:base")
 
         pack_command = [
-            "pack",
+            pack_bin,
             "build",
             image_name,
             "--builder",
             builder,
         ]
         if bp_cpython_version:
             pack_command.extend(["--env", f"BP_CPYTHON_VERSION={bp_cpython_version}"])
@@ -239,7 +239,9 @@
     )
 
     pulumi_root = get_pulumi_root()
     os.makedirs(pulumi_root, exist_ok=True)
     os.environ["PULUMI_BACKEND_URL"] = os.environ.get(
         "PULUMI_BACKEND_URL", f"file://{pulumi_root}"
     )
+    os.environ["PULUMI_DEBUG"] = os.environ.get("PULUMI_DEBUG", "false")
+    os.environ["PULUMI_HOME"] = os.environ.get("PULUMI_HOME", pulumi_root)
```

### Comparing `paka-0.1.5/paka/cluster/aws/cloudwatch.py` & `paka-0.1.6/paka/cluster/aws/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/aws/cluster_autoscaler.py` & `paka-0.1.6/paka/cluster/aws/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/aws/container_registry.py` & `paka-0.1.6/paka/cluster/aws/container_registry.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.6/paka/cluster/aws/ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/aws/eks.py` & `paka-0.1.6/paka/cluster/aws/eks.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/aws/elb.py` & `paka-0.1.6/paka/cluster/aws/elb.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/aws/object_store.py` & `paka-0.1.6/paka/cluster/aws/object_store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/aws/service_account.py` & `paka-0.1.6/paka/cluster/aws/service_account.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/aws/utils.py` & `paka-0.1.6/paka/cluster/aws/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/fluentbit.py` & `paka-0.1.6/paka/cluster/fluentbit.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/keda.py` & `paka-0.1.6/paka/cluster/keda.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/knative.py` & `paka-0.1.6/paka/cluster/knative.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/manager/aws.py` & `paka-0.1.6/paka/cluster/manager/aws.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/manager/base.py` & `paka-0.1.6/paka/cluster/manager/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 from pulumi import automation as auto
 
+from paka.cluster.pulumi import ensure_pulumi
 from paka.config import CloudConfig, Config
-from paka.kube_resources.model_group.ingress import create_model_vservice
-from paka.kube_resources.model_group.service import create_model_group_service
+from paka.k8s.model_group.service import create_model_group_service
 from paka.logger import logger
 from paka.utils import read_cluster_data, save_cluster_data
 
 STACK_NAME = "default"
 
 
 class ClusterManager(ABC):
@@ -43,14 +43,16 @@
             stack_name=STACK_NAME,
             project_name=self.config.cluster.name,
             program=program,
         )
 
     @property
     def _stack(self) -> auto.Stack:
+        ensure_pulumi()
+
         def program() -> None:
             self.provision_k8s()
 
         return self._stack_for_program(program)
 
     def create(self) -> None:
         if self._orig_config.aws:
@@ -68,15 +70,14 @@
         if self.config.modelGroups is None:
             return
 
         namespace = read_cluster_data(self.config.cluster.name, "namespace")
 
         for model_group in self.config.modelGroups:
             create_model_group_service(namespace, self._orig_config, model_group)
-            create_model_vservice(namespace, model_group.name)
 
     def destroy(self) -> None:
         logger.info("Destroying resources...")
         self._stack.destroy(on_output=logger.info)
 
     def refresh(self) -> None:
         logger.info("Refreshing the stack...")
```

### Comparing `paka-0.1.5/paka/cluster/namespace.py` & `paka-0.1.6/paka/cluster/namespace.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/nvidia_device_plugin.py` & `paka-0.1.6/paka/cluster/nvidia_device_plugin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/prometheus.py` & `paka-0.1.6/paka/cluster/prometheus.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/qdrant.py` & `paka-0.1.6/paka/cluster/qdrant.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/redis.py` & `paka-0.1.6/paka/cluster/redis.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/cluster/zipkin.py` & `paka-0.1.6/paka/cluster/zipkin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/config.py` & `paka-0.1.6/paka/config.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/container/ecr.py` & `paka-0.1.6/paka/container/ecr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,43 @@
-import shlex
+import base64
 import subprocess
 
+import boto3
+
 from paka.logger import logger
 from paka.utils import random_str
 
 
+def authenticate_docker_to_ecr(aws_region: str) -> str:
+    try:
+        ecr_client = boto3.client("ecr", region_name=aws_region)
+        token = ecr_client.get_authorization_token()
+        username, password = (
+            base64.b64decode(token["authorizationData"][0]["authorizationToken"])
+            .decode("utf-8")
+            .split(":")
+        )
+        ecr_url = token["authorizationData"][0]["proxyEndpoint"]
+
+        p = subprocess.Popen(
+            ["docker", "login", "-u", username, "--password-stdin", ecr_url],
+            stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        stdout, stderr = p.communicate(input=password.encode())
+        if p.returncode != 0:
+            raise Exception(f"Docker login failed: {stderr.decode()}")
+
+        return ecr_url
+    except Exception as e:
+        print(f"An error occurred: {str(e)}")
+        raise
+
+
 def push_to_ecr(
     image_name: str, repository_uri: str, aws_region: str, app_name: str
 ) -> str:
     """
     Pushes a Docker image to an Amazon ECR repository.
 
     This function tags the Docker image with a version tag and the "latest" tag,
@@ -29,23 +58,14 @@
     Raises:
         subprocess.CalledProcessError: If an error occurs while executing a subprocess command.
 
     Returns:
         str: The version tag of the image that was pushed.
     """
     try:
-        # Get ECR login password
-        login_password = (
-            subprocess.check_output(
-                ["aws", "ecr", "get-login-password", "--region", aws_region]
-            )
-            .decode()
-            .strip()
-        )
-
         # Generate a random version number
         version = random_str()
 
         # Tag the image with the repository URI and the version tag
         version_tag = f"{app_name}-v{version}"
 
         # Tag the image with the repository URI
@@ -67,21 +87,21 @@
                 "tag",
                 f"{image_name}:latest",
                 f"{repository_uri}:{latest_tag}",
             ],
             check=True,
         )
 
-        # Perform Docker login and push in one command
-        login_push_cmd = (
-            f"echo {shlex.quote(login_password)} | "
-            f"docker login --username AWS --password-stdin {repository_uri} && "
-            f"docker push {repository_uri}:{version_tag} && "
-            f"docker push {repository_uri}:{latest_tag}"
+        # Authenticate Docker to the ECR
+        authenticate_docker_to_ecr(aws_region)
+
+        # Push the image to the ECR repository
+        subprocess.run(
+            ["docker", "push", f"{repository_uri}:{version_tag}"], check=True
         )
-        subprocess.run(login_push_cmd, shell=True, check=True, executable="/bin/sh")
+        subprocess.run(["docker", "push", f"{repository_uri}:{latest_tag}"], check=True)
 
         logger.info(f"Successfully pushed {image_name} to {repository_uri}")
         return version_tag
     except subprocess.CalledProcessError as e:
         logger.error(f"An error occurred: {e}")
         raise
```

### Comparing `paka-0.1.5/paka/container/pack.py` & `paka-0.1.6/paka/container/pack.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,105 @@
 import os
 import platform
-import shutil
 import tarfile
 import tempfile
 import zipfile
+from pathlib import Path
 
 import requests
 
 from paka.logger import logger
+from paka.utils import (
+    calculate_sha256,
+    get_gh_release_latest_version,
+    get_project_data_dir,
+)
 
 
-def get_latest_pack_version() -> str:
-    url = "https://api.github.com/repos/buildpacks/pack/releases/latest"
-    response = requests.get(url)
-    response.raise_for_status()
-    data = response.json()
-    return data["tag_name"][1:]  # Remove the 'v' prefix
+def ensure_pack() -> str:
+    paka_home = Path(get_project_data_dir())
 
+    bin_dir = paka_home / "bin"
+    bin_dir.mkdir(parents=True, exist_ok=True)
 
-def install_pack() -> None:
-    if shutil.which("pack"):
-        return
+    pack_files = list(bin_dir.glob("pack-*"))
+    if pack_files:
+        return str(pack_files[0])
+
+    pack_version = get_gh_release_latest_version("buildpacks/pack")
+
+    new_pack_path = bin_dir / f"pack-{pack_version}"
 
     system = platform.system().lower()
     arch = platform.machine().lower()
 
+    if system == "windows":
+        new_pack_path = new_pack_path.with_suffix(".exe")
+
+    if new_pack_path.exists():
+        return str(new_pack_path)
+
+    for old_pack_path in bin_dir.glob("pack-*"):
+        if old_pack_path.is_file():
+            old_pack_path.unlink()
+
     if system == "darwin":
         system = "macos"
 
-    pack_version = get_latest_pack_version()
-
     if system == "windows":
-        pack_file = f"pack-v{pack_version}-windows.zip"
-
-        program_files_dir = os.environ.get("PROGRAMFILES", "C:\\Program Files")
-        bin_dir = os.path.join(
-            program_files_dir, "pack"
-        )  # Replace 'YourAppName' with your application's name
-
-        # Check if the script is running with administrator privileges
-        if not os.path.exists(bin_dir):
-            try:
-                os.makedirs(bin_dir)
-            except PermissionError:
-                logger.error("Administrator privileges required.")
-                raise
+        pack_file = f"pack-{pack_version}-windows.zip"
 
     elif arch in ["amd64", "x86_64"]:
-        pack_file = f"pack-v{pack_version}-{system}.tgz"
+        pack_file = f"pack-{pack_version}-{system}.tgz"
     elif arch == "arm64":
-        pack_file = f"pack-v{pack_version}-{system}-{arch}.tgz"
+        pack_file = f"pack-{pack_version}-{system}-{arch}.tgz"
     else:
         raise Exception(f"Unsupported architecture: {arch}")
 
-    url = f"https://github.com/buildpacks/pack/releases/download/v{pack_version}/{pack_file}"
+    url = f"https://github.com/buildpacks/pack/releases/download/{pack_version}/{pack_file}"
 
     logger.info(f"Downloading {pack_file}...")
-    try:
-        with tempfile.NamedTemporaryFile(delete=False) as tf:
-            with requests.get(url, stream=True) as r:
-                r.raise_for_status()
-                for chunk in r.iter_content(chunk_size=8192):
-                    tf.write(chunk)
-            local_file = tf.name
+
+    with tempfile.NamedTemporaryFile() as tf:
+        with requests.get(url, stream=True) as r:
+            r.raise_for_status()
+            for chunk in r.iter_content(chunk_size=8192):
+                tf.write(chunk)
+
+        tf.flush()
+        os.fsync(tf.fileno())
+
+        archive_file = tf.name
+
+        archive_file_sha256 = calculate_sha256(archive_file)
+
+        # Now, fetch the sha256 file and compare the hash
+        sha256_url = f"{url}.sha256"
+
+        response = requests.get(sha256_url)
+        response.raise_for_status()
+        expected_sha256, expected_filename = response.text.strip().split()
+
+        assert expected_filename == pack_file
+
+        if archive_file_sha256 != expected_sha256:
+            raise Exception(
+                f"SHA256 mismatch: {archive_file_sha256} != {expected_sha256}"
+            )
 
         if system == "windows":
-            with zipfile.ZipFile(local_file, "r") as zip_ref:
+            with zipfile.ZipFile(archive_file, "r") as zip_ref:
                 zip_ref.extractall(bin_dir)
         else:
-            with tarfile.open(local_file, "r:gz") as tar:
-                tar.extractall("/usr/local/bin")
-            os.chmod("/usr/local/bin/pack", 0o755)
-    finally:
-        if local_file is not None:
-            os.unlink(local_file)
+            with tarfile.open(archive_file, "r:gz") as tar:
+                tar.extractall(bin_dir)
+        pack_path = bin_dir / "pack"
+
+        if system == "windows":
+            pack_path = pack_path.with_suffix(".exe")
+
+        pack_path.chmod(0o755)
+        pack_path.rename(new_pack_path)
 
     logger.info("Pack installed successfully.")
+
+    return str(new_pack_path)
```

### Comparing `paka-0.1.5/paka/k8s.py` & `paka-0.1.6/paka/k8s/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,14 @@
     Returns:
         Any: The response from the API call.
 
     Raises:
         ValueError: If the resource kind is unsupported.
         ApiException: If an error occurs while creating or updating the resource.
     """
-
     # Determine the resource kind and prepare the appropriate API client
     kind = resource.kind
     namespace = resource.metadata.namespace
     if not namespace:
         raise ValueError("Namespace is required")
 
     if kind == "Deployment":
@@ -474,17 +473,21 @@
         stop_event.set()
         forward_thread.join()
 
     return ready_event, stop_port_forward
 
 
 def setup_port_forward(
-    label_selector: str, namespace: str, container_port: int
+    label_selector: str,
+    namespace: str,
+    container_port: int,
+    local_port: Optional[int] = None,
 ) -> Tuple[str, Callable[[], None]]:
-    local_port = find_free_port()
+    if local_port is None:
+        local_port = find_free_port()
 
     max_duration = 2
 
     ready_event, stop_forward = run_port_forward(
         label_selector, local_port, container_port, namespace
     )
 
@@ -509,14 +512,15 @@
     logger.debug(f"Port forward from local port {local_port} started")
 
     return str(local_port), stop_forward
 
 
 def try_load_kubeconfig() -> bool:
     try:
+        # read kube config from the file specified by env var KUBECONFIG or the default location ~/.kube/config
         config.load_kube_config()
         return True
     except Exception as e:
         logger.debug(f"Error loading kubeconfig: {e}")
         return False
```

### Comparing `paka-0.1.5/paka/kube_resources/function/service.py` & `paka-0.1.6/paka/k8s/function/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import shlex
 from typing import Any, Literal, Tuple
 
 from kubernetes import client
 from kubernetes.dynamic import DynamicClient
 from kubernetes.dynamic.exceptions import NotFoundError
 
-from paka.k8s import try_load_kubeconfig
+from paka.k8s.utils import try_load_kubeconfig
 
 try_load_kubeconfig()
 
 
 def enable_scale_to_zero(namespace: str = "knative-serving") -> None:
     """
     Enable scale to zero for the knative-serving namespace.
```

### Comparing `paka-0.1.5/paka/kube_resources/job/autoscaler.py` & `paka-0.1.6/paka/k8s/job/autoscaler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from kubernetes import client
 
-from paka.k8s import CustomResource, apply_resource, delete_namespaced_custom_object
+from paka.k8s.utils import (
+    CustomResource,
+    apply_resource,
+    delete_namespaced_custom_object,
+)
 
 
 def create_autoscaler(
     namespace: str,
     redis_svc_name: str,
     queue_name: str,
     trigger_queue_length: int,
```

### Comparing `paka-0.1.5/paka/kube_resources/job/worker.py` & `paka-0.1.6/paka/k8s/job/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shlex
 import time
 
 from kubernetes import client
 
 from paka.constants import ACCESS_ALL_SA
-from paka.k8s import apply_resource, create_namespace, try_load_kubeconfig
-from paka.kube_resources.job.autoscaler import create_autoscaler, delete_autoscaler
+from paka.k8s.job.autoscaler import create_autoscaler, delete_autoscaler
+from paka.k8s.utils import apply_resource, create_namespace, try_load_kubeconfig
 from paka.logger import logger
 
 try_load_kubeconfig()
 
 
 def wait_for_pods_to_drain(namespace: str, deployment_name: str) -> None:
     """
```

### Comparing `paka-0.1.5/paka/kube_resources/model_group/ingress.py` & `paka-0.1.6/paka/k8s/model_group/ingress.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import List
 
 from kubernetes import client
 
-from paka.k8s import CustomResource, apply_resource
+from paka.k8s.utils import CustomResource, apply_resource
 from paka.utils import kubify_name
 
 
 def create_model_vservice(
     namespace: str, model_name: str, hosts: List[str] = ["*"]
 ) -> None:
     istio_virtual_service = CustomResource(
```

### Comparing `paka-0.1.5/paka/kube_resources/model_group/runtime/llama_cpp.py` & `paka-0.1.6/paka/k8s/model_group/runtime/llama_cpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 import re
 from typing import List, Optional
 
 from huggingface_hub import HfFileSystem
 from huggingface_hub.utils import validate_repo_id
 
 from paka.config import CloudModelGroup
+from paka.constants import MODEL_MOUNT_PATH
 from paka.model.base_model import BaseMLModel
 
 
 # Heuristic to determine if the image is a llama.cpp image
 def is_llama_cpp_image(image: str) -> bool:
     return "llama.cpp" in image.lower()
 
 
 def get_model_file_from_model_store(
     model_group: CloudModelGroup,
 ) -> Optional[str]:
     if model_group.model and model_group.model.useModelStore:
         store = BaseMLModel.get_model_store(with_progress_bar=False)
-        # Find the file that ends with .gguf or .ggml from directory /data
+        # Find the file that ends with .gguf or .ggml
         model_files = [
             file
             for file in store.glob(f"{model_group.name}/*")
             if re.search(r"\.(gguf|ggml)$", file, re.IGNORECASE)
         ]
 
         if not model_files:
@@ -35,15 +36,17 @@
                 if any(
                     re.match(file_pattern, file)
                     for file_pattern in model_group.model.files
                 )
             ]
 
         if len(model_files) > 1:
-            raise ValueError("Multiple model files found in /data directory.")
+            raise ValueError(
+                f"Multiple model files found in {model_group.name}/ directory."
+            )
 
         if len(model_files) == 1:
             return os.path.basename(model_files[0])
 
     return None
 
 
@@ -62,15 +65,15 @@
         ):
             return runtime.command
 
     model_file = get_model_file_from_model_store(model_group)
 
     def attach_model_to_command(command: List[str]) -> List[str]:
         if model_file:
-            return command + ["--model", f"/data/{model_file}"]
+            return command + ["--model", f"{MODEL_MOUNT_PATH}/{model_file}"]
         elif model_group.model and model_group.model.hfRepoId:
 
             validate_repo_id(model_group.model.hfRepoId)
             hf_fs = HfFileSystem()
             files = [
                 file
                 for pattern in model_group.model.files
@@ -78,19 +81,25 @@
             ]
 
             if len(files) > 1:
                 raise ValueError("Multiple model files found in HuggingFace repo.")
             if len(files) == 0:
                 raise ValueError("No model file found in HuggingFace repo.")
 
+            hf_file = os.path.basename(files[0])
+
             return command + [
                 "--hf-repo",
                 model_group.model.hfRepoId,
                 "--hf-file",
-                model_group.model.files[0],
+                hf_file,
+                "--model",
+                os.path.basename(
+                    hf_file
+                ),  # This is the model file name that the huggingface model is saved as
             ]
         else:
             raise ValueError("Did not find a model to load.")
 
     if runtime.command:
         return attach_model_to_command(runtime.command)
```

### Comparing `paka-0.1.5/paka/kube_resources/model_group/service.py` & `paka-0.1.6/paka/k8s/model_group/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
-from typing import Any, List, Optional, Tuple
+from typing import List, Optional, Tuple, cast
 
 from kubernetes import client
 
 from paka.config import CloudConfig, CloudModelGroup, Config
-from paka.constants import ACCESS_ALL_SA
-from paka.k8s import CustomResource, apply_resource, try_load_kubeconfig
-from paka.kube_resources.model_group.runtime.llama_cpp import (
+from paka.constants import ACCESS_ALL_SA, MODEL_MOUNT_PATH
+from paka.k8s.model_group.ingress import create_model_vservice
+from paka.k8s.model_group.runtime.llama_cpp import (
     get_runtime_command_llama_cpp,
     is_llama_cpp_image,
 )
+from paka.k8s.utils import CustomResource, apply_resource, try_load_kubeconfig
+from paka.logger import logger
 from paka.model.hf_model import HuggingFaceModel
 from paka.model.store import MODEL_PATH_PREFIX
 from paka.utils import kubify_name, read_cluster_data
 
 try_load_kubeconfig()
 
 
@@ -73,21 +75,21 @@
         name="init-s3-model-download",
         image="amazon/aws-cli",
         command=[
             "aws",
             "s3",
             "cp",
             f"s3://{bucket}/{MODEL_PATH_PREFIX}/{model_group.name}/",
-            "/data/",
+            f"{MODEL_MOUNT_PATH}/",
             "--recursive",
         ],
         volume_mounts=[
             client.V1VolumeMount(
                 name="model-data",
-                mount_path="/data",
+                mount_path=MODEL_MOUNT_PATH,
             )
         ],
     )
 
 
 def create_pod(
     namespace: str,
@@ -123,15 +125,15 @@
     container_args = {
         "name": f"{kubify_name(model_group.name)}",
         "image": model_group.runtime.image,
         "command": get_runtime_command(model_group, port),
         "volume_mounts": [
             client.V1VolumeMount(
                 name="model-data",
-                mount_path="/data",
+                mount_path=MODEL_MOUNT_PATH,
             )
         ],
         "env": [
             client.V1EnvVar(
                 name="PORT",
                 value=str(port),
             ),
@@ -289,15 +291,15 @@
 
 def create_service_monitor(namespace: str, model_group: CloudModelGroup) -> None:
     monitor = CustomResource(
         api_version="monitoring.coreos.com/v1",
         kind="ServiceMonitor",
         plural="servicemonitors",
         metadata=client.V1ObjectMeta(
-            name=f"{model_group.name}-monitor", namespace=namespace
+            name=kubify_name(model_group.name), namespace=namespace
         ),
         spec={
             "selector": {
                 "matchLabels": {"app": "model-group", "model": model_group.name}
             },
             "namespaceSelector": {
                 "matchNames": [namespace],
@@ -358,15 +360,15 @@
                     target_port=sidecar_port,
                 ),
             ],
         ),
     )
 
 
-def filter_services(namespace: str) -> List[Any]:
+def filter_services(namespace: str) -> List[client.V1Service]:
     """
     Filters the Kubernetes Services in a namespace that belong to a model group.
 
     Args:
         namespace (str): The namespace to filter the Services in.
 
     Returns:
@@ -513,15 +515,23 @@
     if model_group.model and model_group.model.useModelStore:
         if model_group.model.hfRepoId:
             model = HuggingFaceModel(
                 name=model_group.name,
                 repo_id=model_group.model.hfRepoId,
                 files=model_group.model.files,
             )
-            model.save()
+            # If the model is not already in the model store, save it
+            # That means users cannot update the model in the model store
+            # They have to create a new model group or delete the old one
+            if not model.model_store.glob(f"{model_group.name}/*"):
+                model.save()
+            else:
+                logger.info(
+                    f"Model {model_group.name} already exists in the model store. Skipping download."
+                )
 
     port = 8000
 
     pod = create_pod(
         namespace,
         config,
         model_group,
@@ -536,7 +546,94 @@
 
     if config.aws.prometheus and config.aws.prometheus.enabled:
         create_service_monitor(namespace, model_group)
 
     scaled_object = create_scaled_object(namespace, model_group, deployment)
     if scaled_object:
         apply_resource(scaled_object)
+
+    # Create a vservice to export the model group to the outside world
+    create_model_vservice(namespace, model_group.name)
+
+
+def cleanup_model_group_service_by_name(
+    namespace: str,
+    model_group_name: str,
+) -> None:
+    """
+    Cleans up a Kubernetes service for a machine learning model group.
+
+    Args:
+        namespace (str): The namespace to clean up the service in.
+        model_group_name (str): The name of the model group to clean up the service for.
+
+    Returns:
+        None
+    """
+
+    api_client = client.AppsV1Api()
+
+    # Delete the deployment
+    api_client.delete_namespaced_deployment(
+        name=kubify_name(model_group_name),
+        namespace=namespace,
+        body=client.V1DeleteOptions(
+            propagation_policy="Foreground", grace_period_seconds=30
+        ),
+    )
+
+    # Delete the service
+    api_client = client.CoreV1Api()
+
+    # Delete the service
+    api_client.delete_namespaced_service(
+        name=kubify_name(model_group_name),
+        namespace=namespace,
+        body=client.V1DeleteOptions(
+            propagation_policy="Foreground", grace_period_seconds=30
+        ),
+    )
+
+    api_client = client.CustomObjectsApi()
+
+    # Best effort deletion
+    try:
+        # Delete the service monitor
+        api_client.delete_namespaced_custom_object(
+            group="monitoring.coreos.com",
+            version="v1",
+            namespace=namespace,
+            plural="servicemonitors",
+            name=kubify_name(model_group_name),
+            body=client.V1DeleteOptions(),
+        )
+    except:
+        pass
+
+    # Delete the scaled object
+    try:
+        api_client.delete_namespaced_custom_object(
+            group="keda.sh",
+            version="v1alpha1",
+            namespace=namespace,
+            plural="scaledobjects",
+            name=kubify_name(model_group_name),
+            body=client.V1DeleteOptions(),
+        )
+    except:
+        pass
+
+
+def cleanup_staled_model_group_services(
+    namespace: str, source_of_truth_model_groups: List[str]
+) -> None:
+    services = filter_services(namespace)
+    model_groups: List[str] = [
+        cast(client.V1ServiceSpec, service.spec).selector.get("model")
+        for service in services
+    ]
+
+    source_of_truth_model_groups_set = set(source_of_truth_model_groups)
+
+    for model_group in model_groups:
+        if model_group not in source_of_truth_model_groups_set:
+            cleanup_model_group_service_by_name(namespace, model_group)
```

### Comparing `paka-0.1.5/paka/logger.py` & `paka-0.1.6/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/model/base_model.py` & `paka-0.1.6/paka/model/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,11 +74,14 @@
         self, path: str, stream: StreamLike, total_size: int, sha256: str = ""
     ) -> None:
         self.model_store.save_stream(path, stream, total_size, sha256)
         fname = os.path.basename(path)
         self.completed_files.append((fname, sha256))
 
     def finish(self) -> None:
+        self.try_close_progress_bar()
         self.save_manifest_yml()
+
+    def try_close_progress_bar(self) -> None:
         pb = getattr(self.model_store, "progress_bar", None)
         if pb:
             pb.close_progress_bar()
```

### Comparing `paka-0.1.5/paka/model/hf_model.py` & `paka-0.1.6/paka/model/hf_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/model/http_model.py` & `paka-0.1.6/paka/model/http_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/model/manifest.py` & `paka-0.1.6/paka/model/manifest.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/model/progress_bar.py` & `paka-0.1.6/paka/model/progress_bar.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/model/settings.py` & `paka-0.1.6/paka/model/settings.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.5/paka/model/store.py` & `paka-0.1.6/paka/model/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,16 @@
         try:
             if self.file_exists(path):
                 self.progress_bar.advance_progress_bar(path, total_size)
                 return
 
             sha256_value = self._upload_to_s3(stream, path)
             if sha256 and sha256 != sha256_value:
+                self.progress_bar.close_progress_bar()
+
                 message = f"SHA256 hash of the downloaded file does not match the expected value for {path}"
                 # Log the error message so that users know why the file was deleted
                 logger.error(message)
                 self.delete_file(path)
 
                 raise Exception(message)
 
@@ -217,15 +219,14 @@
             )
             upload_completed = True
 
             sha256_value = sha256.hexdigest()
             return sha256_value
 
         except Exception as e:
-            logger.error(f"An error occurred in upload_to_s3: {str(e)}")
             raise e
 
         finally:
             if upload_id is not None and not upload_completed:
                 self.s3.abort_multipart_upload(
                     Bucket=self.s3_bucket, Key=s3_file_name, UploadId=upload_id
                 )
```

### Comparing `paka-0.1.5/paka/utils.py` & `paka-0.1.6/paka/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
+import hashlib
 import json
 import os
 import random
 import re
 import string
 from functools import lru_cache
 from io import StringIO
 from pathlib import Path
 from typing import Any, Callable, Dict, Optional
 
+import requests
 from ruamel.yaml import YAML
 
 from paka.constants import HOME_ENV_VAR, PROJECT_NAME
 
 
 def camel_to_kebab(name: str) -> str:
     """
@@ -83,15 +85,15 @@
     If the environment variable HOME_ENV_VAR is set, it returns its value.
     Otherwise, it returns the home directory appended with the kebab-case project name.
 
     Returns:
         str: The absolute path of the project data directory.
     """
     return os.environ.get(
-        HOME_ENV_VAR, os.path.join(Path.home(), f".{camel_to_kebab(PROJECT_NAME)}")
+        HOME_ENV_VAR, str(Path.home() / f".{camel_to_kebab(PROJECT_NAME)}")
     )
 
 
 def call_once(func: Callable) -> Callable:
     """
     Decorator to ensure a function is only executed once.
     """
@@ -182,15 +184,15 @@
 def get_pulumi_root() -> str:
     """
     Get the pulumi data directory.
 
     Returns:
         str: The pulumi data directory.
     """
-    return get_project_data_dir()
+    return str(Path(get_project_data_dir()) / "pulumi")
 
 
 def save_kubeconfig(cluster_name: str, kubeconfig_json: Optional[str]) -> None:
     """
     Save the kubeconfig data as a YAML file named 'kubeconfig.yaml'.
 
     This function takes the kubeconfig data in JSON format, converts it to YAML,
@@ -315,7 +317,45 @@
     Args:
         length (int, optional): The length of the random string to be generated. Defaults to 5.
 
     Returns:
         str: The generated random string.
     """
     return "".join(random.choices(string.ascii_letters + string.digits, k=length))
+
+
+def calculate_sha256(file_path: str) -> str:
+    """
+    Calculate the SHA-256 hash of a file.
+
+    Args:
+        file_path (str): The path to the file for which the SHA-256 hash is to be calculated.
+
+    Returns:
+        str: The SHA-256 hash of the file, as a hexadecimal string.
+    """
+    sha256_hash = hashlib.sha256()
+
+    with open(file_path, "rb") as f:
+        for byte_block in iter(lambda: f.read(4096), b""):
+            sha256_hash.update(byte_block)
+
+    return sha256_hash.hexdigest()
+
+
+def get_gh_release_latest_version(repo: str) -> str:
+    """
+    Get the latest release version of a GitHub repository.
+
+    This function queries the GitHub API to get the latest release version of a repository.
+
+    Args:
+        repo (str): The GitHub repository in the format 'owner/repo'.
+
+    Returns:
+        str: The latest release version of the repository.
+    """
+    url = f"https://api.github.com/repos/{repo}/releases/latest"
+    response = requests.get(url)
+    response.raise_for_status()
+    data = response.json()
+    return data["tag_name"]
```

### Comparing `paka-0.1.5/pyproject.toml` & `paka-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.5"
+version = "0.1.6"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
 check-filenames = true
 
@@ -49,13 +49,14 @@
 pytest = "^8.1.1"
 pytest-snapshot = "^0.9.0"
 types-requests = "2.31.0.6"
 isort = "^5.13.2"
 types-tabulate = "^0.9.0.20240106"
 pulumi-policy = "^1.11.0"
 moto = "^5.0.5"
-boto3-stubs = { extras = ["s3"], version = "^1.34.87" }
+boto3-stubs = { extras = ["ecr", "s3"], version = "^1.34.93" }
 types-tqdm = "^4.66.0.20240417"
+pytest-order = "^1.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `paka-0.1.5/PKG-INFO` & `paka-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.5
+Version: 0.1.6
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
 Author: Jijun Leng
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,15 +26,15 @@
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Welcome to Paka
 
-<img src="docs/img/paka.svg" alt="paka.svg" width="200" height="200">
+<img src="https://raw.githubusercontent.com/jjleng/paka/main/docs/img/paka.svg" alt="paka.svg" width="200" height="200">
 
 **paka** is a versatile LLMOps tool that simplifies the deployment and management of large language model (LLM) apps with a single command.
 
 ## Paka Highlights
 
 - **Cloud-Agnostic Resource Provisioning**: paka starts by breaking down the barriers of cloud vendor lock-in, currently supporting EKS with plans to expand to more cloud services.
 - **Optimized Model Execution**: Designed for efficiency, paka runs LLM models on CPUs and Nvidia GPUs, ensuring optimal performance. Auto-scaling of model replicas based on CPU usage, request rate, and latency.
@@ -125,25 +125,19 @@
 
 ### Destroy a cluster
 ```bash
 paka cluster down -f cluster.yaml
 ```
 
 ## Contributing
+- code changes
+- `make check-all`
 - Open a PR
-- Format and lint code with `make lint`
-- Run tests with `make test`
 
 ## Dependencies
-- docker daemon
-- pack cli (https://buildpacks.io/docs/for-platform-operators/how-to/integrate-ci/pack/)
-- pulumi cli (https://www.pulumi.com/docs/install/)
-- aws cli and credentials for the AWS deployment
+- docker daemon and CLI
+- credentials for the AWS cloud
 ```bash
-# Make sure aws credentials and cli are set up. Your aws credentials should have access to the following services:
-# - S3
-# - ECR
-# - EKS
-# - EC2
-aws configure
+# Ensure your AWS credentials are correctly configured. Execute the command below and verify that the keys `aws_access_key_id` and `aws_secret_access_key` are present.
+cat ~/.aws/credentials
 ```
```

