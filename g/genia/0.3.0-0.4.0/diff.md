# Comparing `tmp/genia-0.3.0.tar.gz` & `tmp/genia-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genia-0.3.0.tar", max compression
+gzip compressed data, was "genia-0.4.0.tar", max compression
```

## Comparing `genia-0.3.0.tar` & `genia-0.4.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    11357 2023-07-25 18:58:10.473401 genia-0.3.0/LICENSE
--rw-r--r--   0        0        0    16951 2023-08-03 20:43:54.347468 genia-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-08-03 18:27:24.994507 genia-0.3.0/genia/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 11:35:19.723328 genia-0.3.0/genia/agents/__init__.py
--rw-r--r--   0        0        0     1390 2023-08-03 13:16:37.105090 genia-0.3.0/genia/agents/adhoc.py
--rw-r--r--   0        0        0      149 2023-07-25 19:10:06.523636 genia-0.3.0/genia/agents/agent.py
--rw-r--r--   0        0        0    10118 2023-08-03 13:35:24.438526 genia-0.3.0/genia/agents/chat.py
--rw-r--r--   0        0        0    11173 2023-08-03 05:18:35.540529 genia-0.3.0/genia/conversation/llm_conversation.py
--rw-r--r--   0        0        0     2633 2023-07-29 18:18:06.111171 genia-0.3.0/genia/conversation/llm_conversation_in_memory_repository.py
--rw-r--r--   0        0        0      368 2023-08-03 20:49:36.376825 genia-0.3.0/genia/entry.py
--rw-r--r--   0        0        0       39 2023-07-29 18:18:06.111310 genia-0.3.0/genia/llm_function/__init__.py
--rw-r--r--   0        0        0      190 2023-07-25 19:10:06.524003 genia-0.3.0/genia/llm_function/llm_function.py
--rw-r--r--   0        0        0    12462 2023-08-03 19:56:58.675311 genia-0.3.0/genia/llm_function/llm_function_repository.py
--rw-r--r--   0        0        0     1071 2023-07-25 19:10:06.524212 genia-0.3.0/genia/llm_function/llm_functions_factory.py
--rw-r--r--   0        0        0      743 2023-07-25 19:10:06.524263 genia-0.3.0/genia/llm_function/llm_skill_function.py
--rw-r--r--   0        0        0     1543 2023-07-25 19:10:06.524315 genia-0.3.0/genia/llm_function/open_api_function.py
--rw-r--r--   0        0        0     2041 2023-07-27 10:09:24.342389 genia-0.3.0/genia/llm_function/python_function.py
--rw-r--r--   0        0        0      660 2023-07-25 19:10:06.524422 genia-0.3.0/genia/llm_function/url_function.py
--rw-r--r--   0        0        0       44 2023-07-29 18:18:06.111705 genia-0.3.0/genia/llm_function_lookup_strategy/__init__.py
--rw-r--r--   0        0        0     2731 2023-07-31 12:24:50.543452 genia-0.3.0/genia/llm_function_lookup_strategy/llm_function_lookup_strategy.py
--rw-r--r--   0        0        0     2264 2023-08-03 20:21:14.053526 genia-0.3.0/genia/main.py
--rw-r--r--   0        0        0     8360 2023-07-25 19:10:06.524521 genia-0.3.0/genia/openai_plugins/openai_plugins_repository.py
--rw-r--r--   0        0        0     5868 2023-08-02 12:35:12.375515 genia-0.3.0/genia/settings/prompts.toml
--rw-r--r--   0        0        0     1003 2023-08-03 13:01:14.459038 genia-0.3.0/genia/settings/settings.toml
--rw-r--r--   0        0        0      299 2023-07-25 19:10:06.524709 genia-0.3.0/genia/settings_loader.py
--rw-r--r--   0        0        0     6098 2023-07-25 19:10:06.524800 genia-0.3.0/genia/token_limiter/token_limiter_openai.py
--rw-r--r--   0        0        0     2639 2023-07-31 13:33:50.543156 genia-0.3.0/genia/tool_validators/llm_tool_validator.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.524931 genia-0.3.0/genia/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.524979 genia-0.3.0/genia/tools/argo/__init__.py
--rw-r--r--   0        0        0     5596 2023-07-25 19:10:06.525050 genia-0.3.0/genia/tools/argo/argo_client.py
--rw-r--r--   0        0        0      796 2023-07-25 19:10:06.525107 genia-0.3.0/genia/tools/argo/workflow_template.json
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.525156 genia-0.3.0/genia/tools/aws_client/__init__.py
--rw-r--r--   0        0        0      506 2023-07-25 19:10:06.525210 genia-0.3.0/genia/tools/aws_client/aws_client.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.525257 genia-0.3.0/genia/tools/aws_client/cloudtrail/__init__.py
--rw-r--r--   0        0        0     2670 2023-07-25 19:10:06.525315 genia-0.3.0/genia/tools/aws_client/cloudtrail/aws_client_cloudtrail.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.525370 genia-0.3.0/genia/tools/aws_client/ec2/__init__.py
--rw-r--r--   0        0        0     2069 2023-07-25 19:10:06.525435 genia-0.3.0/genia/tools/aws_client/ec2/aws_client_ec2.py
--rw-r--r--   0        0        0      461 2023-07-27 12:25:45.909818 genia-0.3.0/genia/tools/aws_client/ecr/aws_client_ecr.py
--rw-r--r--   0        0        0     3851 2023-07-27 12:40:31.519890 genia-0.3.0/genia/tools/aws_client/ecr/repository_info_collector.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.525482 genia-0.3.0/genia/tools/aws_client/ecs/__init__.py
--rw-r--r--   0        0        0     1797 2023-07-25 19:10:06.525540 genia-0.3.0/genia/tools/aws_client/ecs/aws_client_ecs.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.525589 genia-0.3.0/genia/tools/aws_client/events/__init__.py
--rw-r--r--   0        0        0     4893 2023-07-25 19:10:06.525649 genia-0.3.0/genia/tools/aws_client/events/aws_client_events.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.525701 genia-0.3.0/genia/tools/aws_client/iam/__init__.py
--rw-r--r--   0        0        0     3641 2023-07-27 15:10:48.693284 genia-0.3.0/genia/tools/aws_client/iam/aws_client_iam.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.525811 genia-0.3.0/genia/tools/aws_client/lambdas/__init__.py
--rw-r--r--   0        0        0    16060 2023-07-26 20:26:57.682507 genia-0.3.0/genia/tools/aws_client/lambdas/aws_client_lambda.py
--rw-r--r--   0        0        0      290 2023-07-25 19:10:06.525999 genia-0.3.0/genia/tools/aws_client/lambdas/docker/Dockerfile
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.526022 genia-0.3.0/genia/tools/aws_client/lambdas/docker/__init__.py
--rwxr-xr-x   0        0        0      125 2023-07-25 19:10:06.526077 genia-0.3.0/genia/tools/aws_client/lambdas/docker/docker-build.sh
--rwxr-xr-x   0        0        0       97 2023-07-25 19:10:06.526137 genia-0.3.0/genia/tools/aws_client/lambdas/docker/entrypoint.sh
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.526189 genia-0.3.0/genia/tools/aws_client/sqs/__init__.py
--rw-r--r--   0        0        0     3775 2023-07-25 19:10:06.526275 genia-0.3.0/genia/tools/aws_client/sqs/aws_client_sqs.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.526328 genia-0.3.0/genia/tools/github_client/__init__.py
--rw-r--r--   0        0        0     3436 2023-08-03 05:18:35.541349 genia-0.3.0/genia/tools/github_client/github_client.py
--rw-r--r--   0        0        0      553 2023-08-03 05:18:35.541636 genia-0.3.0/genia/tools/github_client/github_enriched_client.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.526513 genia-0.3.0/genia/tools/jenkins/__init__.py
--rw-r--r--   0        0        0     1210 2023-07-25 19:10:06.526581 genia-0.3.0/genia/tools/jenkins/jenkins_client.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.526634 genia-0.3.0/genia/tools/kubernetes_client/__init__.py
--rw-r--r--   0        0        0     3659 2023-07-25 19:10:06.526693 genia-0.3.0/genia/tools/kubernetes_client/cronjob.py
--rw-r--r--   0        0        0    14598 2023-07-31 18:54:23.418163 genia-0.3.0/genia/tools/kubernetes_client/deployment.py
--rw-r--r--   0        0        0      941 2023-07-31 18:54:23.418460 genia-0.3.0/genia/tools/kubernetes_client/events.py
--rw-r--r--   0        0        0      726 2023-07-31 20:19:02.120023 genia-0.3.0/genia/tools/kubernetes_client/global.py
--rw-r--r--   0        0        0     5784 2023-07-25 19:10:06.526969 genia-0.3.0/genia/tools/kubernetes_client/jobs.py
--rw-r--r--   0        0        0      980 2023-07-25 19:10:06.527029 genia-0.3.0/genia/tools/kubernetes_client/kubernetes_clients.py
--rw-r--r--   0        0        0     1504 2023-07-25 19:10:06.527102 genia-0.3.0/genia/tools/kubernetes_client/namespace.py
--rw-r--r--   0        0        0     5262 2023-07-25 19:10:06.527224 genia-0.3.0/genia/tools/kubernetes_client/pod.py
--rw-r--r--   0        0        0      530 2023-07-25 19:10:06.527281 genia-0.3.0/genia/tools/kubernetes_client/secret.py
--rw-r--r--   0        0        0     1377 2023-07-25 19:10:06.527339 genia-0.3.0/genia/tools/kubernetes_client/service.py
--rw-r--r--   0        0        0     1843 2023-07-25 19:10:06.527398 genia-0.3.0/genia/tools/kubernetes_client/utils.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.527452 genia-0.3.0/genia/tools/opa/__init__.py
--rw-r--r--   0        0        0     1147 2023-07-25 19:10:06.527522 genia-0.3.0/genia/tools/opa/opa.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.527594 genia-0.3.0/genia/tools/opa/policies/__init__.py
--rw-r--r--   0        0        0      472 2023-07-25 19:10:06.527661 genia-0.3.0/genia/tools/opa/policies/k8s_policies.rego
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.527724 genia-0.3.0/genia/tools/opa/policies/samples/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.527786 genia-0.3.0/genia/tools/opa/policies/samples/k8s/__init__.py
--rw-r--r--   0        0        0      774 2023-07-25 19:10:06.527927 genia-0.3.0/genia/tools/opa/policies/samples/k8s/not_defining_resource_limits.json
--rw-r--r--   0        0        0      969 2023-07-25 19:10:06.528005 genia-0.3.0/genia/tools/opa/policies/samples/k8s/running_containers_as_root.json
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.528070 genia-0.3.0/genia/tools/pagerduty_client/__init__.py
--rw-r--r--   0        0        0     2490 2023-07-25 19:10:06.528153 genia-0.3.0/genia/tools/pagerduty_client/pagerduty_client.py
--rw-r--r--   0        0        0     3028 2023-07-25 19:10:06.528232 genia-0.3.0/genia/tools/react.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.528297 genia-0.3.0/genia/tools/skills/__init__.py
--rw-r--r--   0        0        0     1573 2023-07-25 19:10:06.528364 genia-0.3.0/genia/tools/skills/skills_repository.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.528421 genia-0.3.0/genia/tools/slack/__init__.py
--rw-r--r--   0        0        0      718 2023-07-26 20:46:54.519405 genia-0.3.0/genia/tools/slack/slack_client.py
--rw-r--r--   0        0        0      238 2023-07-29 18:18:06.112372 genia-0.3.0/genia/tools_config/core/aws/aws_functions.json
--rw-r--r--   0        0        0      158 2023-07-29 18:18:06.112460 genia-0.3.0/genia/tools_config/core/aws/aws_tools.yaml
--rw-r--r--   0        0        0    34082 2023-07-31 18:54:23.422457 genia-0.3.0/genia/tools_config/core/functions.json
--rw-r--r--   0        0        0     9906 2023-08-03 05:18:35.542314 genia-0.3.0/genia/tools_config/core/tools.yaml
--rw-r--r--   0        0        0     3707 2023-08-03 05:18:35.542541 genia-0.3.0/genia/tools_config/extended/README.md
--rw-r--r--   0        0        0      452 2023-08-03 05:18:35.542777 genia-0.3.0/genia/tools_config/extended/github/github_functions.json
--rw-r--r--   0        0        0      193 2023-08-03 05:18:35.542916 genia-0.3.0/genia/tools_config/extended/github/github_tools.yaml
--rw-r--r--   0        0        0     1839 2023-07-25 19:10:06.528988 genia-0.3.0/genia/tools_config/playground/playground_functions.json
--rw-r--r--   0        0        0      491 2023-07-25 19:10:06.529047 genia-0.3.0/genia/tools_config/playground/playground_tools.yaml
--rw-r--r--   0        0        0      917 2023-07-30 07:20:35.471467 genia-0.3.0/genia/tools_config/skills/calculate_rectangle_area.txt
--rw-r--r--   0        0        0      593 2023-07-30 07:20:35.471559 genia-0.3.0/genia/tools_config/skills/grant_production_permissions.txt
--rw-r--r--   0        0        0      739 2023-07-31 07:03:28.818133 genia-0.3.0/genia/tools_config/skills/invoke_lambda_find_ec2_instances_without_label.txt
--rw-r--r--   0        0        0      551 2023-07-30 07:20:35.471657 genia-0.3.0/genia/tools_config/skills/revoke_production_permissions.txt
--rw-r--r--   0        0        0      822 2023-07-30 07:20:35.471792 genia-0.3.0/genia/tools_config/skills/skills_functions.json
--rw-r--r--   0        0        0      208 2023-07-31 12:24:50.543947 genia-0.3.0/genia/tools_config/skills/skills_tools.yaml
--rw-r--r--   0        0        0     8400 2023-07-31 12:24:50.544099 genia-0.3.0/genia/tools_config/skills/test.txt
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.529310 genia-0.3.0/genia/user_interface/__init__.py
--rw-r--r--   0        0        0      250 2023-07-25 19:10:06.529365 genia-0.3.0/genia/user_interface/shell_app.py
--rw-r--r--   0        0        0     4731 2023-07-27 11:43:39.313514 genia-0.3.0/genia/user_interface/slack_app.py
--rw-r--r--   0        0        0     1902 2023-08-03 15:28:15.356336 genia-0.3.0/genia/user_interface/streamlit_app.py
--rw-r--r--   0        0        0        0 2023-07-25 19:10:06.529543 genia-0.3.0/genia/utils/__init__.py
--rw-r--r--   0        0        0     1419 2023-08-03 19:56:04.332715 genia-0.3.0/genia/utils/utils.py
--rw-r--r--   0        0        0     1295 2023-08-03 20:50:06.367403 genia-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    18577 1970-01-01 00:00:00.000000 genia-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-04 09:33:44.476108 genia-0.4.0/LICENSE
+-rw-r--r--   0        0        0    16983 2023-08-04 09:33:44.476108 genia-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.476108 genia-0.4.0/genia/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.476108 genia-0.4.0/genia/agents/__init__.py
+-rw-r--r--   0        0        0     1390 2023-08-04 09:33:44.476108 genia-0.4.0/genia/agents/adhoc.py
+-rw-r--r--   0        0        0      149 2023-08-04 09:33:44.476108 genia-0.4.0/genia/agents/agent.py
+-rw-r--r--   0        0        0    10118 2023-08-04 09:33:44.476108 genia-0.4.0/genia/agents/chat.py
+-rw-r--r--   0        0        0    11173 2023-08-04 09:33:44.476108 genia-0.4.0/genia/conversation/llm_conversation.py
+-rw-r--r--   0        0        0     2633 2023-08-04 09:33:44.476108 genia-0.4.0/genia/conversation/llm_conversation_in_memory_repository.py
+-rw-r--r--   0        0        0      369 2023-08-04 09:33:44.476108 genia-0.4.0/genia/entry.py
+-rw-r--r--   0        0        0       39 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function/__init__.py
+-rw-r--r--   0        0        0      190 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function/llm_function.py
+-rw-r--r--   0        0        0    12462 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function/llm_function_repository.py
+-rw-r--r--   0        0        0     1071 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function/llm_functions_factory.py
+-rw-r--r--   0        0        0      743 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function/llm_skill_function.py
+-rw-r--r--   0        0        0     1543 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function/open_api_function.py
+-rw-r--r--   0        0        0     2041 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function/python_function.py
+-rw-r--r--   0        0        0      660 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function/url_function.py
+-rw-r--r--   0        0        0       44 2023-08-04 09:33:44.476108 genia-0.4.0/genia/llm_function_lookup_strategy/__init__.py
+-rw-r--r--   0        0        0     2731 2023-08-04 09:33:44.480108 genia-0.4.0/genia/llm_function_lookup_strategy/llm_function_lookup_strategy.py
+-rw-r--r--   0        0        0     2253 2023-08-04 09:33:44.480108 genia-0.4.0/genia/main.py
+-rw-r--r--   0        0        0     8360 2023-08-04 09:33:44.480108 genia-0.4.0/genia/openai_plugins/openai_plugins_repository.py
+-rw-r--r--   0        0        0     5868 2023-08-04 09:33:44.480108 genia-0.4.0/genia/settings/prompts.toml
+-rw-r--r--   0        0        0     1003 2023-08-04 09:33:44.480108 genia-0.4.0/genia/settings/settings.toml
+-rw-r--r--   0        0        0      299 2023-08-04 09:33:44.480108 genia-0.4.0/genia/settings_loader.py
+-rw-r--r--   0        0        0     6098 2023-08-04 09:33:44.480108 genia-0.4.0/genia/token_limiter/token_limiter_openai.py
+-rw-r--r--   0        0        0     2639 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tool_validators/llm_tool_validator.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/argo/__init__.py
+-rw-r--r--   0        0        0     5596 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/argo/argo_client.py
+-rw-r--r--   0        0        0      796 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/argo/workflow_template.json
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/__init__.py
+-rw-r--r--   0        0        0      506 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/aws_client.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/cloudtrail/__init__.py
+-rw-r--r--   0        0        0     2670 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/cloudtrail/aws_client_cloudtrail.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/ec2/__init__.py
+-rw-r--r--   0        0        0     2069 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/ec2/aws_client_ec2.py
+-rw-r--r--   0        0        0      461 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/ecr/aws_client_ecr.py
+-rw-r--r--   0        0        0     3851 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/ecr/repository_info_collector.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/ecs/__init__.py
+-rw-r--r--   0        0        0     1797 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/ecs/aws_client_ecs.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/events/__init__.py
+-rw-r--r--   0        0        0     4893 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/events/aws_client_events.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/iam/__init__.py
+-rw-r--r--   0        0        0     3641 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/iam/aws_client_iam.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/lambdas/__init__.py
+-rw-r--r--   0        0        0    16060 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/lambdas/aws_client_lambda.py
+-rw-r--r--   0        0        0      290 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/lambdas/docker/Dockerfile
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/lambdas/docker/__init__.py
+-rwxr-xr-x   0        0        0      125 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/lambdas/docker/docker-build.sh
+-rwxr-xr-x   0        0        0       97 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/lambdas/docker/entrypoint.sh
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/sqs/__init__.py
+-rw-r--r--   0        0        0     3775 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/aws_client/sqs/aws_client_sqs.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/github_client/__init__.py
+-rw-r--r--   0        0        0     3436 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/github_client/github_client.py
+-rw-r--r--   0        0        0      553 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/github_client/github_enriched_client.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/jenkins/__init__.py
+-rw-r--r--   0        0        0     1210 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/jenkins/jenkins_client.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/__init__.py
+-rw-r--r--   0        0        0     3659 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/cronjob.py
+-rw-r--r--   0        0        0    14598 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/deployment.py
+-rw-r--r--   0        0        0      941 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/events.py
+-rw-r--r--   0        0        0      726 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/global.py
+-rw-r--r--   0        0        0     5784 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/jobs.py
+-rw-r--r--   0        0        0      980 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/kubernetes_clients.py
+-rw-r--r--   0        0        0     1504 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/namespace.py
+-rw-r--r--   0        0        0     5262 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/pod.py
+-rw-r--r--   0        0        0      530 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/secret.py
+-rw-r--r--   0        0        0     1377 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/service.py
+-rw-r--r--   0        0        0     1843 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/kubernetes_client/utils.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/opa/__init__.py
+-rw-r--r--   0        0        0     1147 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/opa/opa.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/opa/policies/__init__.py
+-rw-r--r--   0        0        0      472 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/opa/policies/k8s_policies.rego
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/opa/policies/samples/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/opa/policies/samples/k8s/__init__.py
+-rw-r--r--   0        0        0      774 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/opa/policies/samples/k8s/not_defining_resource_limits.json
+-rw-r--r--   0        0        0      969 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/opa/policies/samples/k8s/running_containers_as_root.json
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/pagerduty_client/__init__.py
+-rw-r--r--   0        0        0     2490 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/pagerduty_client/pagerduty_client.py
+-rw-r--r--   0        0        0     3028 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/react.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/skills/__init__.py
+-rw-r--r--   0        0        0     1573 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/skills/skills_repository.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/slack/__init__.py
+-rw-r--r--   0        0        0      718 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools/slack/slack_client.py
+-rw-r--r--   0        0        0      238 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/core/aws/aws_functions.json
+-rw-r--r--   0        0        0      158 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/core/aws/aws_tools.yaml
+-rw-r--r--   0        0        0    34082 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/core/functions.json
+-rw-r--r--   0        0        0     9906 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/core/tools.yaml
+-rw-r--r--   0        0        0     3707 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/extended/README.md
+-rw-r--r--   0        0        0      452 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/extended/github/github_functions.json
+-rw-r--r--   0        0        0      193 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/extended/github/github_tools.yaml
+-rw-r--r--   0        0        0     1839 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/playground/playground_functions.json
+-rw-r--r--   0        0        0      491 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/playground/playground_tools.yaml
+-rw-r--r--   0        0        0      917 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/skills/calculate_rectangle_area.txt
+-rw-r--r--   0        0        0      593 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/skills/grant_production_permissions.txt
+-rw-r--r--   0        0        0      739 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/skills/invoke_lambda_find_ec2_instances_without_label.txt
+-rw-r--r--   0        0        0      551 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/skills/revoke_production_permissions.txt
+-rw-r--r--   0        0        0      822 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/skills/skills_functions.json
+-rw-r--r--   0        0        0      208 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/skills/skills_tools.yaml
+-rw-r--r--   0        0        0     8400 2023-08-04 09:33:44.480108 genia-0.4.0/genia/tools_config/skills/test.txt
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.480108 genia-0.4.0/genia/user_interface/__init__.py
+-rw-r--r--   0        0        0      250 2023-08-04 09:33:44.480108 genia-0.4.0/genia/user_interface/shell_app.py
+-rw-r--r--   0        0        0     4731 2023-08-04 09:33:44.484108 genia-0.4.0/genia/user_interface/slack_app.py
+-rw-r--r--   0        0        0     3965 2023-08-04 09:33:44.484108 genia-0.4.0/genia/user_interface/streamlit_app.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:33:44.484108 genia-0.4.0/genia/utils/__init__.py
+-rw-r--r--   0        0        0     1419 2023-08-04 09:33:44.484108 genia-0.4.0/genia/utils/utils.py
+-rw-r--r--   0        0        0     1295 2023-08-04 09:33:44.752116 genia-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    18609 1970-01-01 00:00:00.000000 genia-0.4.0/PKG-INFO
```

### Comparing `genia-0.3.0/LICENSE` & `genia-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/README.md` & `genia-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 
 <p align=center>
    <a href="https://genia.dev" target="_blank">
       <img src="./media/GeniA_wide_1.png"/>
    </a>
 </p>
 <br>
+<p>
 Imagine a ChatGPT integrated with your team's tools and APIs, capable of executing tasks and handling queries independently, contributing to time and energy efficiency.
-
+<br><br>
 GeniA is an AI assistant developed for engineering tasks. GeniA is a dynamic, intuitive tool capable of managing tasks in your team's Slack channel.
+</p>
 
 ## 📝 Table of Contents
 
 1. [🎉 Introduction](#introduction)
-   - 1.1 [🌟 Features](#features)
-   - 1.2 [🆚 Comparison to LLM](#comparison-to-llm)
-   - 1.3 [🔌 Supported Tools](#supported-tools)
-   - 1.4 [⚙️ Expanding GeniA's Toolbox](#expanding-genias-toolbox)
-   - 1.5 [🚀 Future Plans](#future-plans)
-   - 1.6. [🔒 Security](#security)
+   1. [🌟 Features](#features)
+   2. [🆚 Comparison to LLM](#comparison-to-llm)
+   3. [🔌 Supported Tools](#supported-tools)
+   4. [⚙️ Expanding GeniA's Toolbox](#expanding-genias-toolbox)
+   5. [🚀 Future Plans](#future-plans)
+   6. [🔒 Security
 2. [▶️ Getting started](#getting-started)
-   - 2.1 [🔧 Installation](#installation)
-   - 2.2 [ 📖 Developer Guide](#developer-guide)
-
-[🤝 Contributing](#contributing)    
-[📜 License](#license)    
-[📞 Contact](#contact)    
+   1. [🔧 Installation](#installation)
+   2. [ 📖 Developer Guide](#developer-guide)
+3. [🤝 Contributing](#contributing)
+4. [📜 License](#license)
+5. [📞 Contact](#contact)
 
 ## Introduction
 
-While ChatGPT and CoPilot have garnered significant attention for their ability to assist with writing new code, as software engineers, we understand that coding is merely one aspect of our daily responsibilities and AI present many additional opportunities to minimize bolier plate, time wasters and cross team dependencies.    
+While ChatGPT and CoPilot have garnered significant attention for their ability to assist with writing new code, as software engineers, we understand that coding is merely one aspect of our daily responsibilities and AI present many additional opportunities to minimize bolier plate, time wasters and cross team dependencies.
 
 **Under the hood** GeniA built upon the [function-calling capabilities offered by OpenAI](https://openai.com/blog/function-calling-and-other-api-updates). Azure OpenAI supported as well.
 
 GeniA requires OpenAI API Key, you can generate [here](https://platform.openai.com/account/api-keys)
 
 ### GeniA is 100% open source!
 
@@ -104,15 +105,14 @@
 
 However, with the advent of Language Learning Models (LLMs), Tools 3.0 pushes the boundary further, empowering everyone to write code using natural language. It signifies a shift from proprietary, restrictive design paradigms to a more open, innovative approach where the model assists in understanding and revising complex code snippets.
 
 Tools 3.0 negates the need for proprietary YAML files and vendor-specific domain languages (DSLs), urging users to rely on native code. Rather than waiting for vendor updates to fulfill requirements, users can now instruct LLMs to write code, create it themselves, or utilize the vast range of community-contributed tools.
 
 Remember, any class, method, or API available becomes a learning and application tool for GeniA. Tools 3.0 redefines coding, transforming it into an intuitive, flexible, and democratized process.
 
-
 ## Features
 
 GeniA's unique features include:
 
 1. **Production-Grade**: Engineered for real-world applications.
 2. **Collaborative assistant**: Designed to make the development process more interactive and enjoyable.
 3. **Proactively taking action**: building, coding, executing, summarizing. not just giving you a good advice.
@@ -212,38 +212,39 @@
 
 **We presently advise the integration of GeniA within a designated private channel, accessible exclusively to a whitelist of approved engineers.**
 
 We are actively developing Single Sign-On (SSO) and Role-Based Access Control (RBAC) features for GeniA. These enhancements are slated for release in the near future.
 
 ## Getting started
 
-The easiest way to play with GeniA is [Streamlit](https://streamlit.io/) app:
+The easiest way to get started with GeniA is [Streamlit](https://streamlit.io/) web app. Make sure you have `python3` & `pip3` installed, then run:
 
 ```
-pip install genia
+pip3 install streamlit genia
 ```
 
-Then you can run the streamlit web applciation by:
+Then you can run the streamlit web app by:
+
 ```
 genia
 ```
 
-You can play with GeniA also in terminal local mode. Once you done to play with it you can move to the collaborative mode as a Slack App Bot. For simplicity, we recommend running it locally using [Docker](#run-via-docker). If a local installation is desired, please refer to the [Installation](#installation) section.
+You can also play with GeniA in terminal using the local mode. Once you done to play with it you can move to the collaborative mode as a Slack App Bot. For simplicity, we recommend running it locally using [Docker](#run-via-docker). If a local installation is desired, please refer to the [Installation](#installation) section.
 
-When using Azure OpenAI, you need to configure also those environment variables:
+When using Azure OpenAI, you need to also configure those environment variables:
 
 ```
 OPENAI_API_DEPLOYMENT=
 OPENAI_API_TYPE="azure"
 OPENAI_API_BASE=https://<your-endpoint.openai.azure.com/
 OPENAI_API_VERSION="2023-07-01-preview"
 ```
 
 > **Note:**
-> GeniA using OpenAI, be mindful of cost implications and ensure you set usage limits. You can configure both soft and hard limits at the following URL: https://platform.openai.com/account/billing/limits.
+> GeniA uses OpenAI, be mindful of cost implications and ensure you set usage limits. You can configure both soft and hard limits at the following URL: https://platform.openai.com/account/billing/limits.
 
 By default, GeniA is set to use `gpt-3.5-turbo-0613`. We acknowledge that `gpt-4-0613` often delivers superior results, but have found the 3.5 version to be a more cost-effective choice.
 
 ## Installation
 
 ### Run in Slack App Bot
 
@@ -319,15 +320,14 @@
 ```
 poetry run slack
 ```
 
 ### Run in streamlit mode
 
 ```
-pip install streamlit
 poetry run streamlit
 ```
 
 ### Testing
 
 ```
 poetry run pytest tests
```

#### html2text {}

```diff
@@ -1,39 +1,41 @@
 ![CI](https://github.com/genia-dev/GeniA/actions/workflows/ci.yml/badge.svg) [!
 [License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://
 opensource.org/licenses/Apache-2.0)
                           [./media/GeniA_wide_1.png]
 
 Imagine a ChatGPT integrated with your team's tools and APIs, capable of
 executing tasks and handling queries independently, contributing to time and
-energy efficiency. GeniA is an AI assistant developed for engineering tasks.
-GeniA is a dynamic, intuitive tool capable of managing tasks in your team's
-Slack channel. ## ð Table of Contents 1. [ð Introduction](#introduction)
-- 1.1 [ð Features](#features) - 1.2 [ð Comparison to LLM](#comparison-to-
-llm) - 1.3 [ð Supported Tools](#supported-tools) - 1.4 [âï¸ Expanding
-GeniA's Toolbox](#expanding-genias-toolbox) - 1.5 [ð Future Plans](#future-
-plans) - 1.6. [ð Security](#security) 2. [â¶ï¸ Getting started](#getting-
-started) - 2.1 [ð§ Installation](#installation) - 2.2 [ ð Developer Guide]
-(#developer-guide) [ð¤ Contributing](#contributing) [ð License](#license)
-[ð Contact](#contact) ## Introduction While ChatGPT and CoPilot have
-garnered significant attention for their ability to assist with writing new
-code, as software engineers, we understand that coding is merely one aspect of
-our daily responsibilities and AI present many additional opportunities to
-minimize bolier plate, time wasters and cross team dependencies. **Under the
-hood** GeniA built upon the [function-calling capabilities offered by OpenAI]
-(https://openai.com/blog/function-calling-and-other-api-updates). Azure OpenAI
-supported as well. GeniA requires OpenAI API Key, you can generate [here]
-(https://platform.openai.com/account/api-keys) ### GeniA is 100% open source!
-Built with love by engineers for engineers, our goal is to help teams harness
-the power of LLMs to boost how fast you can go! ### GeniA is Production grade
-we have set ourselves the goal of building a production-grade software right
-off the bat. Now, you can start working with GeniA in production by installing
-the GeniA container, integrate it into your team's Slack channel, and let it
-land on its feet running. ### Imagine a virtual asisstant empowering you with:
-#### Research & Development Scenarios Deployment, troubleshooting, log
+energy efficiency.
+
+GeniA is an AI assistant developed for engineering tasks. GeniA is a dynamic,
+intuitive tool capable of managing tasks in your team's Slack channel.
+## ð Table of Contents 1. [ð Introduction](#introduction) 1. [ð
+Features](#features) 2. [ð Comparison to LLM](#comparison-to-llm) 3. [ð
+Supported Tools](#supported-tools) 4. [âï¸ Expanding GeniA's Toolbox]
+(#expanding-genias-toolbox) 5. [ð Future Plans](#future-plans) 6. [ð
+Security 2. [â¶ï¸ Getting started](#getting-started) 1. [ð§ Installation]
+(#installation) 2. [ ð Developer Guide](#developer-guide) 3. [ð¤
+Contributing](#contributing) 4. [ð License](#license) 5. [ð Contact]
+(#contact) ## Introduction While ChatGPT and CoPilot have garnered significant
+attention for their ability to assist with writing new code, as software
+engineers, we understand that coding is merely one aspect of our daily
+responsibilities and AI present many additional opportunities to minimize
+bolier plate, time wasters and cross team dependencies. **Under the hood**
+GeniA built upon the [function-calling capabilities offered by OpenAI](https://
+openai.com/blog/function-calling-and-other-api-updates). Azure OpenAI supported
+as well. GeniA requires OpenAI API Key, you can generate [here](https://
+platform.openai.com/account/api-keys) ### GeniA is 100% open source! Built with
+love by engineers for engineers, our goal is to help teams harness the power of
+LLMs to boost how fast you can go! ### GeniA is Production grade we have set
+ourselves the goal of building a production-grade software right off the bat.
+Now, you can start working with GeniA in production by installing the GeniA
+container, integrate it into your team's Slack channel, and let it land on its
+feet running. ### Imagine a virtual asisstant empowering you with: ####
+Research & Development Scenarios Deployment, troubleshooting, log
 summarization, build initiation, PR digesting * `Deploy your k8s-based service
 to staging/production using Argo` * `Investigate the cause of the last Argo
 deployment failure` * `Summarize the recent logs from your Node.js service` *
 `Initiate a new Jenkins build` * `Summarize GitHub pull request along with its
 content` #### FinOps Shift-Left Reporting on unused resources, optimising cloud
 expenditure. * `Generate a report detailing unutilized cloud resources per team
 and share it on Slack` * `Create a usage report for AWS ECR (Amazon Elastic
@@ -151,25 +153,27 @@
 On the subject of secrets management, the project currently utilizes
 environment variables, as defined in the [.env.template](.env.template) file.
 However, we are actively developing integrations with standard secrets store
 providers for improved security. **We presently advise the integration of GeniA
 within a designated private channel, accessible exclusively to a whitelist of
 approved engineers.** We are actively developing Single Sign-On (SSO) and Role-
 Based Access Control (RBAC) features for GeniA. These enhancements are slated
-for release in the near future. ## Getting started The easiest way to play with
-GeniA is [Streamlit](https://streamlit.io/) app: ``` pip install genia ``` Then
-you can run the streamlit web applciation by: ``` genia ``` You can play with
-GeniA also in terminal local mode. Once you done to play with it you can move
-to the collaborative mode as a Slack App Bot. For simplicity, we recommend
-running it locally using [Docker](#run-via-docker). If a local installation is
-desired, please refer to the [Installation](#installation) section. When using
-Azure OpenAI, you need to configure also those environment variables: ```
-OPENAI_API_DEPLOYMENT= OPENAI_API_TYPE="azure" OPENAI_API_BASE=https://
+for release in the near future. ## Getting started The easiest way to get
+started with GeniA is [Streamlit](https://streamlit.io/) web app. Make sure you
+have `python3` & `pip3` installed, then run: ``` pip3 install streamlit genia
+``` Then you can run the streamlit web app by: ``` genia ``` You can also play
+with GeniA in terminal using the local mode. Once you done to play with it you
+can move to the collaborative mode as a Slack App Bot. For simplicity, we
+recommend running it locally using [Docker](#run-via-docker). If a local
+installation is desired, please refer to the [Installation](#installation)
+section. When using Azure OpenAI, you need to also configure those environment
+variables: ``` OPENAI_API_DEPLOYMENT= OPENAI_API_TYPE="azure"
+OPENAI_API_BASE=https://
 openai.azure.com/ OPENAI_API_VERSION="2023-07-01-preview" ``` > **Note:** >
-GeniA using OpenAI, be mindful of cost implications and ensure you set usage
+GeniA uses OpenAI, be mindful of cost implications and ensure you set usage
 limits. You can configure both soft and hard limits at the following URL:
 https://platform.openai.com/account/billing/limits. By default, GeniA is set to
 use `gpt-3.5-turbo-0613`. We acknowledge that `gpt-4-0613` often delivers
 superior results, but have found the 3.5 version to be a more cost-effective
 choice. ## Installation ### Run in Slack App Bot #### Create Slack App Bot >
 **Note:** > > When it comes to [Choosing a protocol to connect to Slack](https:
 //api.slack.com/apis/connections), there are two primary options. In this
@@ -203,16 +207,16 @@
 mode ``` docker run -p 5001:5001 --env-file ./.env -it geniadev/genia:latest
 slack ``` ## Developer Guide ### Run GeniA from source :: Docker ``` git clone
 https://github.com/GeniA-dev/GeniA cd GeniA docker build -t geniadev/genia:
 latest . ``` Run via [Docker](#run-via-docker) ### Run GeniA from source ::
 Python #### Poetry install ``` curl -sSL https://install.python-poetry.org |
 python3 - ``` #### Run in local terminal mode ``` poetry run local ``` #### Run
 in slack app bot mode [First install the bot](#create-slack-app-bot) ``` poetry
-run slack ``` ### Run in streamlit mode ``` pip install streamlit poetry run
-streamlit ``` ### Testing ``` poetry run pytest tests ``` # Contributing
+run slack ``` ### Run in streamlit mode ``` poetry run streamlit ``` ###
+Testing ``` poetry run pytest tests ``` # Contributing
 ð©âð»âð¨âð» Fork GeniA repository, make your changes, and submit
 a pull request! We appreciate your contributions! ððð More details can
 be found [here](./CONTRIBUTING.md). # License Licensed under the Apache
 License, Version 2.0 (the "License"); you may not use this file except in
 compliance with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
 to in writing, software distributed under the License is distributed on an "AS
```

### Comparing `genia-0.3.0/genia/agents/adhoc.py` & `genia-0.4.0/genia/agents/adhoc.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/agents/chat.py` & `genia-0.4.0/genia/agents/chat.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/conversation/llm_conversation.py` & `genia-0.4.0/genia/conversation/llm_conversation.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/conversation/llm_conversation_in_memory_repository.py` & `genia-0.4.0/genia/conversation/llm_conversation_in_memory_repository.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/llm_function/llm_function_repository.py` & `genia-0.4.0/genia/llm_function/llm_function_repository.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/llm_function/llm_functions_factory.py` & `genia-0.4.0/genia/llm_function/llm_functions_factory.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/llm_function/llm_skill_function.py` & `genia-0.4.0/genia/llm_function/llm_skill_function.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/llm_function/open_api_function.py` & `genia-0.4.0/genia/llm_function/open_api_function.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/llm_function/python_function.py` & `genia-0.4.0/genia/llm_function/python_function.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/llm_function/url_function.py` & `genia-0.4.0/genia/llm_function/url_function.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/llm_function_lookup_strategy/llm_function_lookup_strategy.py` & `genia-0.4.0/genia/llm_function_lookup_strategy/llm_function_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/main.py` & `genia-0.4.0/genia/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import sys
 import threading
 from dotenv import load_dotenv
 from genia.user_interface.shell_app import ShellApp
 from genia.settings_loader import settings
 from genia.agents.chat import OpenAIChat
 
 from gunicorn.app.base import BaseApplication
```

### Comparing `genia-0.3.0/genia/openai_plugins/openai_plugins_repository.py` & `genia-0.4.0/genia/openai_plugins/openai_plugins_repository.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/settings/prompts.toml` & `genia-0.4.0/genia/settings/prompts.toml`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/settings/settings.toml` & `genia-0.4.0/genia/settings/settings.toml`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/token_limiter/token_limiter_openai.py` & `genia-0.4.0/genia/token_limiter/token_limiter_openai.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tool_validators/llm_tool_validator.py` & `genia-0.4.0/genia/tool_validators/llm_tool_validator.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/argo/argo_client.py` & `genia-0.4.0/genia/tools/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/argo/workflow_template.json` & `genia-0.4.0/genia/tools/argo/workflow_template.json`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/aws_client/cloudtrail/aws_client_cloudtrail.py` & `genia-0.4.0/genia/tools/aws_client/cloudtrail/aws_client_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/aws_client/ec2/aws_client_ec2.py` & `genia-0.4.0/genia/tools/aws_client/ec2/aws_client_ec2.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/aws_client/ecr/repository_info_collector.py` & `genia-0.4.0/genia/tools/aws_client/ecr/repository_info_collector.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/aws_client/ecs/aws_client_ecs.py` & `genia-0.4.0/genia/tools/aws_client/ecs/aws_client_ecs.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/aws_client/events/aws_client_events.py` & `genia-0.4.0/genia/tools/aws_client/events/aws_client_events.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/aws_client/iam/aws_client_iam.py` & `genia-0.4.0/genia/tools/aws_client/iam/aws_client_iam.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/aws_client/lambdas/aws_client_lambda.py` & `genia-0.4.0/genia/tools/aws_client/lambdas/aws_client_lambda.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/aws_client/sqs/aws_client_sqs.py` & `genia-0.4.0/genia/tools/aws_client/sqs/aws_client_sqs.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/github_client/github_client.py` & `genia-0.4.0/genia/tools/github_client/github_client.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/github_client/github_enriched_client.py` & `genia-0.4.0/genia/tools/github_client/github_enriched_client.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/jenkins/jenkins_client.py` & `genia-0.4.0/genia/tools/jenkins/jenkins_client.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/cronjob.py` & `genia-0.4.0/genia/tools/kubernetes_client/cronjob.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/deployment.py` & `genia-0.4.0/genia/tools/kubernetes_client/deployment.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/events.py` & `genia-0.4.0/genia/tools/kubernetes_client/events.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/global.py` & `genia-0.4.0/genia/tools/kubernetes_client/global.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/jobs.py` & `genia-0.4.0/genia/tools/kubernetes_client/jobs.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/kubernetes_clients.py` & `genia-0.4.0/genia/tools/kubernetes_client/kubernetes_clients.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/namespace.py` & `genia-0.4.0/genia/tools/kubernetes_client/namespace.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/pod.py` & `genia-0.4.0/genia/tools/kubernetes_client/pod.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/secret.py` & `genia-0.4.0/genia/tools/kubernetes_client/secret.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/service.py` & `genia-0.4.0/genia/tools/kubernetes_client/service.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/kubernetes_client/utils.py` & `genia-0.4.0/genia/tools/kubernetes_client/utils.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/opa/opa.py` & `genia-0.4.0/genia/tools/opa/opa.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/opa/policies/samples/k8s/not_defining_resource_limits.json` & `genia-0.4.0/genia/tools/opa/policies/samples/k8s/not_defining_resource_limits.json`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/opa/policies/samples/k8s/running_containers_as_root.json` & `genia-0.4.0/genia/tools/opa/policies/samples/k8s/running_containers_as_root.json`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/pagerduty_client/pagerduty_client.py` & `genia-0.4.0/genia/tools/pagerduty_client/pagerduty_client.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/react.py` & `genia-0.4.0/genia/tools/react.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/skills/skills_repository.py` & `genia-0.4.0/genia/tools/skills/skills_repository.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools/slack/slack_client.py` & `genia-0.4.0/genia/tools/slack/slack_client.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/core/functions.json` & `genia-0.4.0/genia/tools_config/core/functions.json`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/core/tools.yaml` & `genia-0.4.0/genia/tools_config/core/tools.yaml`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/extended/README.md` & `genia-0.4.0/genia/tools_config/extended/README.md`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/playground/playground_functions.json` & `genia-0.4.0/genia/tools_config/playground/playground_functions.json`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/skills/calculate_rectangle_area.txt` & `genia-0.4.0/genia/tools_config/skills/calculate_rectangle_area.txt`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/skills/grant_production_permissions.txt` & `genia-0.4.0/genia/tools_config/skills/grant_production_permissions.txt`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/skills/invoke_lambda_find_ec2_instances_without_label.txt` & `genia-0.4.0/genia/tools_config/skills/invoke_lambda_find_ec2_instances_without_label.txt`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/skills/revoke_production_permissions.txt` & `genia-0.4.0/genia/tools_config/skills/revoke_production_permissions.txt`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/skills/skills_functions.json` & `genia-0.4.0/genia/tools_config/skills/skills_functions.json`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/tools_config/skills/test.txt` & `genia-0.4.0/genia/tools_config/skills/test.txt`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/user_interface/slack_app.py` & `genia-0.4.0/genia/user_interface/slack_app.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/genia/utils/utils.py` & `genia-0.4.0/genia/utils/utils.py`

 * *Files identical despite different names*

### Comparing `genia-0.3.0/pyproject.toml` & `genia-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "genia"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Uri Shamay <cmpxchg16@gmail.com>", "Shlomi Shemesh <shlomosh@gmail.com>"]
 readme = "README.md"
 packages = [{include = "genia"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `genia-0.3.0/PKG-INFO` & `genia-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genia
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Uri Shamay
 Author-email: cmpxchg16@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (==4.12.2)
@@ -48,38 +48,39 @@
 
 <p align=center>
    <a href="https://genia.dev" target="_blank">
       <img src="./media/GeniA_wide_1.png"/>
    </a>
 </p>
 <br>
+<p>
 Imagine a ChatGPT integrated with your team's tools and APIs, capable of executing tasks and handling queries independently, contributing to time and energy efficiency.
-
+<br><br>
 GeniA is an AI assistant developed for engineering tasks. GeniA is a dynamic, intuitive tool capable of managing tasks in your team's Slack channel.
+</p>
 
 ## 📝 Table of Contents
 
 1. [🎉 Introduction](#introduction)
-   - 1.1 [🌟 Features](#features)
-   - 1.2 [🆚 Comparison to LLM](#comparison-to-llm)
-   - 1.3 [🔌 Supported Tools](#supported-tools)
-   - 1.4 [⚙️ Expanding GeniA's Toolbox](#expanding-genias-toolbox)
-   - 1.5 [🚀 Future Plans](#future-plans)
-   - 1.6. [🔒 Security](#security)
+   1. [🌟 Features](#features)
+   2. [🆚 Comparison to LLM](#comparison-to-llm)
+   3. [🔌 Supported Tools](#supported-tools)
+   4. [⚙️ Expanding GeniA's Toolbox](#expanding-genias-toolbox)
+   5. [🚀 Future Plans](#future-plans)
+   6. [🔒 Security
 2. [▶️ Getting started](#getting-started)
-   - 2.1 [🔧 Installation](#installation)
-   - 2.2 [ 📖 Developer Guide](#developer-guide)
-
-[🤝 Contributing](#contributing)    
-[📜 License](#license)    
-[📞 Contact](#contact)    
+   1. [🔧 Installation](#installation)
+   2. [ 📖 Developer Guide](#developer-guide)
+3. [🤝 Contributing](#contributing)
+4. [📜 License](#license)
+5. [📞 Contact](#contact)
 
 ## Introduction
 
-While ChatGPT and CoPilot have garnered significant attention for their ability to assist with writing new code, as software engineers, we understand that coding is merely one aspect of our daily responsibilities and AI present many additional opportunities to minimize bolier plate, time wasters and cross team dependencies.    
+While ChatGPT and CoPilot have garnered significant attention for their ability to assist with writing new code, as software engineers, we understand that coding is merely one aspect of our daily responsibilities and AI present many additional opportunities to minimize bolier plate, time wasters and cross team dependencies.
 
 **Under the hood** GeniA built upon the [function-calling capabilities offered by OpenAI](https://openai.com/blog/function-calling-and-other-api-updates). Azure OpenAI supported as well.
 
 GeniA requires OpenAI API Key, you can generate [here](https://platform.openai.com/account/api-keys)
 
 ### GeniA is 100% open source!
 
@@ -149,15 +150,14 @@
 
 However, with the advent of Language Learning Models (LLMs), Tools 3.0 pushes the boundary further, empowering everyone to write code using natural language. It signifies a shift from proprietary, restrictive design paradigms to a more open, innovative approach where the model assists in understanding and revising complex code snippets.
 
 Tools 3.0 negates the need for proprietary YAML files and vendor-specific domain languages (DSLs), urging users to rely on native code. Rather than waiting for vendor updates to fulfill requirements, users can now instruct LLMs to write code, create it themselves, or utilize the vast range of community-contributed tools.
 
 Remember, any class, method, or API available becomes a learning and application tool for GeniA. Tools 3.0 redefines coding, transforming it into an intuitive, flexible, and democratized process.
 
-
 ## Features
 
 GeniA's unique features include:
 
 1. **Production-Grade**: Engineered for real-world applications.
 2. **Collaborative assistant**: Designed to make the development process more interactive and enjoyable.
 3. **Proactively taking action**: building, coding, executing, summarizing. not just giving you a good advice.
@@ -257,38 +257,39 @@
 
 **We presently advise the integration of GeniA within a designated private channel, accessible exclusively to a whitelist of approved engineers.**
 
 We are actively developing Single Sign-On (SSO) and Role-Based Access Control (RBAC) features for GeniA. These enhancements are slated for release in the near future.
 
 ## Getting started
 
-The easiest way to play with GeniA is [Streamlit](https://streamlit.io/) app:
+The easiest way to get started with GeniA is [Streamlit](https://streamlit.io/) web app. Make sure you have `python3` & `pip3` installed, then run:
 
 ```
-pip install genia
+pip3 install streamlit genia
 ```
 
-Then you can run the streamlit web applciation by:
+Then you can run the streamlit web app by:
+
 ```
 genia
 ```
 
-You can play with GeniA also in terminal local mode. Once you done to play with it you can move to the collaborative mode as a Slack App Bot. For simplicity, we recommend running it locally using [Docker](#run-via-docker). If a local installation is desired, please refer to the [Installation](#installation) section.
+You can also play with GeniA in terminal using the local mode. Once you done to play with it you can move to the collaborative mode as a Slack App Bot. For simplicity, we recommend running it locally using [Docker](#run-via-docker). If a local installation is desired, please refer to the [Installation](#installation) section.
 
-When using Azure OpenAI, you need to configure also those environment variables:
+When using Azure OpenAI, you need to also configure those environment variables:
 
 ```
 OPENAI_API_DEPLOYMENT=
 OPENAI_API_TYPE="azure"
 OPENAI_API_BASE=https://<your-endpoint.openai.azure.com/
 OPENAI_API_VERSION="2023-07-01-preview"
 ```
 
 > **Note:**
-> GeniA using OpenAI, be mindful of cost implications and ensure you set usage limits. You can configure both soft and hard limits at the following URL: https://platform.openai.com/account/billing/limits.
+> GeniA uses OpenAI, be mindful of cost implications and ensure you set usage limits. You can configure both soft and hard limits at the following URL: https://platform.openai.com/account/billing/limits.
 
 By default, GeniA is set to use `gpt-3.5-turbo-0613`. We acknowledge that `gpt-4-0613` often delivers superior results, but have found the 3.5 version to be a more cost-effective choice.
 
 ## Installation
 
 ### Run in Slack App Bot
 
@@ -364,15 +365,14 @@
 ```
 poetry run slack
 ```
 
 ### Run in streamlit mode
 
 ```
-pip install streamlit
 poetry run streamlit
 ```
 
 ### Testing
 
 ```
 poetry run pytest tests
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: genia Version: 0.3.0 Summary: Author: Uri Shamay
+Metadata-Version: 2.1 Name: genia Version: 0.4.0 Summary: Author: Uri Shamay
 Author-email: cmpxchg16@gmail.com Requires-Python: >=3.11,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.11 Requires-Dist: beautifulsoup4 (==4.12.2) Requires-Dist: boto3
 (==1.26.165) Requires-Dist: bravado (>=11.0.3,<12.0.0) Requires-Dist: docker
 (>=6.1.3,<7.0.0) Requires-Dist: dynaconf (>=3.1.12,<4.0.0) Requires-Dist:
 faiss-cpu (==1.7.4) Requires-Dist: flask (>=2.3.2,<3.0.0) Requires-Dist: gcloud
 (>=0.18.3,<0.19.0) Requires-Dist: google-search-results (==2.4.2) Requires-
@@ -23,39 +23,41 @@
 genia-dev/GeniA/actions/workflows/ci.yml/badge.svg) [![License](https://
 img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/
 licenses/Apache-2.0)
                           [./media/GeniA_wide_1.png]
 
 Imagine a ChatGPT integrated with your team's tools and APIs, capable of
 executing tasks and handling queries independently, contributing to time and
-energy efficiency. GeniA is an AI assistant developed for engineering tasks.
-GeniA is a dynamic, intuitive tool capable of managing tasks in your team's
-Slack channel. ## ð Table of Contents 1. [ð Introduction](#introduction)
-- 1.1 [ð Features](#features) - 1.2 [ð Comparison to LLM](#comparison-to-
-llm) - 1.3 [ð Supported Tools](#supported-tools) - 1.4 [âï¸ Expanding
-GeniA's Toolbox](#expanding-genias-toolbox) - 1.5 [ð Future Plans](#future-
-plans) - 1.6. [ð Security](#security) 2. [â¶ï¸ Getting started](#getting-
-started) - 2.1 [ð§ Installation](#installation) - 2.2 [ ð Developer Guide]
-(#developer-guide) [ð¤ Contributing](#contributing) [ð License](#license)
-[ð Contact](#contact) ## Introduction While ChatGPT and CoPilot have
-garnered significant attention for their ability to assist with writing new
-code, as software engineers, we understand that coding is merely one aspect of
-our daily responsibilities and AI present many additional opportunities to
-minimize bolier plate, time wasters and cross team dependencies. **Under the
-hood** GeniA built upon the [function-calling capabilities offered by OpenAI]
-(https://openai.com/blog/function-calling-and-other-api-updates). Azure OpenAI
-supported as well. GeniA requires OpenAI API Key, you can generate [here]
-(https://platform.openai.com/account/api-keys) ### GeniA is 100% open source!
-Built with love by engineers for engineers, our goal is to help teams harness
-the power of LLMs to boost how fast you can go! ### GeniA is Production grade
-we have set ourselves the goal of building a production-grade software right
-off the bat. Now, you can start working with GeniA in production by installing
-the GeniA container, integrate it into your team's Slack channel, and let it
-land on its feet running. ### Imagine a virtual asisstant empowering you with:
-#### Research & Development Scenarios Deployment, troubleshooting, log
+energy efficiency.
+
+GeniA is an AI assistant developed for engineering tasks. GeniA is a dynamic,
+intuitive tool capable of managing tasks in your team's Slack channel.
+## ð Table of Contents 1. [ð Introduction](#introduction) 1. [ð
+Features](#features) 2. [ð Comparison to LLM](#comparison-to-llm) 3. [ð
+Supported Tools](#supported-tools) 4. [âï¸ Expanding GeniA's Toolbox]
+(#expanding-genias-toolbox) 5. [ð Future Plans](#future-plans) 6. [ð
+Security 2. [â¶ï¸ Getting started](#getting-started) 1. [ð§ Installation]
+(#installation) 2. [ ð Developer Guide](#developer-guide) 3. [ð¤
+Contributing](#contributing) 4. [ð License](#license) 5. [ð Contact]
+(#contact) ## Introduction While ChatGPT and CoPilot have garnered significant
+attention for their ability to assist with writing new code, as software
+engineers, we understand that coding is merely one aspect of our daily
+responsibilities and AI present many additional opportunities to minimize
+bolier plate, time wasters and cross team dependencies. **Under the hood**
+GeniA built upon the [function-calling capabilities offered by OpenAI](https://
+openai.com/blog/function-calling-and-other-api-updates). Azure OpenAI supported
+as well. GeniA requires OpenAI API Key, you can generate [here](https://
+platform.openai.com/account/api-keys) ### GeniA is 100% open source! Built with
+love by engineers for engineers, our goal is to help teams harness the power of
+LLMs to boost how fast you can go! ### GeniA is Production grade we have set
+ourselves the goal of building a production-grade software right off the bat.
+Now, you can start working with GeniA in production by installing the GeniA
+container, integrate it into your team's Slack channel, and let it land on its
+feet running. ### Imagine a virtual asisstant empowering you with: ####
+Research & Development Scenarios Deployment, troubleshooting, log
 summarization, build initiation, PR digesting * `Deploy your k8s-based service
 to staging/production using Argo` * `Investigate the cause of the last Argo
 deployment failure` * `Summarize the recent logs from your Node.js service` *
 `Initiate a new Jenkins build` * `Summarize GitHub pull request along with its
 content` #### FinOps Shift-Left Reporting on unused resources, optimising cloud
 expenditure. * `Generate a report detailing unutilized cloud resources per team
 and share it on Slack` * `Create a usage report for AWS ECR (Amazon Elastic
@@ -173,25 +175,27 @@
 On the subject of secrets management, the project currently utilizes
 environment variables, as defined in the [.env.template](.env.template) file.
 However, we are actively developing integrations with standard secrets store
 providers for improved security. **We presently advise the integration of GeniA
 within a designated private channel, accessible exclusively to a whitelist of
 approved engineers.** We are actively developing Single Sign-On (SSO) and Role-
 Based Access Control (RBAC) features for GeniA. These enhancements are slated
-for release in the near future. ## Getting started The easiest way to play with
-GeniA is [Streamlit](https://streamlit.io/) app: ``` pip install genia ``` Then
-you can run the streamlit web applciation by: ``` genia ``` You can play with
-GeniA also in terminal local mode. Once you done to play with it you can move
-to the collaborative mode as a Slack App Bot. For simplicity, we recommend
-running it locally using [Docker](#run-via-docker). If a local installation is
-desired, please refer to the [Installation](#installation) section. When using
-Azure OpenAI, you need to configure also those environment variables: ```
-OPENAI_API_DEPLOYMENT= OPENAI_API_TYPE="azure" OPENAI_API_BASE=https://
+for release in the near future. ## Getting started The easiest way to get
+started with GeniA is [Streamlit](https://streamlit.io/) web app. Make sure you
+have `python3` & `pip3` installed, then run: ``` pip3 install streamlit genia
+``` Then you can run the streamlit web app by: ``` genia ``` You can also play
+with GeniA in terminal using the local mode. Once you done to play with it you
+can move to the collaborative mode as a Slack App Bot. For simplicity, we
+recommend running it locally using [Docker](#run-via-docker). If a local
+installation is desired, please refer to the [Installation](#installation)
+section. When using Azure OpenAI, you need to also configure those environment
+variables: ``` OPENAI_API_DEPLOYMENT= OPENAI_API_TYPE="azure"
+OPENAI_API_BASE=https://
 openai.azure.com/ OPENAI_API_VERSION="2023-07-01-preview" ``` > **Note:** >
-GeniA using OpenAI, be mindful of cost implications and ensure you set usage
+GeniA uses OpenAI, be mindful of cost implications and ensure you set usage
 limits. You can configure both soft and hard limits at the following URL:
 https://platform.openai.com/account/billing/limits. By default, GeniA is set to
 use `gpt-3.5-turbo-0613`. We acknowledge that `gpt-4-0613` often delivers
 superior results, but have found the 3.5 version to be a more cost-effective
 choice. ## Installation ### Run in Slack App Bot #### Create Slack App Bot >
 **Note:** > > When it comes to [Choosing a protocol to connect to Slack](https:
 //api.slack.com/apis/connections), there are two primary options. In this
@@ -225,16 +229,16 @@
 mode ``` docker run -p 5001:5001 --env-file ./.env -it geniadev/genia:latest
 slack ``` ## Developer Guide ### Run GeniA from source :: Docker ``` git clone
 https://github.com/GeniA-dev/GeniA cd GeniA docker build -t geniadev/genia:
 latest . ``` Run via [Docker](#run-via-docker) ### Run GeniA from source ::
 Python #### Poetry install ``` curl -sSL https://install.python-poetry.org |
 python3 - ``` #### Run in local terminal mode ``` poetry run local ``` #### Run
 in slack app bot mode [First install the bot](#create-slack-app-bot) ``` poetry
-run slack ``` ### Run in streamlit mode ``` pip install streamlit poetry run
-streamlit ``` ### Testing ``` poetry run pytest tests ``` # Contributing
+run slack ``` ### Run in streamlit mode ``` poetry run streamlit ``` ###
+Testing ``` poetry run pytest tests ``` # Contributing
 ð©âð»âð¨âð» Fork GeniA repository, make your changes, and submit
 a pull request! We appreciate your contributions! ððð More details can
 be found [here](./CONTRIBUTING.md). # License Licensed under the Apache
 License, Version 2.0 (the "License"); you may not use this file except in
 compliance with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
 to in writing, software distributed under the License is distributed on an "AS
```

