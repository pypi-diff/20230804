# Comparing `tmp/truss-0.5.3.tar.gz` & `tmp/truss-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.5.3.tar", max compression
+gzip compressed data, was "truss-0.5.4.tar", max compression
```

## Comparing `truss-0.5.3.tar` & `truss-0.5.4.tar`

### file list

```diff
@@ -1,222 +1,227 @@
--rw-r--r--   0        0        0     5483 2023-07-31 20:34:42.276205 truss-0.5.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2418 2023-07-31 20:34:42.276205 truss-0.5.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-07-31 20:34:42.276205 truss-0.5.3/LICENSE
--rw-r--r--   0        0        0     3518 2023-07-31 20:34:42.276205 truss-0.5.3/README.md
--rw-r--r--   0        0        0      933 2023-07-31 20:34:42.276205 truss-0.5.3/context_builder.Dockerfile
--rw-r--r--   0        0        0     2546 2023-07-31 20:34:42.388206 truss-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      330 2023-07-31 20:34:42.388206 truss-0.5.3/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-07-31 20:34:42.388206 truss-0.5.3/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-07-31 20:34:42.388206 truss-0.5.3/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-07-31 20:34:42.388206 truss-0.5.3/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13363 2023-07-31 20:34:42.388206 truss-0.5.3/truss/build.py
--rw-r--r--   0        0        0       51 2023-07-31 20:34:42.388206 truss-0.5.3/truss/cli/__init__.py
--rw-r--r--   0        0        0    11384 2023-07-31 20:34:42.388206 truss-0.5.3/truss/cli/cli.py
--rw-r--r--   0        0        0     1015 2023-07-31 20:34:42.388206 truss-0.5.3/truss/cli/create.py
--rw-r--r--   0        0        0     2873 2023-07-31 20:34:42.388206 truss-0.5.3/truss/constants.py
--rw-r--r--   0        0        0      338 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/cache_warmer.py
--rw-r--r--   0        0        0     1294 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     8321 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4684 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1893 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2120 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     1072 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/truss_file_syncer.py
--rw-r--r--   0        0        0     5801 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-07-31 20:34:42.388206 truss-0.5.3/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-07-31 20:34:42.388206 truss-0.5.3/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-07-31 20:34:42.388206 truss-0.5.3/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-07-31 20:34:42.388206 truss-0.5.3/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-07-31 20:34:42.388206 truss-0.5.3/truss/errors.py
--rw-r--r--   0        0        0      824 2023-07-31 20:34:42.388206 truss-0.5.3/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-07-31 20:34:42.388206 truss-0.5.3/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1230 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2403 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1225 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     5425 2023-07-31 20:34:42.388206 truss-0.5.3/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-07-31 20:34:42.388206 truss-0.5.3/truss/notebook.py
--rw-r--r--   0        0        0    15420 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      139 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/constants.py
--rw-r--r--   0        0        0      774 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/hash.py
--rw-r--r--   0        0        0     2930 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/local_truss_patch_applier.py
--rw-r--r--   0        0        0      468 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/signature.py
--rw-r--r--   0        0        0     3075 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/truss_dir_patch_applier.py
--rw-r--r--   0        0        0      937 2023-07-31 20:34:42.388206 truss-0.5.3/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-07-31 20:34:42.388206 truss-0.5.3/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-07-31 20:34:42.388206 truss-0.5.3/truss/readme_generator.py
--rw-r--r--   0        0        0      176 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/__init__.py
--rw-r--r--   0        0        0     4919 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/api.py
--rw-r--r--   0        0        0      752 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/auth.py
--rw-r--r--   0        0        0     3616 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/core.py
--rw-r--r--   0        0        0      943 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/error.py
--rw-r--r--   0        0        0     4741 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/remote.py
--rw-r--r--   0        0        0     1156 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/service.py
--rw-r--r--   0        0        0     2001 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/utils/tar.py
--rw-r--r--   0        0        0      985 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/baseten/utils/transfer.py
--rw-r--r--   0        0        0     1407 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/remote_cli.py
--rw-r--r--   0        0        0     4219 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/remote_factory.py
--rw-r--r--   0        0        0     5970 2023-07-31 20:34:42.388206 truss-0.5.3/truss/remote/truss_remote.py
--rw-r--r--   0        0        0     2482 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/__init__.py
--rw-r--r--   0        0        0     1967 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     3819 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     5103 2023-07-31 20:34:42.388206 truss-0.5.3/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     6317 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     4026 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2652 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0      998 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/__init__.py
--rw-r--r--   0        0        0     1842 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
--rw-r--r--   0        0        0     7386 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
--rw-r--r--   0        0        0      551 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
--rw-r--r--   0        0        0      208 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/truss_patch/system_packages.py
--rw-r--r--   0        0        0     5930 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     2319 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      144 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     2382 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     2340 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/termination_handler_middleware.py
--rw-r--r--   0        0        0    12328 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      727 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0    11624 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      274 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     3279 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/logging.py
--rw-r--r--   0        0        0     1430 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0     3318 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/serialization.py
--rw-r--r--   0        0        0     1863 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/shared/util.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0      521 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/tgi/proxy.conf
--rw-r--r--   0        0        0      491 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/tgi/supervisord.conf.jinja
--rw-r--r--   0        0        0      586 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/tgi/tgi.Dockerfile.jinja
--rw-r--r--   0        0        0     3400 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-07-31 20:34:42.392206 truss-0.5.3/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0      739 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-07-31 20:34:42.392206 truss-0.5.3/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1550 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0      669 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0      739 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_async_truss/config.yaml
--rw-r--r--   0        0        0      646 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_async_truss/model/model.py
--rw-r--r--   0        0        0       34 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_concurrency_truss/config.yaml
--rw-r--r--   0        0        0      547 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_concurrency_truss/model/model.py
--rw-r--r--   0        0        0      739 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_streaming_async_generator_truss/config.yaml
--rw-r--r--   0        0        0      521 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_streaming_async_generator_truss/model/model.py
--rw-r--r--   0        0        0      773 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_streaming_truss/config.yaml
--rw-r--r--   0        0        0      568 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_streaming_truss/model/model.py
--rw-r--r--   0        0        0      669 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        6 2023-07-31 20:34:42.396206 truss-0.5.3/truss/test_data/test_truss/packages/test_package/test.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/__init__.py
--rw-r--r--   0        0        0    22226 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/conftest.py
--rw-r--r--   0        0        0     1255 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    18726 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0     1929 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_truss_dir_patch_applier.py
--rw-r--r--   0        0        0      273 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0     2073 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/baseten/test_api.py
--rw-r--r--   0        0        0      580 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/baseten/test_auth.py
--rw-r--r--   0        0        0      835 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/baseten/test_core.py
--rw-r--r--   0        0        0     4316 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/test_remote_factory.py
--rw-r--r--   0        0        0     2394 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/remote/test_truss_remote.py
--rw-r--r--   0        0        0    10415 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     6081 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
--rw-r--r--   0        0        0      964 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
--rw-r--r--   0        0        0     7513 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0     8326 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/control/control/test_server_integration.py
--rw-r--r--   0        0        0     1560 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/core/server/common/test_truss_server.py
--rw-r--r--   0        0        0      821 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2605 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/server/common/test_termination_handler_middleware.py
--rw-r--r--   0        0        0     2252 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/test_build.py
--rw-r--r--   0        0        0     8657 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-07-31 20:34:42.396206 truss-0.5.3/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0    14982 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_control_truss_patching.py
--rw-r--r--   0        0        0      517 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_docker.py
--rw-r--r--   0        0        0    12242 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    30057 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0     1865 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/test_validation.py
--rw-r--r--   0        0        0     4974 2023-07-31 20:34:42.400206 truss-0.5.3/truss/tests/util/test_path.py
--rw-r--r--   0        0        0    15932 2023-07-31 20:34:42.400206 truss-0.5.3/truss/truss_config.py
--rw-r--r--   0        0        0     2698 2023-07-31 20:34:42.400206 truss-0.5.3/truss/truss_gatherer.py
--rw-r--r--   0        0        0    41143 2023-07-31 20:34:42.400206 truss-0.5.3/truss/truss_handle.py
--rw-r--r--   0        0        0     5671 2023-07-31 20:34:42.400206 truss-0.5.3/truss/truss_spec.py
--rw-r--r--   0        0        0     2782 2023-07-31 20:34:42.400206 truss-0.5.3/truss/types.py
--rw-r--r--   0        0        0     3121 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/.truss_ignore
--rw-r--r--   0        0        0      379 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/data_structures.py
--rw-r--r--   0        0        0     2552 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/download.py
--rw-r--r--   0        0        0      553 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/jinja.py
--rw-r--r--   0        0        0     6040 2023-07-31 20:34:42.400206 truss-0.5.3/truss/util/path.py
--rw-r--r--   0        0        0     2736 2023-07-31 20:34:42.400206 truss-0.5.3/truss/validation.py
--rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 truss-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-08-03 21:57:44.634620 truss-0.5.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2418 2023-08-03 21:57:44.634620 truss-0.5.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-08-03 21:57:44.634620 truss-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3518 2023-08-03 21:57:44.634620 truss-0.5.4/README.md
+-rw-r--r--   0        0        0      933 2023-08-03 21:57:44.634620 truss-0.5.4/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2546 2023-08-03 21:57:44.714620 truss-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-08-03 21:57:44.714620 truss-0.5.4/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-08-03 21:57:44.714620 truss-0.5.4/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-08-03 21:57:44.714620 truss-0.5.4/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-08-03 21:57:44.714620 truss-0.5.4/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13363 2023-08-03 21:57:44.714620 truss-0.5.4/truss/build.py
+-rw-r--r--   0        0        0       51 2023-08-03 21:57:44.714620 truss-0.5.4/truss/cli/__init__.py
+-rw-r--r--   0        0        0    11384 2023-08-03 21:57:44.714620 truss-0.5.4/truss/cli/cli.py
+-rw-r--r--   0        0        0     1251 2023-08-03 21:57:44.714620 truss-0.5.4/truss/cli/create.py
+-rw-r--r--   0        0        0     2873 2023-08-03 21:57:44.714620 truss-0.5.4/truss/constants.py
+-rw-r--r--   0        0        0     1065 2023-08-03 21:57:44.714620 truss-0.5.4/truss/contexts/image_builder/cache_warmer.py
+-rw-r--r--   0        0        0     1294 2023-08-03 21:57:44.714620 truss-0.5.4/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0    10455 2023-08-03 21:57:44.714620 truss-0.5.4/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-08-03 21:57:44.714620 truss-0.5.4/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1893 2023-08-03 21:57:44.714620 truss-0.5.4/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2120 2023-08-03 21:57:44.718621 truss-0.5.4/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-08-03 21:57:44.718621 truss-0.5.4/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-08-03 21:57:44.718621 truss-0.5.4/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     1072 2023-08-03 21:57:44.718621 truss-0.5.4/truss/contexts/local_loader/truss_file_syncer.py
+-rw-r--r--   0        0        0     5801 2023-08-03 21:57:44.718621 truss-0.5.4/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-08-03 21:57:44.718621 truss-0.5.4/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-08-03 21:57:44.718621 truss-0.5.4/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-08-03 21:57:44.718621 truss-0.5.4/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-08-03 21:57:44.718621 truss-0.5.4/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-08-03 21:57:44.718621 truss-0.5.4/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-08-03 21:57:44.718621 truss-0.5.4/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-08-03 21:57:44.718621 truss-0.5.4/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-08-03 21:57:44.718621 truss-0.5.4/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1230 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2403 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1225 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     5425 2023-08-03 21:57:44.718621 truss-0.5.4/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-08-03 21:57:44.718621 truss-0.5.4/truss/notebook.py
+-rw-r--r--   0        0        0    15420 2023-08-03 21:57:44.718621 truss-0.5.4/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      139 2023-08-03 21:57:44.718621 truss-0.5.4/truss/patch/constants.py
+-rw-r--r--   0        0        0      774 2023-08-03 21:57:44.718621 truss-0.5.4/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-08-03 21:57:44.718621 truss-0.5.4/truss/patch/hash.py
+-rw-r--r--   0        0        0     2930 2023-08-03 21:57:44.718621 truss-0.5.4/truss/patch/local_truss_patch_applier.py
+-rw-r--r--   0        0        0      468 2023-08-03 21:57:44.718621 truss-0.5.4/truss/patch/signature.py
+-rw-r--r--   0        0        0     3075 2023-08-03 21:57:44.718621 truss-0.5.4/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      937 2023-08-03 21:57:44.718621 truss-0.5.4/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-08-03 21:57:44.718621 truss-0.5.4/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-08-03 21:57:44.718621 truss-0.5.4/truss/readme_generator.py
+-rw-r--r--   0        0        0      176 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/__init__.py
+-rw-r--r--   0        0        0     4919 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/api.py
+-rw-r--r--   0        0        0      752 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/auth.py
+-rw-r--r--   0        0        0     3616 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/core.py
+-rw-r--r--   0        0        0      943 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/error.py
+-rw-r--r--   0        0        0     4741 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/remote.py
+-rw-r--r--   0        0        0     1156 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/service.py
+-rw-r--r--   0        0        0     2001 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/utils/tar.py
+-rw-r--r--   0        0        0      985 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/baseten/utils/transfer.py
+-rw-r--r--   0        0        0     1407 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/remote_cli.py
+-rw-r--r--   0        0        0     4219 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/remote_factory.py
+-rw-r--r--   0        0        0     5970 2023-08-03 21:57:44.718621 truss-0.5.4/truss/remote/truss_remote.py
+-rw-r--r--   0        0        0     2482 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1967 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     3819 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     5103 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     6317 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     4026 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2652 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0      998 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1842 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     7386 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     5930 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     2319 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      144 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     2382 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     2340 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/common/termination_handler_middleware.py
+-rw-r--r--   0        0        0    11957 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      727 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0    13415 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      274 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     3273 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1352 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/shared/logging.py
+-rw-r--r--   0        0        0     1430 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0     3318 2023-08-03 21:57:44.718621 truss-0.5.4/truss/templates/shared/serialization.py
+-rw-r--r--   0        0        0     1863 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/shared/util.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0      521 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/tgi/proxy.conf
+-rw-r--r--   0        0        0      521 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/tgi/supervisord.conf.jinja
+-rw-r--r--   0        0        0      586 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/tgi/tgi.Dockerfile.jinja
+-rw-r--r--   0        0        0     3400 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0      527 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/vllm/proxy.conf.jinja
+-rw-r--r--   0        0        0      463 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/vllm/supervisord.conf.jinja
+-rw-r--r--   0        0        0      522 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/vllm/vllm.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-08-03 21:57:44.722621 truss-0.5.4/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0      739 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1550 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      739 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_async_truss/config.yaml
+-rw-r--r--   0        0        0      646 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_async_truss/model/model.py
+-rw-r--r--   0        0        0       34 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_concurrency_truss/config.yaml
+-rw-r--r--   0        0        0      547 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_concurrency_truss/model/model.py
+-rw-r--r--   0        0        0      739 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_streaming_async_generator_truss/config.yaml
+-rw-r--r--   0        0        0      521 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_streaming_async_generator_truss/model/model.py
+-rw-r--r--   0        0        0      773 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_streaming_truss/config.yaml
+-rw-r--r--   0        0        0      606 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_streaming_truss/model/model.py
+-rw-r--r--   0        0        0      773 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_streaming_truss_with_error/config.yaml
+-rw-r--r--   0        0        0      673 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_streaming_truss_with_error/model/model.py
+-rw-r--r--   0        0        0      669 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        6 2023-08-03 21:57:44.722621 truss-0.5.4/truss/test_data/test_truss/packages/test_package/test.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/__init__.py
+-rw-r--r--   0        0        0    22226 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    18726 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     1929 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0     2073 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/remote/baseten/test_api.py
+-rw-r--r--   0        0        0      580 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/remote/baseten/test_auth.py
+-rw-r--r--   0        0        0      835 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/remote/baseten/test_core.py
+-rw-r--r--   0        0        0     4316 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/remote/test_remote_factory.py
+-rw-r--r--   0        0        0     2394 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/remote/test_truss_remote.py
+-rw-r--r--   0        0        0    10415 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     6081 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     7513 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0     8326 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/control/control/test_server_integration.py
+-rw-r--r--   0        0        0     1560 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/core/server/common/test_truss_server.py
+-rw-r--r--   0        0        0      821 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2605 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/server/common/test_termination_handler_middleware.py
+-rw-r--r--   0        0        0     2252 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/test_build.py
+-rw-r--r--   0        0        0     8657 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-08-03 21:57:44.722621 truss-0.5.4/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0    14982 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/test_control_truss_patching.py
+-rw-r--r--   0        0        0      517 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/test_docker.py
+-rw-r--r--   0        0        0    15016 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    30057 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0     1865 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     4974 2023-08-03 21:57:44.726621 truss-0.5.4/truss/tests/util/test_path.py
+-rw-r--r--   0        0        0    16461 2023-08-03 21:57:44.726621 truss-0.5.4/truss/truss_config.py
+-rw-r--r--   0        0        0     2698 2023-08-03 21:57:44.726621 truss-0.5.4/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41215 2023-08-03 21:57:44.726621 truss-0.5.4/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-08-03 21:57:44.726621 truss-0.5.4/truss/truss_spec.py
+-rw-r--r--   0        0        0     2782 2023-08-03 21:57:44.726621 truss-0.5.4/truss/types.py
+-rw-r--r--   0        0        0     3121 2023-08-03 21:57:44.726621 truss-0.5.4/truss/util/.truss_ignore
+-rw-r--r--   0        0        0      379 2023-08-03 21:57:44.726621 truss-0.5.4/truss/util/data_structures.py
+-rw-r--r--   0        0        0     2552 2023-08-03 21:57:44.726621 truss-0.5.4/truss/util/download.py
+-rw-r--r--   0        0        0      553 2023-08-03 21:57:44.726621 truss-0.5.4/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-08-03 21:57:44.726621 truss-0.5.4/truss/util/jinja.py
+-rw-r--r--   0        0        0     6040 2023-08-03 21:57:44.726621 truss-0.5.4/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-08-03 21:57:44.726621 truss-0.5.4/truss/validation.py
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 truss-0.5.4/PKG-INFO
```

### Comparing `truss-0.5.3/CODE_OF_CONDUCT.md` & `truss-0.5.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/CONTRIBUTING.md` & `truss-0.5.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/LICENSE` & `truss-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/README.md` & `truss-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/context_builder.Dockerfile` & `truss-0.5.4/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/pyproject.toml` & `truss-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.5.3"
+version = "0.5.4"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.5.3/truss/blob/blob_backend_registry.py` & `truss-0.5.4/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/blob/http_public_blob_backend.py` & `truss-0.5.4/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/build.py` & `truss-0.5.4/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/cli/cli.py` & `truss-0.5.4/truss/cli/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/constants.py` & `truss-0.5.4/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/image_builder/image_builder.py` & `truss-0.5.4/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.5.4/truss/contexts/image_builder/serving_image_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import yaml
 from huggingface_hub import list_repo_files
+from huggingface_hub.utils import filter_repo_objects
 from truss.constants import (
     BASE_SERVER_REQUIREMENTS_TXT_FILENAME,
     CONTROL_SERVER_CODE_DIR,
     MODEL_DOCKERFILE_NAME,
     REQUIREMENTS_TXT_FILENAME,
     SERVER_CODE_DIR,
     SERVER_DOCKERFILE_TEMPLATE_NAME,
@@ -66,14 +67,49 @@
         TEMPLATES_DIR, "tgi/supervisord.conf.jinja"
     )
     supervisord_contents = supervisord_template.render(extra_args=args)
     supervisord_filepath = build_dir / "supervisord.conf"
     supervisord_filepath.write_text(supervisord_contents)
 
 
+def create_vllm_build_dir(config: TrussConfig, build_dir: Path):
+    server_endpoint_config = {
+        "Completions": "/v1/completions",
+        "ChatCompletions": "/v1/chat/completions",
+    }
+    if not build_dir.exists():
+        build_dir.mkdir(parents=True)
+
+    build_config: Build = config.build
+    server_endpoint = server_endpoint_config[build_config.arguments.pop("endpoint")]
+    hf_access_token = config.secrets.get(HF_ACCESS_TOKEN_SECRET_NAME)
+    dockerfile_template = read_template_from_fs(
+        TEMPLATES_DIR, "vllm/vllm.Dockerfile.jinja"
+    )
+    nginx_template = read_template_from_fs(TEMPLATES_DIR, "vllm/proxy.conf.jinja")
+
+    dockerfile_content = dockerfile_template.render(hf_access_token=hf_access_token)
+    dockerfile_filepath = build_dir / "Dockerfile"
+    dockerfile_filepath.write_text(dockerfile_content)
+
+    nginx_content = nginx_template.render(server_endpoint=server_endpoint)
+    nginx_filepath = build_dir / "nginx.proxy"
+    nginx_filepath.write_text(nginx_content)
+
+    args = " ".join(
+        [f"--{k.replace('_', '-')}={v}" for k, v in build_config.arguments.items()]
+    )
+    supervisord_template = read_template_from_fs(
+        TEMPLATES_DIR, "vllm/supervisord.conf.jinja"
+    )
+    supervisord_contents = supervisord_template.render(extra_args=args)
+    supervisord_filepath = build_dir / "supervisord.conf"
+    supervisord_filepath.write_text(supervisord_contents)
+
+
 class ServingImageBuilderContext(TrussContext):
     @staticmethod
     def run(truss_dir: Path):
         return ServingImageBuilder(truss_dir)
 
 
 class ServingImageBuilder(ImageBuilder):
@@ -81,29 +117,34 @@
         self._truss_dir = truss_dir
         self._spec = TrussSpec(truss_dir)
 
     @property
     def default_tag(self):
         return f"{self._spec.model_framework_name}-model:latest"
 
-    def prepare_image_build_dir(self, build_dir: Optional[Path] = None):
+    def prepare_image_build_dir(
+        self, build_dir: Optional[Path] = None, use_hf_secret: bool = False
+    ):
         """
         Prepare a directory for building the docker image from.
         """
         truss_dir = self._truss_dir
         spec = self._spec
         config = spec.config
         model_framework_name = spec.model_framework_name
         if build_dir is None:
             # TODO(pankaj) We probably don't need model framework specific directory.
             build_dir = build_truss_target_directory(model_framework_name)
 
         if config.build.model_server is ModelServer.TGI:
             create_tgi_build_dir(config, build_dir)
             return
+        elif config.build.model_server is ModelServer.VLLM:
+            create_vllm_build_dir(config, build_dir)
+            return
 
         data_dir = build_dir / config.data_dir  # type: ignore[operator]
 
         def copy_into_build_dir(from_path: Path, path_in_build_dir: str):
             copy_tree_or_file(from_path, build_dir / path_in_build_dir)  # type: ignore[operator]
 
         # Copy over truss
@@ -120,16 +161,27 @@
         model_files = {}
         if config.hf_cache:
             curr_dir = Path(__file__).parent.resolve()
             copy_into_build_dir(curr_dir / "cache_warmer.py", "cache_warmer.py")
             for model in config.hf_cache.models:
                 repo_id = model.repo_id
                 revision = model.revision
+
+                allow_patterns = model.allow_patterns
+                ignore_patterns = model.ignore_patterns
+
+                filtered_repo_files = list(
+                    filter_repo_objects(
+                        items=list_repo_files(repo_id, revision=revision),
+                        allow_patterns=allow_patterns,
+                        ignore_patterns=ignore_patterns,
+                    )
+                )
                 model_files[repo_id] = {
-                    "files": list_repo_files(repo_id, revision=revision),
+                    "files": filtered_repo_files,
                     "revision": revision,
                 }
 
         # Copy inference server code
         copy_into_build_dir(SERVER_CODE_DIR, BUILD_SERVER_DIR_NAME)
         copy_into_build_dir(
             SHARED_SERVING_AND_TRAINING_CODE_DIR,
@@ -163,22 +215,23 @@
         if should_install_server_requirements:
             copy_into_build_dir(server_reqs_filepath, SERVER_REQUIREMENTS_TXT_FILENAME)
 
         (build_dir / REQUIREMENTS_TXT_FILENAME).write_text(spec.requirements_txt)
         (build_dir / SYSTEM_PACKAGES_TXT_FILENAME).write_text(spec.system_packages_txt)
 
         self._render_dockerfile(
-            build_dir, should_install_server_requirements, model_files
+            build_dir, should_install_server_requirements, model_files, use_hf_secret
         )
 
     def _render_dockerfile(
         self,
         build_dir: Path,
         should_install_server_requirements: bool,
         model_files: Dict[str, Any],
+        use_hf_secret: bool,
     ):
         config = self._spec.config
         data_dir = build_dir / config.data_dir
         bundled_packages_dir = build_dir / config.bundled_packages_dir
         dockerfile_template = read_template_from_fs(
             TEMPLATES_DIR, SERVER_DOCKERFILE_TEMPLATE_NAME
         )
@@ -207,10 +260,11 @@
             config=config,
             python_version=python_version,
             live_reload=config.live_reload,
             data_dir_exists=data_dir.exists(),
             bundled_packages_dir_exists=bundled_packages_dir.exists(),
             truss_hash=directory_content_hash(self._truss_dir),
             models=model_files,
+            use_hf_secret=use_hf_secret,
         )
         docker_file_path = build_dir / MODEL_DOCKERFILE_NAME
         docker_file_path.write_text(dockerfile_contents)
```

### Comparing `truss-0.5.3/truss/contexts/image_builder/training_image_builder.py` & `truss-0.5.4/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/image_builder/util.py` & `truss-0.5.4/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.5.4/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/local_loader/load_model_local.py` & `truss-0.5.4/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/local_loader/train_local.py` & `truss-0.5.4/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/local_loader/truss_file_syncer.py` & `truss-0.5.4/truss/contexts/local_loader/truss_file_syncer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.5.4/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/contexts/local_loader/utils.py` & `truss-0.5.4/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/docker.py` & `truss-0.5.4/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/environment_inference/requirements_inference.py` & `truss-0.5.4/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/errors.py` & `truss-0.5.4/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/local/local_config.py` & `truss-0.5.4/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/local/local_config_handler.py` & `truss-0.5.4/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_framework.py` & `truss-0.5.4/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_frameworks/__init__.py` & `truss-0.5.4/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_frameworks/huggingface_transformer.py` & `truss-0.5.4/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_frameworks/keras.py` & `truss-0.5.4/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_frameworks/lightgbm.py` & `truss-0.5.4/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_frameworks/mlflow.py` & `truss-0.5.4/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_frameworks/pytorch.py` & `truss-0.5.4/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_frameworks/sklearn.py` & `truss-0.5.4/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_frameworks/xgboost.py` & `truss-0.5.4/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/model_inference.py` & `truss-0.5.4/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/patch/calc_patch.py` & `truss-0.5.4/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/patch/dir_signature.py` & `truss-0.5.4/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/patch/hash.py` & `truss-0.5.4/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/patch/local_truss_patch_applier.py` & `truss-0.5.4/truss/patch/local_truss_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/patch/truss_dir_patch_applier.py` & `truss-0.5.4/truss/patch/truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/patch/types.py` & `truss-0.5.4/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/readme_generator.py` & `truss-0.5.4/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/baseten/api.py` & `truss-0.5.4/truss/remote/baseten/api.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/baseten/auth.py` & `truss-0.5.4/truss/remote/baseten/auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/baseten/core.py` & `truss-0.5.4/truss/remote/baseten/core.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/baseten/error.py` & `truss-0.5.4/truss/remote/baseten/error.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/baseten/remote.py` & `truss-0.5.4/truss/remote/baseten/remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/baseten/service.py` & `truss-0.5.4/truss/remote/baseten/service.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/baseten/utils/tar.py` & `truss-0.5.4/truss/remote/baseten/utils/tar.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/baseten/utils/transfer.py` & `truss-0.5.4/truss/remote/baseten/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/remote_cli.py` & `truss-0.5.4/truss/remote/remote_cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/remote_factory.py` & `truss-0.5.4/truss/remote/remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/remote/truss_remote.py` & `truss-0.5.4/truss/remote/truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/README.md.jinja` & `truss-0.5.4/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/base.Dockerfile.jinja` & `truss-0.5.4/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/application.py` & `truss-0.5.4/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/endpoints.py` & `truss-0.5.4/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/errors.py` & `truss-0.5.4/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.5.4/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.5.4/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.5.4/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/truss_patch/__init__.py` & `truss-0.5.4/truss/templates/control/control/helpers/truss_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py` & `truss-0.5.4/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py` & `truss-0.5.4/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py` & `truss-0.5.4/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/helpers/types.py` & `truss-0.5.4/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/control/control/server.py` & `truss-0.5.4/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/custom/model/model.py` & `truss-0.5.4/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/huggingface_transformer/model/model.py` & `truss-0.5.4/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/keras/model/model.py` & `truss-0.5.4/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/lightgbm/model/model.py` & `truss-0.5.4/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/mlflow/model/model.py` & `truss-0.5.4/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/pytorch/model/model.py` & `truss-0.5.4/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/server/common/errors.py` & `truss-0.5.4/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.5.4/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/server/common/patches.py` & `truss-0.5.4/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/server/common/retry.py` & `truss-0.5.4/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/server/common/termination_handler_middleware.py` & `truss-0.5.4/truss/templates/server/common/termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/server/common/truss_server.py` & `truss-0.5.4/truss/templates/server/common/truss_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import concurrent.futures
 import json
 import logging
 import multiprocessing
 import os
 import signal
 import socket
 import sys
@@ -115,15 +114,15 @@
         """
         return await self.predict(self._model.name, request, body_raw)
 
     async def predict(
         self, model_name: str, request: Request, body_raw: bytes = Depends(parse_body)
     ) -> Response:
         """
-        This method is called by FastAPI, which introspects that it's not async, and schedules it on a thread
+        This method calls the user-provided predict method
         """
         model: ModelWrapper = self._safe_lookup_model(model_name)
 
         self.check_healthy(model)
 
         body: Dict
         if self.is_binary(request):
@@ -290,21 +289,16 @@
                         "level": "INFO",
                         "propagate": False,
                     },
                 },
             },
         )
 
-        max_asyncio_workers = min(32, utils.cpu_count() + 4)
-        logging.info(f"Setting max asyncio worker threads as {max_asyncio_workers}")
         # Call this so uvloop gets used
         cfg.setup_event_loop()
-        asyncio.get_event_loop().set_default_executor(
-            concurrent.futures.ThreadPoolExecutor(max_workers=max_asyncio_workers)
-        )
 
         async def serve():
             serversocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             serversocket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             serversocket.bind((cfg.host, cfg.port))
             serversocket.listen(5)
```

### Comparing `truss-0.5.3/truss/templates/server/inference_server.py` & `truss-0.5.4/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/server/model_wrapper.py` & `truss-0.5.4/truss/templates/server/model_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import inspect
 import logging
 import os
 import sys
 import time
 import traceback
 from collections.abc import Generator
+from contextlib import asynccontextmanager
 from enum import Enum
 from pathlib import Path
 from threading import Lock, Thread
 from typing import Any, AsyncGenerator, Dict, Optional, Set, Union
 
 from anyio import Semaphore, to_thread
 from common.patches import apply_patches
@@ -20,14 +21,52 @@
 MODEL_BASENAME = "model"
 
 NUM_LOAD_RETRIES = int(os.environ.get("NUM_LOAD_RETRIES_TRUSS", "3"))
 STREAMING_RESPONSE_QUEUE_READ_TIMEOUT_SECS = 60
 DEFAULT_PREDICT_CONCURRENCY = 1
 
 
+class DeferredSemaphoreManager:
+    """
+    Helper class for supported deferred semaphore release.
+    """
+
+    def __init__(self, semaphore: Semaphore):
+        self.semaphore = semaphore
+        self.deferred = False
+
+    def defer(self):
+        """
+        Track that this semaphore is to be deferred, and return
+        a release method that the context block can use to release
+        the semaphore.
+        """
+        self.deferred = True
+
+        return self.semaphore.release
+
+
+@asynccontextmanager
+async def deferred_semaphore(semaphore: Semaphore):
+    """
+    Context manager that allows deferring the release of a semaphore.
+    It yields a DeferredSemaphoreManager -- in your use of this context manager,
+    if you call DeferredSemaphoreManager.defer(), you will get back a function that releases
+    the semaphore that you must call.
+    """
+    semaphore_manager = DeferredSemaphoreManager(semaphore)
+    await semaphore.acquire()
+
+    try:
+        yield semaphore_manager
+    finally:
+        if not semaphore_manager.deferred:
+            semaphore.release()
+
+
 class ModelWrapper:
     class Status(Enum):
         NOT_READY = 0
         LOADING = 1
         READY = 2
         FAILED = 3
 
@@ -202,18 +241,21 @@
             return await self._model.postprocess(response)
 
         return await to_thread.run_sync(self._model.postprocess, response)
 
     async def write_response_to_queue(
         self, queue: asyncio.Queue, generator: AsyncGenerator
     ):
-        async for chunk in generator:
-            await queue.put(ResponseChunk(chunk))
-
-        await queue.put(None)
+        try:
+            async for chunk in generator:
+                await queue.put(ResponseChunk(chunk))
+        except Exception as e:
+            self._logger.exception("Exception while reading stream response: " + str(e))
+        finally:
+            await queue.put(None)
 
     async def __call__(
         self, body: Any, headers: Optional[Dict[str, str]] = None
     ) -> Union[Dict, Generator]:
         """Method to call predictor or explainer with the given input.
 
         Args:
@@ -223,15 +265,15 @@
         Returns:
             Dict: Response output from preprocess -> predictor -> postprocess
             Generator: In case of streaming response
         """
 
         payload = await self.preprocess(body, headers)
 
-        async with self._predict_semaphore:
+        async with deferred_semaphore(self._predict_semaphore) as semaphore_manager:
             response = await self.predict(payload, headers)
 
             processed_response = await self.postprocess(response)
 
             # Streaming cases
             if inspect.isgenerator(response) or inspect.isasyncgen(response):
                 async_generator = _force_async_generator(response)
@@ -247,16 +289,24 @@
                 # exit the semaphore block.
                 response_queue: asyncio.Queue = asyncio.Queue()
 
                 # This task will be triggered and run in the background.
                 task = asyncio.create_task(
                     self.write_response_to_queue(response_queue, async_generator)
                 )
+
+                # We add the task to the ModelWrapper instance to ensure it does
+                # not get garbage collected after the predict method completes,
+                # and continues running.
                 self._background_tasks.add(task)
 
+                # Defer the release of the semaphore until the write_response_to_queue
+                # task.
+                semaphore_release_function = semaphore_manager.defer()
+                task.add_done_callback(lambda _: semaphore_release_function())
                 task.add_done_callback(self._background_tasks.discard)
 
                 async def _response_generator():
                     while True:
                         chunk = await asyncio.wait_for(
                             response_queue.get(),
                             timeout=STREAMING_RESPONSE_QUEUE_READ_TIMEOUT_SECS,
```

### Comparing `truss-0.5.3/truss/templates/server.Dockerfile.jinja` & `truss-0.5.4/truss/templates/server.Dockerfile.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -44,21 +44,17 @@
     {%- endif %}
 {{ super() }}
 {% endblock %}
 
 {% block cache_weights %}
     {%- if config.hf_cache != None %}
 COPY ./cache_warmer.py /cache_warmer.py
-        {% for repo, data in models.items() %}
-            {% for file in data.files %}
-                {%- if data.revision != None %}
-RUN $PYTHON_EXECUTABLE /cache_warmer.py {{file}} {{repo}} {{data.revision}}
-                {%- else %}
-RUN $PYTHON_EXECUTABLE /cache_warmer.py {{file}} {{repo}}
-                {%- endif %}
+        {% for repo, hf_dir in models.items() %}
+            {% for file in hf_dir.files %}
+{{ "RUN --mount=type=secret,id=hf_access_token,dst=/etc/secrets/hf_access_token" if use_hf_secret else "RUN" }} $PYTHON_EXECUTABLE /cache_warmer.py {{file}} {{repo}} {% if hf_dir.revision != None %}{{hf_dir.revision}}{% endif %}
             {% endfor %}
         {% endfor %}
     {%- endif %}
 {% endblock %}
 
 
 {% block app_copy %}
```

### Comparing `truss-0.5.3/truss/templates/shared/logging.py` & `truss-0.5.4/truss/templates/shared/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/shared/secrets_resolver.py` & `truss-0.5.4/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/shared/serialization.py` & `truss-0.5.4/truss/templates/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/shared/util.py` & `truss-0.5.4/truss/templates/shared/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/sklearn/model/model.py` & `truss-0.5.4/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/tgi/proxy.conf` & `truss-0.5.4/truss/templates/tgi/proxy.conf`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/tgi/tgi.Dockerfile.jinja` & `truss-0.5.4/truss/templates/tgi/tgi.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/training/job.py` & `truss-0.5.4/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/templates/xgboost/model/model.py` & `truss-0.5.4/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/auto-mpg.data` & `truss-0.5.4/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/happy.ipynb` & `truss-0.5.4/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/model_load_failure_test/config.yaml` & `truss-0.5.4/truss/test_data/model_load_failure_test/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.5.4/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/patch_ping_test_server/app.py` & `truss-0.5.4/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/pima-indians-diabetes.csv` & `truss-0.5.4/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/readme_int_example.md` & `truss-0.5.4/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/readme_no_example.md` & `truss-0.5.4/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/readme_str_example.md` & `truss-0.5.4/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/server.Dockerfile` & `truss-0.5.4/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/server_conformance_test_truss/config.yaml` & `truss-0.5.4/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.5.4/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/test_async_truss/config.yaml` & `truss-0.5.4/truss/test_data/test_async_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/test_async_truss/model/model.py` & `truss-0.5.4/truss/test_data/test_async_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/test_concurrency_truss/model/model.py` & `truss-0.5.4/truss/test_data/test_concurrency_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/test_streaming_async_generator_truss/config.yaml` & `truss-0.5.4/truss/test_data/test_streaming_async_generator_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/test_streaming_async_generator_truss/model/model.py` & `truss-0.5.4/truss/test_data/test_streaming_async_generator_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/test_streaming_truss/config.yaml` & `truss-0.5.4/truss/test_data/test_streaming_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/test_streaming_truss/model/model.py` & `truss-0.5.4/truss/test_data/test_truss/model/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import Any, Dict, List
+from typing import Any
 
 
 class Model:
     def __init__(self, **kwargs) -> None:
         self._data_dir = kwargs["data_dir"]
         self._config = kwargs["config"]
         self._secrets = kwargs["secrets"]
         self._model = None
 
     def load(self):
         # Load model here and assign to self._model.
         pass
 
-    def predict(self, model_input: Any) -> Dict[str, List]:
+    def predict(self, model_input: Any) -> Any:
+        model_output = {}
         # Invoke model on model_input and calculate predictions here.
-        def inner():
-            for i in range(5):
-                yield str(i)
-
-        return inner()
+        model_output["predictions"] = []
+        return model_output
```

### Comparing `truss-0.5.3/truss/test_data/test_truss/config.yaml` & `truss-0.5.4/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/test_data/test_truss/model/model.py` & `truss-0.5.4/truss/test_data/test_streaming_truss/model/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from typing import Any
+import time
+from typing import Any, Dict, List
 
 
 class Model:
     def __init__(self, **kwargs) -> None:
         self._data_dir = kwargs["data_dir"]
         self._config = kwargs["config"]
         self._secrets = kwargs["secrets"]
         self._model = None
 
     def load(self):
         # Load model here and assign to self._model.
         pass
 
-    def predict(self, model_input: Any) -> Any:
-        model_output = {}
+    def predict(self, model_input: Any) -> Dict[str, List]:
         # Invoke model on model_input and calculate predictions here.
-        model_output["predictions"] = []
-        return model_output
+        def inner():
+            time.sleep(2)
+            for i in range(5):
+                yield str(i)
+
+        return inner()
```

### Comparing `truss-0.5.3/truss/tests/conftest.py` & `truss-0.5.4/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.5.4/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.5.4/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.5.4/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.5.4/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/local/test_local_config_handler.py` & `truss-0.5.4/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.5.4/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.5.4/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.5.4/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.5.4/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.5.4/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.5.4/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/patch/test_calc_patch.py` & `truss-0.5.4/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/patch/test_hash.py` & `truss-0.5.4/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/patch/test_truss_dir_patch_applier.py` & `truss-0.5.4/truss/tests/patch/test_truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/remote/baseten/test_api.py` & `truss-0.5.4/truss/tests/remote/baseten/test_api.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/remote/baseten/test_auth.py` & `truss-0.5.4/truss/tests/remote/baseten/test_auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/remote/baseten/test_core.py` & `truss-0.5.4/truss/tests/remote/baseten/test_core.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/remote/test_remote_factory.py` & `truss-0.5.4/truss/tests/remote/test_remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/remote/test_truss_remote.py` & `truss-0.5.4/truss/tests/remote/test_truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/samples.py` & `truss-0.5.4/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py` & `truss-0.5.4/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py` & `truss-0.5.4/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/control/control/test_server.py` & `truss-0.5.4/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/control/control/test_server_integration.py` & `truss-0.5.4/truss/tests/templates/control/control/test_server_integration.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/core/server/common/test_truss_server.py` & `truss-0.5.4/truss/tests/templates/core/server/common/test_truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/core/server/common/test_util.py` & `truss-0.5.4/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.5.4/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/server/common/test_retry.py` & `truss-0.5.4/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/server/common/test_termination_handler_middleware.py` & `truss-0.5.4/truss/tests/templates/server/common/test_termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.5.4/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_backward.py` & `truss-0.5.4/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_build.py` & `truss-0.5.4/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_config.py` & `truss-0.5.4/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_context_builder_image.py` & `truss-0.5.4/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_control_truss_patching.py` & `truss-0.5.4/truss/tests/test_control_truss_patching.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_docker.py` & `truss-0.5.4/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_model_inference.py` & `truss-0.5.4/truss/tests/test_model_inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import concurrent
 import logging
 import tempfile
 import time
+from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 from threading import Thread
 
 import numpy as np
 import pytest
 import requests
 from requests.exceptions import RequestException
@@ -241,51 +243,108 @@
             headers={"accept": "application/json"},
         )
         assert "transfer-encoding" not in predict_non_stream_response.headers
         assert predict_non_stream_response.json() == "01234"
 
 
 @pytest.mark.integration
+def test_streaming_with_error():
+    with ensure_kill_all():
+        truss_root = Path(__file__).parent.parent.parent.resolve() / "truss"
+
+        truss_dir = truss_root / "test_data" / "test_streaming_truss_with_error"
+
+        tr = TrussHandle(truss_dir)
+
+        _ = tr.docker_run(local_port=8090, detach=True, wait_for_server_ready=True)
+        truss_server_addr = "http://localhost:8090"
+        predict_url = f"{truss_server_addr}/v1/models/model:predict"
+
+        predict_error_response = requests.post(
+            predict_url, json={"throw_error": True}, stream=True, timeout=2
+        )
+
+        # In error cases, the response will return whatever the stream returned,
+        # in this case, the first 3 items. We timeout after 2 seconds to ensure that
+        # stream finishes reading and releases the predict semaphore.
+        assert [
+            byte_string.decode()
+            for byte_string in predict_error_response.iter_content()
+        ] == ["0", "1", "2"]
+
+        # Test that we are able to continue to make requests successfully
+        predict_non_error_response = requests.post(
+            predict_url, json={"throw_error": False}, stream=True, timeout=2
+        )
+
+        assert [
+            byte_string.decode()
+            for byte_string in predict_non_error_response.iter_content()
+        ] == ["0", "1", "2", "3", "4"]
+
+
+@pytest.mark.integration
 def test_streaming_truss():
     with ensure_kill_all():
         truss_root = Path(__file__).parent.parent.parent.resolve() / "truss"
         truss_dir = truss_root / "test_data" / "test_streaming_truss"
         tr = TrussHandle(truss_dir)
 
         _ = tr.docker_run(local_port=8090, detach=True, wait_for_server_ready=True)
 
         truss_server_addr = "http://localhost:8090"
+        predict_url = f"{truss_server_addr}/v1/models/model:predict"
 
         # A request for which response is not completely read
-        predict_response = requests.post(
-            f"{truss_server_addr}/v1/models/model:predict", json={}, stream=True
-        )
+        predict_response = requests.post(predict_url, json={}, stream=True)
         # We just read the first part and leave it hanging here
         next(predict_response.iter_content())
 
-        predict_response = requests.post(
-            f"{truss_server_addr}/v1/models/model:predict", json={}, stream=True
-        )
+        predict_response = requests.post(predict_url, json={}, stream=True)
 
         assert predict_response.headers.get("transfer-encoding") == "chunked"
         assert [
             byte_string.decode()
             for byte_string in list(predict_response.iter_content())
         ] == ["0", "1", "2", "3", "4"]
 
         # When accept is set to application/json, the response is not streamed.
         predict_non_stream_response = requests.post(
-            f"{truss_server_addr}/v1/models/model:predict",
+            predict_url,
             json={},
             stream=True,
             headers={"accept": "application/json"},
         )
         assert "transfer-encoding" not in predict_non_stream_response.headers
         assert predict_non_stream_response.json() == "01234"
 
+        # Test that concurrency work correctly. The streaming Truss has a configured
+        # concurrency of 1, so only one request can be in flight at a time. Each request
+        # takes 2 seconds, so with a timeout of 3 seconds, we expect the first request to
+        # succeed and for the second to timeout.
+        #
+        # Note that with streamed requests, requests.post raises a ReadTimeout exception if
+        # `timeout` seconds has passed since receiving any data from the server.
+        def make_request(delay: int):
+            # For streamed responses, requests does not start receiving content from server until
+            # `iter_content` is called, so we must call this in order to get an actual timeout.
+            time.sleep(delay)
+            list(requests.post(predict_url, json={}, stream=True).iter_content())
+
+        with ThreadPoolExecutor() as e:
+            # We use concurrent.futures.wait instead of the timeout property
+            # on requests, since requests timeout property has a complex interaction
+            # with streaming.
+            first_request = e.submit(make_request, 0)
+            second_request = e.submit(make_request, 0.2)
+            futures = [first_request, second_request]
+            done, not_done = concurrent.futures.wait(futures, timeout=3)
+            assert first_request in done
+            assert second_request in not_done
+
 
 @pytest.mark.integration
 def test_slow_truss():
     with ensure_kill_all():
         truss_root = Path(__file__).parent.parent.parent.resolve() / "truss"
         truss_dir = truss_root / "test_data" / "server_conformance_test_truss"
         tr = TrussHandle(truss_dir)
```

### Comparing `truss-0.5.3/truss/tests/test_notebooks.py` & `truss-0.5.4/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.5.4/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_truss_gatherer.py` & `truss-0.5.4/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_truss_handle.py` & `truss-0.5.4/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/test_validation.py` & `truss-0.5.4/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/tests/util/test_path.py` & `truss-0.5.4/truss/tests/util/test_path.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/truss_config.py` & `truss-0.5.4/truss/truss_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,47 @@
         return AcceleratorSpec(accelerator=acc, count=count)
 
 
 @dataclass
 class HuggingFaceModel:
     repo_id: str = ""
     revision: Optional[str] = None
+    allow_patterns: Optional[List[str]] = None
+    ignore_patterns: Optional[List[str]] = None
 
     @staticmethod
     def from_dict(d):
         repo_id = d.get("repo_id")
         if repo_id is None or repo_id == "":
             raise ValueError("Repo ID for Hugging Face model cannot be empty.")
         revision = d.get("revision", None)
 
-        return HuggingFaceModel(repo_id=repo_id, revision=revision)
+        allow_patterns = d.get("allow_patterns", None)
+        ignore_pattenrs = d.get("ignore_patterns", None)
+
+        return HuggingFaceModel(
+            repo_id=repo_id,
+            revision=revision,
+            allow_patterns=allow_patterns,
+            ignore_patterns=ignore_pattenrs,
+        )
 
     def to_dict(self, verbose=False):
-        if verbose or self.revision is not None:
-            return {"repo_id": self.repo_id, "revision": self.revision}
-        return {"repo_id": self.repo_id}
+        data = {
+            "repo_id": self.repo_id,
+            "revision": self.revision,
+            "allow_patterns": self.allow_patterns,
+            "ignore_patterns": self.ignore_patterns,
+        }
+
+        if not verbose:
+            # only show changed values
+            data = {k: v for k, v in data.items() if v is not None}
+
+        return data
 
 
 @dataclass
 class HuggingFaceCache:
     models: List[HuggingFaceModel]
 
     @staticmethod
```

### Comparing `truss-0.5.3/truss/truss_gatherer.py` & `truss-0.5.4/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/truss_handle.py` & `truss-0.5.4/truss/truss_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,23 +379,25 @@
         rmtree(str(output_dir))
         rmtree(str(variables_dir))
 
     def local_train(self, variables: Optional[dict] = None):
         LocalTrainer.run(self._truss_dir)(variables)
 
     @proxy_to_shadow_if_scattered
-    def docker_build_setup(self, build_dir: Optional[Path] = None):
+    def docker_build_setup(
+        self, build_dir: Optional[Path] = None, use_hf_secret: bool = False
+    ):
         """
         Set up a directory to build docker image from.
 
         Returns:
             docker build command.
         """
         image_builder = ServingImageBuilderContext.run(self._truss_dir)
-        image_builder.prepare_image_build_dir(build_dir)
+        image_builder.prepare_image_build_dir(build_dir, use_hf_secret=use_hf_secret)
         return image_builder.docker_build_command(build_dir)
 
     @proxy_to_shadow_if_scattered
     def training_docker_build_setup(self, build_dir: Optional[Path] = None):
         """
         Set up a directory to build training docker image from.
```

### Comparing `truss-0.5.3/truss/truss_spec.py` & `truss-0.5.4/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/types.py` & `truss-0.5.4/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/util/.truss_ignore` & `truss-0.5.4/truss/util/.truss_ignore`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/util/download.py` & `truss-0.5.4/truss/util/download.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/util/gpu.py` & `truss-0.5.4/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/util/path.py` & `truss-0.5.4/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/truss/validation.py` & `truss-0.5.4/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.3/PKG-INFO` & `truss-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.5.3
+Version: 0.5.4
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
```

