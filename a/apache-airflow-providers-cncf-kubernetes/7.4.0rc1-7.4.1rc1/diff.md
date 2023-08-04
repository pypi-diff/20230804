# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-7.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-7.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.4.0rc1.tar", last modified: Sat Jul 29 12:08:13 2023, max compression
+gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.4.1rc1.tar", last modified: Fri Aug  4 21:40:55 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1.tar` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.233596 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-07-29 12:08:11.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4637 2023-07-29 12:08:13.234305 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2963 2023-07-29 12:08:11.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.028423 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.029770 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.031174 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.115362 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)     1584 2023-07-29 12:01:19.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.121187 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.127824 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.143163 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30257 2023-07-29 09:53:35.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
--rw-r--r--   0 root         (0) root         (0)    21132 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
--rw-r--r--   0 root         (0) root         (0)     9983 2023-07-29 06:50:08.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-07-29 12:08:11.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.149392 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23140 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kube_client.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kube_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.152575 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.169619 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1262 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    41271 2023-07-29 09:53:35.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0 root         (0) root         (0)     7387 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)    23849 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py
--rw-r--r--   0 root         (0) root         (0)    12129 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
--rw-r--r--   0 root         (0) root         (0)    12039 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.172463 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.178255 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.186594 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    11511 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.202681 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py
--rw-r--r--   0 root         (0) root         (0)    28943 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.230124 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4637 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2931 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-29 12:08:13.236467 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-29 12:08:11.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.958168 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-08-04 21:40:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-08-04 21:40:55.958772 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-08-04 21:40:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.764664 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.765711 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.766783 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.846230 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-08-04 21:33:34.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.853709 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.860425 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.875097 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30457 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
+-rw-r--r--   0 root         (0) root         (0)    21132 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-07-29 06:50:08.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)    15886 2023-08-04 21:40:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.880849 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23948 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/k8s_model.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kube_client.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kube_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.883891 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.898723 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    41626 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0 root         (0) root         (0)     7387 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)    23849 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_generator.py
+-rw-r--r--   0 root         (0) root         (0)    12129 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0 root         (0) root         (0)    12039 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.901607 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.907390 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/template_rendering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.916333 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    11511 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.931113 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)    29231 2023-08-04 19:44:14.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:55.955467 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2931 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:55.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-08-04 21:40:55.960691 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-08-04 21:40:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.4.0rc1
+Version: 7.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.4.0rc1``
+Release: ``7.4.1rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -105,8 +105,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/README.rst` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.4.0rc1``
+Release: ``7.4.1rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -71,8 +71,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "7.4.0"
+__version__ = "7.4.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 .. seealso::
     For more information on how the KubernetesExecutor works, take a look at the guide:
     :ref:`executor:KubernetesExecutor`
 """
 from __future__ import annotations
 
+import argparse
 import json
 import logging
 import multiprocessing
 import time
 from collections import defaultdict
 from contextlib import suppress
 from datetime import datetime
@@ -723,7 +724,15 @@
         return [
             GroupCommand(
                 name="kubernetes",
                 help="Tools to help run the KubernetesExecutor",
                 subcommands=KUBERNETES_COMMANDS,
             )
         ]
+
+
+def _get_parser() -> argparse.ArgumentParser:
+    """This method is used by Sphinx to generate documentation.
+
+    :meta private:
+    """
+    return KubernetesExecutor._get_parser()
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "suspended": False,
         "versions": [
+            "7.4.1",
             "7.4.0",
             "7.3.0",
             "7.2.0",
             "7.1.0",
             "7.0.0",
             "6.1.0",
             "6.0.0",
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import contextlib
+import json
 import tempfile
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, Generator
 
 from asgiref.sync import sync_to_async
 from kubernetes import client, config, watch
 from kubernetes.client.models import V1Pod
@@ -95,14 +96,20 @@
             "kube_config": StringField(
                 lazy_gettext("Kube config (JSON format)"), widget=BS3TextFieldWidget()
             ),
             "namespace": StringField(lazy_gettext("Namespace"), widget=BS3TextFieldWidget()),
             "cluster_context": StringField(lazy_gettext("Cluster context"), widget=BS3TextFieldWidget()),
             "disable_verify_ssl": BooleanField(lazy_gettext("Disable SSL")),
             "disable_tcp_keepalive": BooleanField(lazy_gettext("Disable TCP keepalive")),
+            "xcom_sidecar_container_image": StringField(
+                lazy_gettext("XCom sidecar image"), widget=BS3TextFieldWidget()
+            ),
+            "xcom_sidecar_container_resources": StringField(
+                lazy_gettext("XCom sidecar resources (JSON format)"), widget=BS3TextFieldWidget()
+            ),
         }
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
         """Returns custom field behaviour."""
         return {
             "hidden_fields": ["host", "schema", "login", "password", "port", "extra"],
@@ -352,14 +359,25 @@
 
     def get_namespace(self) -> str | None:
         """Returns the namespace that defined in the connection."""
         if self.conn_id:
             return self._get_field("namespace")
         return None
 
+    def get_xcom_sidecar_container_image(self):
+        """Returns the xcom sidecar image that defined in the connection."""
+        return self._get_field("xcom_sidecar_container_image")
+
+    def get_xcom_sidecar_container_resources(self):
+        """Returns the xcom sidecar resources that defined in the connection."""
+        field = self._get_field("xcom_sidecar_container_resources")
+        if not field:
+            return None
+        return json.loads(field)
+
     def get_pod_log_stream(
         self,
         pod_name: str,
         container: str | None = "",
         namespace: str | None = None,
     ) -> tuple[watch.Watch, Generator[str, None, None]]:
         """
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/k8s_model.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kube_client.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kube_config.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,17 +357,15 @@
         self.secrets = secrets or []
         self.in_cluster = in_cluster
         self.cluster_context = cluster_context
         self.reattach_on_restart = reattach_on_restart
         self.get_logs = get_logs
         self.container_logs = container_logs
         if self.container_logs == KubernetesPodOperator.BASE_CONTAINER_NAME:
-            self.container_logs = (
-                base_container_name if base_container_name else KubernetesPodOperator.BASE_CONTAINER_NAME
-            )
+            self.container_logs = base_container_name if base_container_name else self.BASE_CONTAINER_NAME
         self.image_pull_policy = image_pull_policy
         self.node_selector = node_selector or {}
         self.annotations = annotations or {}
         self.affinity = convert_affinity(affinity) if affinity else {}
         self.container_resources = container_resources
         self.config_file = config_file
         self.image_pull_secrets = convert_image_pull_secrets(image_pull_secrets) if image_pull_secrets else []
@@ -588,15 +586,17 @@
 
             if self.get_logs:
                 self.pod_manager.fetch_requested_container_logs(
                     pod=self.pod,
                     container_logs=self.container_logs,
                     follow_logs=True,
                 )
-            else:
+            if not self.get_logs or (
+                self.container_logs is not True and self.base_container_name not in self.container_logs
+            ):
                 self.pod_manager.await_container_completion(
                     pod=self.pod, container_name=self.base_container_name
                 )
 
             if self.do_xcom_push:
                 self.pod_manager.await_xcom_sidecar_container_start(pod=self.pod)
                 result = self.extract_xcom(pod=self.pod)
@@ -758,15 +758,18 @@
                 if should_delete_pod:
                     self.log.info("Deleting pod: %s", pod.metadata.name)
                     self.pod_manager.delete_pod(pod)
                 else:
                     self.log.info("Skipping deleting pod: %s", pod.metadata.name)
 
     def _build_find_pod_label_selector(self, context: Context | None = None, *, exclude_checked=True) -> str:
-        labels = self._get_ti_pod_labels(context, include_try_number=False)
+        labels = {
+            **self.labels,
+            **self._get_ti_pod_labels(context, include_try_number=False),
+        }
         label_strings = [f"{label_id}={label}" for label_id, label in sorted(labels.items())]
         labels_value = ",".join(label_strings)
         if exclude_checked:
             labels_value += f",{self.POD_CHECKED_KEY}!=True"
         labels_value += ",!airflow-worker"
         return labels_value
 
@@ -876,15 +879,19 @@
             pod.metadata.namespace = pod_namespace
 
         for secret in self.secrets:
             self.log.debug("Adding secret to task %s", self.task_id)
             pod = secret.attach_to_pod(pod)
         if self.do_xcom_push:
             self.log.debug("Adding xcom sidecar to task %s", self.task_id)
-            pod = xcom_sidecar.add_xcom_sidecar(pod)
+            pod = xcom_sidecar.add_xcom_sidecar(
+                pod,
+                sidecar_container_image=self.hook.get_xcom_sidecar_container_image(),
+                sidecar_container_resources=self.hook.get_xcom_sidecar_container_resources(),
+            )
 
         labels = self._get_ti_pod_labels(context)
         self.log.info("Building pod %s with labels: %s", pod.metadata.name, labels)
 
         # Merge Pod Identifying labels with labels passed to operator
         pod.metadata.labels.update(labels)
         # Add Airflow Version to the label
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_generator.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/secret.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/template_rendering.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,20 @@
 
     def get_pod(self, name: str, namespace: str) -> V1Pod:
         """Read pod object from kubernetes API."""
 
     def get_namespace(self) -> str | None:
         """Returns the namespace that defined in the connection."""
 
+    def get_xcom_sidecar_container_image(self) -> str | None:
+        """Returns the xcom sidecar image that defined in the connection."""
+
+    def get_xcom_sidecar_container_resources(self) -> str | None:
+        """Returns the xcom sidecar resources that defined in the connection."""
+
 
 def get_container_status(pod: V1Pod, container_name: str) -> V1ContainerStatus | None:
     """Retrieves container status."""
     container_statuses = pod.status.container_statuses if pod and pod.status else None
     if container_statuses:
         # In general the variable container_statuses can store multiple items matching different containers.
         # The following generator expression yields all items that have name equal to the container_name.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.4.0rc1
+Version: 7.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.4.0rc1``
+Release: ``7.4.1rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -105,8 +105,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
     "test_*.py",
+    "example_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
 required-imports = ["from __future__ import annotations"]
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/setup.py` & `apache-airflow-providers-cncf-kubernetes-7.4.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.4.0"
+version = "7.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
```

