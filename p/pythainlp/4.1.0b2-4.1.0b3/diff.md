# Comparing `tmp/pythainlp-4.1.0b2.tar.gz` & `tmp/pythainlp-4.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythainlp-4.1.0b2.tar", last modified: Thu Jul 27 13:55:16 2023, max compression
+gzip compressed data, was "pythainlp-4.1.0b3.tar", last modified: Fri Aug  4 06:03:02 2023, max compression
```

## Comparing `pythainlp-4.1.0b2.tar` & `pythainlp-4.1.0b3.tar`

### file list

```diff
@@ -1,239 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.579702 pythainlp-4.1.0b2/
--rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-07-27 13:55:16.579702 pythainlp-4.1.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    15412 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/README_TH.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.543702 pythainlp-4.1.0b2/pythainlp/
--rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.543702 pythainlp-4.1.0b2/pythainlp/augment/
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.547702 pythainlp-4.1.0b2/pythainlp/augment/lm/
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/lm/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/lm/wangchanberta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.547702 pythainlp-4.1.0b2/pythainlp/augment/word2vec/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/word2vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/word2vec/bpemb_wv.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/word2vec/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/word2vec/ltw2v.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/word2vec/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/augment/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.547702 pythainlp-4.1.0b2/pythainlp/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/benchmarks/word_tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.547702 pythainlp-4.1.0b2/pythainlp/chat/
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/chat/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.547702 pythainlp-4.1.0b2/pythainlp/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/cli/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/cli/soundex.py
--rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/cli/tag.py
--rw-r--r--   0 runner    (1001) docker     (122)     5275 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/cli/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.547702 pythainlp-4.1.0b2/pythainlp/cls/
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/cls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/cls/param_free.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.551702 pythainlp-4.1.0b2/pythainlp/coref/
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/coref/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/coref/_fastcoref.py
--rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/coref/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      930 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/coref/han_coref.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.551702 pythainlp-4.1.0b2/pythainlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11287 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/corpus/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/corpus/conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    17555 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/corpus/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/corpus/oscar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-07-27 13:54:59.000000 pythainlp-4.1.0b2/pythainlp/corpus/th_en_translit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/corpus/tnc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/corpus/ttc.py
--rw-r--r--   0 runner    (1001) docker     (122)     5102 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/corpus/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    14410 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/corpus/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.551702 pythainlp-4.1.0b2/pythainlp/el/
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/el/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/el/_multiel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/el/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.551702 pythainlp-4.1.0b2/pythainlp/generate/
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/generate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/generate/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (122)     7627 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/generate/wangchanglm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.551702 pythainlp-4.1.0b2/pythainlp/khavee/
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/khavee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20883 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/khavee/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/khavee/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.555702 pythainlp-4.1.0b2/pythainlp/parse/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5878 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/parse/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/parse/esupar_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/parse/spacy_thai_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4903 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/parse/transformers_ud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/parse/ud_goeswith.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.555702 pythainlp-4.1.0b2/pythainlp/soundex/
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/soundex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/soundex/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/soundex/lk82.py
--rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/soundex/metasound.py
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/soundex/prayut_and_somchaip.py
--rw-r--r--   0 runner    (1001) docker     (122)     2835 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/soundex/sound.py
--rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/soundex/udom83.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.555702 pythainlp-4.1.0b2/pythainlp/spell/
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/spell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/spell/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/spell/phunspell.py
--rw-r--r--   0 runner    (1001) docker     (122)    11880 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/spell/pn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/spell/symspellpy.py
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/spell/tltk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.555702 pythainlp-4.1.0b2/pythainlp/summarize/
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12359 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/summarize/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/summarize/freq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/summarize/keybert.py
--rw-r--r--   0 runner    (1001) docker     (122)     3006 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/summarize/mt5.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.559702 pythainlp-4.1.0b2/pythainlp/tag/
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/_tag_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/chunk.py
--rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/crfchunk.py
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/locations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5974 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/orchid.py
--rw-r--r--   0 runner    (1001) docker     (122)     2617 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/pos_tag.py
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/thai_nner.py
--rw-r--r--   0 runner    (1001) docker     (122)     8068 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/thainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/unigram.py
--rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tag/wangchanberta_onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.563702 pythainlp-4.1.0b2/pythainlp/tokenize/
--rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/attacut.py
--rw-r--r--   0 runner    (1001) docker     (122)    29817 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/crfcls.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/crfcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/deepcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/etcc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/longest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/multi_cut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/nercut.py
--rw-r--r--   0 runner    (1001) docker     (122)     7383 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/newmm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/nlpo3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/oskut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/sefr_cut.py
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/ssg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/tcc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/tcc_p.py
--rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/thaisumcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tokenize/wtsplit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.563702 pythainlp-4.1.0b2/pythainlp/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tools/misspell.py
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/tools/path.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.567702 pythainlp-4.1.0b2/pythainlp/translate/
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/translate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/translate/en_th.py
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/translate/small100.py
--rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/translate/th_fr.py
--rw-r--r--   0 runner    (1001) docker     (122)    15964 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/translate/tokenization_small100.py
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/translate/zh_th.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.567702 pythainlp-4.1.0b2/pythainlp/transliterate/
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/ipa.py
--rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/iso_11940.py
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/lookup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/royin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/spoonerism.py
--rw-r--r--   0 runner    (1001) docker     (122)    11993 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/thai2rom.py
--rw-r--r--   0 runner    (1001) docker     (122)     6477 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/thai2rom_onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/thaig2p.py
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/w2p.py
--rw-r--r--   0 runner    (1001) docker     (122)     5848 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/transliterate/wunsen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.567702 pythainlp-4.1.0b2/pythainlp/ulmfit/
--rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/ulmfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/ulmfit/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/ulmfit/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/ulmfit/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.571702 pythainlp-4.1.0b2/pythainlp/util/
--rw-r--r--   0 runner    (1001) docker     (122)     3545 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/abbreviation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    12287 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/date.py
--rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/digitconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    93944 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/emojiconv.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/encoding.py
--rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/keywords.py
--rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/normalize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/numtoword.py
--rw-r--r--   0 runner    (1001) docker     (122)     5284 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/phoneme.py
--rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/spell_words.py
--rw-r--r--   0 runner    (1001) docker     (122)    13782 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/strftime.py
--rw-r--r--   0 runner    (1001) docker     (122)    10169 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/syllable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/thai.py
--rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/thaiwordcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     7102 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/util/wordtonum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.575702 pythainlp-4.1.0b2/pythainlp/wangchanberta/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/wangchanberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8662 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/wangchanberta/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.575702 pythainlp-4.1.0b2/pythainlp/word_vector/
--rw-r--r--   0 runner    (1001) docker     (122)      800 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/word_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14056 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/word_vector/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.575702 pythainlp-4.1.0b2/pythainlp/wsd/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/wsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5449 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/pythainlp/wsd/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.543702 pythainlp-4.1.0b2/pythainlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-07-27 13:55:16.000000 pythainlp-4.1.0b2/pythainlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5717 2023-07-27 13:55:16.000000 pythainlp-4.1.0b2/pythainlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 13:55:16.000000 pythainlp-4.1.0b2/pythainlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-27 13:55:16.000000 pythainlp-4.1.0b2/pythainlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 13:55:16.000000 pythainlp-4.1.0b2/pythainlp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-07-27 13:55:16.000000 pythainlp-4.1.0b2/pythainlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-27 13:55:16.000000 pythainlp-4.1.0b2/pythainlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      702 2023-07-27 13:55:16.579702 pythainlp-4.1.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     6572 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.579702 pythainlp-4.1.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 13:55:16.579702 pythainlp-4.1.0b2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/data/eval-details-input.json
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/data/eval-input.yml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/data/input.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/data/sentences.yml
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_cls.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_coref.py
--rw-r--r--   0 runner    (1001) docker     (122)     7255 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_el.py
--rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_khavee.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_misspell.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_soundex.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_spell.py
--rw-r--r--   0 runner    (1001) docker     (122)     5810 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (122)    17423 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (122)    56445 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_transliterate.py
--rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_ulmfit.py
--rw-r--r--   0 runner    (1001) docker     (122)    37455 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_wangchanberta.py
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_word_vector.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-27 13:55:00.000000 pythainlp-4.1.0b2/tests/test_wsd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.507603 pythainlp-4.1.0b3/
+-rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-08-04 06:02:46.000000 pythainlp-4.1.0b3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-08-04 06:02:46.000000 pythainlp-4.1.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-08-04 06:02:46.000000 pythainlp-4.1.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-08-04 06:03:02.507603 pythainlp-4.1.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-08-04 06:02:46.000000 pythainlp-4.1.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    15412 2023-08-04 06:02:46.000000 pythainlp-4.1.0b3/README_TH.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.479603 pythainlp-4.1.0b3/pythainlp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.479603 pythainlp-4.1.0b3/pythainlp/augment/
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.483603 pythainlp-4.1.0b3/pythainlp/augment/lm/
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/lm/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/lm/wangchanberta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.483603 pythainlp-4.1.0b3/pythainlp/augment/word2vec/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/word2vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/word2vec/bpemb_wv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/word2vec/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/word2vec/ltw2v.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/word2vec/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/augment/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.483603 pythainlp-4.1.0b3/pythainlp/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/benchmarks/word_tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.483603 pythainlp-4.1.0b3/pythainlp/chat/
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/chat/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.483603 pythainlp-4.1.0b3/pythainlp/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/cli/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/cli/soundex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/cli/tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5275 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/cli/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.483603 pythainlp-4.1.0b3/pythainlp/cls/
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/cls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/cls/param_free.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.483603 pythainlp-4.1.0b3/pythainlp/coref/
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/coref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/coref/_fastcoref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/coref/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      930 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/coref/han_coref.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.487603 pythainlp-4.1.0b3/pythainlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11287 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17555 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/oscar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/th_en_translit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/tnc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/ttc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5102 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14410 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/corpus/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.487603 pythainlp-4.1.0b3/pythainlp/el/
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/el/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/el/_multiel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/el/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.487603 pythainlp-4.1.0b3/pythainlp/generate/
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/generate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/generate/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7627 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/generate/wangchanglm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.487603 pythainlp-4.1.0b3/pythainlp/khavee/
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/khavee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20883 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/khavee/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/khavee/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.487603 pythainlp-4.1.0b3/pythainlp/parse/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5878 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/parse/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/parse/esupar_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/parse/spacy_thai_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4903 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/parse/transformers_ud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/parse/ud_goeswith.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.487603 pythainlp-4.1.0b3/pythainlp/soundex/
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/soundex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/soundex/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/soundex/lk82.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/soundex/metasound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/soundex/prayut_and_somchaip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2835 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/soundex/sound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/soundex/udom83.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.491603 pythainlp-4.1.0b3/pythainlp/spell/
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/spell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/spell/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/spell/phunspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11880 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/spell/pn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/spell/symspellpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/spell/tltk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.491603 pythainlp-4.1.0b3/pythainlp/summarize/
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12359 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/summarize/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/summarize/freq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/summarize/keybert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3006 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/summarize/mt5.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.491603 pythainlp-4.1.0b3/pythainlp/tag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/_tag_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/crfchunk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/locations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5974 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/orchid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2617 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/pos_tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/thai_nner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8068 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/thainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/unigram.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tag/wangchanberta_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.495603 pythainlp-4.1.0b3/pythainlp/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/attacut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30220 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/crfcls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/crfcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/deepcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/etcc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/han_solo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/longest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/multi_cut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/nercut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7383 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/newmm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/nlpo3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/oskut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/sefr_cut.py
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/ssg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/tcc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/tcc_p.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/thaisumcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tokenize/wtsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.495603 pythainlp-4.1.0b3/pythainlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tools/misspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/tools/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.495603 pythainlp-4.1.0b3/pythainlp/translate/
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/translate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/translate/en_th.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/translate/small100.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/translate/th_fr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15964 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/translate/tokenization_small100.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/translate/zh_th.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.499603 pythainlp-4.1.0b3/pythainlp/transliterate/
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/iso_11940.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/royin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/spoonerism.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11993 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/thai2rom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6477 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/thai2rom_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/thaig2p.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/w2p.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5848 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/transliterate/wunsen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.499603 pythainlp-4.1.0b3/pythainlp/ulmfit/
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/ulmfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/ulmfit/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/ulmfit/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/ulmfit/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.499603 pythainlp-4.1.0b3/pythainlp/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     3545 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/abbreviation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12287 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/digitconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93944 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/emojiconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/numtoword.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5284 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/phoneme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/spell_words.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13782 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10169 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/syllable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/thai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/thaiwordcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7102 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/util/wordtonum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.503603 pythainlp-4.1.0b3/pythainlp/wangchanberta/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/wangchanberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8662 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/wangchanberta/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.503603 pythainlp-4.1.0b3/pythainlp/word_vector/
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/word_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14056 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/word_vector/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.503603 pythainlp-4.1.0b3/pythainlp/wsd/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/wsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5449 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/pythainlp/wsd/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.479603 pythainlp-4.1.0b3/pythainlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-08-04 06:03:02.000000 pythainlp-4.1.0b3/pythainlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-08-04 06:03:02.000000 pythainlp-4.1.0b3/pythainlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 06:03:02.000000 pythainlp-4.1.0b3/pythainlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-08-04 06:03:02.000000 pythainlp-4.1.0b3/pythainlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 06:03:02.000000 pythainlp-4.1.0b3/pythainlp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-08-04 06:03:02.000000 pythainlp-4.1.0b3/pythainlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-04 06:03:02.000000 pythainlp-4.1.0b3/pythainlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      702 2023-08-04 06:03:02.507603 pythainlp-4.1.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     6572 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.503603 pythainlp-4.1.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 06:03:02.507603 pythainlp-4.1.0b3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/data/eval-details-input.json
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/data/eval-input.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/data/input.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/data/sentences.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_cls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_coref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7255 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_el.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_khavee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_misspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_soundex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_spell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5810 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17423 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56962 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_ulmfit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37455 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_wangchanberta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_word_vector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-08-04 06:02:47.000000 pythainlp-4.1.0b3/tests/test_wsd.py
```

### Comparing `pythainlp-4.1.0b2/CONTRIBUTING.md` & `pythainlp-4.1.0b3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/LICENSE` & `pythainlp-4.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/PKG-INFO` & `pythainlp-4.1.0b3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 4.1.0b2
+Version: 4.1.0b3
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://pythainlp.github.io/docs/4.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
```

### Comparing `pythainlp-4.1.0b2/README.md` & `pythainlp-4.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/README_TH.md` & `pythainlp-4.1.0b3/README_TH.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/__init__.py` & `pythainlp-4.1.0b3/pythainlp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # URL: <https://pythainlp.github.io/>
 # For license information, see LICENSE
-__version__ = "4.1.0beta2"
+__version__ = "4.1.0beta3"
 
 thai_consonants = "กขฃคฅฆงจฉชซฌญฎฏฐฑฒณดตถทธนบปผฝพฟภมยรลวศษสหฬอฮ"  # 44 chars
 
 thai_vowels = (
     "\u0e24\u0e26\u0e30\u0e31\u0e32\u0e33\u0e34\u0e35\u0e36\u0e37"
     + "\u0e38\u0e39\u0e40\u0e41\u0e42\u0e43\u0e44\u0e45\u0e4d\u0e47"
 )  # 20
```

### Comparing `pythainlp-4.1.0b2/pythainlp/__main__.py` & `pythainlp-4.1.0b3/pythainlp/__main__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/__init__.py` & `pythainlp-4.1.0b3/pythainlp/augment/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/lm/__init__.py` & `pythainlp-4.1.0b3/pythainlp/augment/lm/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/lm/fasttext.py` & `pythainlp-4.1.0b3/pythainlp/augment/lm/fasttext.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/lm/wangchanberta.py` & `pythainlp-4.1.0b3/pythainlp/augment/lm/wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/word2vec/__init__.py` & `pythainlp-4.1.0b3/pythainlp/augment/word2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/word2vec/bpemb_wv.py` & `pythainlp-4.1.0b3/pythainlp/augment/word2vec/bpemb_wv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/word2vec/core.py` & `pythainlp-4.1.0b3/pythainlp/augment/word2vec/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/word2vec/ltw2v.py` & `pythainlp-4.1.0b3/pythainlp/augment/word2vec/ltw2v.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/word2vec/thai2fit.py` & `pythainlp-4.1.0b3/pythainlp/augment/word2vec/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/augment/wordnet.py` & `pythainlp-4.1.0b3/pythainlp/augment/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/benchmarks/__init__.py` & `pythainlp-4.1.0b3/pythainlp/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/benchmarks/word_tokenization.py` & `pythainlp-4.1.0b3/pythainlp/benchmarks/word_tokenization.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/chat/__init__.py` & `pythainlp-4.1.0b3/pythainlp/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/chat/core.py` & `pythainlp-4.1.0b3/pythainlp/chat/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/cli/__init__.py` & `pythainlp-4.1.0b3/pythainlp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/cli/benchmark.py` & `pythainlp-4.1.0b3/pythainlp/cli/benchmark.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/cli/data.py` & `pythainlp-4.1.0b3/pythainlp/cli/data.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/cli/soundex.py` & `pythainlp-4.1.0b3/pythainlp/cli/soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/cli/tag.py` & `pythainlp-4.1.0b3/pythainlp/cli/tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/cli/tokenize.py` & `pythainlp-4.1.0b3/pythainlp/cli/tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/cls/__init__.py` & `pythainlp-4.1.0b3/pythainlp/cls/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/cls/param_free.py` & `pythainlp-4.1.0b3/pythainlp/cls/param_free.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/coref/__init__.py` & `pythainlp-4.1.0b3/pythainlp/coref/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/coref/_fastcoref.py` & `pythainlp-4.1.0b3/pythainlp/coref/_fastcoref.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/coref/core.py` & `pythainlp-4.1.0b3/pythainlp/coref/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/coref/han_coref.py` & `pythainlp-4.1.0b3/pythainlp/coref/han_coref.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/__init__.py` & `pythainlp-4.1.0b3/pythainlp/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/common.py` & `pythainlp-4.1.0b3/pythainlp/corpus/common.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/conceptnet.py` & `pythainlp-4.1.0b3/pythainlp/corpus/conceptnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/core.py` & `pythainlp-4.1.0b3/pythainlp/corpus/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/oscar.py` & `pythainlp-4.1.0b3/pythainlp/corpus/oscar.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/th_en_translit.py` & `pythainlp-4.1.0b3/pythainlp/corpus/th_en_translit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/tnc.py` & `pythainlp-4.1.0b3/pythainlp/corpus/tnc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/ttc.py` & `pythainlp-4.1.0b3/pythainlp/corpus/ttc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/util.py` & `pythainlp-4.1.0b3/pythainlp/corpus/util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/corpus/wordnet.py` & `pythainlp-4.1.0b3/pythainlp/corpus/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/el/__init__.py` & `pythainlp-4.1.0b3/pythainlp/el/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/el/_multiel.py` & `pythainlp-4.1.0b3/pythainlp/el/_multiel.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/el/core.py` & `pythainlp-4.1.0b3/pythainlp/el/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/generate/__init__.py` & `pythainlp-4.1.0b3/pythainlp/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/generate/core.py` & `pythainlp-4.1.0b3/pythainlp/generate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/generate/thai2fit.py` & `pythainlp-4.1.0b3/pythainlp/generate/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/generate/wangchanglm.py` & `pythainlp-4.1.0b3/pythainlp/generate/wangchanglm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/khavee/__init__.py` & `pythainlp-4.1.0b3/pythainlp/khavee/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/khavee/core.py` & `pythainlp-4.1.0b3/pythainlp/khavee/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/khavee/example.py` & `pythainlp-4.1.0b3/pythainlp/khavee/example.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/parse/__init__.py` & `pythainlp-4.1.0b3/pythainlp/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/parse/core.py` & `pythainlp-4.1.0b3/pythainlp/parse/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/parse/esupar_engine.py` & `pythainlp-4.1.0b3/pythainlp/parse/esupar_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/parse/spacy_thai_engine.py` & `pythainlp-4.1.0b3/pythainlp/parse/spacy_thai_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/parse/transformers_ud.py` & `pythainlp-4.1.0b3/pythainlp/parse/transformers_ud.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/parse/ud_goeswith.py` & `pythainlp-4.1.0b3/pythainlp/parse/ud_goeswith.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/soundex/__init__.py` & `pythainlp-4.1.0b3/pythainlp/soundex/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/soundex/core.py` & `pythainlp-4.1.0b3/pythainlp/soundex/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/soundex/lk82.py` & `pythainlp-4.1.0b3/pythainlp/soundex/lk82.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/soundex/metasound.py` & `pythainlp-4.1.0b3/pythainlp/soundex/metasound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/soundex/prayut_and_somchaip.py` & `pythainlp-4.1.0b3/pythainlp/soundex/prayut_and_somchaip.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/soundex/sound.py` & `pythainlp-4.1.0b3/pythainlp/soundex/sound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/soundex/udom83.py` & `pythainlp-4.1.0b3/pythainlp/soundex/udom83.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/spell/__init__.py` & `pythainlp-4.1.0b3/pythainlp/spell/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/spell/core.py` & `pythainlp-4.1.0b3/pythainlp/spell/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/spell/phunspell.py` & `pythainlp-4.1.0b3/pythainlp/spell/phunspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/spell/pn.py` & `pythainlp-4.1.0b3/pythainlp/spell/pn.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/spell/symspellpy.py` & `pythainlp-4.1.0b3/pythainlp/spell/symspellpy.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/spell/tltk.py` & `pythainlp-4.1.0b3/pythainlp/spell/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/summarize/__init__.py` & `pythainlp-4.1.0b3/pythainlp/summarize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/summarize/core.py` & `pythainlp-4.1.0b3/pythainlp/summarize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/summarize/freq.py` & `pythainlp-4.1.0b3/pythainlp/summarize/freq.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/summarize/keybert.py` & `pythainlp-4.1.0b3/pythainlp/summarize/keybert.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/summarize/mt5.py` & `pythainlp-4.1.0b3/pythainlp/summarize/mt5.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/__init__.py` & `pythainlp-4.1.0b3/pythainlp/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/_tag_perceptron.py` & `pythainlp-4.1.0b3/pythainlp/tag/_tag_perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/blackboard.py` & `pythainlp-4.1.0b3/pythainlp/tag/blackboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/chunk.py` & `pythainlp-4.1.0b3/pythainlp/tag/chunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/crfchunk.py` & `pythainlp-4.1.0b3/pythainlp/tag/crfchunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/locations.py` & `pythainlp-4.1.0b3/pythainlp/tag/locations.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/named_entity.py` & `pythainlp-4.1.0b3/pythainlp/tag/named_entity.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/orchid.py` & `pythainlp-4.1.0b3/pythainlp/tag/orchid.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/perceptron.py` & `pythainlp-4.1.0b3/pythainlp/tag/perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/pos_tag.py` & `pythainlp-4.1.0b3/pythainlp/tag/pos_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/thai_nner.py` & `pythainlp-4.1.0b3/pythainlp/tag/thai_nner.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/thainer.py` & `pythainlp-4.1.0b3/pythainlp/tag/thainer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/tltk.py` & `pythainlp-4.1.0b3/pythainlp/tag/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/unigram.py` & `pythainlp-4.1.0b3/pythainlp/tag/unigram.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tag/wangchanberta_onnx.py` & `pythainlp-4.1.0b3/pythainlp/tag/wangchanberta_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/__init__.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/_utils.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/_utils.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/attacut.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/attacut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/core.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -526,18 +526,23 @@
     :param str text: text to be tokenized
     :param str engine: the name subword tokenizer
     :return: list of subwords
     :rtype: list[str]
     **Options for engine**
         * *dict* - newmm word tokenizer with a syllable dictionary
         * *etcc* - Enhanced Thai Character Cluster (Inrut et al. 2001)
-        * *ssg* - CRF syllable segmenter for Thai
+        * *han_solo* - CRF syllable segmenter for Thai that can work in the \
+            Thai social media domain. See `PyThaiNLP/Han-solo \
+        <https://github.com/PyThaiNLP/Han-solo>`_.
+        * *ssg* - CRF syllable segmenter for Thai. See `ponrawee/ssg \
+        <https://github.com/ponrawee/ssg>`_.
         * *tcc* (default) - Thai Character Cluster (Theeramunkong et al. 2000)
         * *tcc_p* - Thai Character Cluster + improve the rule that used in newmm
-        * *tltk* - syllable tokenizer from tltk
+        * *tltk* - syllable tokenizer from tltk. See `tltk \
+        <https://pypi.org/project/tltk/>`_.
         * *wangchanberta* - SentencePiece from wangchanberta model
     :Example:
 
     Tokenize text into subword based on *tcc*::
 
         from pythainlp.tokenize import subword_tokenize
 
@@ -596,14 +601,16 @@
                     text=word, custom_dict=DEFAULT_SYLLABLE_DICT_TRIE
                 )
             )
     elif engine == "ssg":
         from pythainlp.tokenize.ssg import segment
     elif engine == "tltk":
         from pythainlp.tokenize.tltk import syllable_tokenize as segment
+    elif engine == "han_solo":
+        from pythainlp.tokenize.han_solo import segment
     else:
         raise ValueError(
             f"""Tokenizer \"{engine}\" not found.
             It might be a typo; if not, please consult our document."""
         )
 
     if segments == []:
```

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/crfcls.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/crfcls.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/crfcut.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/crfcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/deepcut.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/deepcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/etcc.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/etcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/longest.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/longest.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/multi_cut.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/multi_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/nercut.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/nercut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/newmm.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/newmm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/nlpo3.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/nlpo3.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/oskut.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/oskut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/pyicu.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/sefr_cut.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/sefr_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/ssg.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/ssg.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/tcc.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/tcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/tcc_p.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/tcc_p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/thaisumcut.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/thaisumcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/tltk.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tokenize/wtsplit.py` & `pythainlp-4.1.0b3/pythainlp/tokenize/wtsplit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tools/__init__.py` & `pythainlp-4.1.0b3/pythainlp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tools/misspell.py` & `pythainlp-4.1.0b3/pythainlp/tools/misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/tools/path.py` & `pythainlp-4.1.0b3/pythainlp/tools/path.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/translate/__init__.py` & `pythainlp-4.1.0b3/pythainlp/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/translate/core.py` & `pythainlp-4.1.0b3/pythainlp/translate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/translate/en_th.py` & `pythainlp-4.1.0b3/pythainlp/translate/en_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/translate/small100.py` & `pythainlp-4.1.0b3/pythainlp/translate/small100.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/translate/th_fr.py` & `pythainlp-4.1.0b3/pythainlp/translate/th_fr.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/translate/tokenization_small100.py` & `pythainlp-4.1.0b3/pythainlp/translate/tokenization_small100.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/translate/zh_th.py` & `pythainlp-4.1.0b3/pythainlp/translate/zh_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/__init__.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/core.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/ipa.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/ipa.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/iso_11940.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/iso_11940.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/lookup.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/lookup.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/pyicu.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/royin.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/royin.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/spoonerism.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/spoonerism.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/thai2rom.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/thai2rom.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/thai2rom_onnx.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/thai2rom_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/thaig2p.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/thaig2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/tltk.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/w2p.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/w2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/transliterate/wunsen.py` & `pythainlp-4.1.0b3/pythainlp/transliterate/wunsen.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/ulmfit/__init__.py` & `pythainlp-4.1.0b3/pythainlp/ulmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/ulmfit/core.py` & `pythainlp-4.1.0b3/pythainlp/ulmfit/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/ulmfit/preprocess.py` & `pythainlp-4.1.0b3/pythainlp/ulmfit/preprocess.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/ulmfit/tokenizer.py` & `pythainlp-4.1.0b3/pythainlp/ulmfit/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/__init__.py` & `pythainlp-4.1.0b3/pythainlp/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/abbreviation.py` & `pythainlp-4.1.0b3/pythainlp/util/abbreviation.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/collate.py` & `pythainlp-4.1.0b3/pythainlp/util/collate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/date.py` & `pythainlp-4.1.0b3/pythainlp/util/date.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/digitconv.py` & `pythainlp-4.1.0b3/pythainlp/util/digitconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/emojiconv.py` & `pythainlp-4.1.0b3/pythainlp/util/emojiconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/encoding.py` & `pythainlp-4.1.0b3/pythainlp/util/encoding.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/keyboard.py` & `pythainlp-4.1.0b3/pythainlp/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/keywords.py` & `pythainlp-4.1.0b3/pythainlp/util/keywords.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/normalize.py` & `pythainlp-4.1.0b3/pythainlp/util/normalize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/numtoword.py` & `pythainlp-4.1.0b3/pythainlp/util/numtoword.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/phoneme.py` & `pythainlp-4.1.0b3/pythainlp/util/phoneme.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/spell_words.py` & `pythainlp-4.1.0b3/pythainlp/util/spell_words.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/strftime.py` & `pythainlp-4.1.0b3/pythainlp/util/strftime.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/syllable.py` & `pythainlp-4.1.0b3/pythainlp/util/syllable.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/thai.py` & `pythainlp-4.1.0b3/pythainlp/util/thai.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/thaiwordcheck.py` & `pythainlp-4.1.0b3/pythainlp/util/thaiwordcheck.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/time.py` & `pythainlp-4.1.0b3/pythainlp/util/time.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/trie.py` & `pythainlp-4.1.0b3/pythainlp/util/trie.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/util/wordtonum.py` & `pythainlp-4.1.0b3/pythainlp/util/wordtonum.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/wangchanberta/__init__.py` & `pythainlp-4.1.0b3/pythainlp/wangchanberta/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/wangchanberta/core.py` & `pythainlp-4.1.0b3/pythainlp/wangchanberta/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/word_vector/__init__.py` & `pythainlp-4.1.0b3/pythainlp/word_vector/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/word_vector/core.py` & `pythainlp-4.1.0b3/pythainlp/word_vector/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/wsd/__init__.py` & `pythainlp-4.1.0b3/pythainlp/wsd/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp/wsd/core.py` & `pythainlp-4.1.0b3/pythainlp/wsd/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/pythainlp.egg-info/PKG-INFO` & `pythainlp-4.1.0b3/pythainlp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 4.1.0b2
+Version: 4.1.0b3
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://pythainlp.github.io/docs/4.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
```

### Comparing `pythainlp-4.1.0b2/pythainlp.egg-info/SOURCES.txt` & `pythainlp-4.1.0b3/pythainlp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 pythainlp/tokenize/_utils.py
 pythainlp/tokenize/attacut.py
 pythainlp/tokenize/core.py
 pythainlp/tokenize/crfcls.py
 pythainlp/tokenize/crfcut.py
 pythainlp/tokenize/deepcut.py
 pythainlp/tokenize/etcc.py
+pythainlp/tokenize/han_solo.py
 pythainlp/tokenize/longest.py
 pythainlp/tokenize/multi_cut.py
 pythainlp/tokenize/nercut.py
 pythainlp/tokenize/newmm.py
 pythainlp/tokenize/nlpo3.py
 pythainlp/tokenize/oskut.py
 pythainlp/tokenize/pyicu.py
```

### Comparing `pythainlp-4.1.0b2/pythainlp.egg-info/requires.txt` & `pythainlp-4.1.0b3/pythainlp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/setup.cfg` & `pythainlp-4.1.0b3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.1.0beta2
+current_version = 4.1.0beta3
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `pythainlp-4.1.0b2/setup.py` & `pythainlp-4.1.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         "sentence-transformers>=2.2.2",
         "khamyo>=0.2.0",
     ],
 }
 
 setup(
     name="pythainlp",
-    version="4.1.0beta2",
+    version="4.1.0beta3",
     description="Thai Natural Language Processing library",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="PyThaiNLP",
     author_email="email@wannaphong.com",
     url="https://github.com/PyThaiNLP/pythainlp",
     packages=find_packages(exclude=["tests", "tests.*"]),
```

### Comparing `pythainlp-4.1.0b2/tests/data/eval-details-input.json` & `pythainlp-4.1.0b3/tests/data/eval-details-input.json`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/data/sentences.yml` & `pythainlp-4.1.0b3/tests/data/sentences.yml`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_augment.py` & `pythainlp-4.1.0b3/tests/test_augment.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_benchmarks.py` & `pythainlp-4.1.0b3/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_cli.py` & `pythainlp-4.1.0b3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_cls.py` & `pythainlp-4.1.0b3/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_corpus.py` & `pythainlp-4.1.0b3/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_generate.py` & `pythainlp-4.1.0b3/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_khavee.py` & `pythainlp-4.1.0b3/tests/test_khavee.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_misspell.py` & `pythainlp-4.1.0b3/tests/test_misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_parse.py` & `pythainlp-4.1.0b3/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_soundex.py` & `pythainlp-4.1.0b3/tests/test_soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_spell.py` & `pythainlp-4.1.0b3/tests/test_spell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_summarize.py` & `pythainlp-4.1.0b3/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_tag.py` & `pythainlp-4.1.0b3/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_tokenize.py` & `pythainlp-4.1.0b3/tests/test_tokenize.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,23 +395,33 @@
             subword_tokenize("สวัสดีชาวโลก", engine="dict"),
             ["สวัส", "ดี", "ชาว", "โลก"],
         )
         self.assertFalse(
             "า" in subword_tokenize("สวัสดีชาวโลก", engine="dict")
         )
         self.assertEqual(subword_tokenize(None, engine="ssg"), [])
+        self.assertEqual(subword_tokenize(None, engine="han_solo"), [])
         self.assertEqual(
             subword_tokenize("แมวกินปลา", engine="ssg"), ["แมว", "กิน", "ปลา"]
         )
         self.assertTrue(
             "ดาว" in subword_tokenize("สวัสดีดาวอังคาร", engine="ssg")
         )
         self.assertFalse(
             "า" in subword_tokenize("สวัสดีดาวอังคาร", engine="ssg")
         )
+        self.assertEqual(
+            subword_tokenize("แมวกินปลา", engine="han_solo"), ["แมว", "กิน", "ปลา"]
+        )
+        self.assertTrue(
+            "ดาว" in subword_tokenize("สวัสดีดาวอังคาร", engine="han_solo")
+        )
+        self.assertFalse(
+            "า" in subword_tokenize("สวัสดีดาวอังคาร", engine="han_solo")
+        )
         self.assertFalse(
             " " in subword_tokenize("พันธมิตร ชา นม", keep_whitespace=False)
         )
         self.assertEqual(subword_tokenize(None, engine="tltk"), [])
         self.assertEqual(subword_tokenize("", engine="tltk"), [])
         self.assertIsInstance(
             subword_tokenize("สวัสดิีดาวอังคาร", engine="tltk"), list
```

### Comparing `pythainlp-4.1.0b2/tests/test_translate.py` & `pythainlp-4.1.0b3/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_transliterate.py` & `pythainlp-4.1.0b3/tests/test_transliterate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_ulmfit.py` & `pythainlp-4.1.0b3/tests/test_ulmfit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_util.py` & `pythainlp-4.1.0b3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_wangchanberta.py` & `pythainlp-4.1.0b3/tests/test_wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_word_vector.py` & `pythainlp-4.1.0b3/tests/test_word_vector.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.1.0b2/tests/test_wsd.py` & `pythainlp-4.1.0b3/tests/test_wsd.py`

 * *Files identical despite different names*

