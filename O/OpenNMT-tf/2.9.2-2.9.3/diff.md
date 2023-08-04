# Comparing `tmp/OpenNMT-tf-2.9.2.tar.gz` & `tmp/OpenNMT-tf-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OpenNMT-tf-2.9.2.tar", last modified: Wed Apr 22 08:59:01 2020, max compression
+gzip compressed data, was "dist/OpenNMT-tf-2.9.3.tar", last modified: Wed May  6 08:28:35 2020, max compression
```

## Comparing `OpenNMT-tf-2.9.2.tar` & `OpenNMT-tf-2.9.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10988 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      212 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      313 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    10988 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8472 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20535 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/training.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/optimizers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4227 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/optimizers/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/optimizers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19797 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/runner.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/inputters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3339 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/inputters/record_inputter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21160 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/inputters/inputter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21047 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/inputters/text_inputter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/inputters/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/encoders/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3244 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/encoders/self_attention_encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8526 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/encoders/rnn_encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      491 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/encoders/mean_encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2194 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/encoders/conv_encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      647 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/encoders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7273 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/encoders/encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      235 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4588 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/data/text.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8887 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/data/vocab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23906 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/data/dataset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8642 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/data/noise.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)      602 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/bin/tokenize_text.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3374 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/bin/build_vocab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4574 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/bin/ark_to_records.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      610 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/bin/detokenize_text.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      471 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/bin/merge_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9889 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/bin/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/bin/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/layers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3539 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/layers/position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5572 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/layers/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9099 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/layers/rnn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6653 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/layers/reducer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18214 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/layers/transformer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/layers/bridge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1482 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/layers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21213 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/models/sequence_to_sequence.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/models/sequence_classifier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8039 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/models/sequence_tagger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6380 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/models/transformer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11872 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/models/catalog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10023 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/models/language_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13832 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/models/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9419 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/schedules/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7411 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/schedules/lr_schedules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      476 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/schedules/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10887 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/checkpoint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12780 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      627 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/ter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3001 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/exporters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      664 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/tensor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3022 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/fmeasure.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19873 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/decoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      648 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7121 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/losses.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3894 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/scorers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1391 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/utils/wer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13494 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/evaluation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/tokenizers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1336 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/tokenizers/opennmt_tokenizer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      512 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/tokenizers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11565 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/tokenizers/tokenizer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      542 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 08:59:01.000000 OpenNMT-tf-2.9.2/opennmt/decoders/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16540 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/decoders/decoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9668 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/decoders/rnn_decoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7077 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/decoders/self_attention_decoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/opennmt/decoders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2020-04-22 08:48:11.000000 OpenNMT-tf-2.9.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10988 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      212 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      313 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10988 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8472 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20535 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/training.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/optimizers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4227 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/optimizers/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      150 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/optimizers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19797 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/runner.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/inputters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3339 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/inputters/record_inputter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21160 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/inputters/inputter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21047 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/inputters/text_inputter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/inputters/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/encoders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3244 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/encoders/self_attention_encoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8526 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/encoders/rnn_encoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      491 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/encoders/mean_encoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2194 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/encoders/conv_encoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      647 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/encoders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7273 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/encoders/encoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      235 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4588 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/data/text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8887 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/data/vocab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23906 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/data/dataset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8642 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/data/noise.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      602 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/bin/tokenize_text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3374 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/bin/build_vocab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4574 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/bin/ark_to_records.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/bin/detokenize_text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/bin/merge_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9889 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/bin/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/bin/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/layers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3539 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/layers/position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5572 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/layers/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9099 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/layers/rnn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6653 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/layers/reducer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18214 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/layers/transformer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/layers/bridge.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1482 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/layers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21213 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/models/sequence_to_sequence.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/models/sequence_classifier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8039 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/models/sequence_tagger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6380 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/models/transformer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11872 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/models/catalog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10023 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/models/language_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13832 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/models/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9419 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/schedules/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7411 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/schedules/lr_schedules.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      476 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/schedules/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10887 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/checkpoint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12780 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      627 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/ter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3001 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/exporters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      664 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/tensor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3022 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/fmeasure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19873 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/decoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      648 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7121 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/losses.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3894 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/scorers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1391 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/utils/wer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13494 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/evaluation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/tokenizers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1336 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/tokenizers/opennmt_tokenizer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      512 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/tokenizers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11582 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/tokenizers/tokenizer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      542 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-06 08:28:35.000000 OpenNMT-tf-2.9.3/opennmt/decoders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16540 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/decoders/decoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9668 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/decoders/rnn_decoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7077 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/decoders/self_attention_decoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/opennmt/decoders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2020-05-06 08:19:03.000000 OpenNMT-tf-2.9.3/setup.py
```

### Comparing `OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/PKG-INFO` & `OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenNMT-tf
-Version: 2.9.2
+Version: 2.9.3
 Summary: Neural machine translation and sequence learning using TensorFlow
 Home-page: https://opennmt.net
 Author: OpenNMT
 Author-email: guillaume.klein@systrangroup.com
 License: MIT
 Project-URL: Documentation, https://opennmt.net/OpenNMT-tf/
 Project-URL: Forum, https://forum.opennmt.net/
```

### Comparing `OpenNMT-tf-2.9.2/OpenNMT_tf.egg-info/SOURCES.txt` & `OpenNMT-tf-2.9.3/OpenNMT_tf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/PKG-INFO` & `OpenNMT-tf-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenNMT-tf
-Version: 2.9.2
+Version: 2.9.3
 Summary: Neural machine translation and sequence learning using TensorFlow
 Home-page: https://opennmt.net
 Author: OpenNMT
 Author-email: guillaume.klein@systrangroup.com
 License: MIT
 Project-URL: Documentation, https://opennmt.net/OpenNMT-tf/
 Project-URL: Forum, https://forum.opennmt.net/
```

### Comparing `OpenNMT-tf-2.9.2/README.md` & `OpenNMT-tf-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/training.py` & `OpenNMT-tf-2.9.3/opennmt/training.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/optimizers/utils.py` & `OpenNMT-tf-2.9.3/opennmt/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/runner.py` & `OpenNMT-tf-2.9.3/opennmt/runner.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/inputters/record_inputter.py` & `OpenNMT-tf-2.9.3/opennmt/inputters/record_inputter.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/inputters/inputter.py` & `OpenNMT-tf-2.9.3/opennmt/inputters/inputter.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/inputters/text_inputter.py` & `OpenNMT-tf-2.9.3/opennmt/inputters/text_inputter.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/inputters/__init__.py` & `OpenNMT-tf-2.9.3/opennmt/inputters/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/encoders/self_attention_encoder.py` & `OpenNMT-tf-2.9.3/opennmt/encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/encoders/rnn_encoder.py` & `OpenNMT-tf-2.9.3/opennmt/encoders/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/encoders/conv_encoder.py` & `OpenNMT-tf-2.9.3/opennmt/encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/encoders/__init__.py` & `OpenNMT-tf-2.9.3/opennmt/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/encoders/encoder.py` & `OpenNMT-tf-2.9.3/opennmt/encoders/encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/data/text.py` & `OpenNMT-tf-2.9.3/opennmt/data/text.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/data/vocab.py` & `OpenNMT-tf-2.9.3/opennmt/data/vocab.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/data/dataset.py` & `OpenNMT-tf-2.9.3/opennmt/data/dataset.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/data/__init__.py` & `OpenNMT-tf-2.9.3/opennmt/data/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/data/noise.py` & `OpenNMT-tf-2.9.3/opennmt/data/noise.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/bin/tokenize_text.py` & `OpenNMT-tf-2.9.3/opennmt/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/bin/build_vocab.py` & `OpenNMT-tf-2.9.3/opennmt/bin/build_vocab.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/bin/ark_to_records.py` & `OpenNMT-tf-2.9.3/opennmt/bin/ark_to_records.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/bin/detokenize_text.py` & `OpenNMT-tf-2.9.3/opennmt/bin/detokenize_text.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/bin/main.py` & `OpenNMT-tf-2.9.3/opennmt/bin/main.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/layers/position.py` & `OpenNMT-tf-2.9.3/opennmt/layers/position.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/layers/common.py` & `OpenNMT-tf-2.9.3/opennmt/layers/common.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/layers/rnn.py` & `OpenNMT-tf-2.9.3/opennmt/layers/rnn.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/layers/reducer.py` & `OpenNMT-tf-2.9.3/opennmt/layers/reducer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/layers/transformer.py` & `OpenNMT-tf-2.9.3/opennmt/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/layers/bridge.py` & `OpenNMT-tf-2.9.3/opennmt/layers/bridge.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/layers/__init__.py` & `OpenNMT-tf-2.9.3/opennmt/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/models/sequence_to_sequence.py` & `OpenNMT-tf-2.9.3/opennmt/models/sequence_to_sequence.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/models/sequence_classifier.py` & `OpenNMT-tf-2.9.3/opennmt/models/sequence_classifier.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/models/sequence_tagger.py` & `OpenNMT-tf-2.9.3/opennmt/models/sequence_tagger.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/models/transformer.py` & `OpenNMT-tf-2.9.3/opennmt/models/transformer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/models/catalog.py` & `OpenNMT-tf-2.9.3/opennmt/models/catalog.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/models/language_model.py` & `OpenNMT-tf-2.9.3/opennmt/models/language_model.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/models/__init__.py` & `OpenNMT-tf-2.9.3/opennmt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/models/model.py` & `OpenNMT-tf-2.9.3/opennmt/models/model.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/config.py` & `OpenNMT-tf-2.9.3/opennmt/config.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/schedules/lr_schedules.py` & `OpenNMT-tf-2.9.3/opennmt/schedules/lr_schedules.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/checkpoint.py` & `OpenNMT-tf-2.9.3/opennmt/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/misc.py` & `OpenNMT-tf-2.9.3/opennmt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/ter.py` & `OpenNMT-tf-2.9.3/opennmt/utils/ter.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/exporters.py` & `OpenNMT-tf-2.9.3/opennmt/utils/exporters.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/tensor.py` & `OpenNMT-tf-2.9.3/opennmt/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/fmeasure.py` & `OpenNMT-tf-2.9.3/opennmt/utils/fmeasure.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/decoding.py` & `OpenNMT-tf-2.9.3/opennmt/utils/decoding.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/compat.py` & `OpenNMT-tf-2.9.3/opennmt/utils/compat.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/losses.py` & `OpenNMT-tf-2.9.3/opennmt/utils/losses.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/scorers.py` & `OpenNMT-tf-2.9.3/opennmt/utils/scorers.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/__init__.py` & `OpenNMT-tf-2.9.3/opennmt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/utils/wer.py` & `OpenNMT-tf-2.9.3/opennmt/utils/wer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/evaluation.py` & `OpenNMT-tf-2.9.3/opennmt/evaluation.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/tokenizers/opennmt_tokenizer.py` & `OpenNMT-tf-2.9.3/opennmt/tokenizers/opennmt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/tokenizers/__init__.py` & `OpenNMT-tf-2.9.3/opennmt/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/tokenizers/tokenizer.py` & `OpenNMT-tf-2.9.3/opennmt/tokenizers/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
     Returns:
       A 1-D string ``tf.Tensor``.
     """
     def _python_wrapper(string_t):
       string = tf.compat.as_text(string_t.numpy())
       tokens = self._tokenize_string(string)
-      return tf.constant(tokens)
+      return tf.constant(tokens, dtype=tf.string)
     tokens = tf.py_function(_python_wrapper, [text], tf.string)
     tokens.set_shape([None])
     return tokens
 
   def _tokenize_batch_tensor(self, text):
     """Tokenizes a batch of texts.
```

### Comparing `OpenNMT-tf-2.9.2/opennmt/__init__.py` & `OpenNMT-tf-2.9.3/opennmt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """OpenNMT module."""
 
-__version__ = "2.9.2"
+__version__ = "2.9.3"
 
 from opennmt.config import convert_to_v2_config
 from opennmt.config import load_config
 from opennmt.config import load_model
 
 from opennmt.constants import END_OF_SENTENCE_ID
 from opennmt.constants import END_OF_SENTENCE_TOKEN
```

### Comparing `OpenNMT-tf-2.9.2/opennmt/decoders/decoder.py` & `OpenNMT-tf-2.9.3/opennmt/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/decoders/rnn_decoder.py` & `OpenNMT-tf-2.9.3/opennmt/decoders/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/opennmt/decoders/self_attention_decoder.py` & `OpenNMT-tf-2.9.3/opennmt/decoders/self_attention_decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-tf-2.9.2/setup.py` & `OpenNMT-tf-2.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def get_long_description():
     readme_path = os.path.join(os.path.dirname(__file__), "README.md")
     with open(readme_path, encoding="utf-8") as readme_file:
         return readme_file.read()
 
 setup(
     name="OpenNMT-tf",
-    version="2.9.2",
+    version="2.9.3",
     license="MIT",
     description="Neural machine translation and sequence learning using TensorFlow",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="OpenNMT",
     author_email="guillaume.klein@systrangroup.com",
     url="https://opennmt.net",
```

