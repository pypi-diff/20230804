# Comparing `tmp/solutions_builder-1.17.6.tar.gz` & `tmp/solutions_builder-1.17.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solutions_builder-1.17.6.tar", max compression
+gzip compressed data, was "solutions_builder-1.17.7.tar", max compression
```

## Comparing `solutions_builder-1.17.6.tar` & `solutions_builder-1.17.7.tar`

### file list

```diff
@@ -1,202 +1,201 @@
--rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.17.6/LICENSE
--rw-r--r--   0        0        0     4828 2023-07-31 15:22:50.618546 solutions_builder-1.17.6/README.md
--rw-r--r--   0        0        0     1150 2023-07-31 21:38:15.340949 solutions_builder-1.17.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622568 solutions_builder-1.17.6/solutions_builder/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622645 solutions_builder-1.17.6/solutions_builder/cli/__init__.py
--rw-r--r--   0        0        0     6551 2023-07-31 21:20:56.712072 solutions_builder-1.17.6/solutions_builder/cli/cli.py
--rw-r--r--   0        0        0     4630 2023-07-31 19:26:47.632344 solutions_builder-1.17.6/solutions_builder/cli/cli_utils.py
--rw-r--r--   0        0        0     6527 2023-07-31 21:28:04.069345 solutions_builder-1.17.6/solutions_builder/cli/component.py
--rw-r--r--   0        0        0     5883 2023-07-31 19:26:47.633561 solutions_builder-1.17.6/solutions_builder/cli/infra.py
--rw-r--r--   0        0        0     2313 2023-07-31 19:26:47.634344 solutions_builder-1.17.6/solutions_builder/cli/set.py
--rw-r--r--   0        0        0     1416 2023-07-31 19:26:06.133259 solutions_builder-1.17.6/solutions_builder/cli/template.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.624032 solutions_builder-1.17.6/solutions_builder/copier_extensions/__init__.py
--rw-r--r--   0        0        0     4617 2023-07-31 19:26:47.636088 solutions_builder-1.17.6/solutions_builder/copier_extensions/st_helpers.py
--rw-r--r--   0        0        0      101 2023-07-31 15:22:50.624510 solutions_builder-1.17.6/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
--rw-r--r--   0        0        0      766 2023-07-31 15:22:50.624649 solutions_builder-1.17.6/solutions_builder/module_template/README.md
--rw-r--r--   0        0        0      865 2023-07-31 15:22:50.624799 solutions_builder-1.17.6/solutions_builder/module_template/copier.yaml
--rw-r--r--   0        0        0       89 2023-07-31 15:22:50.625018 solutions_builder-1.17.6/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
--rw-r--r--   0        0        0     1135 2023-07-31 15:22:50.625172 solutions_builder-1.17.6/solutions_builder/module_template/template_copier.yaml
--rw-r--r--   0        0        0     3878 2023-07-31 19:26:06.134447 solutions_builder-1.17.6/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
--rw-r--r--   0        0        0      566 2023-07-31 15:22:50.625671 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
--rw-r--r--   0        0        0      109 2023-07-31 15:22:50.625798 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
--rw-r--r--   0        0        0     3204 2023-07-31 15:22:50.625960 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
--rw-r--r--   0        0        0      590 2023-07-31 19:26:06.135288 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.626261 solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
--rw-r--r--   0        0        0      736 2023-07-31 19:26:06.135779 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
--rw-r--r--   0        0        0      636 2023-07-31 19:26:06.136084 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
--rw-r--r--   0        0        0      836 2023-07-31 19:26:06.136404 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
--rw-r--r--   0        0        0      777 2023-07-31 19:26:06.137072 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
--rw-r--r--   0        0        0      858 2023-07-31 19:26:06.137649 solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.627394 solutions_builder-1.17.6/solutions_builder/modules/restful_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1363 2023-07-31 15:22:50.627536 solutions_builder-1.17.6/solutions_builder/modules/restful_service/README.md
--rw-r--r--   0        0        0      545 2023-07-31 15:22:50.627695 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0     1257 2023-07-31 15:22:50.628306 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.628605 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.628881 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0       98 2023-07-31 15:22:50.629046 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     2974 2023-07-31 15:22:50.629209 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      862 2023-07-31 19:26:06.138139 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1711 2023-07-31 19:26:06.138427 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1664 2023-07-31 19:26:06.138760 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.629799 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     3876 2023-07-31 19:26:06.139176 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
--rw-r--r--   0        0        0     1222 2023-07-31 19:26:06.139854 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.630283 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.630545 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-07-31 15:22:50.630703 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       60 2023-07-31 15:22:50.630849 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-07-31 15:22:50.630997 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-07-31 15:22:50.631183 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-07-31 15:22:50.631328 solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2305 2023-07-31 19:26:47.637120 solutions_builder-1.17.6/solutions_builder/modules/restful_service/copier.yaml
--rw-r--r--   0        0        0      120 2023-07-31 15:22:50.631626 solutions_builder-1.17.6/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-07-31 15:22:50.631734 solutions_builder-1.17.6/solutions_builder/modules/restful_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      263 2023-07-31 15:22:50.631945 solutions_builder-1.17.6/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
--rw-r--r--   0        0        0     3223 2023-07-31 15:22:50.632152 solutions_builder-1.17.6/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
--rw-r--r--   0        0        0     3269 2023-07-31 15:22:50.632352 solutions_builder-1.17.6/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.632549 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1572 2023-07-31 15:22:50.632676 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/README.md
--rw-r--r--   0        0        0      545 2023-07-31 15:22:50.632822 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.632992 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.633061 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0      143 2023-07-31 15:22:50.633183 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     3193 2023-07-31 15:22:50.633333 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      942 2023-07-31 19:26:06.140161 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1751 2023-07-31 19:26:06.140436 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1550 2023-07-31 19:26:06.140868 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.633781 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     5195 2023-07-31 19:26:06.141312 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
--rw-r--r--   0        0        0     1196 2023-07-31 19:26:06.141730 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634163 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634237 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
--rw-r--r--   0        0        0      430 2023-07-31 15:22:50.634359 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
--rw-r--r--   0        0        0     1348 2023-07-31 15:22:50.634473 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
--rw-r--r--   0        0        0     1138 2023-07-31 15:22:50.634593 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
--rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.634791 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-07-31 15:22:50.634913 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       97 2023-07-31 15:22:50.635030 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-07-31 15:22:50.635163 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-07-31 15:22:50.635357 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-07-31 15:22:50.635506 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2667 2023-07-31 15:22:50.635659 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/copier.yaml
--rw-r--r--   0        0        0       71 2023-07-31 15:22:50.635866 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       92 2023-07-31 15:22:50.635986 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      719 2023-07-31 19:26:06.142418 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
--rw-r--r--   0        0        0     2693 2023-07-31 19:26:06.142972 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
--rw-r--r--   0        0        0      930 2023-07-31 19:26:06.143419 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
--rw-r--r--   0        0        0     1280 2023-07-31 19:26:06.143751 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
--rw-r--r--   0        0        0     2076 2023-07-31 19:26:06.144059 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
--rw-r--r--   0        0        0     3851 2023-07-31 19:26:06.144531 solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.637527 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1398 2023-07-31 21:24:12.019665 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/copier.yaml
--rw-r--r--   0        0        0      794 2023-07-31 15:22:50.637941 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
--rw-r--r--   0        0        0       59 2023-07-31 21:38:07.061173 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/skaffold.yaml.patch
--rw-r--r--   0        0        0      701 2023-07-31 19:26:06.144964 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.145601 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf
--rw-r--r--   0        0        0     2486 2023-07-31 19:26:06.145978 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf
--rw-r--r--   0        0        0     1783 2023-07-31 19:26:06.146393 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf
--rw-r--r--   0        0        0      268 2023-07-31 15:22:50.639380 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
--rw-r--r--   0        0        0     1553 2023-07-31 19:26:06.146871 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.641148 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     2186 2023-07-31 19:26:47.638488 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/copier.yaml
--rw-r--r--   0        0        0      180 2023-07-31 15:22:50.641792 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
--rw-r--r--   0        0        0      658 2023-07-31 15:22:50.641933 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
--rw-r--r--   0        0        0      145 2023-07-31 15:22:50.642056 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
--rw-r--r--   0        0        0      185 2023-07-31 15:22:50.642172 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
--rw-r--r--   0        0        0      378 2023-07-31 15:22:50.642293 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
--rw-r--r--   0        0        0       59 2023-07-31 15:22:50.642402 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
--rw-r--r--   0        0        0     2420 2023-07-31 19:26:06.147317 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
--rw-r--r--   0        0        0      670 2023-07-31 19:26:06.147738 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
--rw-r--r--   0        0        0     1264 2023-07-31 19:26:06.148024 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
--rw-r--r--   0        0        0      709 2023-07-31 19:26:06.148386 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.148713 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf
--rw-r--r--   0        0        0     1695 2023-07-31 19:26:06.149003 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf
--rw-r--r--   0        0        0     1877 2023-07-31 19:26:06.149312 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf
--rw-r--r--   0        0        0      480 2023-07-31 15:22:50.643659 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/terraform.tfvars
--rw-r--r--   0        0        0     1802 2023-07-31 19:26:06.149801 solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf
--rw-r--r--   0        0        0       80 2023-07-31 15:22:50.644034 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0     1048 2023-07-31 19:26:47.639062 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
--rw-r--r--   0        0        0      834 2023-07-31 19:26:06.150138 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
--rw-r--r--   0        0        0     2760 2023-07-31 15:22:50.644547 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
--rw-r--r--   0        0        0      670 2023-07-31 19:26:06.150553 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
--rw-r--r--   0        0        0     1298 2023-07-31 19:26:06.151001 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.644903 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
--rw-r--r--   0        0        0      196 2023-07-31 15:22:50.645021 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
--rw-r--r--   0        0        0     1984 2023-07-31 19:26:06.151475 solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
--rw-r--r--   0        0        0       90 2023-07-31 15:22:50.645285 solutions_builder-1.17.6/solutions_builder/requirements.txt
--rw-r--r--   0        0        0    68957 2023-07-31 15:22:50.645771 solutions_builder-1.17.6/solutions_builder/template_root/.github/assets/setup_local.png
--rw-r--r--   0        0        0   239307 2023-07-31 15:22:50.647206 solutions_builder-1.17.6/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
--rw-r--r--   0        0        0     2639 2023-07-31 15:22:50.647454 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
--rw-r--r--   0        0        0     2690 2023-07-31 15:22:50.647592 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
--rw-r--r--   0        0        0     5786 2023-07-31 19:26:47.639716 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
--rw-r--r--   0        0        0     8049 2023-07-31 19:26:47.640169 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
--rw-r--r--   0        0        0     3131 2023-07-31 15:22:50.648490 solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
--rw-r--r--   0        0        0      471 2023-07-31 15:22:50.648622 solutions_builder-1.17.6/solutions_builder/template_root/.gitignore
--rw-r--r--   0        0        0    14552 2023-07-31 15:22:50.648747 solutions_builder-1.17.6/solutions_builder/template_root/.pylintrc
--rw-r--r--   0        0        0      711 2023-07-31 15:22:50.649129 solutions_builder-1.17.6/solutions_builder/template_root/README.md
--rw-r--r--   0        0        0      398 2023-07-31 15:22:50.649329 solutions_builder-1.17.6/solutions_builder/template_root/components/README.md
--rw-r--r--   0        0        0      211 2023-07-31 15:22:50.649479 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
--rw-r--r--   0        0        0      395 2023-07-31 15:22:50.649633 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
--rw-r--r--   0        0        0       77 2023-07-31 15:22:50.649720 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
--rw-r--r--   0        0        0      131 2023-07-31 15:22:50.649904 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
--rw-r--r--   0        0        0      571 2023-07-31 15:22:50.650164 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.650248 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
--rw-r--r--   0        0        0      831 2023-07-31 19:26:06.151862 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
--rw-r--r--   0        0        0      695 2023-07-31 19:26:06.153743 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
--rw-r--r--   0        0        0       35 2023-07-31 15:22:50.650730 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
--rw-r--r--   0        0        0       91 2023-07-31 15:22:50.650873 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
--rw-r--r--   0        0        0     1376 2023-07-31 19:26:06.154070 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651072 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
--rw-r--r--   0        0        0      754 2023-07-31 19:26:06.154613 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
--rw-r--r--   0        0        0     1006 2023-07-31 19:26:06.155093 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
--rw-r--r--   0        0        0     2243 2023-07-31 19:26:06.155755 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651579 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
--rw-r--r--   0        0        0     1002 2023-07-31 19:26:06.156062 solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
--rw-r--r--   0        0        0     2130 2023-07-31 15:22:50.651893 solutions_builder-1.17.6/solutions_builder/template_root/copier.yaml
--rw-r--r--   0        0        0       97 2023-07-31 15:22:50.652011 solutions_builder-1.17.6/solutions_builder/template_root/firebase.json
--rw-r--r--   0        0        0       98 2023-07-31 15:22:50.652089 solutions_builder-1.17.6/solutions_builder/template_root/setup.cfg
--rw-r--r--   0        0        0      215 2023-07-31 15:22:50.652207 solutions_builder-1.17.6/solutions_builder/template_root/skaffold.yaml
--rw-r--r--   0        0        0      359 2023-07-31 15:22:50.652564 solutions_builder-1.17.6/solutions_builder/template_root/st.yaml
--rw-r--r--   0        0        0      921 2023-07-31 19:26:06.156495 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
--rw-r--r--   0        0        0      730 2023-07-31 19:26:06.157029 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
--rw-r--r--   0        0        0     3585 2023-07-31 19:26:06.157569 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
--rw-r--r--   0        0        0     1178 2023-07-31 19:26:06.158072 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
--rw-r--r--   0        0        0     5024 2023-07-31 19:26:06.158367 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
--rw-r--r--   0        0        0      190 2023-07-31 15:22:50.653603 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
--rw-r--r--   0        0        0     1186 2023-07-31 19:26:06.158842 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
--rw-r--r--   0        0        0     1601 2023-07-31 19:26:06.159185 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
--rw-r--r--   0        0        0     2364 2023-07-31 19:26:06.159491 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/firebase/main.tf
--rw-r--r--   0        0        0     1194 2023-07-31 19:26:06.160029 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/firebase/variables.tf
--rw-r--r--   0        0        0     3860 2023-07-31 19:26:06.160499 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/main.tf
--rw-r--r--   0        0        0      832 2023-07-31 19:26:06.160786 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/outputs.tf
--rw-r--r--   0        0        0     3386 2023-07-31 19:26:06.161064 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/variables.tf
--rw-r--r--   0        0        0     2926 2023-07-31 19:26:06.161342 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
--rw-r--r--   0        0        0      692 2023-07-31 19:26:06.161609 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
--rw-r--r--   0        0        0     1087 2023-07-31 19:26:06.161883 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
--rw-r--r--   0        0        0      827 2023-07-31 19:26:06.162157 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/project_services/main.tf
--rw-r--r--   0        0        0      774 2023-07-31 19:26:06.162534 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/project_services/variables.tf
--rw-r--r--   0        0        0      953 2023-07-31 19:26:06.162825 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/service_account/main.tf
--rw-r--r--   0        0        0     1037 2023-07-31 19:26:06.163149 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/service_account/variables.tf
--rw-r--r--   0        0        0     1529 2023-07-31 19:26:06.163558 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
--rw-r--r--   0        0        0      678 2023-07-31 19:26:06.163969 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
--rw-r--r--   0        0        0     1333 2023-07-31 19:26:06.164360 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
--rw-r--r--   0        0        0     1269 2023-07-31 19:26:06.164825 solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
--rw-r--r--   0        0        0     2306 2023-07-31 19:39:45.308006 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
--rw-r--r--   0        0        0      730 2023-07-31 19:26:06.165370 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
--rw-r--r--   0        0        0       66 2023-07-31 15:22:50.656645 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
--rw-r--r--   0        0        0     1071 2023-07-31 19:26:06.165664 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
--rw-r--r--   0        0        0      826 2023-07-31 19:26:06.166236 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
--rw-r--r--   0        0        0      517 2023-07-31 15:22:50.657065 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
--rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.166512 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
--rw-r--r--   0        0        0     4400 2023-07-31 19:26:06.167078 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
--rw-r--r--   0        0        0      991 2023-07-31 19:26:06.167766 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
--rw-r--r--   0        0        0      835 2023-07-31 19:26:06.168129 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
--rw-r--r--   0        0        0      606 2023-07-31 15:22:50.657649 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
--rw-r--r--   0        0        0     2546 2023-07-31 19:26:06.168711 solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.657846 solutions_builder-1.17.6/solutions_builder/template_root/tests/__init__.py
--rw-r--r--   0        0        0      825 2023-07-31 15:22:50.658012 solutions_builder-1.17.6/solutions_builder/template_root/tests/e2e/e2e_utils.py
--rwxr-xr-x   0        0        0      364 2023-07-31 15:22:50.658190 solutions_builder-1.17.6/solutions_builder/template_root/utils/disable_org_policies.sh
--rwxr-xr-x   0        0        0      990 2023-07-31 19:26:06.169251 solutions_builder-1.17.6/solutions_builder/template_root/utils/init_env_vars.sh
--rw-r--r--   0        0        0       81 2023-07-31 15:22:50.658645 solutions_builder-1.17.6/solutions_builder/template_root/{{_copier_conf.answers_file}}
--rw-r--r--   0        0        0        0 2023-07-31 15:22:50.658746 solutions_builder-1.17.6/solutions_builder/tests/__init__.py
--rw-r--r--   0        0        0     5942 1970-01-01 00:00:00.000000 solutions_builder-1.17.6/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_builder-1.17.7/LICENSE
+-rw-r--r--   0        0        0     5040 2023-08-02 23:47:18.606276 solutions_builder-1.17.7/README.md
+-rw-r--r--   0        0        0     1150 2023-08-03 18:52:28.219315 solutions_builder-1.17.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622568 solutions_builder-1.17.7/solutions_builder/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.622645 solutions_builder-1.17.7/solutions_builder/cli/__init__.py
+-rw-r--r--   0        0        0     6551 2023-08-03 18:45:23.114761 solutions_builder-1.17.7/solutions_builder/cli/cli.py
+-rw-r--r--   0        0        0     4630 2023-08-03 18:45:23.093710 solutions_builder-1.17.7/solutions_builder/cli/cli_utils.py
+-rw-r--r--   0        0        0     6537 2023-08-03 18:45:23.108265 solutions_builder-1.17.7/solutions_builder/cli/component.py
+-rw-r--r--   0        0        0     5883 2023-08-03 18:45:23.113099 solutions_builder-1.17.7/solutions_builder/cli/infra.py
+-rw-r--r--   0        0        0     2313 2023-08-03 18:45:23.103492 solutions_builder-1.17.7/solutions_builder/cli/set.py
+-rw-r--r--   0        0        0     1416 2023-07-31 19:26:06.133259 solutions_builder-1.17.7/solutions_builder/cli/template.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.624032 solutions_builder-1.17.7/solutions_builder/copier_extensions/__init__.py
+-rw-r--r--   0        0        0     4617 2023-08-03 18:45:23.138550 solutions_builder-1.17.7/solutions_builder/copier_extensions/st_helpers.py
+-rw-r--r--   0        0        0      101 2023-07-31 15:22:50.624510 solutions_builder-1.17.7/solutions_builder/module_template/.st/module_answers/{{'{{component_name}}'}}.yaml
+-rw-r--r--   0        0        0      766 2023-07-31 15:22:50.624649 solutions_builder-1.17.7/solutions_builder/module_template/README.md
+-rw-r--r--   0        0        0      865 2023-07-31 15:22:50.624799 solutions_builder-1.17.7/solutions_builder/module_template/copier.yaml
+-rw-r--r--   0        0        0       89 2023-07-31 15:22:50.625018 solutions_builder-1.17.7/solutions_builder/module_template/docs/components/{{'{{component_name}}'}}.md
+-rw-r--r--   0        0        0     1135 2023-07-31 15:22:50.625172 solutions_builder-1.17.7/solutions_builder/module_template/template_copier.yaml
+-rw-r--r--   0        0        0     3878 2023-07-31 19:26:06.134447 solutions_builder-1.17.7/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml
+-rw-r--r--   0        0        0      566 2023-07-31 15:22:50.625671 solutions_builder-1.17.7/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile
+-rw-r--r--   0        0        0      109 2023-07-31 15:22:50.625798 solutions_builder-1.17.7/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/requirements.txt
+-rw-r--r--   0        0        0     3204 2023-07-31 15:22:50.625960 solutions_builder-1.17.7/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml
+-rw-r--r--   0        0        0      590 2023-07-31 19:26:06.135288 solutions_builder-1.17.7/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.626261 solutions_builder-1.17.7/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/st_module.yaml
+-rw-r--r--   0        0        0      736 2023-07-31 19:26:06.135779 solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf
+-rw-r--r--   0        0        0      636 2023-07-31 19:26:06.136084 solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf
+-rw-r--r--   0        0        0      836 2023-07-31 19:26:06.136404 solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf
+-rw-r--r--   0        0        0      777 2023-07-31 19:26:06.137072 solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars
+-rw-r--r--   0        0        0      858 2023-07-31 19:26:06.137649 solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.627394 solutions_builder-1.17.7/solutions_builder/modules/restful_service/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1363 2023-07-31 15:22:50.627536 solutions_builder-1.17.7/solutions_builder/modules/restful_service/README.md
+-rw-r--r--   0        0        0      545 2023-07-31 15:22:50.627695 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1257 2023-07-31 15:22:50.628306 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.628605 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.628881 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0       98 2023-07-31 15:22:50.629046 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     2974 2023-07-31 15:22:50.629209 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      862 2023-07-31 19:26:06.138139 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1711 2023-07-31 19:26:06.138427 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1664 2023-07-31 19:26:06.138760 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.629799 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     3876 2023-07-31 19:26:06.139176 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
+-rw-r--r--   0        0        0     1222 2023-07-31 19:26:06.139854 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.630283 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.630545 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2023-07-31 15:22:50.630703 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2023-07-31 15:22:50.630849 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2023-07-31 15:22:50.630997 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2023-07-31 15:22:50.631183 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2023-07-31 15:22:50.631328 solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2305 2023-07-31 19:26:47.637120 solutions_builder-1.17.7/solutions_builder/modules/restful_service/copier.yaml
+-rw-r--r--   0        0        0      120 2023-07-31 15:22:50.631626 solutions_builder-1.17.7/solutions_builder/modules/restful_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2023-07-31 15:22:50.631734 solutions_builder-1.17.7/solutions_builder/modules/restful_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      263 2023-07-31 15:22:50.631945 solutions_builder-1.17.7/solutions_builder/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
+-rw-r--r--   0        0        0     3223 2023-07-31 15:22:50.632152 solutions_builder-1.17.7/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
+-rw-r--r--   0        0        0     3269 2023-07-31 15:22:50.632352 solutions_builder-1.17.7/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.632549 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1572 2023-07-31 15:22:50.632676 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/README.md
+-rw-r--r--   0        0        0      545 2023-07-31 15:22:50.632822 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.632992 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.633061 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0      143 2023-07-31 15:22:50.633183 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     3193 2023-07-31 15:22:50.633333 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      942 2023-07-31 19:26:06.140161 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1751 2023-07-31 19:26:06.140436 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1550 2023-07-31 19:26:06.140868 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.633781 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     5195 2023-07-31 19:26:06.141312 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py
+-rw-r--r--   0        0        0     1196 2023-07-31 19:26:06.141730 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634163 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.634237 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-31 15:22:50.634359 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/example.yaml
+-rw-r--r--   0        0        0     1348 2023-07-31 15:22:50.634473 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py
+-rw-r--r--   0        0        0     1138 2023-07-31 15:22:50.634593 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py
+-rw-r--r--   0        0        0     1232 2023-07-31 15:22:50.634791 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2023-07-31 15:22:50.634913 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       97 2023-07-31 15:22:50.635030 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2023-07-31 15:22:50.635163 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2023-07-31 15:22:50.635357 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2023-07-31 15:22:50.635506 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2667 2023-07-31 15:22:50.635659 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/copier.yaml
+-rw-r--r--   0        0        0       71 2023-07-31 15:22:50.635866 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0       92 2023-07-31 15:22:50.635986 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      719 2023-07-31 19:26:06.142418 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf
+-rw-r--r--   0        0        0     2693 2023-07-31 19:26:06.142972 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf
+-rw-r--r--   0        0        0      930 2023-07-31 19:26:06.143419 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf
+-rw-r--r--   0        0        0     1280 2023-07-31 19:26:06.143751 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars
+-rw-r--r--   0        0        0     2076 2023-07-31 19:26:06.144059 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf
+-rw-r--r--   0        0        0     3851 2023-07-31 19:26:06.144531 solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.637527 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1398 2023-07-31 21:24:12.019665 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/copier.yaml
+-rw-r--r--   0        0        0      794 2023-07-31 15:22:50.637941 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md
+-rw-r--r--   0        0        0      701 2023-07-31 19:26:06.144964 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.145601 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf
+-rw-r--r--   0        0        0     2486 2023-07-31 19:26:06.145978 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf
+-rw-r--r--   0        0        0     1783 2023-07-31 19:26:06.146393 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf
+-rw-r--r--   0        0        0      268 2023-07-31 15:22:50.639380 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
+-rw-r--r--   0        0        0     1553 2023-07-31 19:26:06.146871 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.641148 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/.sb/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     2306 2023-08-03 18:47:45.206580 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/copier.yaml
+-rw-r--r--   0        0        0      180 2023-07-31 15:22:50.641792 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/frontend_config.yaml
+-rw-r--r--   0        0        0      658 2023-07-31 15:22:50.641933 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml
+-rw-r--r--   0        0        0      145 2023-07-31 15:22:50.642056 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/kustomization.yaml
+-rw-r--r--   0        0        0      185 2023-07-31 15:22:50.642172 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/managed_cert.yaml
+-rw-r--r--   0        0        0      378 2023-07-31 15:22:50.642293 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/ingress/skaffold.yaml
+-rw-r--r--   0        0        0       59 2023-08-03 16:02:48.218741 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/skaffold.yaml.patch
+-rw-r--r--   0        0        0     1560 2023-07-31 22:10:20.848482 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf
+-rw-r--r--   0        0        0      670 2023-07-31 19:26:06.147738 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf
+-rw-r--r--   0        0        0     1264 2023-07-31 19:26:06.148024 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf
+-rw-r--r--   0        0        0      709 2023-07-31 19:26:06.148386 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.148713 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf
+-rw-r--r--   0        0        0     1695 2023-07-31 19:26:06.149003 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf
+-rw-r--r--   0        0        0     1877 2023-07-31 19:26:06.149312 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf
+-rw-r--r--   0        0        0      480 2023-07-31 15:22:50.643659 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/terraform.tfvars
+-rw-r--r--   0        0        0     1802 2023-07-31 19:26:06.149801 solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf
+-rw-r--r--   0        0        0       80 2023-07-31 15:22:50.644034 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0     1048 2023-07-31 19:26:47.639062 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml
+-rw-r--r--   0        0        0      834 2023-07-31 19:26:06.150138 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
+-rw-r--r--   0        0        0     2760 2023-07-31 15:22:50.644547 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
+-rw-r--r--   0        0        0      670 2023-07-31 19:26:06.150553 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
+-rw-r--r--   0        0        0     1298 2023-07-31 19:26:06.151001 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.644903 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
+-rw-r--r--   0        0        0      196 2023-07-31 15:22:50.645021 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
+-rw-r--r--   0        0        0     1984 2023-07-31 19:26:06.151475 solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
+-rw-r--r--   0        0        0       90 2023-07-31 15:22:50.645285 solutions_builder-1.17.7/solutions_builder/requirements.txt
+-rw-r--r--   0        0        0    68957 2023-07-31 15:22:50.645771 solutions_builder-1.17.7/solutions_builder/template_root/.github/assets/setup_local.png
+-rw-r--r--   0        0        0   239307 2023-07-31 15:22:50.647206 solutions_builder-1.17.7/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png
+-rw-r--r--   0        0        0     2639 2023-07-31 15:22:50.647454 solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml
+-rw-r--r--   0        0        0     2690 2023-07-31 15:22:50.647592 solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml
+-rw-r--r--   0        0        0     5786 2023-08-03 18:45:22.906528 solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
+-rw-r--r--   0        0        0     8049 2023-08-03 18:45:22.906215 solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml
+-rw-r--r--   0        0        0     3131 2023-07-31 15:22:50.648490 solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml
+-rw-r--r--   0        0        0      471 2023-07-31 15:22:50.648622 solutions_builder-1.17.7/solutions_builder/template_root/.gitignore
+-rw-r--r--   0        0        0    14552 2023-07-31 15:22:50.648747 solutions_builder-1.17.7/solutions_builder/template_root/.pylintrc
+-rw-r--r--   0        0        0      711 2023-07-31 15:22:50.649129 solutions_builder-1.17.7/solutions_builder/template_root/README.md
+-rw-r--r--   0        0        0      398 2023-07-31 15:22:50.649329 solutions_builder-1.17.7/solutions_builder/template_root/components/README.md
+-rw-r--r--   0        0        0      211 2023-07-31 15:22:50.649479 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile
+-rw-r--r--   0        0        0      395 2023-07-31 15:22:50.649633 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/Dockerfile.unittest
+-rw-r--r--   0        0        0       77 2023-07-31 15:22:50.649720 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/requirements-test.txt
+-rw-r--r--   0        0        0      131 2023-07-31 15:22:50.649904 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/requirements.txt
+-rw-r--r--   0        0        0      571 2023-07-31 15:22:50.650164 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.650248 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/__init__.py
+-rw-r--r--   0        0        0      831 2023-07-31 19:26:06.151862 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py
+-rw-r--r--   0        0        0      695 2023-07-31 19:26:06.153743 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py
+-rw-r--r--   0        0        0       35 2023-07-31 15:22:50.650730 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/README.md
+-rw-r--r--   0        0        0       91 2023-07-31 15:22:50.650873 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/__init__.py
+-rw-r--r--   0        0        0     1376 2023-07-31 19:26:06.154070 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651072 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/__init__.py
+-rw-r--r--   0        0        0      754 2023-07-31 19:26:06.154613 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py
+-rw-r--r--   0        0        0     1006 2023-07-31 19:26:06.155093 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py
+-rw-r--r--   0        0        0     2243 2023-07-31 19:26:06.155755 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.651579 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-31 19:26:06.156062 solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py
+-rw-r--r--   0        0        0     2204 2023-08-03 20:00:32.823441 solutions_builder-1.17.7/solutions_builder/template_root/copier.yaml
+-rw-r--r--   0        0        0       97 2023-07-31 15:22:50.652011 solutions_builder-1.17.7/solutions_builder/template_root/firebase.json
+-rw-r--r--   0        0        0      359 2023-07-31 15:22:50.652564 solutions_builder-1.17.7/solutions_builder/template_root/sb.yaml
+-rw-r--r--   0        0        0       98 2023-07-31 15:22:50.652089 solutions_builder-1.17.7/solutions_builder/template_root/setup.cfg
+-rw-r--r--   0        0        0      215 2023-07-31 15:22:50.652207 solutions_builder-1.17.7/solutions_builder/template_root/skaffold.yaml
+-rw-r--r--   0        0        0      921 2023-07-31 19:26:06.156495 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf
+-rw-r--r--   0        0        0      730 2023-07-31 19:26:06.157029 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf
+-rw-r--r--   0        0        0     3585 2023-07-31 19:26:06.157569 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/cloudrun/main.tf
+-rw-r--r--   0        0        0     1178 2023-07-31 19:26:06.158072 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf
+-rw-r--r--   0        0        0     5024 2023-07-31 19:26:06.158367 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/compute_backend/main.tf
+-rw-r--r--   0        0        0      190 2023-07-31 15:22:50.653603 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/compute_backend/outputs.tf
+-rw-r--r--   0        0        0     1186 2023-07-31 19:26:06.158842 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf
+-rw-r--r--   0        0        0     1601 2023-07-31 19:26:06.159185 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf
+-rw-r--r--   0        0        0     2364 2023-07-31 19:26:06.159491 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/firebase/main.tf
+-rw-r--r--   0        0        0     1194 2023-07-31 19:26:06.160029 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/firebase/variables.tf
+-rw-r--r--   0        0        0     3860 2023-07-31 19:26:06.160499 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/gke/main.tf
+-rw-r--r--   0        0        0      832 2023-07-31 19:26:06.160786 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/gke/outputs.tf
+-rw-r--r--   0        0        0     3386 2023-07-31 19:26:06.161064 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/gke/variables.tf
+-rw-r--r--   0        0        0     3012 2023-07-31 22:08:39.134770 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf
+-rw-r--r--   0        0        0      692 2023-07-31 19:26:06.161609 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf
+-rw-r--r--   0        0        0     1087 2023-07-31 19:26:06.161883 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf
+-rw-r--r--   0        0        0      827 2023-07-31 19:26:06.162157 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/project_services/main.tf
+-rw-r--r--   0        0        0      774 2023-07-31 19:26:06.162534 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/project_services/variables.tf
+-rw-r--r--   0        0        0      953 2023-07-31 19:26:06.162825 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/service_account/main.tf
+-rw-r--r--   0        0        0     1037 2023-07-31 19:26:06.163149 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/service_account/variables.tf
+-rw-r--r--   0        0        0     1529 2023-07-31 19:26:06.163558 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf
+-rw-r--r--   0        0        0      678 2023-07-31 19:26:06.163969 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf
+-rw-r--r--   0        0        0     1333 2023-07-31 19:26:06.164360 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/vpc_network/main.tf
+-rw-r--r--   0        0        0     1269 2023-07-31 19:26:06.164825 solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf
+-rw-r--r--   0        0        0     2306 2023-07-31 19:39:45.308006 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf
+-rw-r--r--   0        0        0      730 2023-07-31 19:26:06.165370 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf
+-rw-r--r--   0        0        0       66 2023-07-31 15:22:50.656645 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/1-bootstrap/terraform.tfvars
+-rw-r--r--   0        0        0     1071 2023-07-31 19:26:06.165664 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf
+-rw-r--r--   0        0        0      826 2023-07-31 19:26:06.166236 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf
+-rw-r--r--   0        0        0      517 2023-07-31 15:22:50.657065 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf
+-rw-r--r--   0        0        0     1568 2023-07-31 19:26:06.166512 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf
+-rw-r--r--   0        0        0     4491 2023-08-03 22:34:41.699008 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/main.tf
+-rw-r--r--   0        0        0      991 2023-07-31 19:26:06.167766 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf
+-rw-r--r--   0        0        0      835 2023-07-31 19:26:06.168129 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf
+-rw-r--r--   0        0        0      606 2023-08-03 18:50:12.852345 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars
+-rw-r--r--   0        0        0     2546 2023-07-31 19:26:06.168711 solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.657846 solutions_builder-1.17.7/solutions_builder/template_root/tests/__init__.py
+-rw-r--r--   0        0        0      825 2023-07-31 15:22:50.658012 solutions_builder-1.17.7/solutions_builder/template_root/tests/e2e/e2e_utils.py
+-rwxr-xr-x   0        0        0      364 2023-07-31 15:22:50.658190 solutions_builder-1.17.7/solutions_builder/template_root/utils/disable_org_policies.sh
+-rwxr-xr-x   0        0        0      990 2023-07-31 19:26:06.169251 solutions_builder-1.17.7/solutions_builder/template_root/utils/init_env_vars.sh
+-rw-r--r--   0        0        0       81 2023-07-31 15:22:50.658645 solutions_builder-1.17.7/solutions_builder/template_root/{{_copier_conf.answers_file}}
+-rw-r--r--   0        0        0        0 2023-07-31 15:22:50.658746 solutions_builder-1.17.7/solutions_builder/tests/__init__.py
+-rw-r--r--   0        0        0     6154 1970-01-01 00:00:00.000000 solutions_builder-1.17.7/PKG-INFO
```

### Comparing `solutions_builder-1.17.6/LICENSE` & `solutions_builder-1.17.7/LICENSE`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/README.md` & `solutions_builder-1.17.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,28 +45,35 @@
 
 With `pipx`:
 ```
 pip install --user pipx
 pipx install solutions-builder
 ```
 
-## Getting Started
+## Quick Start
+
+This quick start steps will do the following:
+- Create a new GCP project and initialize Cloud foundation.
+- Add a RESTful API service for managing Todo list.
+- Deploy the service to Cloud Run.
 
 Set up GCP project
 ```
-# Optional: create a new GCP project. You can also use an existing GCP project.
-gcloud projects create my-solution-gcp-id
+export PROJECT_ID=my-solution-gcp-id
+
+# (Optional) Create a new GCP project. You can also use an existing GCP project.
+gcloud projects create $PROJECT_ID
 
 # Set gcloud CLI to the GCP project.
-gcloud config set project my-solutions-gcp-id
+gcloud config set project $PROJECT_ID
 ```
 
 Generate a new solution folder.
 ```
-sb new my-solution .
+sb new my-solution
 ```
 
 This will prompt options and variables:
 ```
 🎤 What is your project name? (Spaces are allowed.)
    my-solution
 🎤 What is your Google Cloud project ID?
```

### Comparing `solutions_builder-1.17.6/pyproject.toml` & `solutions_builder-1.17.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solutions-builder"
-version = "1.17.6"
+version = "1.17.7"
 description = "A solution framework to generate a project with built-in structure and modules"
 authors = ["Jon Chen <jonchen@google.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/GoogleCloudPlatform/solutions-builder"
 repository = "https://github.com/GoogleCloudPlatform/solutions-builder"
 packages = [
```

### Comparing `solutions_builder-1.17.6/solutions_builder/cli/cli.py` & `solutions_builder-1.17.7/solutions_builder/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,31 +92,31 @@
     raise FileNotFoundError(f"Solution folder {solution_path} does not exist.")
 
   confirm(
       f"\nThis will update solution root folder at '{solution_path}'. Continue?"
   )
 
   # Copy template_root to destination, excluding skaffold.yaml.
-  orig_st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  orig_st_yaml = read_yaml(f"{solution_path}/sb.yaml")
 
   if not template_path:
     current_dir = os.path.dirname(__file__)
     template_path = f"{current_dir}/../template_root"
     if not os.path.exists(template_path):
       raise FileNotFoundError(f"{template_path} does not exist.")
   worker = run_auto(template_path,
                     solution_path,
-                    exclude=["skaffold.yaml", "st.yaml"])
+                    exclude=["skaffold.yaml", "sb.yaml"])
   answers = worker.answers.last
 
-  # Restore some fields in st.yaml.
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  # Restore some fields in sb.yaml.
+  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   st_yaml["created_at"] = orig_st_yaml["created_at"]
   st_yaml["components"] = orig_st_yaml["components"]
-  write_yaml(f"{solution_path}/st.yaml", st_yaml)
+  write_yaml(f"{solution_path}/sb.yaml", st_yaml)
 
   print_success(f"Complete. Solution folder updated at {solution_path}.\n")
 
 
 # Build and deploy services.
 @app.command()
 def deploy(profile: str = DEFAULT_DEPLOY_PROFILE,
@@ -126,15 +126,15 @@
                                     typer.Argument()] = ".",
            yes: Optional[bool] = False):
   """
   Build and deploy services.
   """
   validate_solution_folder(solution_path)
 
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   project_id = st_yaml["project_id"]
   terraform_gke = st_yaml["components"].get("terraform_gke")
   commands = []
 
   if component:
     component_flag = f" -m {component} "
   else:
@@ -172,15 +172,15 @@
                                     typer.Argument()] = ".",
            yes: Optional[bool] = False):
   """
   Delete deployment.
   """
   validate_solution_folder(solution_path)
 
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   project_id = st_yaml["project_id"]
 
   if component:
     component_flag = f" -m {component} "
   else:
     component_flag = ""
```

### Comparing `solutions_builder-1.17.6/solutions_builder/cli/cli_utils.py` & `solutions_builder-1.17.7/solutions_builder/cli/cli_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 
 
 def confirm(msg, skip=False, default=True):
   if not skip:
     typer.confirm(msg, abort=True, default=default)
 
 
-# Check if the solution folder has st.yaml file.
+# Check if the solution folder has sb.yaml file.
 def validate_solution_folder(path):
-  if not os.path.isfile(path + "/st.yaml"):
+  if not os.path.isfile(path + "/sb.yaml"):
     raise FileNotFoundError(
-        f"Path {path} is not a valid solution folder: missing st.yaml")
+        f"Path {path} is not a valid solution folder: missing sb.yaml")
   return True
 
 
 def get_copier_yaml(path):
   filepath = f"{path}/copier.yaml"
 
   if not os.path.isfile(filepath):
```

### Comparing `solutions_builder-1.17.6/solutions_builder/cli/component.py` & `solutions_builder-1.17.7/solutions_builder/cli/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,47 +64,47 @@
   print_success(
       f"Complete. Component {component_name} updated to solution at {solution_path}\n"
   )
 
 
 def update_component_to_root_yaml(component_name, answers, solution_path):
   # Update Solution root YAML with new component name.
-  solution_yaml_dict = read_yaml(f"{solution_path}/st.yaml") or {}
+  solution_yaml_dict = read_yaml(f"{solution_path}/sb.yaml") or {}
   components = solution_yaml_dict["components"] or {}
   components[component_name] = answers
   solution_yaml_dict["components"] = components
-  write_yaml(f"{solution_path}/st.yaml", solution_yaml_dict)
+  write_yaml(f"{solution_path}/sb.yaml", solution_yaml_dict)
 
 
 def process_component(method,
                       component_name,
                       solution_path,
                       data={},
                       use_existing_answers=False):
   destination_path = "."
   current_dir = os.path.dirname(__file__)
   answers_file = None
 
-  # Get basic info from root st.yaml.
-  root_st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  # Get basic info from root sb.yaml.
+  root_st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   component_answers = {}
 
   # If the component name is a Git URL, use the URL as-is in copier.
   if check_git_url(component_name):
     print(f"Loading component from remote Git URL: {component_name}")
     template_path = component_name
 
   # Otherwise, try to locate the component in local modules/ folder.
   else:
 
     if method == "update":
       data["component_name"] = component_name
       if component_name not in root_st_yaml["components"]:
         raise NameError(
-            f"Component {component_name} is not defined in the root yaml 'st.yaml' file."
+            f"Component {component_name} is not defined in the root yaml 'sb.yaml' file."
         )
       component_answers = root_st_yaml["components"][component_name]
       component_template = component_answers["component_template"]
       template_path = f"{current_dir}/../modules/{component_template}"
       answers_file = f".st/module_answers/{component_name}.yaml"
 
       # Use existing answer values in data, skipping the prompt.
@@ -141,32 +141,33 @@
   for key, value in worker.answers.default.items():
     if key not in answers:
       answers[key] = component_answers.get(key) or value
   answers["component_template"] = component_template
   answers["destination_path"] = copier_dict["_metadata"].get(
       "destination_path")
 
-  # Update component's answer back to st.yaml.
+  # Update component's answer back to sb.yaml.
   update_component_to_root_yaml(answers["component_name"], answers,
                                 solution_path)
 
   # Patch skaffold.yaml
   for patch_file in copier_dict.get("_patch", []):
     print(f"Patching {patch_file}...")
     new_yaml = patch_yaml(f"{solution_path}/{patch_file}",
                           f"{solution_path}/{patch_file}.patch")
     new_yaml["requires"] = dedupe(new_yaml["requires"])
     write_yaml(f"{solution_path}/{patch_file}", new_yaml)
     os.remove(f"{solution_path}/{patch_file}.patch")
 
+  print()
 
 # List installed components.
 @component_app.command()
 def list(solution_path: Annotated[Optional[str], typer.Argument()] = ".", ):
-  root_st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  root_st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   components = root_st_yaml.get("components", [])
   print("Installed components:\n")
   for component_name, properties in components.items():
     typer.echo(
         typer.style(f"- {component_name} ", fg=typer.colors.WHITE, bold=True) +
         typer.style(f"(from: {properties['component_template']})",
                     fg=typer.colors.BLACK,
```

### Comparing `solutions_builder-1.17.6/solutions_builder/cli/infra.py` & `solutions_builder-1.17.7/solutions_builder/cli/infra.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
   if not yes:
     auto_approve_flag = ""
   else:
     auto_approve_flag = "-auto-approve"
 
   # Get project ID from the existing root yaml.
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   project_id = st_yaml["project_id"]
 
   confirm(f"""
   This will initialize the solution with the following steps:
   - Set gcloud project to '{project_id}'
   - Run terraform init and apply in 'bootstrap' stage.
   - Run terraform init and apply in 'foundation' stage.
@@ -104,15 +104,15 @@
   This will initialize the solution with the following steps:
   - Run terraform init and apply in '{stage}' stage.
 
   This will take a few minutes. Continue?""",
           skip=yes)
 
   # Get project_id
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   project_id = st_yaml["project_id"]
 
   # Get impersonate service account email
   env_var_cluase = get_impersonate_clause(impersonate, impersonate_email,
                                           project_id)
   working_dir = f"{solution_path}/terraform/stages/{stage}"
   exec_shell(f"{env_var_cluase} terraform init", working_dir=working_dir)
@@ -148,15 +148,15 @@
   confirm(f"""
   WARNING! This will destory all resources created by 'terraform/{stage}'.
 
   This will take a few minutes. Continue?""",
           skip=yes)
 
   # Get project ID from the existing root yaml.
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   project_id = st_yaml["project_id"]
 
   # Get impersonate service account email
   env_var_cluase = get_impersonate_clause(impersonate, impersonate_email,
                                           project_id)
   working_dir = f"{solution_path}/terraform/stages/{stage}"
   exec_shell(f"{env_var_cluase} terraform init", working_dir=working_dir)
```

### Comparing `solutions_builder-1.17.6/solutions_builder/cli/set.py` & `solutions_builder-1.17.7/solutions_builder/cli/set.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 @set_app.command()
 def project_id(
     new_project_id,
     solution_path: Annotated[Optional[str], typer.Argument()] = ".",
     yes: Optional[bool] = False,
 ):
   validate_solution_folder(solution_path)
-  root_st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  root_st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   old_project_id = root_st_yaml.get("project_id")
-  assert old_project_id, "project_id does not exist in st.yaml"
+  assert old_project_id, "project_id does not exist in sb.yaml"
 
   confirm(
       f"This will replace all project-id '{old_project_id}' to '{new_project_id}' in folder '{solution_path}'. "
       + "Continue?",
       skip=yes)
 
   root_st_yaml["project_id"] = new_project_id
   root_st_yaml["project_number"] = get_project_number(new_project_id)
-  write_yaml(f"{solution_path}/st.yaml", root_st_yaml)
+  write_yaml(f"{solution_path}/sb.yaml", root_st_yaml)
 
   file_set = set()
   # Adding includes.
   for pattern in INCLUDE_PATTERNS:
     file_list = pathlib.Path(solution_path).rglob(f"{pattern}")
     file_set.update(set([str(x) for x in file_list]))
```

### Comparing `solutions_builder-1.17.6/solutions_builder/cli/template.py` & `solutions_builder-1.17.7/solutions_builder/cli/template.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/copier_extensions/st_helpers.py` & `solutions_builder-1.17.7/solutions_builder/copier_extensions/st_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,15 +102,15 @@
   return exec_gcloud_output(command)
 
 
 def get_services_from_yaml(solution_path):
   """
     Get the service list from root yaml.
     """
-  st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  st_yaml = read_yaml(f"{solution_path}/sb.yaml")
   services = []
   components = st_yaml.get("components", {})
   for component_name, properties in components.items():
     if properties.get("service_path"):
       services.append(properties["resource_name"])
   return ",".join(services)
```

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/README.md` & `solutions_builder-1.17.7/solutions_builder/module_template/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/copier.yaml` & `solutions_builder-1.17.7/solutions_builder/module_template/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/template_copier.yaml` & `solutions_builder-1.17.7/solutions_builder/module_template/template_copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml` & `solutions_builder-1.17.7/solutions_builder/module_template/{{"{{'.github' if use_github_action}}"}}/workflows/{{"unit_test_linter_{{component_name}}"}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile` & `solutions_builder-1.17.7/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml` & `solutions_builder-1.17.7/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py` & `solutions_builder-1.17.7/solutions_builder/module_template/{{'components' if has_component}}/{{'{{component_name}}'}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf` & `solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf` & `solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf` & `solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars` & `solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf` & `solutions_builder-1.17.7/solutions_builder/module_template/{{'terraform' if has_terraform_stage}}/stages/{{terraform_stage if has_terraform_stage}}/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/README.md` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/README.md` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/copier.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/README.md` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/models/task.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/routes/tasks.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/schemas/task.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/src/workflow/workflow_test.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/components/{{component_name}}/{{'kustomize' if default_deploy=='gke' else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/copier.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/terraform/stages/3-task-dispatch/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/task_dispatch_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/copier.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/docs/components/{{component_name}}.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke/terraform/stages/2-gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/copier.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/copier.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -37,17 +37,23 @@
   default: "{{('privateClusterConfig.publicEndpoint', cluster_name, gcp_region) | get_cluster_value}}"
 
 kubernetes_services:
   type: str
   help: Kubernetes service names in ingress? (comma-separated string)
   default: "{{solution_path | get_services_from_yaml}}"
 
+use_custom_domain:
+  type: bool
+  help: Use a custom Domain with cert?
+  default: true
+
 domains:
   type: str
   help: DNS domains (comma-separated string)?
+  when: "{{use_custom_domain}}"
 
 cors_allow_origins:
   type: str
   help: Allow domains for CORS? (comma-seperated)
   default: "http://localhost:4200,http://localhost:3000"
 
 cert_issuer_email:
```

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/ingress/kustomize/gke/ingress.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/main.tf`

 * *Files 15% similar despite different names*

```diff
@@ -53,41 +53,7 @@
 }
 
 resource "google_compute_ssl_policy" "gke-ingress-ssl-policy" {
   name            = "gke-ingress-ssl-policy"
   profile         = "MODERN"
   min_tls_version = "TLS_1_2"
 }
-
-# resource "kubernetes_ingress_v1" "default_ingress" {
-
-#   metadata {
-#     name = "default-ingress"
-#     annotations = {
-#       "kubernetes.io/ingress.class"                 = "gce"
-#       "kubernetes.io/ingress.global-static-ip-name" = local.global_static_ip_name
-#       "networking.gke.io/managed-certificates"      = var.managed_cert_name
-#       "networking.gke.io/v1beta1.FrontendConfig"    = var.frontend_config_name
-#     }
-#   }
-
-#   spec {
-#     rule {
-#       host = var.domains[0]
-#       http {
-#         # Sample Service
-#         path {
-#           backend {
-#             service {
-#               name = "sample-service"
-#               port {
-#                 number = 80
-#               }
-#             }
-#           }
-#           path_type = "Prefix"
-#           path      = "/sample_service"
-#         }
-#       }
-#     }
-#   }
-# }
```

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/modules/ingress_gce/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_gke_ingress/terraform/stages/3-gke-ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf` & `solutions_builder-1.17.7/solutions_builder/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/.github/assets/setup_local.png` & `solutions_builder-1.17.7/solutions_builder/template_root/.github/assets/setup_local.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png` & `solutions_builder-1.17.7/solutions_builder/template_root/.github/assets/skaffold_dev_terminal.png`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml` & `solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/deployment_cloudrun_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml` & `solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/deployment_gke_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml` & `solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/e2e_cloudrun_api_test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     paths:
       - "microservices/**"
       - "common/**"
       - "e2e/cloudrun_api_tests/**"
       - "e2e/requirements.txt"
       - "e2e/utils/**"
       - "utils/**"
-      - ".github/workflows/e2e_cloudrun_api_test.yaml"
+      - ".github/workflows/e2e_cloudrun_api_tesb.yaml"
   workflow_dispatch:
 env:
   PROJECT_ID: {{project_id}}
   REGION: {{gcp_region}}
   ENV: dev
 
 # copoier:raw {% raw %}
```

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml` & `solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/e2e_gke_api_test.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     paths:
       - "microservices/**"
       - "common/**"
       - "e2e/gke_api_tests/**"
       - "e2e/requirements.txt"
       - "e2e/utils/**"
       - "utils/**"
-      - ".github/workflows/e2e_gke_api_test.yaml"
+      - ".github/workflows/e2e_gke_api_tesb.yaml"
   workflow_dispatch:
 env:
   PROJECT_ID: {{project_id}}
   SKAFFOLD_DEFAULT_REPO: gcr.io/{{project_id}}
   SKAFFOLD_NAMESPACE: default
   GKE_CLUSTER: main-cluster
   GKE_ZONE: {{gcp_region}}
```

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml` & `solutions_builder-1.17.7/solutions_builder/template_root/.github/workflows/unit_test_linter_common.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/.pylintrc` & `solutions_builder-1.17.7/solutions_builder/template_root/.pylintrc`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/README.md` & `solutions_builder-1.17.7/solutions_builder/template_root/README.md`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml` & `solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py` & `solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/config.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py` & `solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/db_client.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py` & `solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/models/example.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py` & `solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/bq_client_fixture.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py` & `solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/client_with_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py` & `solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/testing/firestore_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py` & `solutions_builder-1.17.7/solutions_builder/template_root/components/{{'common' if has_common}}/src/common/utils/logging_handler.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/copier.yaml` & `solutions_builder-1.17.7/solutions_builder/template_root/copier.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 gcp_region:
   type: str
   help: Which Google Cloud region?
   default: us-central1
 
 has_common:
   type: bool
-  help: Include a common component (for shared data models, utils, etc)?
+  help: Include a common container image for shared libraries, data models, utils, etc?
   default: true
 
 terraform_backend_gcs:
   type: bool
   help: Use GCS Bucket for Terraform backend?
   default: true
 
@@ -37,27 +37,27 @@
   type: bool
   help: Show advanced settings (VPC, Storage region, etc)?
   default: false
 
 create_vpc_network:
   type: bool
   help: Create a default VPC Network?
-  default: false
+  default: true
   when: "{{advanced_settings}}"
 
 vpc_network:
   type: str
   help: VPC Network ID?
-  default: default-vpc
+  default: "{{'default-vpc' if create_vpc_network}}"
   when: "{{advanced_settings and create_vpc_network}}"
 
 vpc_subnetwork:
   type: str
   help: VPC Subnetwork ID?
-  default: default-vpc-subnet
+  default: "{{'default-vpc-subset' if create_vpc_network}}"
   when: "{{advanced_settings and create_vpc_network}}"
 
 ip_cidr_range:
   type: str
   help: IP CIDR range?
   default: 10.0.0.0/16
   when: "{{advanced_settings and create_vpc_network}}"
```

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/cloudbuild/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/cloudbuild/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudrun/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/compute_backend/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/compute_backend/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/compute_backend/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/firebase/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/firebase/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/firebase/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/firebase/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/gke/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/outputs.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/gke/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/gke/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/ingress_nginx/main.tf`

 * *Files 17% similar despite different names*

```diff
@@ -57,53 +57,53 @@
 
   # TODO: does this require cert_manager up and running or can they be completed in parallel
   depends_on = [
     module.cert_manager, kubernetes_namespace.ingress_nginx
   ]
 }
 
-resource "kubernetes_ingress_v1" "default_ingress" {
-  depends_on = [
-    module.nginx-controller
-  ]
+# resource "kubernetes_ingress_v1" "default_ingress" {
+#   depends_on = [
+#     module.nginx-controller
+#   ]
 
-  metadata {
-    name = "default-ingress"
-    annotations = {
-      "kubernetes.io/ingress.class"                        = "nginx"
-      "cert-manager.io/cluster-issuer"                     = module.cert_manager.cluster_issuer_name
-      "nginx.ingress.kubernetes.io/enable-cors"            = "true"
-      "nginx.ingress.kubernetes.io/cors-allow-methods"     = "PUT,GET,POST,DELETE,OPTIONS"
-      "nginx.ingress.kubernetes.io/cors-allow-origin"      = var.cors_allow_origins
-      "nginx.ingress.kubernetes.io/cors-allow-credentials" = "true"
-      "nginx.ingress.kubernetes.io/proxy-read-timeout"     = "3600"
-    }
-  }
+#   metadata {
+#     name = "default-ingress"
+#     annotations = {
+#       "kubernetes.io/ingress.class"                        = "nginx"
+#       "cert-manager.io/cluster-issuer"                     = module.cert_manager.cluster_issuer_name
+#       "nginx.ingress.kubernetes.io/enable-cors"            = "true"
+#       "nginx.ingress.kubernetes.io/cors-allow-methods"     = "PUT,GET,POST,DELETE,OPTIONS"
+#       "nginx.ingress.kubernetes.io/cors-allow-origin"      = var.cors_allow_origins
+#       "nginx.ingress.kubernetes.io/cors-allow-credentials" = "true"
+#       "nginx.ingress.kubernetes.io/proxy-read-timeout"     = "3600"
+#     }
+#   }
 
-  spec {
-    rule {
-      http {
-        # Sample Service
-        path {
-          backend {
-            service {
-              name = "sample-service"
-              port {
-                number = 80
-              }
-            }
-          }
-          path_type = "Prefix"
-          path      = "/sample_service"
-        }
-      }
-    }
+#   spec {
+#     rule {
+#       http {
+#         # Sample Service
+#         path {
+#           backend {
+#             service {
+#               name = "sample-service"
+#               port {
+#                 number = 80
+#               }
+#             }
+#           }
+#           path_type = "Prefix"
+#           path      = "/sample_service"
+#         }
+#       }
+#     }
 
-    tls {
-      hosts = [
-        var.api_domain,
-        google_compute_address.ingress_ip_address.address,
-      ]
-      secret_name = "cert-manager-private-key"
-    }
-  }
-}
+#     tls {
+#       hosts = [
+#         var.api_domain,
+#         google_compute_address.ingress_ip_address.address,
+#       ]
+#       secret_name = "cert-manager-private-key"
+#     }
+#   }
+# }
```

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/ingress_nginx/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/ingress_nginx/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/project_services/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/project_services/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/project_services/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/project_services/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/service_account/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/service_account/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/service_account/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/service_account/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/terraform_cicd/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/terraform_cicd/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/vpc_network/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/vpc_network/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/modules/vpc_network/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/1-bootstrap/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/1-bootstrap/output.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/1-bootstrap/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/firestore_setup.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/main.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/main.tf`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 module "project_services" {
   source     = "../../modules/project_services"
   project_id = var.project_id
   services   = local.services
 }
 
 module "vpc_network" {
+  count                     = ((var.vpc_network != null && var.vpc_network != "") ? 1 : 0)
   depends_on                = [module.project_services]
   source                    = "../../modules/vpc_network"
   project_id                = var.project_id
   vpc_network               = var.vpc_network
   region                    = var.region
   vpc_subnetwork            = var.vpc_subnetwork
   subnet_ip                 = var.ip_cidr_range
```

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf` & `solutions_builder-1.17.7/solutions_builder/template_root/terraform/stages/2-foundation/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/tests/e2e/e2e_utils.py` & `solutions_builder-1.17.7/solutions_builder/template_root/tests/e2e/e2e_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/solutions_builder/template_root/utils/init_env_vars.sh` & `solutions_builder-1.17.7/solutions_builder/template_root/utils/init_env_vars.sh`

 * *Files identical despite different names*

### Comparing `solutions_builder-1.17.6/PKG-INFO` & `solutions_builder-1.17.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solutions-builder
-Version: 1.17.6
+Version: 1.17.7
 Summary: A solution framework to generate a project with built-in structure and modules
 Home-page: https://github.com/GoogleCloudPlatform/solutions-builder
 License: Apache
 Author: Jon Chen
 Author-email: jonchen@google.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -72,28 +72,35 @@
 
 With `pipx`:
 ```
 pip install --user pipx
 pipx install solutions-builder
 ```
 
-## Getting Started
+## Quick Start
+
+This quick start steps will do the following:
+- Create a new GCP project and initialize Cloud foundation.
+- Add a RESTful API service for managing Todo list.
+- Deploy the service to Cloud Run.
 
 Set up GCP project
 ```
-# Optional: create a new GCP project. You can also use an existing GCP project.
-gcloud projects create my-solution-gcp-id
+export PROJECT_ID=my-solution-gcp-id
+
+# (Optional) Create a new GCP project. You can also use an existing GCP project.
+gcloud projects create $PROJECT_ID
 
 # Set gcloud CLI to the GCP project.
-gcloud config set project my-solutions-gcp-id
+gcloud config set project $PROJECT_ID
 ```
 
 Generate a new solution folder.
 ```
-sb new my-solution .
+sb new my-solution
 ```
 
 This will prompt options and variables:
 ```
 🎤 What is your project name? (Spaces are allowed.)
    my-solution
 🎤 What is your Google Cloud project ID?
```

