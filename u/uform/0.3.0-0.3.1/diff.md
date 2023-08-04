# Comparing `tmp/uform-0.3.0.tar.gz` & `tmp/uform-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uform-0.3.0.tar", last modified: Tue Aug  1 11:25:08 2023, max compression
+gzip compressed data, was "uform-0.3.1.tar", last modified: Fri Aug  4 12:55:07 2023, max compression
```

## Comparing `uform-0.3.0.tar` & `uform-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:08.020973 uform-0.3.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11356 2023-08-01 11:24:56.000000 uform-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-08-01 11:25:08.020973 uform-0.3.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7482 2023-08-01 11:24:56.000000 uform-0.3.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1474 2023-08-01 11:24:56.000000 uform-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:25:08.020973 uform-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:08.020973 uform-0.3.0/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:24:56.000000 uform-0.3.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:25:08.020973 uform-0.3.0/src/uform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-08-01 11:25:08.000000 uform-0.3.0/src/uform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-01 11:25:08.000000 uform-0.3.0/src/uform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:25:08.000000 uform-0.3.0/src/uform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:25:08.000000 uform-0.3.0/src/uform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:25:08.000000 uform-0.3.0/src/uform.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    16681 2023-08-01 11:24:56.000000 uform-0.3.0/src/uform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:55:07.257181 uform-0.3.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11356 2023-08-04 12:54:52.000000 uform-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-08-04 12:55:07.257181 uform-0.3.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7753 2023-08-04 12:54:52.000000 uform-0.3.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1570 2023-08-04 12:54:52.000000 uform-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:55:07.257181 uform-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:55:07.253181 uform-0.3.1/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:54:52.000000 uform-0.3.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-08-04 12:54:52.000000 uform-0.3.1/src/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:55:07.253181 uform-0.3.1/src/uform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-08-04 12:55:07.000000 uform-0.3.1/src/uform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-04 12:55:07.000000 uform-0.3.1/src/uform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:55:07.000000 uform-0.3.1/src/uform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 12:55:07.000000 uform-0.3.1/src/uform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:55:07.000000 uform-0.3.1/src/uform.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-08-04 12:54:52.000000 uform-0.3.1/src/uform.py
```

### Comparing `uform-0.3.0/LICENSE` & `uform-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uform-0.3.0/PKG-INFO` & `uform-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: uform
-Version: 0.3.0
+Version: 0.3.1
 Summary: Multi-Modal Transformers library for Semantic Search and other Vision-Language tasks
-Author-email: Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
-Maintainer-email: unum <info@unum.cloud>
+Author-email: Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>, Ash Vardanian <ash.vardanian@unum.cloud>
+Maintainer-email: Unum Cloud <info@unum.cloud>
 Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -73,14 +73,16 @@
 
 ## Installation
 
 ```bash
 pip install uform
 ```
 
+UForm v0.3.0 and below depends on `transformers` and `timm` libraries, all newer versions depend only on PyTorch (except libraries for the text tokenization and checkpoint downloading). For the best performance, Pytorch v2.0.0 and above is recommended.
+
 ## Usage
 
 To load the model:
 
 ```python
 import uform
 
@@ -198,16 +200,16 @@
 | Code     | Language | #    | Code     | Language             | #    | Code     | Language |
 | :------- | :------- | :--- | :------- | :------------------- | :--- | :------- | :------- |
 | eng_Latn | English  | #    | fra_Latn | French               | #    | kor_Hang | Korean   |
 | deu_Latn | German   | #    | ita_Latn | Italian              | #    | pol_Latn | Polish   |
 | ita_Latn | Spanish  | #    | jpn_Jpan | Japanese             | #    | rus_Cyrl | Russian  |
 | tur_Latn | Turkish  | #    | zho_Hans | Chinese (Simplified) | #    | .        | .        |
 
-[weights-e]: https://huggingface.co/unum-cloud/uform/resolve/main/english/weight.pt
-[weights-m]: https://huggingface.co/unum-cloud/uform/resolve/main/multilingual/weight.pt
+[weights-e]: https://huggingface.co/unum-cloud/uform-vl-english/resolve/main/torch_weight.pt
+[weights-m]: https://huggingface.co/unum-cloud/uform-vl-multilingual/resolve/main/torch_weight.pt
 
 ### Performance
 
 On RTX 3090, the following performance is expected from `uform` on text encoding.
 
 | Model                     | Multilingual | Sequences per Second |    Speedup |
 | :------------------------ | -----------: | -------------------: | ---------: |
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: uform Version: 0.3.0 Summary: Multi-Modal
+Metadata-Version: 2.1 Name: uform Version: 0.3.1 Summary: Multi-Modal
 Transformers library for Semantic Search and other Vision-Language tasks
 Author-email: Mikhail Kim
 kim@unum.cloud>, Vladimir Orshulevich
-orshulevich@unum.cloud> Maintainer-email: unum
+orshulevich@unum.cloud>, Ash Vardanian
+vardanian@unum.cloud> Maintainer-email: Unum Cloud
 unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
 Engineering :: Image Recognition Classifier: Natural Language :: English
@@ -38,67 +39,70 @@
 both modalities jointly so they can take into account fine-grained features.
 Usually, these models are used for re-ranking relatively small retrieval
 results. __Mid-fusion models__ are the golden midpoint between the previous two
 types. Mid-fusion models consist of two parts â unimodal and multimodal. The
 unimodal part allows encoding each modality separately as late-fusion models
 do. The multimodal part takes unimodal features from the unimodal part as input
 and enhances them with a cross-attention mechanism. This tiny package will help
-you deal with the last! ## Installation ```bash pip install uform ``` ## Usage
-To load the model: ```python import uform model = uform.get_model('unum-cloud/
-uform-vl-english') model = uform.get_model('unum-cloud/uform-vl-multilingual')
-``` You can also load your own Mid-fusion model. Just upload it on HuggingFace
-and pass model name to `get_model`. To encode data: ```python from PIL import
-Image text = 'a small red panda in a zoo' image = Image.open('red_panda.jpg')
-image_data = model.preprocess_image(image) text_data = model.preprocess_text
-(text) image_embedding = model.encode_image(image_data) text_embedding =
-model.encode_text(text_data) joint_embedding = model.encode_multimodal
-(image=image_data, text=text_data) ``` Retrieving features is also trivial:
-```python image_features, image_embedding = model.encode_image(image_data,
-return_features=True) text_features, text_embedding = model.encode_text
-(text_data, return_features=True) ``` These features can later be used to
-produce joint multimodal encodings faster, as the first layers of the
-transformer can be skipped: ```python joint_embedding = model.encode_multimodal
-( image_features=image_features, text_features=text_features,
-attention_mask=text_data['attention_mask'] ) ``` ### Remote Procedure Calls for
-Cloud Deployments You can also use our larger, faster, better proprietary
-models deployed in optimized cloud environments. For that, please, choose the
-cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm
-with optional dependencies: ```bash pip install uform[remote] ``` The only
-thing that changes after that is calling `get_client` with the IP address of
-your instance instead of using `get_model` for local usage. ```python model =
-uform.get_client('0.0.0.0:7000') ``` ## Evaluation There are two options to
-calculate semantic compatibility between an image and a text: [Cosine
-Similarity](#cosine-similarity) and [Matching Score](#matching-score). ###
-Cosine Similarity ```python import torch.nn.functional as F similarity =
-F.cosine_similarity(image_embedding, text_embedding) ``` The `similarity` will
-belong to the `[-1, 1]` range, `1` meaning the absolute match. __Pros__: -
-Computationally cheap. - Only unimodal embeddings are required, unimodal
-encoding is faster than joint encoding. - Suitable for retrieval in large
-collections. __Cons__: - Takes into account only coarse-grained features. ###
-Matching Score Unlike cosine similarity, unimodal embedding are not enough.
-Joint embedding will be needed and the resulting `score` will belong to the `
-[0, 1]` range, `1` meaning the absolute match. ```python score =
-model.get_matching_scores(joint_embedding) ``` __Pros__: - Joint embedding
-captures fine-grained features. - Suitable for re-ranking - sorting retrieval
-result. __Cons__: - Resource-intensive. - Not suitable for retrieval in large
-collections. ## Models ### Architecture | Model | Language Tower | Image Tower
-| Multimodal Part | URL | | :----------- | :------------: | :---------: | :----
----------: | ----------------------: | | English | BERT, 2 layers | ViT-B/16 |
-2 layers | [weights.pt][weights-e] | | Multilingual | BERT, 8 layers | ViT-B/16
-| 4 layers | [weights.pt][weights-m] | The Multilingual model supports 11
-languages, after being trained on a balanced dataset. For pre-training we used
-translated captions made with [NLLB](https://github.com/facebookresearch/
-fairseq/tree/nllb). | Code | Language | # | Code | Language | # | Code |
-Language | | :------- | :------- | :--- | :------- | :------------------- | :--
-- | :------- | :------- | | eng_Latn | English | # | fra_Latn | French | # |
-kor_Hang | Korean | | deu_Latn | German | # | ita_Latn | Italian | # | pol_Latn
-| Polish | | ita_Latn | Spanish | # | jpn_Jpan | Japanese | # | rus_Cyrl |
-Russian | | tur_Latn | Turkish | # | zho_Hans | Chinese (Simplified) | # | . |
-. | [weights-e]: https://huggingface.co/unum-cloud/uform/resolve/main/english/
-weight.pt [weights-m]: https://huggingface.co/unum-cloud/uform/resolve/main/
-multilingual/weight.pt ### Performance On RTX 3090, the following performance
-is expected from `uform` on text encoding. | Model | Multilingual | Sequences
-per Second | Speedup | | :------------------------ | -----------: | -----------
---------: | ---------: | | `bert-base-uncased` | No | 1'612 | | | `distilbert-
-base-uncased` | No | 3'174 | x 1.96 | | `MiniLM-L12` | Yes | 3'604 | x 2.24 | |
-`MiniLM-L6` | No | 6'107 | x 3.79 | | | | | | | `uform` | Yes | 6'809 | __x
-4.22__ |
+you deal with the last! ## Installation ```bash pip install uform ``` UForm
+v0.3.0 and below depends on `transformers` and `timm` libraries, all newer
+versions depend only on PyTorch (except libraries for the text tokenization and
+checkpoint downloading). For the best performance, Pytorch v2.0.0 and above is
+recommended. ## Usage To load the model: ```python import uform model =
+uform.get_model('unum-cloud/uform-vl-english') model = uform.get_model('unum-
+cloud/uform-vl-multilingual') ``` You can also load your own Mid-fusion model.
+Just upload it on HuggingFace and pass model name to `get_model`. To encode
+data: ```python from PIL import Image text = 'a small red panda in a zoo' image
+= Image.open('red_panda.jpg') image_data = model.preprocess_image(image)
+text_data = model.preprocess_text(text) image_embedding = model.encode_image
+(image_data) text_embedding = model.encode_text(text_data) joint_embedding =
+model.encode_multimodal(image=image_data, text=text_data) ``` Retrieving
+features is also trivial: ```python image_features, image_embedding =
+model.encode_image(image_data, return_features=True) text_features,
+text_embedding = model.encode_text(text_data, return_features=True) ``` These
+features can later be used to produce joint multimodal encodings faster, as the
+first layers of the transformer can be skipped: ```python joint_embedding =
+model.encode_multimodal( image_features=image_features,
+text_features=text_features, attention_mask=text_data['attention_mask'] ) ```
+### Remote Procedure Calls for Cloud Deployments You can also use our larger,
+faster, better proprietary models deployed in optimized cloud environments. For
+that, please, choose the cloud of liking, search the marketplace for "Unum
+UForm" and reinstall UForm with optional dependencies: ```bash pip install
+uform[remote] ``` The only thing that changes after that is calling
+`get_client` with the IP address of your instance instead of using `get_model`
+for local usage. ```python model = uform.get_client('0.0.0.0:7000') ``` ##
+Evaluation There are two options to calculate semantic compatibility between an
+image and a text: [Cosine Similarity](#cosine-similarity) and [Matching Score]
+(#matching-score). ### Cosine Similarity ```python import torch.nn.functional
+as F similarity = F.cosine_similarity(image_embedding, text_embedding) ``` The
+`similarity` will belong to the `[-1, 1]` range, `1` meaning the absolute
+match. __Pros__: - Computationally cheap. - Only unimodal embeddings are
+required, unimodal encoding is faster than joint encoding. - Suitable for
+retrieval in large collections. __Cons__: - Takes into account only coarse-
+grained features. ### Matching Score Unlike cosine similarity, unimodal
+embedding are not enough. Joint embedding will be needed and the resulting
+`score` will belong to the `[0, 1]` range, `1` meaning the absolute match.
+```python score = model.get_matching_scores(joint_embedding) ``` __Pros__: -
+Joint embedding captures fine-grained features. - Suitable for re-ranking -
+sorting retrieval result. __Cons__: - Resource-intensive. - Not suitable for
+retrieval in large collections. ## Models ### Architecture | Model | Language
+Tower | Image Tower | Multimodal Part | URL | | :----------- | :------------: |
+:---------: | :-------------: | ----------------------: | | English | BERT, 2
+layers | ViT-B/16 | 2 layers | [weights.pt][weights-e] | | Multilingual | BERT,
+8 layers | ViT-B/16 | 4 layers | [weights.pt][weights-m] | The Multilingual
+model supports 11 languages, after being trained on a balanced dataset. For
+pre-training we used translated captions made with [NLLB](https://github.com/
+facebookresearch/fairseq/tree/nllb). | Code | Language | # | Code | Language |
+# | Code | Language | | :------- | :------- | :--- | :------- | :--------------
+----- | :--- | :------- | :------- | | eng_Latn | English | # | fra_Latn |
+French | # | kor_Hang | Korean | | deu_Latn | German | # | ita_Latn | Italian |
+# | pol_Latn | Polish | | ita_Latn | Spanish | # | jpn_Jpan | Japanese | # |
+rus_Cyrl | Russian | | tur_Latn | Turkish | # | zho_Hans | Chinese (Simplified)
+| # | . | . | [weights-e]: https://huggingface.co/unum-cloud/uform-vl-english/
+resolve/main/torch_weight.pt [weights-m]: https://huggingface.co/unum-cloud/
+uform-vl-multilingual/resolve/main/torch_weight.pt ### Performance On RTX 3090,
+the following performance is expected from `uform` on text encoding. | Model |
+Multilingual | Sequences per Second | Speedup | | :------------------------ | -
+----------: | -------------------: | ---------: | | `bert-base-uncased` | No |
+1'612 | | | `distilbert-base-uncased` | No | 3'174 | x 1.96 | | `MiniLM-L12` |
+Yes | 3'604 | x 2.24 | | `MiniLM-L6` | No | 6'107 | x 3.79 | | | | | | |
+`uform` | Yes | 6'809 | __x 4.22__ |
```

### Comparing `uform-0.3.0/README.md` & `uform-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
 ## Installation
 
 ```bash
 pip install uform
 ```
 
+UForm v0.3.0 and below depends on `transformers` and `timm` libraries, all newer versions depend only on PyTorch (except libraries for the text tokenization and checkpoint downloading). For the best performance, Pytorch v2.0.0 and above is recommended.
+
 ## Usage
 
 To load the model:
 
 ```python
 import uform
 
@@ -168,22 +170,22 @@
 | Code     | Language | #    | Code     | Language             | #    | Code     | Language |
 | :------- | :------- | :--- | :------- | :------------------- | :--- | :------- | :------- |
 | eng_Latn | English  | #    | fra_Latn | French               | #    | kor_Hang | Korean   |
 | deu_Latn | German   | #    | ita_Latn | Italian              | #    | pol_Latn | Polish   |
 | ita_Latn | Spanish  | #    | jpn_Jpan | Japanese             | #    | rus_Cyrl | Russian  |
 | tur_Latn | Turkish  | #    | zho_Hans | Chinese (Simplified) | #    | .        | .        |
 
-[weights-e]: https://huggingface.co/unum-cloud/uform/resolve/main/english/weight.pt
-[weights-m]: https://huggingface.co/unum-cloud/uform/resolve/main/multilingual/weight.pt
+[weights-e]: https://huggingface.co/unum-cloud/uform-vl-english/resolve/main/torch_weight.pt
+[weights-m]: https://huggingface.co/unum-cloud/uform-vl-multilingual/resolve/main/torch_weight.pt
 
 ### Performance
 
 On RTX 3090, the following performance is expected from `uform` on text encoding.
 
 | Model                     | Multilingual | Sequences per Second |    Speedup |
 | :------------------------ | -----------: | -------------------: | ---------: |
 | `bert-base-uncased`       |           No |                1'612 |            |
 | `distilbert-base-uncased` |           No |                3'174 |     x 1.96 |
 | `MiniLM-L12`              |          Yes |                3'604 |     x 2.24 |
 | `MiniLM-L6`               |           No |                6'107 |     x 3.79 |
 |                           |              |                      |            |
-| `uform`                   |          Yes |                6'809 | __x 4.22__ |
+| `uform`                   |          Yes |                6'809 | __x 4.22__ |
```

#### html2text {}

```diff
@@ -19,67 +19,70 @@
 both modalities jointly so they can take into account fine-grained features.
 Usually, these models are used for re-ranking relatively small retrieval
 results. __Mid-fusion models__ are the golden midpoint between the previous two
 types. Mid-fusion models consist of two parts â unimodal and multimodal. The
 unimodal part allows encoding each modality separately as late-fusion models
 do. The multimodal part takes unimodal features from the unimodal part as input
 and enhances them with a cross-attention mechanism. This tiny package will help
-you deal with the last! ## Installation ```bash pip install uform ``` ## Usage
-To load the model: ```python import uform model = uform.get_model('unum-cloud/
-uform-vl-english') model = uform.get_model('unum-cloud/uform-vl-multilingual')
-``` You can also load your own Mid-fusion model. Just upload it on HuggingFace
-and pass model name to `get_model`. To encode data: ```python from PIL import
-Image text = 'a small red panda in a zoo' image = Image.open('red_panda.jpg')
-image_data = model.preprocess_image(image) text_data = model.preprocess_text
-(text) image_embedding = model.encode_image(image_data) text_embedding =
-model.encode_text(text_data) joint_embedding = model.encode_multimodal
-(image=image_data, text=text_data) ``` Retrieving features is also trivial:
-```python image_features, image_embedding = model.encode_image(image_data,
-return_features=True) text_features, text_embedding = model.encode_text
-(text_data, return_features=True) ``` These features can later be used to
-produce joint multimodal encodings faster, as the first layers of the
-transformer can be skipped: ```python joint_embedding = model.encode_multimodal
-( image_features=image_features, text_features=text_features,
-attention_mask=text_data['attention_mask'] ) ``` ### Remote Procedure Calls for
-Cloud Deployments You can also use our larger, faster, better proprietary
-models deployed in optimized cloud environments. For that, please, choose the
-cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm
-with optional dependencies: ```bash pip install uform[remote] ``` The only
-thing that changes after that is calling `get_client` with the IP address of
-your instance instead of using `get_model` for local usage. ```python model =
-uform.get_client('0.0.0.0:7000') ``` ## Evaluation There are two options to
-calculate semantic compatibility between an image and a text: [Cosine
-Similarity](#cosine-similarity) and [Matching Score](#matching-score). ###
-Cosine Similarity ```python import torch.nn.functional as F similarity =
-F.cosine_similarity(image_embedding, text_embedding) ``` The `similarity` will
-belong to the `[-1, 1]` range, `1` meaning the absolute match. __Pros__: -
-Computationally cheap. - Only unimodal embeddings are required, unimodal
-encoding is faster than joint encoding. - Suitable for retrieval in large
-collections. __Cons__: - Takes into account only coarse-grained features. ###
-Matching Score Unlike cosine similarity, unimodal embedding are not enough.
-Joint embedding will be needed and the resulting `score` will belong to the `
-[0, 1]` range, `1` meaning the absolute match. ```python score =
-model.get_matching_scores(joint_embedding) ``` __Pros__: - Joint embedding
-captures fine-grained features. - Suitable for re-ranking - sorting retrieval
-result. __Cons__: - Resource-intensive. - Not suitable for retrieval in large
-collections. ## Models ### Architecture | Model | Language Tower | Image Tower
-| Multimodal Part | URL | | :----------- | :------------: | :---------: | :----
----------: | ----------------------: | | English | BERT, 2 layers | ViT-B/16 |
-2 layers | [weights.pt][weights-e] | | Multilingual | BERT, 8 layers | ViT-B/16
-| 4 layers | [weights.pt][weights-m] | The Multilingual model supports 11
-languages, after being trained on a balanced dataset. For pre-training we used
-translated captions made with [NLLB](https://github.com/facebookresearch/
-fairseq/tree/nllb). | Code | Language | # | Code | Language | # | Code |
-Language | | :------- | :------- | :--- | :------- | :------------------- | :--
-- | :------- | :------- | | eng_Latn | English | # | fra_Latn | French | # |
-kor_Hang | Korean | | deu_Latn | German | # | ita_Latn | Italian | # | pol_Latn
-| Polish | | ita_Latn | Spanish | # | jpn_Jpan | Japanese | # | rus_Cyrl |
-Russian | | tur_Latn | Turkish | # | zho_Hans | Chinese (Simplified) | # | . |
-. | [weights-e]: https://huggingface.co/unum-cloud/uform/resolve/main/english/
-weight.pt [weights-m]: https://huggingface.co/unum-cloud/uform/resolve/main/
-multilingual/weight.pt ### Performance On RTX 3090, the following performance
-is expected from `uform` on text encoding. | Model | Multilingual | Sequences
-per Second | Speedup | | :------------------------ | -----------: | -----------
---------: | ---------: | | `bert-base-uncased` | No | 1'612 | | | `distilbert-
-base-uncased` | No | 3'174 | x 1.96 | | `MiniLM-L12` | Yes | 3'604 | x 2.24 | |
-`MiniLM-L6` | No | 6'107 | x 3.79 | | | | | | | `uform` | Yes | 6'809 | __x
-4.22__ |
+you deal with the last! ## Installation ```bash pip install uform ``` UForm
+v0.3.0 and below depends on `transformers` and `timm` libraries, all newer
+versions depend only on PyTorch (except libraries for the text tokenization and
+checkpoint downloading). For the best performance, Pytorch v2.0.0 and above is
+recommended. ## Usage To load the model: ```python import uform model =
+uform.get_model('unum-cloud/uform-vl-english') model = uform.get_model('unum-
+cloud/uform-vl-multilingual') ``` You can also load your own Mid-fusion model.
+Just upload it on HuggingFace and pass model name to `get_model`. To encode
+data: ```python from PIL import Image text = 'a small red panda in a zoo' image
+= Image.open('red_panda.jpg') image_data = model.preprocess_image(image)
+text_data = model.preprocess_text(text) image_embedding = model.encode_image
+(image_data) text_embedding = model.encode_text(text_data) joint_embedding =
+model.encode_multimodal(image=image_data, text=text_data) ``` Retrieving
+features is also trivial: ```python image_features, image_embedding =
+model.encode_image(image_data, return_features=True) text_features,
+text_embedding = model.encode_text(text_data, return_features=True) ``` These
+features can later be used to produce joint multimodal encodings faster, as the
+first layers of the transformer can be skipped: ```python joint_embedding =
+model.encode_multimodal( image_features=image_features,
+text_features=text_features, attention_mask=text_data['attention_mask'] ) ```
+### Remote Procedure Calls for Cloud Deployments You can also use our larger,
+faster, better proprietary models deployed in optimized cloud environments. For
+that, please, choose the cloud of liking, search the marketplace for "Unum
+UForm" and reinstall UForm with optional dependencies: ```bash pip install
+uform[remote] ``` The only thing that changes after that is calling
+`get_client` with the IP address of your instance instead of using `get_model`
+for local usage. ```python model = uform.get_client('0.0.0.0:7000') ``` ##
+Evaluation There are two options to calculate semantic compatibility between an
+image and a text: [Cosine Similarity](#cosine-similarity) and [Matching Score]
+(#matching-score). ### Cosine Similarity ```python import torch.nn.functional
+as F similarity = F.cosine_similarity(image_embedding, text_embedding) ``` The
+`similarity` will belong to the `[-1, 1]` range, `1` meaning the absolute
+match. __Pros__: - Computationally cheap. - Only unimodal embeddings are
+required, unimodal encoding is faster than joint encoding. - Suitable for
+retrieval in large collections. __Cons__: - Takes into account only coarse-
+grained features. ### Matching Score Unlike cosine similarity, unimodal
+embedding are not enough. Joint embedding will be needed and the resulting
+`score` will belong to the `[0, 1]` range, `1` meaning the absolute match.
+```python score = model.get_matching_scores(joint_embedding) ``` __Pros__: -
+Joint embedding captures fine-grained features. - Suitable for re-ranking -
+sorting retrieval result. __Cons__: - Resource-intensive. - Not suitable for
+retrieval in large collections. ## Models ### Architecture | Model | Language
+Tower | Image Tower | Multimodal Part | URL | | :----------- | :------------: |
+:---------: | :-------------: | ----------------------: | | English | BERT, 2
+layers | ViT-B/16 | 2 layers | [weights.pt][weights-e] | | Multilingual | BERT,
+8 layers | ViT-B/16 | 4 layers | [weights.pt][weights-m] | The Multilingual
+model supports 11 languages, after being trained on a balanced dataset. For
+pre-training we used translated captions made with [NLLB](https://github.com/
+facebookresearch/fairseq/tree/nllb). | Code | Language | # | Code | Language |
+# | Code | Language | | :------- | :------- | :--- | :------- | :--------------
+----- | :--- | :------- | :------- | | eng_Latn | English | # | fra_Latn |
+French | # | kor_Hang | Korean | | deu_Latn | German | # | ita_Latn | Italian |
+# | pol_Latn | Polish | | ita_Latn | Spanish | # | jpn_Jpan | Japanese | # |
+rus_Cyrl | Russian | | tur_Latn | Turkish | # | zho_Hans | Chinese (Simplified)
+| # | . | . | [weights-e]: https://huggingface.co/unum-cloud/uform-vl-english/
+resolve/main/torch_weight.pt [weights-m]: https://huggingface.co/unum-cloud/
+uform-vl-multilingual/resolve/main/torch_weight.pt ### Performance On RTX 3090,
+the following performance is expected from `uform` on text encoding. | Model |
+Multilingual | Sequences per Second | Speedup | | :------------------------ | -
+----------: | -------------------: | ---------: | | `bert-base-uncased` | No |
+1'612 | | | `distilbert-base-uncased` | No | 3'174 | x 1.96 | | `MiniLM-L12` |
+Yes | 3'604 | x 2.24 | | `MiniLM-L6` | No | 6'107 | x 3.79 | | | | | | |
+`uform` | Yes | 6'809 | __x 4.22__ |
```

### Comparing `uform-0.3.0/pyproject.toml` & `uform-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uform"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Mikhail Kim", email="mike.kim@unum.cloud" },
   { name="Vladimir Orshulevich", email="vladimir.orshulevich@unum.cloud" },
+  { name="Ash Vardanian", email="ash.vardanian@unum.cloud" },
 ]
 maintainers = [
-  { name="unum", email="info@unum.cloud" },
+  { name="Unum Cloud", email="info@unum.cloud" },
 ]
 dependencies = [
-  "transformers>=4.22.0",
-  "timm>0.6.11",
+  "torch>=1.13.1",
+  "tokenizers>=0.13.3",
+  "huggingface_hub>=0.16.4"
 ]
 description = "Multi-Modal Transformers library for Semantic Search and other Vision-Language tasks"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `uform-0.3.0/src/uform.egg-info/PKG-INFO` & `uform-0.3.1/src/uform.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: uform
-Version: 0.3.0
+Version: 0.3.1
 Summary: Multi-Modal Transformers library for Semantic Search and other Vision-Language tasks
-Author-email: Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>
-Maintainer-email: unum <info@unum.cloud>
+Author-email: Mikhail Kim <mike.kim@unum.cloud>, Vladimir Orshulevich <vladimir.orshulevich@unum.cloud>, Ash Vardanian <ash.vardanian@unum.cloud>
+Maintainer-email: Unum Cloud <info@unum.cloud>
 Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -73,14 +73,16 @@
 
 ## Installation
 
 ```bash
 pip install uform
 ```
 
+UForm v0.3.0 and below depends on `transformers` and `timm` libraries, all newer versions depend only on PyTorch (except libraries for the text tokenization and checkpoint downloading). For the best performance, Pytorch v2.0.0 and above is recommended.
+
 ## Usage
 
 To load the model:
 
 ```python
 import uform
 
@@ -198,16 +200,16 @@
 | Code     | Language | #    | Code     | Language             | #    | Code     | Language |
 | :------- | :------- | :--- | :------- | :------------------- | :--- | :------- | :------- |
 | eng_Latn | English  | #    | fra_Latn | French               | #    | kor_Hang | Korean   |
 | deu_Latn | German   | #    | ita_Latn | Italian              | #    | pol_Latn | Polish   |
 | ita_Latn | Spanish  | #    | jpn_Jpan | Japanese             | #    | rus_Cyrl | Russian  |
 | tur_Latn | Turkish  | #    | zho_Hans | Chinese (Simplified) | #    | .        | .        |
 
-[weights-e]: https://huggingface.co/unum-cloud/uform/resolve/main/english/weight.pt
-[weights-m]: https://huggingface.co/unum-cloud/uform/resolve/main/multilingual/weight.pt
+[weights-e]: https://huggingface.co/unum-cloud/uform-vl-english/resolve/main/torch_weight.pt
+[weights-m]: https://huggingface.co/unum-cloud/uform-vl-multilingual/resolve/main/torch_weight.pt
 
 ### Performance
 
 On RTX 3090, the following performance is expected from `uform` on text encoding.
 
 | Model                     | Multilingual | Sequences per Second |    Speedup |
 | :------------------------ | -----------: | -------------------: | ---------: |
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: uform Version: 0.3.0 Summary: Multi-Modal
+Metadata-Version: 2.1 Name: uform Version: 0.3.1 Summary: Multi-Modal
 Transformers library for Semantic Search and other Vision-Language tasks
 Author-email: Mikhail Kim
 kim@unum.cloud>, Vladimir Orshulevich
-orshulevich@unum.cloud> Maintainer-email: unum
+orshulevich@unum.cloud>, Ash Vardanian
+vardanian@unum.cloud> Maintainer-email: Unum Cloud
 unum.cloud> Project-URL: Homepage, https://github.com/unum-cloud/uform
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Image Processing Classifier: Topic :: Scientific/
 Engineering :: Image Recognition Classifier: Natural Language :: English
@@ -38,67 +39,70 @@
 both modalities jointly so they can take into account fine-grained features.
 Usually, these models are used for re-ranking relatively small retrieval
 results. __Mid-fusion models__ are the golden midpoint between the previous two
 types. Mid-fusion models consist of two parts â unimodal and multimodal. The
 unimodal part allows encoding each modality separately as late-fusion models
 do. The multimodal part takes unimodal features from the unimodal part as input
 and enhances them with a cross-attention mechanism. This tiny package will help
-you deal with the last! ## Installation ```bash pip install uform ``` ## Usage
-To load the model: ```python import uform model = uform.get_model('unum-cloud/
-uform-vl-english') model = uform.get_model('unum-cloud/uform-vl-multilingual')
-``` You can also load your own Mid-fusion model. Just upload it on HuggingFace
-and pass model name to `get_model`. To encode data: ```python from PIL import
-Image text = 'a small red panda in a zoo' image = Image.open('red_panda.jpg')
-image_data = model.preprocess_image(image) text_data = model.preprocess_text
-(text) image_embedding = model.encode_image(image_data) text_embedding =
-model.encode_text(text_data) joint_embedding = model.encode_multimodal
-(image=image_data, text=text_data) ``` Retrieving features is also trivial:
-```python image_features, image_embedding = model.encode_image(image_data,
-return_features=True) text_features, text_embedding = model.encode_text
-(text_data, return_features=True) ``` These features can later be used to
-produce joint multimodal encodings faster, as the first layers of the
-transformer can be skipped: ```python joint_embedding = model.encode_multimodal
-( image_features=image_features, text_features=text_features,
-attention_mask=text_data['attention_mask'] ) ``` ### Remote Procedure Calls for
-Cloud Deployments You can also use our larger, faster, better proprietary
-models deployed in optimized cloud environments. For that, please, choose the
-cloud of liking, search the marketplace for "Unum UForm" and reinstall UForm
-with optional dependencies: ```bash pip install uform[remote] ``` The only
-thing that changes after that is calling `get_client` with the IP address of
-your instance instead of using `get_model` for local usage. ```python model =
-uform.get_client('0.0.0.0:7000') ``` ## Evaluation There are two options to
-calculate semantic compatibility between an image and a text: [Cosine
-Similarity](#cosine-similarity) and [Matching Score](#matching-score). ###
-Cosine Similarity ```python import torch.nn.functional as F similarity =
-F.cosine_similarity(image_embedding, text_embedding) ``` The `similarity` will
-belong to the `[-1, 1]` range, `1` meaning the absolute match. __Pros__: -
-Computationally cheap. - Only unimodal embeddings are required, unimodal
-encoding is faster than joint encoding. - Suitable for retrieval in large
-collections. __Cons__: - Takes into account only coarse-grained features. ###
-Matching Score Unlike cosine similarity, unimodal embedding are not enough.
-Joint embedding will be needed and the resulting `score` will belong to the `
-[0, 1]` range, `1` meaning the absolute match. ```python score =
-model.get_matching_scores(joint_embedding) ``` __Pros__: - Joint embedding
-captures fine-grained features. - Suitable for re-ranking - sorting retrieval
-result. __Cons__: - Resource-intensive. - Not suitable for retrieval in large
-collections. ## Models ### Architecture | Model | Language Tower | Image Tower
-| Multimodal Part | URL | | :----------- | :------------: | :---------: | :----
----------: | ----------------------: | | English | BERT, 2 layers | ViT-B/16 |
-2 layers | [weights.pt][weights-e] | | Multilingual | BERT, 8 layers | ViT-B/16
-| 4 layers | [weights.pt][weights-m] | The Multilingual model supports 11
-languages, after being trained on a balanced dataset. For pre-training we used
-translated captions made with [NLLB](https://github.com/facebookresearch/
-fairseq/tree/nllb). | Code | Language | # | Code | Language | # | Code |
-Language | | :------- | :------- | :--- | :------- | :------------------- | :--
-- | :------- | :------- | | eng_Latn | English | # | fra_Latn | French | # |
-kor_Hang | Korean | | deu_Latn | German | # | ita_Latn | Italian | # | pol_Latn
-| Polish | | ita_Latn | Spanish | # | jpn_Jpan | Japanese | # | rus_Cyrl |
-Russian | | tur_Latn | Turkish | # | zho_Hans | Chinese (Simplified) | # | . |
-. | [weights-e]: https://huggingface.co/unum-cloud/uform/resolve/main/english/
-weight.pt [weights-m]: https://huggingface.co/unum-cloud/uform/resolve/main/
-multilingual/weight.pt ### Performance On RTX 3090, the following performance
-is expected from `uform` on text encoding. | Model | Multilingual | Sequences
-per Second | Speedup | | :------------------------ | -----------: | -----------
---------: | ---------: | | `bert-base-uncased` | No | 1'612 | | | `distilbert-
-base-uncased` | No | 3'174 | x 1.96 | | `MiniLM-L12` | Yes | 3'604 | x 2.24 | |
-`MiniLM-L6` | No | 6'107 | x 3.79 | | | | | | | `uform` | Yes | 6'809 | __x
-4.22__ |
+you deal with the last! ## Installation ```bash pip install uform ``` UForm
+v0.3.0 and below depends on `transformers` and `timm` libraries, all newer
+versions depend only on PyTorch (except libraries for the text tokenization and
+checkpoint downloading). For the best performance, Pytorch v2.0.0 and above is
+recommended. ## Usage To load the model: ```python import uform model =
+uform.get_model('unum-cloud/uform-vl-english') model = uform.get_model('unum-
+cloud/uform-vl-multilingual') ``` You can also load your own Mid-fusion model.
+Just upload it on HuggingFace and pass model name to `get_model`. To encode
+data: ```python from PIL import Image text = 'a small red panda in a zoo' image
+= Image.open('red_panda.jpg') image_data = model.preprocess_image(image)
+text_data = model.preprocess_text(text) image_embedding = model.encode_image
+(image_data) text_embedding = model.encode_text(text_data) joint_embedding =
+model.encode_multimodal(image=image_data, text=text_data) ``` Retrieving
+features is also trivial: ```python image_features, image_embedding =
+model.encode_image(image_data, return_features=True) text_features,
+text_embedding = model.encode_text(text_data, return_features=True) ``` These
+features can later be used to produce joint multimodal encodings faster, as the
+first layers of the transformer can be skipped: ```python joint_embedding =
+model.encode_multimodal( image_features=image_features,
+text_features=text_features, attention_mask=text_data['attention_mask'] ) ```
+### Remote Procedure Calls for Cloud Deployments You can also use our larger,
+faster, better proprietary models deployed in optimized cloud environments. For
+that, please, choose the cloud of liking, search the marketplace for "Unum
+UForm" and reinstall UForm with optional dependencies: ```bash pip install
+uform[remote] ``` The only thing that changes after that is calling
+`get_client` with the IP address of your instance instead of using `get_model`
+for local usage. ```python model = uform.get_client('0.0.0.0:7000') ``` ##
+Evaluation There are two options to calculate semantic compatibility between an
+image and a text: [Cosine Similarity](#cosine-similarity) and [Matching Score]
+(#matching-score). ### Cosine Similarity ```python import torch.nn.functional
+as F similarity = F.cosine_similarity(image_embedding, text_embedding) ``` The
+`similarity` will belong to the `[-1, 1]` range, `1` meaning the absolute
+match. __Pros__: - Computationally cheap. - Only unimodal embeddings are
+required, unimodal encoding is faster than joint encoding. - Suitable for
+retrieval in large collections. __Cons__: - Takes into account only coarse-
+grained features. ### Matching Score Unlike cosine similarity, unimodal
+embedding are not enough. Joint embedding will be needed and the resulting
+`score` will belong to the `[0, 1]` range, `1` meaning the absolute match.
+```python score = model.get_matching_scores(joint_embedding) ``` __Pros__: -
+Joint embedding captures fine-grained features. - Suitable for re-ranking -
+sorting retrieval result. __Cons__: - Resource-intensive. - Not suitable for
+retrieval in large collections. ## Models ### Architecture | Model | Language
+Tower | Image Tower | Multimodal Part | URL | | :----------- | :------------: |
+:---------: | :-------------: | ----------------------: | | English | BERT, 2
+layers | ViT-B/16 | 2 layers | [weights.pt][weights-e] | | Multilingual | BERT,
+8 layers | ViT-B/16 | 4 layers | [weights.pt][weights-m] | The Multilingual
+model supports 11 languages, after being trained on a balanced dataset. For
+pre-training we used translated captions made with [NLLB](https://github.com/
+facebookresearch/fairseq/tree/nllb). | Code | Language | # | Code | Language |
+# | Code | Language | | :------- | :------- | :--- | :------- | :--------------
+----- | :--- | :------- | :------- | | eng_Latn | English | # | fra_Latn |
+French | # | kor_Hang | Korean | | deu_Latn | German | # | ita_Latn | Italian |
+# | pol_Latn | Polish | | ita_Latn | Spanish | # | jpn_Jpan | Japanese | # |
+rus_Cyrl | Russian | | tur_Latn | Turkish | # | zho_Hans | Chinese (Simplified)
+| # | . | . | [weights-e]: https://huggingface.co/unum-cloud/uform-vl-english/
+resolve/main/torch_weight.pt [weights-m]: https://huggingface.co/unum-cloud/
+uform-vl-multilingual/resolve/main/torch_weight.pt ### Performance On RTX 3090,
+the following performance is expected from `uform` on text encoding. | Model |
+Multilingual | Sequences per Second | Speedup | | :------------------------ | -
+----------: | -------------------: | ---------: | | `bert-base-uncased` | No |
+1'612 | | | `distilbert-base-uncased` | No | 3'174 | x 1.96 | | `MiniLM-L12` |
+Yes | 3'604 | x 2.24 | | `MiniLM-L6` | No | 6'107 | x 3.79 | | | | | | |
+`uform` | Yes | 6'809 | __x 4.22__ |
```

### Comparing `uform-0.3.0/src/uform.py` & `uform-0.3.1/src/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,512 +1,597 @@
-from json import load
-from typing import Optional, Union
+from os import PathLike
+from dataclasses import dataclass
+from typing import Optional, Dict, Tuple, Union, List
 
-import timm
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
-from torchvision.transforms import Compose, Resize, CenterCrop, ToTensor, Normalize, InterpolationMode
-from transformers import AutoTokenizer
-from transformers import BertConfig, BertModel, RobertaConfig, RobertaModel, XLMRobertaConfig, XLMRobertaModel
-from transformers.models.bert.modeling_bert import BertAttention
-from transformers.models.roberta.modeling_roberta import RobertaAttention
-from transformers.models.xlm_roberta.modeling_xlm_roberta import XLMRobertaAttention
-from huggingface_hub import snapshot_download, hf_hub_download
+from torchvision.transforms import (
+    Compose,
+    Resize,
+    CenterCrop,
+    ToTensor,
+    Normalize,
+    InterpolationMode,
+)
+
+from tokenizers import Tokenizer
+from PIL.Image import Image
+
+
+# lambda is not pickable
+def convert_to_rgb(image):
+    return image.convert("RGB")
+
+
+@dataclass(eq=False)
+class Attention(nn.Module):
+    dim: int
+    num_heads: int
+    dropout_prob: float = 0
 
+    def __post_init__(self):
+        super().__init__()
 
-class VisualEncoder(nn.Module):
-    def __init__(
+        self.use_sdp = int(torch.__version__[0]) > 1
+
+        self.query = nn.Linear(self.dim, self.dim)
+        self.key = nn.Linear(self.dim, self.dim)
+        self.value = nn.Linear(self.dim, self.dim)
+        self.out = nn.Linear(self.dim, self.dim)
+
+        self.head_dim = self.dim // self.num_heads
+        self.scale = self.head_dim**-0.5
+
+    def forward(
         self,
-        backbone,
-        backbone_type: str,
-        dim: int,
-        output_dim: int,
-        pooling='cls',
-    ):
+        x: Tensor,
+        attn_mask: Optional[Tensor] = None,
+        context: Optional[Tensor] = None,
+        is_causal: bool = False,
+    ) -> Tensor:
+        query = self.reshape(self.query(x))
+        key = self.reshape(self.key(x if context is None else context))
+        value = self.reshape(self.value(x if context is None else context))
+
+        if self.use_sdp:
+            x = F.scaled_dot_product_attention(
+                query,
+                key,
+                value,
+                attn_mask,
+                dropout_p=self.dropout_prob if self.training else 0,
+                is_causal=is_causal,
+            )
+        else:
+            attn = query @ key.transpose(-2, -1) * self.scale
+            if attn_mask is not None:
+                attn += attn_mask
+
+            attn = attn.softmax(dim=-1)
+            x = attn @ value
+
+        return self.out(x.transpose(2, 1).flatten(2))
+
+    def reshape(self, x: Tensor) -> Tensor:
+        batch_size, seq_len, _ = x.shape
+        x = x.view(batch_size, seq_len, self.num_heads, self.head_dim)
+        return x.transpose(2, 1)
+
+
+@dataclass(eq=False)
+class MLP(nn.Module):
+    dim: int
+    dim_expand_factor: int = 4
 
+    def __post_init__(self):
         super().__init__()
-        self.encoder = timm.create_model(
-            backbone,
-            pretrained=False,
-            num_classes=0,
-        )
-        self.backbone_type = backbone_type
-        self.pooling = pooling
-
-        if self.pooling == 'attention':
-            self.attention_pooling = nn.MultiheadAttention(
-                embed_dim=dim,
-                num_heads=1,
-                batch_first=True,
-                dropout=0.1,
-            )
-            self.queries = nn.Parameter(torch.randn(1, 197, dim))
 
-        self.proj = nn.Linear(dim, output_dim, bias=False)
-        self.dim = dim
+        self.hidden_layer = nn.Linear(self.dim, self.dim * self.dim_expand_factor)
+        self.output_layer = nn.Linear(self.dim * self.dim_expand_factor, self.dim)
+
+    def forward(self, x: Tensor) -> Tensor:
+        x = F.gelu(self.hidden_layer(x))
+        return self.output_layer(x)
+
 
-        if hasattr(self.encoder, 'fc_norm'):
-            self.encoder.fc_norm = nn.Identity()
+@dataclass(eq=False)
+class LayerScale(nn.Module):
+    dim: int
+    init_values: float = 1e-5
+    inplace: bool = False
 
-        if hasattr(self.encoder, 'head'):
-            self.encoder.head = nn.Identity()
+    def __post_init__(self):
+        super().__init__()
+        self.gamma = nn.Parameter(self.init_values * torch.ones(self.dim))
 
     def forward(self, x: Tensor) -> Tensor:
-        features = self.forward_features(x)
-        return features, self.get_embedding(features)
+        return x.mul_(self.gamma) if self.inplace else x * self.gamma
 
-    def forward_features(self, x: Tensor) -> Tensor:
-        if self.backbone_type == 'vit':
-            features = self.forward_features_vit(x)
-        else:
-            features = self.forward_features_conv(x)
 
-        if self.pooling == 'attention':
-            return self.attention_pooling(
-                self.queries.expand(x.shape[0], -1, -1),
-                features,
-                features,
-            )[0]
+@dataclass(eq=False)
+class TextEncoderBlock(nn.Module):
+    dim: int
+    num_heads: int
+    dropout_prob: float
+    cross_attention: bool = False
 
-        return features
+    def __post_init__(self):
+        super().__init__()
 
-    def forward_features_conv(self, x: Tensor) -> Tensor:
-        return self.encoder.forward_features(x).flatten(2).permute(0, 2, 1)
+        self.norm_attn = nn.LayerNorm(self.dim, eps=1e-12)
+        self.attention = Attention(self.dim, self.num_heads, self.dropout_prob)
 
-    def forward_features_vit(self, x: Tensor) -> Tensor:
-        x = self.encoder.patch_embed(x)
-        x = self.encoder._pos_embed(x)
-        x = self.encoder.norm_pre(x)
+        if self.cross_attention:
+            self.norm_crossattn = nn.LayerNorm(self.dim, eps=1e-12)
+            self.crossattn = Attention(self.dim, self.num_heads, self.dropout_prob)
 
-        for block in self.encoder.blocks:
-            x = block(x)
+        self.norm_mlp = nn.LayerNorm(self.dim, eps=1e-12)
+        self.mlp = MLP(self.dim)
 
-        x = self.encoder.norm(x)
+        self.dropout = nn.Dropout(self.dropout_prob)
 
-        return x
+    def forward(
+        self, x: Tensor, attn_mask: Tensor, context: Optional[Tensor] = None
+    ) -> Tensor:
+        x = self.norm_attn(x + self.dropout(self.attention(x, attn_mask)))
 
-    def get_embedding(self, x: Tensor, project: bool = True) -> Tensor:
-        if isinstance(x, list):
-            x = x[-1]
+        if self.cross_attention and context is not None:
+            x = self.norm_crossattn(
+                x + self.dropout(self.crossattn(x, context=context))
+            )
+
+        return self.norm_mlp(x + self.dropout(self.mlp(x)))
 
-        if self.pooling == 'cls' or self.pooling == 'attention':
-            x = x[:, 0]
-        elif self.pooling == 'mean':
-            x = x.mean(dim=1)
 
-        if project:
-            return self.proj(x)
+@dataclass(eq=False)
+class VisualEncoderBlock(nn.Module):
+    dim: int
+    num_heads: int
 
+    def __post_init__(self):
+        super().__init__()
+        self.norm1 = nn.LayerNorm(self.dim, eps=1e-6)
+        self.attn = Attention(self.dim, self.num_heads)
+        self.ls1 = LayerScale(self.dim)
+
+        self.norm2 = nn.LayerNorm(self.dim, eps=1e-6)
+        self.mlp = MLP(self.dim)
+        self.ls2 = LayerScale(self.dim)
+
+    def forward(self, x: Tensor) -> Tensor:
+        x = x + self.ls1(self.attn(self.norm1(x)))
+        x = x + self.ls2(self.mlp(self.norm2(x)))
         return x
 
 
+@dataclass(eq=False)
 class TextEncoder(nn.Module):
-    def __init__(
-        self,
-        backbone,
-        backbone_type: str,
-        unimodal_n_layers: int,
-        context_dim: int,
-        dim: int,
-        output_dim: int,
-        pooling: str = 'cls',
-        head_one_neuron: bool = False,
-    ):
+    model_type: str
+    dim: int
+    context_dim: int
+    vocab_size: int
+    padding_idx: int
+    num_layers: int
+    num_heads: int
+    embedding_dim: int
+    multimodal_layers_ids: tuple
+    head_one_neuron: bool
+    pooling: str = "cls"
+    max_position_embeddings: int = 77
+    dropout_prob: float = 0
 
+    def __post_init__(self):
         super().__init__()
-        self.backbone = TextEncoderBackbone(
-            backbone, backbone_type, unimodal_n_layers)
-        if context_dim != dim:
-            self.context_proj = nn.Linear(context_dim, dim, bias=False)
-        else:
-            self.context_proj = nn.Identity()
 
-        self.pooling = pooling
-        self.proj = nn.Linear(dim, output_dim, bias=False)
-        self.clf_head = nn.Linear(dim, 1 if head_one_neuron else 2)
-        self.head_one_neuron = head_one_neuron
-        self.dim = dim
-
-    def forward(self, x: Tensor, attention_mask: Tensor, causal: bool = False) -> Tensor:
-        features = self.forward_unimodal(x, attention_mask, causal)
-        return features, self.get_embedding(features, attention_mask)
-
-    def forward_unimodal(self, x: Tensor, attention_mask: Tensor, causal: bool = False) -> Tensor:
-        prep_attention_mask = self.prepare_attention_mask(
-            attention_mask, causal)
-        x = self.backbone.embeddings(x)
+        self.word_embeddings = nn.Embedding(
+            self.vocab_size, self.dim, padding_idx=self.padding_idx
+        )
+        self.position_embeddings = nn.Embedding(self.max_position_embeddings, self.dim)
+
+        if self.model_type == "bert":
+            self.register_buffer(
+                "position_ids",
+                torch.arange(self.max_position_embeddings).unsqueeze(0),
+                persistent=False,
+            )
+
+        self.layer_norm = nn.LayerNorm(self.dim, eps=1e-12)
+        self.dropout = nn.Dropout(self.dropout_prob)
+
+        self.blocks = nn.ModuleList(
+            [
+                TextEncoderBlock(
+                    self.dim,
+                    self.num_heads,
+                    self.dropout_prob,
+                    layer_id in self.multimodal_layers_ids,
+                )
+                for layer_id in range(self.num_layers)
+            ]
+        )
+
+        self.embedding_projection = nn.Linear(self.dim, self.embedding_dim, bias=False)
+        self.matching_head = nn.Linear(self.dim, 1 if self.head_one_neuron else 2)
+
+        if self.context_dim != self.dim:
+            self.context_projection = nn.Linear(self.context_dim, self.dim, bias=False)
+        else:
+            self.context_projection = nn.Identity()
 
-        for layer in self.backbone.unimodal_encoder:
-            x = layer(x, prep_attention_mask)[0]
+    def forward_features(self, x: Tensor, attn_mask: Tensor) -> Tensor:
+        x = self.embed_text(x)
+        attn_mask = self.get_attention_mask(attn_mask, x.dtype)
+
+        for block in self.blocks:
+            if not block.cross_attention:
+                x = block(x, attn_mask)
 
         return x
 
     def forward_multimodal(
-        self,
-        x: Tensor,
-        attention_mask: Tensor,
-        context: Tensor,
-        causal: bool = False,
+        self, x: Tensor, attn_mask: Tensor, context: Tensor
     ) -> Tensor:
-        prep_attention_mask = self.prepare_attention_mask(
-            attention_mask,
-            causal,
-        )
-        context = self.context_proj(context)
-        for layer in self.backbone.multimodal_encoder:
-            x, _, _ = layer(x, prep_attention_mask, context)
-
-        return self.get_embedding(x, attention_mask, project=False)
-
-    def get_matching_scores(self, x: Tensor, attention_mask: Tensor, context) -> Tensor:
-        embeddings = self.forward_multimodal(
-            x, attention_mask, context, False)
-        return self._logit_and_norm(embeddings)
+        context = self.context_projection(context)
+        expanded_attn_mask = self.get_attention_mask(attn_mask, x.dtype)
+        for block in self.blocks:
+            if block.cross_attention:
+                x = block(x, expanded_attn_mask, context)
+
+        return self.pool_features(x, attn_mask)
+
+    def forward_embedding(self, x: Tensor, attn_mask: Tensor) -> Tensor:
+        return self.embedding_projection(self.pool_features(x, attn_mask))
 
-    def _logit_and_norm(self, embeddings: Tensor) -> Tensor:
-        logits = self.clf_head(embeddings)
+    def forward_matching(self, x: Tensor) -> Tensor:
+        logits = self.matching_head(x)
         if self.head_one_neuron:
             return torch.sigmoid(logits)[:, 0]
 
         return F.softmax(logits, dim=1)[:, 1]
 
-    def get_embedding(self, x: Tensor, attention_mask: Tensor, project: bool = True) -> Tensor:
-        if self.pooling == 'mean':
-            mask_expanded = attention_mask.unsqueeze(2)
-            vec_sum = (x * mask_expanded).sum(dim=1)
-            x = vec_sum / mask_expanded.sum(dim=1)
+    def pool_features(self, x: Tensor, attn_mask: Tensor) -> Tensor:
+        if self.pooling == "cls":
+            return x[:, 0]
 
-        elif self.pooling == 'cls':
-            x = x[:, 0]
+        attn_mask = attn_mask.unsqueeze(2).type_as(x)
 
-        if project:
-            return self.proj(x)
+        return (x * attn_mask).sum(dim=1) / attn_mask.sum(dim=1)
 
-        return x
+    def get_attention_mask(self, attn_mask: Tensor, dtype: torch.dtype) -> Tensor:
+        attn_mask = attn_mask.to(dtype)
+        attn_mask = (1.0 - attn_mask) * torch.finfo(dtype).min
+        return attn_mask.unsqueeze(1).expand(-1, attn_mask.shape[1], -1).unsqueeze(1)
+
+    def get_position_ids(self, x: Tensor) -> Tensor:
+        if self.model_type == "roberta":
+            mask = x.ne(self.padding_idx).int()
+            return (
+                torch.cumsum(mask, dim=1).type_as(mask) * mask
+            ).long() + self.padding_idx
 
-    def prepare_attention_mask(self, mask: Tensor, causal: bool = False) -> Tensor:
-        if causal:
-            causal_mask = torch.ones(
-                mask.size(1), mask.size(1), device=mask.device).tril()
-            # bs x seq_len x seq_len
-            mask = mask[:, None, :] * causal_mask[None, :, :]
-            mask = (1 - mask) * -10e9
-            return mask[:, None]
-
-        mask = (1 - mask) * -10e9
-        return mask[:, None, None, :]
-
-
-class TextEncoderBackbone(nn.Module):
-    type2classes = {
-        'bert': (BertConfig, BertModel, BertAttention),
-        'roberta': (RobertaConfig, RobertaModel, RobertaAttention),
-        'xlm_roberta': (XLMRobertaConfig, XLMRobertaModel, XLMRobertaAttention)
-    }
+        return self.position_ids[:, : x.shape[1]]
 
-    def __init__(self, pretrained: str, backbone_type: str, unimodal_n_layers: int):
+    def embed_text(self, x: Tensor) -> Tensor:
+        positional_embedding = self.position_embeddings(self.get_position_ids(x))
+        x = self.word_embeddings(x) + positional_embedding
+        return self.dropout(self.layer_norm(x))
+
+
+@dataclass(eq=False)
+class VisualEncoder(nn.Module):
+    dim: int
+    patch_size: int
+    image_size: int
+    num_layers: int
+    num_heads: int
+    embedding_dim: int
+    pooling: str
+
+    def __post_init__(self):
         super().__init__()
-        self.unimodal_n_layers = unimodal_n_layers
 
-        config_file = hf_hub_download(
-            repo_id=pretrained,
-            filename='config.json',
-        )
-        config_cls, model_cls, attention_layer_cls = self.type2classes[backbone_type]
-        config = config_cls.from_json_file(config_file)
-        model = model_cls(config)
-
-        self.construct_model(model, attention_layer_cls, config)
-
-    def construct_model(self, backbone, attention_layer_cls: type, config: dict):
-
-        self.unimodal_encoder = backbone.encoder.layer[:self.unimodal_n_layers]
-        self.embeddings = backbone.embeddings
-        self.multimodal_encoder = []
-
-        for layer in backbone.encoder.layer[self.unimodal_n_layers:]:
-            self.multimodal_encoder.append(
-                FusedTransformerLayer(
-                    config,
-                    attention_layer_cls,
-                    layer,
-                )
-            )
+        seq_len = (self.image_size // self.patch_size) ** 2
+        self.patch_embed = nn.Conv2d(3, self.dim, self.patch_size, self.patch_size)
+        self.pos_embed = nn.Parameter(torch.randn(1, seq_len, self.dim) * 0.02)
+        self.cls_token = nn.Parameter(torch.zeros(1, 1, self.dim))
+
+        self.blocks = nn.Sequential(
+            *[
+                VisualEncoderBlock(self.dim, self.num_heads)
+                for _ in range(self.num_layers)
+            ]
+        )
 
-        self.multimodal_encoder = nn.ModuleList(self.multimodal_encoder)
+        self.norm = nn.LayerNorm(self.dim, eps=1e-6)
+        self.embedding_projection = nn.Linear(self.dim, self.embedding_dim, bias=False)
 
+    def forward_features(self, x: Tensor) -> Tensor:
+        x = self.patch_embed(x).flatten(start_dim=2).transpose(2, 1)
+        x = x + self.pos_embed
+        x = torch.cat((self.cls_token.expand(x.shape[0], -1, -1), x), dim=1)
+        x = self.blocks(x)
 
-class FusedTransformerLayer(nn.Module):
+        return self.norm(x)
 
-    def __init__(self, config, attention_layer_cls, base_layer):
-        super().__init__()
+    def forward_embedding(self, x: Tensor) -> Tensor:
+        if self.pooling == "cls":
+            x = x[:, 0]
+        else:
+            x = x.mean(dim=1)
 
-        self.self_attention = base_layer.attention
-        self.intermediate = base_layer.intermediate
-        self.output = base_layer.output
-        self.cross_attention = attention_layer_cls(config)
-
-    def forward(self, x: Tensor, attention_mask: Tensor, context: Tensor) -> tuple[Tensor, Tensor, Tensor]:
-        attention_output, self_attention_probs = self.self_attention(
-            x,
-            attention_mask,
-            output_attentions=True,
-        )
-        attention_output, cross_attention_probs = self.cross_attention(
-            attention_output,
-            encoder_hidden_states=context,
-            output_attentions=True,
-        )  # [0]
-        intermediate_output = self.intermediate(attention_output)
-        layer_output = self.output(intermediate_output, attention_output)
-        return layer_output, self_attention_probs, cross_attention_probs
+        return self.embedding_projection(x)
 
 
 class VLM(nn.Module):
     """
     Vision-Language Model for multi-modal embeddings.
-
-    ...
-
-    Attributes
-    ----------
-    text_encoder : TextEncoder
-        Textual Encoder. Generally a BERT-like transformer.
-    image_encoder : VisualEncoder
-        Visual Encoder. Generally a ViT or a ConvNet.
-    dim : int
-        Dimensionality of the multi-modal embedding.
-        It is generally larger than `text_encoder.dim` and `image_encoder.dim`.
-
-    Methods
-    -------
-    preprocess_text(text)
-        Transforms one or more strings into Torch Tensors of tokens.
-    encode_text(text_data)
-        Passes the pre-processed texts through `text_encoder` to produce embeddings.
-    preprocess_image(image)
-        Transforms one or more Pillow images into Torch Tensors.
-    encode_image(image_data)
-        Passes the pre-processed images through `image_encoder` to produce embeddings.
-    encode_multimodal(image=image, text=text)
-        Passes pre-processed texts and images through both towers, mixing the signal.
-    get_matching_scores(multimodal_embedding)
-        Computes the probability that there is a match between image and text based on their multimodal embedding
     """
 
-    def __init__(self, config: dict):
+    def __init__(self, config: Dict, tokenizer_path: PathLike):
+        """
+        :param config: Model config
+        """
+
         super().__init__()
-        self.text_encoder = TextEncoder(**config['text_encoder'])
-        self.image_encoder = VisualEncoder(**config['img_encoder'])
-        self._tokenizer = AutoTokenizer.from_pretrained(
-            config['text_encoder']['backbone'])
+        self._max_seq_len = config["text_encoder"]["max_position_embeddings"]
+        self._embedding_dim = config["text_encoder"]["embedding_dim"]
+        self._image_size = config["image_encoder"]["image_size"]
+
+        self.text_encoder = TextEncoder(**config["text_encoder"])
+        self.image_encoder = VisualEncoder(**config["image_encoder"])
+
+        self._tokenizer = Tokenizer.from_file(tokenizer_path)
+        self._tokenizer.no_padding()
+        self._pad_token_idx = self.text_encoder.padding_idx
+
+        self._image_transform = Compose(
+            [
+                Resize(self._image_size, interpolation=InterpolationMode.BICUBIC),
+                convert_to_rgb,
+                CenterCrop(self._image_size),
+                ToTensor(),
+                Normalize(
+                    mean=(0.48145466, 0.4578275, 0.40821073),
+                    std=(0.26862954, 0.26130258, 0.27577711),
+                ),
+            ]
+        )
+
+    def encode_image(
+        self,
+        images: Tensor,
+        return_features: bool = False,
+    ) -> Union[Tensor, Tuple[Tensor, Tensor]]:
+        """Passes the pre-processed images through `image_encoder` to produce images features (optional) and embeddings.
 
-        self._embedding_dim = config['text_encoder']['output_dim']
+        :param images: Preprocessed image
+        :param return_features: Whether to return images features or return only embeddings
+        """
 
-    def encode_image(self, x: Tensor, return_features: bool = False) -> Tensor:
-        features, embs = self.image_encoder(x)
+        features = self.image_encoder.forward_features(images)
+        embeddings = self.image_encoder.forward_embedding(features)
 
         if return_features:
-            return features, embs
+            return features, embeddings
+
+        return embeddings
+
+    def encode_text(
+        self,
+        texts: Dict[str, Tensor],
+        return_features: bool = False,
+    ) -> Union[Tensor, Tuple[Tensor, Tensor]]:
+        """Passes the pre-processed texts through `text_encoder` to produce texts features (optional) and embeddings.
 
-        return embs
+        :param texts: Dictionary with tokenized texts and attention masks
+        :param return_features: Whether to return texts features or return only embeddings
+        """
 
-    def encode_text(self, x: dict, return_features: bool = False) -> Tensor:
-        features, embs = self.text_encoder(x['input_ids'], x['attention_mask'])
+        features = self.text_encoder.forward_features(
+            texts["input_ids"], texts["attention_mask"]
+        )
+        embeddings = self.text_encoder.forward_embedding(
+            features, texts["attention_mask"]
+        )
 
         if return_features:
-            return features, embs
+            return features, embeddings
 
-        return embs
+        return embeddings
 
     def encode_multimodal(
         self,
-        *,
         image: Optional[Tensor] = None,
-        text: Optional[dict] = None,
+        text: Optional[Dict] = None,
         image_features: Optional[Tensor] = None,
         text_features: Optional[Tensor] = None,
         attention_mask: Optional[Tensor] = None,
     ) -> Tensor:
+        """Passes preprocessed texts (or precomputed texts features) and
+            preprocessed images (or precomputed images features) through multimodal encoded to produce multimodal joint embeddings.
 
-        assert image is not None or image_features is not None, 'Either `image` or `image_features` should be non None'
-        assert text is not None or text_features is not None, 'Either `text_data` or `text_features` should be non None'
+        :param image: Preprocessed images
+        :param text: Preprocesses texts
+        :param image_features: Precomputed images features
+        :param text_features: Precomputed text features
+        :param attention_mask: Attention masks, not required if pass `text` instead of text_features
+        """
+
+        assert (
+            image is not None or image_features is not None
+        ), "Either `image` or `image_features` should be non None"
+        assert (
+            text is not None or text_features is not None
+        ), "Either `text_data` or `text_features` should be non None"
 
         if text_features is not None:
-            assert attention_mask is not None, 'if `text_features` is not None, then you should pass `attention_mask`'
+            assert (
+                attention_mask is not None
+            ), "if `text_features` is not None, then you should pass `attention_mask`"
 
         if image_features is None:
             image_features = self.image_encoder.forward_features(image)
 
         if text_features is None:
-            text_features = self.text_encoder.forward_unimodal(
-                text['input_ids'],
-                text['attention_mask']
+            text_features = self.text_encoder.forward_features(
+                text["input_ids"], text["attention_mask"]
             )
 
         return self.text_encoder.forward_multimodal(
             text_features,
-            attention_mask if attention_mask is not None else text['attention_mask'],
-            image_features
+            attention_mask if attention_mask is not None else text["attention_mask"],
+            image_features,
         )
 
-    def get_matching_scores(self, x: Tensor):
-        return self.text_encoder._logit_and_norm(x)
+    def get_matching_scores(self, embeddings: Tensor) -> Tensor:
+        """Computes the probability that there is a match between images and texts based on their multimodal embeddings
+
+        :param embeddings: multimodal joint embeddings
+        """
 
-    def preprocess_text(self, x) -> dict:
-        x = self._tokenizer(
-            x,
-            padding='max_length',
-            truncation=True,
-            return_tensors='pt',
-            pad_to_max_length=True,
-            max_length=77,
+        return self.text_encoder.forward_matching(embeddings)
+
+    def preprocess_text(self, texts: Union[str, List[str]]) -> Dict[str, Tensor]:
+        """Transforms one or more strings into dictionary with tokenized strings and attention masks.
+
+        :param texts: text of list of texts to tokenizer
+        """
+        if isinstance(texts, str):
+            texts = [texts]
+
+        input_ids = torch.full(
+            (len(texts), self.text_encoder.max_position_embeddings),
+            fill_value=self._pad_token_idx,
+            dtype=torch.int64,
         )
-        if 'token_type_ids' in x:
-            del x['token_type_ids']
 
-        return x
+        attention_mask = torch.zeros(
+            len(texts), self.text_encoder.max_position_embeddings, dtype=torch.int32
+        )
+        encoded = self._tokenizer.encode_batch(texts)
 
-    def preprocess_image(self, x) -> Tensor:
-        preprocessor = Compose([
-            Resize(224, interpolation=InterpolationMode.BICUBIC),
-            lambda x: x.convert('RGB'),
-            CenterCrop(224),
-            ToTensor(),
-            Normalize(
-                mean=(0.48145466, 0.4578275, 0.40821073),
-                std=(0.26862954, 0.26130258, 0.27577711)
+        for i, seq in enumerate(encoded):
+            seq_len = min(len(seq), self.text_encoder.max_position_embeddings)
+            input_ids[i, :seq_len] = torch.LongTensor(
+                seq.ids[: self.text_encoder.max_position_embeddings]
             )
-        ])
-        if isinstance(x, list):
-            images = []
-            for image in x:
-                images.append(preprocessor(image))
+            attention_mask[i, :seq_len] = 1
+
+        return {"input_ids": input_ids, "attention_mask": attention_mask}
+
+    def preprocess_image(self, images: Union[Image, List[Image]]) -> Tensor:
+        """Transforms one or more Pillow images into Torch Tensors.
+
+        :param images: image or list of images to preprocess
+        """
+
+        if isinstance(images, list):
+            batch_images = torch.empty(
+                (len(images), 3, self._image_size, self._image_size),
+                dtype=torch.float32,
+            )
+
+            for i, image in enumerate(images):
+                batch_images[i] = self._image_transform(image)
 
-            batch_images = torch.stack(images, dim=0)
             return batch_images
         else:
-            return preprocessor(x).unsqueeze(0)
+            return self._image_transform(images).unsqueeze(0)
 
     @property
     def text_features_dim(self) -> int:
+        """Dimensionality of the text encoder features."""
+
         return self.text_encoder.dim
 
     @property
     def image_features_dim(self) -> int:
+        """Dimensionality of the image encoder features."""
+
         return self.image_encoder.dim
 
     @property
     def embedding_dim(self) -> int:
+        """Dimensionality of shared space embedding."""
+
         return self._embedding_dim
-    
+
     @property
     def multimodal_embedding_dim(self) -> int:
+        """Dimensionality of multimodal joint embedding."""
         return self.text_encoder.dim
 
 
 class TritonClient(VLM):
     """
     Nvidia Triton client to connect to the remote VLM inference server.
     """
 
-    def __init__(self, url: str = 'localhost:7001'):
+    def __init__(self, url: str = "localhost:7001"):
         import tritonclient.http as httpclient
+        from transformers import AutoTokenizer
+
         self._client = httpclient
-        self._triton_client = self._client.InferenceServerClient(
-            url=url
-        )
+        self._triton_client = self._client.InferenceServerClient(url=url)
         self._tokenizer = AutoTokenizer.from_pretrained(
-            'google/bert_uncased_L-4_H-768_A-12'
+            "google/bert_uncased_L-4_H-768_A-12"
         )
 
     def encode_image(
         self,
-        imgs,
+        imgs: Tensor,
     ):
         """
-        Returns the image embedding.
-            Parameters:
-                imgs (numpy.ndarray): Pre-processed image
+        Passes the pre-processed images through `image_encoder` to produce images embeddings.
 
-            Returns:
-                output_data (numpy.ndarray): Image embedding
+        :param imgs: Preprocessed image
         """
+
         # images prep
         inputs = []
         outputs = []
         imgs = imgs.cpu().detach().numpy()
-        inputs.append(
-            self._client.InferInput('inputs', imgs.shape, 'FP32')
-        )
+        inputs.append(self._client.InferInput("inputs", imgs.shape, "FP32"))
         inputs[0].set_data_from_numpy(imgs)
-        outputs.append(self._client.InferRequestedOutput('output'))
+        outputs.append(self._client.InferRequestedOutput("output"))
 
         # Querying the server
         results = self._triton_client.infer(
-            model_name='vit',
-            inputs=inputs,
-            outputs=outputs
+            model_name="vit", inputs=inputs, outputs=outputs
         )
-        output_data = torch.from_numpy(results.as_numpy('output'))
+        output_data = torch.from_numpy(results.as_numpy("output"))
         return output_data
 
     def encode_text(
         self,
-        text,
+        text: Dict[str, Tensor],
     ):
         """
-        Returns the image embedding.
-            Parameters:
-                text (dict): Tokenized Text
+        Passes the pre-processed texts through `text_encoder` to produce texts embeddings.
 
-            Returns:
-                output_vec (numpy.ndarray): Text embedding
+        :param text: Dictionary with tokenized texts and attention masks
         """
+
         # texts prep
         inputs = []
-        input_ids, attention_mask = text['input_ids'], text['attention_mask']
+        input_ids, attention_mask = text["input_ids"], text["attention_mask"]
         input_ids = input_ids.type(dtype=torch.int32).cpu().detach().numpy()
-        attention_mask = attention_mask.type(
-            dtype=torch.int32).cpu().detach().numpy()
-        inputs.append(self._client.InferInput(
-            'attention_mask', attention_mask.shape, 'INT32'))
-        inputs.append(self._client.InferInput(
-            'input_ids', input_ids.shape, 'INT32'))
+        attention_mask = attention_mask.type(dtype=torch.int32).cpu().detach().numpy()
+        inputs.append(
+            self._client.InferInput("attention_mask", attention_mask.shape, "INT32")
+        )
+        inputs.append(self._client.InferInput("input_ids", input_ids.shape, "INT32"))
         inputs[0].set_data_from_numpy(attention_mask)
         inputs[1].set_data_from_numpy(input_ids)
-        test_output = self._client.InferRequestedOutput('output')
+        test_output = self._client.InferRequestedOutput("output")
 
         # Querying the server
         results = self._triton_client.infer(
-            model_name='albef',
-            inputs=inputs,
-            outputs=[test_output]
+            model_name="albef", inputs=inputs, outputs=[test_output]
         )
-        output_vec = torch.from_numpy(results.as_numpy('output'))
+        output_vec = torch.from_numpy(results.as_numpy("output"))
         return output_vec
 
     def encode_multimodal(self, *args, **kwargs):
-        raise NotImplementedError('Multimodal encodings coming soon!')
-
-
-def get_model(model_name: str, token: Optional[Union[bool, str]] = None) -> VLM:
-    model_path = snapshot_download(
-        repo_id=model_name,
-        token=token,
-    )
-    config_path = f'{model_path}/config.json'
-    state = torch.load(f'{model_path}/weight.pt')
-
-    with open(config_path, 'r') as f:
-        model = VLM(load(f))
-
-    model.image_encoder.load_state_dict(state['img_encoder'])
-    model.text_encoder.load_state_dict(state['text_encoder'], strict=False)
-
-    return model.eval()
-
-
-def get_client(url: str) -> TritonClient:
-    return TritonClient(url)
+        raise NotImplementedError("Multimodal encodings coming soon!")
```

