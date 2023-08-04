# Comparing `tmp/hezar-0.19.0.tar.gz` & `tmp/hezar-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.19.0.tar", max compression
+gzip compressed data, was "hezar-0.20.0.tar", max compression
```

## Comparing `hezar-0.19.0.tar` & `hezar-0.20.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1065 2023-08-03 08:30:44.744121 hezar-0.19.0/LICENSE
--rw-r--r--   0        0        0     3698 2023-08-03 08:30:44.744121 hezar-0.19.0/README.md
--rw-r--r--   0        0        0      260 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/__init__.py
--rw-r--r--   0        0        0     5336 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/builders.py
--rw-r--r--   0        0        0    11489 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/configs.py
--rw-r--r--   0        0        0     2072 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/__init__.py
--rw-r--r--   0        0        0     6365 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      312 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1709 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4502 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3627 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     3555 2023-08-03 08:30:44.744121 hezar-0.19.0/hezar/data/datasets/text_summarization.py
--rw-r--r--   0        0        0       26 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      273 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1604 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1676 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1634 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11719 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/model.py
--rw-r--r--   0        0        0      152 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3971 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     4132 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      877 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0       47 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text2text/__init__.py
--rw-r--r--   0        0        0       89 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text2text/t5/__init__.py
--rw-r--r--   0        0        0     3838 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text2text/t5/t5_text2text.py
--rw-r--r--   0        0        0      764 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text2text/t5/t5_text2text_config.py
--rw-r--r--   0        0        0      240 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3530 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3666 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3809 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0      142 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     3603 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/normalizer.py
--rw-r--r--   0        0        0     4119 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      324 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4965 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    19342 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8828 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2644 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2243 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17688 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      164 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5614 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3660 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/logging.py
--rw-r--r--   0        0        0      936 2023-08-03 08:30:44.748121 hezar-0.19.0/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     1648 2023-08-03 08:30:44.748121 hezar-0.19.0/pyproject.toml
--rw-r--r--   0        0        0     6180 1970-01-01 00:00:00.000000 hezar-0.19.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-04 08:49:04.037069 hezar-0.20.0/LICENSE
+-rw-r--r--   0        0        0     4145 2023-08-04 08:49:04.037069 hezar-0.20.0/README.md
+-rw-r--r--   0        0        0      260 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5336 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/builders.py
+-rw-r--r--   0        0        0    11489 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/configs.py
+-rw-r--r--   0        0        0     2072 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6365 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      320 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1758 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4545 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3653 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     3581 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0       26 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      273 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1614 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1686 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1644 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11719 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/model.py
+-rw-r--r--   0        0        0      152 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3981 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     4142 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text2text/__init__.py
+-rw-r--r--   0        0        0       89 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text2text/t5/__init__.py
+-rw-r--r--   0        0        0     3848 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text2text/t5/t5_text2text.py
+-rw-r--r--   0        0        0      764 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text2text/t5/t5_text2text_config.py
+-rw-r--r--   0        0        0      240 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3540 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3676 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3819 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     4119 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     3633 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      324 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4965 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    19342 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8828 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2644 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2282 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17990 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      164 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5614 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3660 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0      936 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     1648 2023-08-04 08:49:04.045070 hezar-0.20.0/pyproject.toml
+-rw-r--r--   0        0        0     6627 1970-01-01 00:00:00.000000 hezar-0.20.0/PKG-INFO
```

### Comparing `hezar-0.19.0/LICENSE` & `hezar-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/README.md` & `hezar-0.20.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 ![](hezar.png)
 
-_<p align="center"> A seamless AI library for Persian</p>_
+_<p align="center"> A seamless multi-task AI library for Persian</p>_
 
 **Hezar** (meaning **_thousand_** in Persian) is a multipurpose AI library built to make AI easy for the Persian community!
 
 Hezar is a library that:
 - brings together all the best works in AI for Persian
 - makes using AI models as easy as a couple of lines of code
 - seamlessly integrates with Hugging Face Hub for all of its models
@@ -27,27 +27,39 @@
 pip install ./hezar
 ```
 
 ## Quick Tour
 ### Ready-to-use models from Hub
 There's a bunch of ready-to-use trained models for different tasks on the Hub. See them [here](https://huggingface.co/hezarai)!
 
-For example, you can grab a BERT-based model for sentiment analysis like so: 
+#### Text classification (sentiment analysis) 
 ```python
 from hezar import Model
 
 example = ["هزار، کتابخانه‌ای کامل برای به کارگیری آسان هوش مصنوعی"]
 model = Model.load("hezarai/bert-fa-sentiment-digikala-snappfood")
 outputs = model.predict(example)
 print(outputs)
 ```
 ```commandline
 {'labels': ['positive'], 'probs': [0.812910258769989]}
 ```
+#### Sequence labeling (part-of-speech tagging)
+```python
+from hezar import Model
 
+hub_path = "hezarai/bert-fa-pos-lscp-500k"
+model = Model.load(hub_path)
+inputs = ["سلام بر فارسی زبانان شریف"]
+outputs = model.predict(inputs)
+print(outputs)
+```
+```commandline
+[[{'token': 'سلام', 'tag': 'N'}, {'token': 'بر', 'tag': 'P'}, {'token': 'فارسی', 'tag': 'Ne'}, {'token': 'زبانان', 'tag': 'Ne'}, {'token': 'شریف', 'tag': 'AJ'}]]
+```
 ### Write your own model
 It's fairly easy to extend this library or add your own model. Hezar has its own `Model` base class that is simply a normal PyTorch `nn.Module` but with some extra features!
 
 Here's a simple example:
 ```python
 from dataclasses import dataclass
```

### Comparing `hezar-0.19.0/hezar/builders.py` & `hezar-0.20.0/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/configs.py` & `hezar-0.20.0/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/constants.py` & `hezar-0.20.0/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/data/data_collators.py` & `hezar-0.20.0/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/data/datasets/dataset.py` & `hezar-0.20.0/hezar/data/datasets/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 from typing import Optional, Union
 
 from torch.utils.data import Dataset as TorchDataset
 
 from ...configs import DatasetConfig
-from ...constants import DEFAULT_DATASET_CONFIG_FILE, ConfigType, RepoType, SplitType
+from ...constants import DEFAULT_DATASET_CONFIG_FILE, ConfigType, RepoType, SplitType, HEZAR_CACHE_DIR
 from ...utils import get_module_class
 
 
 class Dataset(TorchDataset):
     """
     Base class for all datasets in Hezar.
 
     Args:
         config:
         **kwargs:
     """
     config_filename = DEFAULT_DATASET_CONFIG_FILE
+    cache_dir = HEZAR_CACHE_DIR
 
     def __init__(self, config: DatasetConfig, **kwargs):
         self.config = config.update(kwargs)
         self.preprocessor = None
         self.data_collator = None
 
     def __len__(self):
```

### Comparing `hezar-0.19.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.20.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Dict, List, Tuple
 
 from datasets import load_dataset
 
 from ...configs import DatasetConfig
-from ...constants import TaskType
+from ...constants import TaskType, HEZAR_CACHE_DIR
 from ...preprocessors import Tokenizer
 from ...registry import register_dataset
 from ...utils import get_logger
 from ..data_collators import SequenceLabelingDataCollator
 from .dataset import Dataset
 
 
@@ -56,15 +56,15 @@
         Args:
             split: Dataset split
 
         Returns:
             The whole dataset
         """
         # TODO: In case we want to make this class work on other types like csv, json, etc. we have to do it here.
-        dataset = load_dataset(self.config.path, split=split)
+        dataset = load_dataset(self.config.path, split=split, cache_dir=self.cache_dir)
         return dataset
 
     def _build_tokenizer(self):
         if self.config.tokenizer_path:
             tokenizer = Tokenizer.load(self.config.tokenizer_path)
         else:
             logger.warning("This dataset requires a tokenizer to work. Provide it in config as `tokenizer_path` "
```

### Comparing `hezar-0.19.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.20.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         Args:
             split: Dataset split
 
         Returns:
             The whole dataset
         """
         # TODO: In case we want to make this class work on other types like csv, json, etc. we have to do it here.
-        dataset = load_dataset(self.config.path, split=split)
+        dataset = load_dataset(self.config.path, split=split, cache_dir=self.cache_dir)
         return dataset
 
     def _build_tokenizer(self):
         if self.config.tokenizer_path:
             tokenizer = Tokenizer.load(self.config.tokenizer_path)
         else:
             logger.warning("This dataset requires a tokenizer to work. Provide it in config as `tokenizer_path` "
```

### Comparing `hezar-0.19.0/hezar/data/datasets/text_summarization.py` & `hezar-0.20.0/hezar/data/datasets/text_summarization_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         Args:
             split: Dataset split
 
         Returns:
             The whole dataset
         """
         # TODO: In case we want to make this class work on other types like csv, json, etc. we have to do it here.
-        dataset = load_dataset(self.config.path, split=split)
+        dataset = load_dataset(self.config.path, split=split, cache_dir=self.cache_dir)
         return dataset
 
     def _build_tokenizer(self):
         if self.config.tokenizer_path:
             tokenizer = Tokenizer.load(self.config.tokenizer_path)
         else:
             logger.warning("This dataset requires a tokenizer to work. Provide it in config as `tokenizer_path` "
```

### Comparing `hezar-0.19.0/hezar/data/utils/data_utils.py` & `hezar-0.20.0/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/embeddings/embedding.py` & `hezar-0.20.0/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/embeddings/fasttext.py` & `hezar-0.20.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/embeddings/word2vec.py` & `hezar-0.20.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/metrics/f1.py` & `hezar-0.20.0/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/metrics/metric.py` & `hezar-0.20.0/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/metrics/recall.py` & `hezar-0.20.0/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/metrics/seqeval.py` & `hezar-0.20.0/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.20.0/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,16 @@
             **kwargs,
         )
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["wordpiece_tokenizer"]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         hidden_states = inputs.get("hidden_states", None)
```

### Comparing `hezar-0.19.0/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.20.0/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.20.0/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,16 @@
             **kwargs,
         )
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["wordpiece_tokenizer"]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         hidden_states = inputs.get("hidden_states", None)
```

### Comparing `hezar-0.19.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.20.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.20.0/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,16 @@
             **kwargs,
         )
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["bpe_tokenizer"]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         hidden_states = inputs.get("hidden_states", None)
```

### Comparing `hezar-0.19.0/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.20.0/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/model.py` & `hezar-0.20.0/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.20.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
             **inputs
         }
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["wordpiece_tokenizer"]
         inputs = tokenizer(
             inputs,
             return_word_ids=True,
             return_tokens=True,
             padding=True,
```

### Comparing `hezar-0.19.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.20.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.20.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,16 @@
             **inputs
         }
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["wordpiece_tokenizer"]
         inputs = tokenizer(
             inputs,
             return_word_ids=True,
             return_tokens=True,
             padding=True,
```

### Comparing `hezar-0.19.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.20.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/text2text/t5/t5_text2text.py` & `hezar-0.20.0/hezar/models/text2text/t5/t5_text2text.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
             outputs = {"output_ids": output_ids}
 
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["sentencepiece_unigram_tokenizer"]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         records = []
```

### Comparing `hezar-0.19.0/hezar/models/text2text/t5/t5_text2text_config.py` & `hezar-0.20.0/hezar/models/text2text/t5/t5_text2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.20.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
             "attentions": lm_outputs.attentions,
         }
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["wordpiece_tokenizer"]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs) -> Dict:
         logits = inputs["logits"]
```

### Comparing `hezar-0.19.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.20.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.20.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             "attentions": lm_outputs.attentions,
         }
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["wordpiece_tokenizer"]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs) -> Dict:
         logits = inputs["logits"]
```

### Comparing `hezar-0.19.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.20.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.20.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,16 +52,16 @@
             "attentions": lm_outputs.attentions,
         }
         return outputs
 
     def preprocess(self, inputs: Union[str, List[str]], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
-        if "normalizer" in self.preprocessor:
-            normalizer = self.preprocessor["normalizer"]
+        if "text_normalizer" in self.preprocessor:
+            normalizer = self.preprocessor["text_normalizer"]
             inputs = normalizer(inputs)
         tokenizer = self.preprocessor["bpe_tokenizer"]
         inputs = tokenizer(inputs, return_tensors="pt", device=self.device)
         return inputs
 
     def post_process(self, inputs, **kwargs):
         logits = inputs["logits"]
```

### Comparing `hezar-0.19.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.20.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/preprocessors/normalizer.py` & `hezar-0.20.0/hezar/preprocessors/text_normalizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 from .preprocessor import Preprocessor
 
 
 logger = get_logger(__name__)
 
 
 @dataclass
-class NormalizerConfig(PreprocessorConfig):
-    name: str = field(default="normalizer")
+class TextNormalizerConfig(PreprocessorConfig):
+    name: str = field(default="text_normalizer")
     replace_pattern: str = None
     nfkd: bool = True
     nfkc: bool = True
 
 
-@register_preprocessor("normalizer", config_class=NormalizerConfig)
-class Normalizer(Preprocessor):
+@register_preprocessor("text_normalizer", config_class=TextNormalizerConfig)
+class TextNormalizer(Preprocessor):
     """
     A simple configurable text normalizer
     """
     preprocessor_subfolder = DEFAULT_PREPROCESSOR_SUBFOLDER
     normalizer_config_file = DEFAULT_NORMALIZER_CONFIG_FILE
 
-    def __init__(self, config: NormalizerConfig, **kwargs):
+    def __init__(self, config: TextNormalizerConfig, **kwargs):
         super().__init__(config, **kwargs)
 
     def __call__(
         self,
         inputs: Union[str, List[str]],
         replace_pattern: str = None,
         nfkd: bool = None,
@@ -64,15 +64,15 @@
         hub_or_local_path,
         subfolder=None,
         config_filename=None,
         **kwargs
     ):
         config_filename = config_filename or cls.normalizer_config_file
         subfolder = subfolder or cls.preprocessor_subfolder
-        config = NormalizerConfig.load(
+        config = TextNormalizerConfig.load(
             hub_or_local_path,
             filename=config_filename,
             subfolder=subfolder,
         )
         normalizer = build_preprocessor(config.name, config, **kwargs)
         return normalizer
```

### Comparing `hezar-0.19.0/hezar/preprocessors/preprocessor.py` & `hezar-0.20.0/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.20.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.20.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.20.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.20.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.20.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/registry.py` & `hezar-0.20.0/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.20.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.20.0/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 
 import numpy as np
 import torch
 
-from hezar.constants import MetricType
 
+from ...constants import MetricType
 from ...configs import TrainerConfig
 from ...data.datasets import Dataset
 from ...models import Model
 from ...utils import get_logger
 from ..trainer import Trainer
 
 
@@ -21,14 +21,15 @@
 
     Args:
         model ([`Model`] or `torch.nn.Module`): The main model to train and evaluate
         config (TrainerConfig): Training configuration and parameters
         train_dataset (Dataset): Train dataset
         eval_dataset (Dataset): Evaluation dataset
         data_collator: Collate function, usually included in the dataset object itself
+        preprocessor: Preprocessor object
         optimizer (optim.Optimizer): Model optimizer
         lr_scheduler: Optional learning-rate scheduler
 
     """
     AVAILABLE_METRICS = [
         MetricType.ACCURACY,
         MetricType.RECALL,
```

### Comparing `hezar-0.19.0/hezar/trainers/trainer.py` & `hezar-0.20.0/hezar/trainers/trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     "reduce_on_plateau": torch.optim.lr_scheduler.ReduceLROnPlateau,
     "cosine_lr": torch.optim.lr_scheduler.CosineAnnealingLR,
 }
 
 
 class Trainer:
     """
-    A general but fully featured model trainer/evaluator for Hezar models.
+    Base trainer class for training all Hezar models. This class is inherited by other task-specific trainers which
+    implement their own customized functionalities  (`compute_loss()` and `compute_metrics()` in most cases).
 
     Args:
         model ([`Model`] or `torch.nn.Module`): The main model to train and evaluate
         config (TrainerConfig): Training configuration and parameters
         train_dataset (Dataset): Train dataset
         eval_dataset (Dataset): Evaluation dataset
         data_collator: Collate function, usually included in the dataset object itself
@@ -106,16 +107,14 @@
         np.random.seed(seed)
         random.seed(seed)
 
     def _prepare_model(self, model: Model) -> Model:
         """
         Download the model from HuggingFace Hub if `init_weights_from` is given in the config. Load the model to the
         device and return it.
-        :param model:
-        :return:
         """
         if model is None:
             raise ValueError("`model` must be given to the Trainer!")
         hub_path = self.config.init_weights_from
         if hub_path is not None:
             local_path = hf_hub_download(hub_path, filename=model.model_filename, cache_dir=HEZAR_CACHE_DIR)
             model.load_state_dict(torch.load(local_path, map_location="cpu"))
@@ -251,15 +250,17 @@
         Returns:
             The loss tensor
         """
         raise NotImplementedError
 
     def compute_metrics(self, predictions, labels, **kwargs) -> Dict[str, float]:
         """
-        Compute metric values on the predictions and labels
+        Compute metric values on the predictions and labels. This method must be implemented in derived classes but in
+        case a trainer does not support any metric, this method will output an empty dict so that the training works
+        fine.
 
         Args:
             predictions: A list of all predictions
             labels: A list of all labels
 
         Returns:
             A dictionary of the results for every metric specified by the trainer
```

### Comparing `hezar-0.19.0/hezar/trainers/trainer_utils.py` & `hezar-0.20.0/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/utils/common_utils.py` & `hezar-0.20.0/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/utils/core_utils.py` & `hezar-0.20.0/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/utils/hub_utils.py` & `hezar-0.20.0/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/hezar/utils/registry_utils.py` & `hezar-0.20.0/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.19.0/pyproject.toml` & `hezar-0.20.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.19.0"
+version = "0.20.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.19.0/PKG-INFO` & `hezar-0.20.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.19.0
+Version: 0.20.0
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
@@ -35,15 +35,15 @@
 Project-URL: Documentation, https://github.com/hezarai/docs
 Project-URL: Repository, https://github.com/hezarai/hezar
 Description-Content-Type: text/markdown
 
 
 ![](hezar.png)
 
-_<p align="center"> A seamless AI library for Persian</p>_
+_<p align="center"> A seamless multi-task AI library for Persian</p>_
 
 **Hezar** (meaning **_thousand_** in Persian) is a multipurpose AI library built to make AI easy for the Persian community!
 
 Hezar is a library that:
 - brings together all the best works in AI for Persian
 - makes using AI models as easy as a couple of lines of code
 - seamlessly integrates with Hugging Face Hub for all of its models
@@ -65,27 +65,39 @@
 pip install ./hezar
 ```
 
 ## Quick Tour
 ### Ready-to-use models from Hub
 There's a bunch of ready-to-use trained models for different tasks on the Hub. See them [here](https://huggingface.co/hezarai)!
 
-For example, you can grab a BERT-based model for sentiment analysis like so: 
+#### Text classification (sentiment analysis) 
 ```python
 from hezar import Model
 
 example = ["هزار، کتابخانه‌ای کامل برای به کارگیری آسان هوش مصنوعی"]
 model = Model.load("hezarai/bert-fa-sentiment-digikala-snappfood")
 outputs = model.predict(example)
 print(outputs)
 ```
 ```commandline
 {'labels': ['positive'], 'probs': [0.812910258769989]}
 ```
+#### Sequence labeling (part-of-speech tagging)
+```python
+from hezar import Model
 
+hub_path = "hezarai/bert-fa-pos-lscp-500k"
+model = Model.load(hub_path)
+inputs = ["سلام بر فارسی زبانان شریف"]
+outputs = model.predict(inputs)
+print(outputs)
+```
+```commandline
+[[{'token': 'سلام', 'tag': 'N'}, {'token': 'بر', 'tag': 'P'}, {'token': 'فارسی', 'tag': 'Ne'}, {'token': 'زبانان', 'tag': 'Ne'}, {'token': 'شریف', 'tag': 'AJ'}]]
+```
 ### Write your own model
 It's fairly easy to extend this library or add your own model. Hezar has its own `Model` base class that is simply a normal PyTorch `nn.Module` but with some extra features!
 
 Here's a simple example:
 ```python
 from dataclasses import dataclass
```

