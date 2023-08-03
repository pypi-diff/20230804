# Comparing `tmp/agbenchmark-0.0.2.tar.gz` & `tmp/agbenchmark-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agbenchmark-0.0.2.tar", max compression
+gzip compressed data, was "agbenchmark-0.0.3.tar", max compression
```

## Comparing `agbenchmark-0.0.2.tar` & `agbenchmark-0.0.3.tar`

### file list

```diff
@@ -1,122 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/LICENSE
--rw-r--r--   0        0        0     1753 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/README.md
--rw-r--r--   0        0        0     2780 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/README.md
--rw-r--r--   0        0        0     2336 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/ReportManager.py
--rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/__init__.py
--rw-r--r--   0        0        0     2530 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/agent_interface.py
--rw-r--r--   0        0        0     5140 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenge.py
--rw-r--r--   0        0        0     2581 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/README.md
--rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_in/__init__.py
--rw-r--r--   0        0        0      325 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_in/code.py
--rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_in/test.py
--rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_out/__init__.py
--rw-r--r--   0        0        0      312 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_out/code.py
--rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/artifacts_out/test.py
--rw-r--r--   0        0        0      645 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d1_debug/data.json
--rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_in/__init__.py
--rw-r--r--   0        0        0      325 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_in/code.py
--rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_in/test.py
--rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_out/__init__.py
--rw-r--r--   0        0        0      312 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_out/code.py
--rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/artifacts_out/test.py
--rw-r--r--   0        0        0      612 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d2_vague/data.json
--rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/artifacts_out/__init__.py
--rw-r--r--   0        0        0      312 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/artifacts_out/code.py
--rw-r--r--   0        0        0      893 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/custom_python/test.py
--rw-r--r--   0        0        0      869 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d3_two_sum/data.json
--rw-r--r--   0        0        0     1171 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d4_web_server/custom_python/api_tests.py
--rw-r--r--   0        0        0      757 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d4_web_server/data.json
--rw-r--r--   0        0        0        0 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/artifacts_out/__init__.py
--rw-r--r--   0        0        0      809 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/artifacts_out/code.py
--rw-r--r--   0        0        0      921 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/custom_python/test.py
--rw-r--r--   0        0        0      933 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/code/d5_three_sum/data.json
--rw-r--r--   0        0        0     2076 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/define_task_types.py
--rw-r--r--   0        0        0       13 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/read_file/artifacts_in/file_to_check.txt
--rw-r--r--   0        0        0       27 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/read_file/artifacts_out/file_to_check.txt
--rw-r--r--   0        0        0      517 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/read_file/data.json
--rw-r--r--   0        0        0       38 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/search/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      547 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/search/data.json
--rw-r--r--   0        0        0       11 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/write_file/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      519 2023-07-24 12:12:47.323733 agbenchmark-0.0.2/agbenchmark/challenges/interface/write_file/data.json
--rw-r--r--   0        0        0       60 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_1.txt
--rw-r--r--   0        0        0       33 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_2.txt
--rw-r--r--   0        0        0       33 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_3.txt
--rw-r--r--   0        0        0       33 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_4.txt
--rw-r--r--   0        0        0       63 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_in/instructions_5.txt
--rw-r--r--   0        0        0        5 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/artifacts_out/result.txt
--rw-r--r--   0        0        0      598 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m1_id/data.json
--rw-r--r--   0        0        0       62 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_1.txt
--rw-r--r--   0        0        0       62 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_2.txt
--rw-r--r--   0        0        0       62 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_3.txt
--rw-r--r--   0        0        0       62 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_4.txt
--rw-r--r--   0        0        0       64 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_in/instructions_5.txt
--rw-r--r--   0        0        0       20 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/artifacts_out/result.txt
--rw-r--r--   0        0        0      667 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m2_multiple/data.json
--rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_1.txt
--rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_2.txt
--rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_3.txt
--rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_4.txt
--rw-r--r--   0        0        0     1068 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_in/instructions_5.txt
--rw-r--r--   0        0        0       20 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/artifacts_out/result.txt
--rw-r--r--   0        0        0      774 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m3_noise/data.json
--rw-r--r--   0        0        0     1127 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_1.txt
--rw-r--r--   0        0        0     1124 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_2.txt
--rw-r--r--   0        0        0     1117 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_3.txt
--rw-r--r--   0        0        0     1126 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_4.txt
--rw-r--r--   0        0        0     1072 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_in/instructions_5.txt
--rw-r--r--   0        0        0      226 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/artifacts_out/result.txt
--rw-r--r--   0        0        0     1234 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/memory/m4_phrases/data.json
--rw-r--r--   0        0        0        6 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r1_book_price/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      555 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r1_book_price/data.json
--rw-r--r--   0        0        0       16 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.1_specific/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      510 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.1_specific/data.json
--rw-r--r--   0        0        0       16 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.2_formatting/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      678 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2.2_formatting/data.json
--rw-r--r--   0        0        0       16 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2_tesla_revenue/artifacts_out/random_file.txt
--rw-r--r--   0        0        0      473 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r2_tesla_revenue/data.json
--rw-r--r--   0        0        0      220 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r3/artifacts_out/random_file.txt
--rw-r--r--   0        0        0     1079 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/retrieval/r3/data.json
--rw-r--r--   0        0        0     2317 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/challenges/test_all.py
--rw-r--r--   0        0        0       61 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/config.json
--rw-r--r--   0        0        0     9449 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/conftest.py
--rw-r--r--   0        0        0      466 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/metrics.py
--rw-r--r--   0        0        0     1841 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/regression_tests.json
--rw-r--r--   0        0        0     2706 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/internal_info.json
--rw-r--r--   0        0        0      648 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/1.1_TestWriteFile.json
--rw-r--r--   0        0        0     1086 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/10.1_TestRememberMultipleWithNoise.json
--rw-r--r--   0        0        0     1200 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/10_TestRememberMultipleWithNoise.json
--rw-r--r--   0        0        0     1444 2023-07-24 12:12:47.327733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.1_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1444 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.2_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1444 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.3_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1377 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.4_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1446 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11.5_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1444 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/11_TestRememberMultiplePhrasesWithNoise.json
--rw-r--r--   0        0        0     1059 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.1_TestDebugSimpleTypoWithGuidance.json
--rw-r--r--   0        0        0     1060 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.2_TestDebugSimpleTypoWithGuidance.json
--rw-r--r--   0        0        0     1066 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12.3_TestDebugSimpleTypoWithGuidance.json
--rw-r--r--   0        0        0      980 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/12_TestDebugSimpleTypoWithGuidance.json
--rw-r--r--   0        0        0      639 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/1_TestWriteFIle.json
--rw-r--r--   0        0        0      644 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/2.1_TestReadFile.json
--rw-r--r--   0        0        0      636 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/2_TestReadFile.json
--rw-r--r--   0        0        0      638 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/3.1_TestSearch.json
--rw-r--r--   0        0        0      630 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/3_TestSearch.json
--rw-r--r--   0        0        0      634 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/4.1_TestBasicRetrieval.json
--rw-r--r--   0        0        0      641 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/4_TestBasicRetrieval.json
--rw-r--r--   0        0        0      814 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/5.1_TestRetrieval2.0.json
--rw-r--r--   0        0        0      753 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/5_TestRetrieval2.0.json
--rw-r--r--   0        0        0      841 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.1_TestRetrieval2.1.json
--rw-r--r--   0        0        0      836 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.2_TestRetrieval2.1.json
--rw-r--r--   0        0        0      836 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.3_TestRetrieval2.1.json
--rw-r--r--   0        0        0      908 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6.4_TestRetrieval2.1.json
--rw-r--r--   0        0        0      823 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/6_TestRetrieval2.1.json
--rw-r--r--   0        0        0     1073 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/7.1_TestRetrieval2.2.json
--rw-r--r--   0        0        0      893 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/7_TestRetrieval2.2.json
--rw-r--r--   0        0        0      908 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/8.1_TestBasicMemory.json
--rw-r--r--   0        0        0     1041 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/8_TestBasicMemory.json
--rw-r--r--   0        0        0      982 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/9.1_TestRememberMultipleIds.json
--rw-r--r--   0        0        0     1110 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/reports/mini-agi/9_TestRememberMultipleIds.json
--rw-r--r--   0        0        0     3843 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/start_benchmark.py
--rw-r--r--   0        0        0     6977 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/agbenchmark/utils.py
--rw-r--r--   0        0        0     1646 2023-07-24 12:12:47.331733 agbenchmark-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 agbenchmark-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/LICENSE
+-rw-r--r--   0        0        0      934 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/README.md
+-rw-r--r--   0        0        0     2914 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/__init__.py
+-rw-r--r--   0        0        0     2698 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/agent_interface.py
+-rw-r--r--   0        0        0     9130 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/conftest.py
+-rw-r--r--   0        0        0     7855 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/generate_test.py
+-rw-r--r--   0        0        0     2864 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/reports/ReportManager.py
+-rw-r--r--   0        0        0     1355 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/reports/processing/gen_combined_chart.py
+-rw-r--r--   0        0        0     1151 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/reports/processing/get_files.py
+-rw-r--r--   0        0        0     6297 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/reports/processing/graphs.py
+-rw-r--r--   0        0        0     2362 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/reports/processing/process_report.py
+-rw-r--r--   0        0        0     1044 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/reports/processing/report_types.py
+-rw-r--r--   0        0        0    10599 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/reports/reports.py
+-rw-r--r--   0        0        0     4646 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/start_benchmark.py
+-rw-r--r--   0        0        0     9946 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/utils/challenge.py
+-rw-r--r--   0        0        0     7676 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/utils/data_types.py
+-rw-r--r--   0        0        0     2289 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/utils/get_data_from_helicone.py
+-rw-r--r--   0        0        0     2657 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/utils/prompts.py
+-rw-r--r--   0        0        0     9558 2023-08-03 23:47:50.835981 agbenchmark-0.0.3/agbenchmark/utils/utils.py
+-rw-r--r--   0        0        0     1779 2023-08-03 23:47:50.839981 agbenchmark-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2038 1970-01-01 00:00:00.000000 agbenchmark-0.0.3/PKG-INFO
```

### Comparing `agbenchmark-0.0.2/LICENSE` & `agbenchmark-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agbenchmark-0.0.2/agbenchmark/README.md` & `agbenchmark-0.0.3/agbenchmark/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 ### To run the existing mocks
 
 1. clone the repo `auto-gpt-benchmarks`
 2. `pip install poetry`
 3. `poetry shell`
 4. `poetry install`
 5. `cp .env_example .env`
-6. `agbenchmark start --mock`
+6. `git submodule update --init --remote --recursive`
+7. `agbenchmark start --mock`
    Keep config the same and watch the logs :)
 
 ### To run with mini-agi
 
 1. Navigate to `auto-gpt-benchmarks/agent/mini-agi`
 2. `pip install -r requirements.txt`
 3. `cp .env_example .env`, set `PROMPT_USER=false` and add your `OPENAI_API_KEY=`. Sset `MODEL="gpt-3.5-turbo"` if you don't have access to `gpt-4` yet. Also make sure you have Python 3.10^ installed
-4. Make sure to follow the commands above, and remove mock flag `agbenchmark start`
+4. set `AGENT_NAME=mini-agi` in `.env` file and where you want your `REPORT_LOCATION` to be
+5. Make sure to follow the commands above, and remove mock flag `agbenchmark start`
 
 - To add requirements `poetry add requirement`.
 
 Feel free to create prs to merge with `main` at will (but also feel free to ask for review) - if you can't send msg in R&D chat for access.
 
 If you push at any point and break things - it'll happen to everyone - fix it asap. Step 1 is to revert `master` to last working commit
 
@@ -61,10 +63,10 @@
 https://github.com/Significant-Gravitas/Auto-GPT-Benchmarks/pull/48/files
 
 ## How do I run agent in different environments?
 
 **To just use as the benchmark for your agent**. `pip install` the package and run `agbenchmark start`
 
 **For internal Auto-GPT ci runs**, specify the `AGENT_NAME` you want you use and set the `HOME_ENV`.
-Ex. `HOME_ENV=ci AGENT_NAME=mini-agi`
+Ex. `AGENT_NAME=mini-agi`
 
 **To develop agent alongside benchmark**, you can specify the `AGENT_NAME` you want you use and add as a submodule to the repo
```

### Comparing `agbenchmark-0.0.2/agbenchmark/ReportManager.py` & `agbenchmark-0.0.3/agbenchmark/reports/ReportManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import json
 import os
 import sys
 import time
 from datetime import datetime
-from typing import Any, Dict, Optional
+from pathlib import Path
+from typing import Any, Dict
 
-from agbenchmark.utils import get_highest_success_difficulty
+from agbenchmark.reports.processing.graphs import save_single_radar_chart
+from agbenchmark.reports.processing.process_report import get_agent_category
+from agbenchmark.reports.processing.report_types import Report
+from agbenchmark.start_benchmark import (
+    AGENT_GIT_COMMIT_SHA,
+    BENCHMARK_GIT_COMMIT_SHA,
+    BENCHMARK_START_TIME,
+    REPORTS_PATH,
+)
+from agbenchmark.utils.utils import get_highest_success_difficulty
 
 
 class ReportManager:
     """Abstracts interaction with the regression tests file"""
 
     def __init__(self, filename: str):
         self.filename = filename
@@ -33,41 +43,42 @@
             self.tests = {}
         self.save()
 
     def save(self) -> None:
         with open(self.filename, "w") as f:
             json.dump(self.tests, f, indent=4)
 
-    def add_test(
-        self,
-        test_name: str,
-        test_details: dict | list,
-        agent_name: Optional[str] = None,
-    ) -> None:
-        if agent_name:
-            if agent_name not in self.tests:
-                self.tests[agent_name] = {}
-            self.tests[agent_name][test_name] = test_details
-        else:
-            self.tests[test_name] = test_details
+    def add_test(self, test_name: str, test_details: dict | list) -> None:
+        self.tests[test_name] = test_details
 
         self.save()
 
     def remove_test(self, test_name: str) -> None:
         if test_name in self.tests:
             del self.tests[test_name]
             self.save()
 
     def end_info_report(self, config: Dict[str, Any]) -> None:
         command = " ".join(sys.argv)
         self.tests = {
             "command": command.split(os.sep)[-1],
+            "benchmark_git_commit_sha": BENCHMARK_GIT_COMMIT_SHA,
+            "agent_git_commit_sha": AGENT_GIT_COMMIT_SHA,
             "completion_time": datetime.now().strftime("%Y-%m-%d-%H:%M"),
+            "benchmark_start_time": BENCHMARK_START_TIME,
             "metrics": {
                 "run_time": str(round(time.time() - self.start_time, 2)) + " seconds",
                 "highest_difficulty": get_highest_success_difficulty(self.tests),
             },
             "tests": self.tests,
             "config": config,
         }
 
+        converted_data = Report.parse_obj(self.tests)
+
+        agent_categories = get_agent_category(converted_data)
+
+        save_single_radar_chart(
+            agent_categories, Path(REPORTS_PATH) / "radar_chart.png"
+        )
+
         self.save()
```

### Comparing `agbenchmark-0.0.2/agbenchmark/agent_interface.py` & `agbenchmark-0.0.3/agbenchmark/agent_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import select
 import shutil
 import subprocess
 import sys
 import time
 from typing import Any, Dict
 
 from dotenv import load_dotenv
@@ -12,53 +13,55 @@
 load_dotenv()
 
 mock_test_str = os.getenv("MOCK_TEST")
 MOCK_FLAG = mock_test_str.lower() == "true" if mock_test_str else False
 
 
 def run_agent(
-    task: str, config: Dict[str, Any], challenge_location: str, cutoff: int
+    task: str, config: Dict[str, Any], artifacts_location: str, cutoff: int
 ) -> None:
     """Calling to get a response"""
 
     if MOCK_FLAG:
+        print("Running mock agent")
         copy_artifacts_into_workspace(
-            config["workspace"], "artifacts_out", challenge_location
+            config["workspace"], "artifacts_out", artifacts_location
         )
     else:
         entry_path = "agbenchmark.benchmarks"
 
         timeout = cutoff
         if "--nc" in sys.argv:
             timeout = 100000
 
-        print(f"Running Python function '{entry_path}' with timeout {timeout}")
+        print(f"Running '{entry_path}' with timeout {timeout}")
+
         command = [sys.executable, "-m", entry_path, str(task)]
         process = subprocess.Popen(
             command,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             universal_newlines=True,
             cwd=HOME_DIRECTORY,
+            bufsize=1,
         )
 
         start_time = time.time()
 
         while True:
-            output = ""
-            if process.stdout is not None:
-                output = process.stdout.readline()
-                print(output.strip())
+            try:
+                # This checks if there's data to be read from stdout without blocking.
+                if process.stdout and select.select([process.stdout], [], [], 0)[0]:
+                    output = process.stdout.readline()
+                    print(output.strip())
+            except Exception as e:
+                continue
 
             # Check if process has ended, has no more output, or exceeded timeout
-            if (
-                process.poll() is not None
-                or output == ""
-                or (time.time() - start_time > timeout)
-            ):
+            if process.poll() is not None or (time.time() - start_time > timeout):
                 break
 
         if time.time() - start_time > timeout:
             print("The Python function has exceeded the time limit and was terminated.")
             process.kill()
         else:
             print("The Python function has finished running.")
```

### Comparing `agbenchmark-0.0.2/agbenchmark/start_benchmark.py` & `agbenchmark-0.0.3/agbenchmark/start_benchmark.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,146 @@
 import json
 import os
 import sys
+from datetime import datetime
 from pathlib import Path
 from typing import Any
 
 import click
 import pytest
+from helicone.lock import HeliconeLockManager
 
-from agbenchmark.utils import calculate_dynamic_paths
+from agbenchmark.utils.utils import (
+    AGENT_NAME,
+    calculate_dynamic_paths,
+    get_git_commit_sha,
+)
 
 CURRENT_DIRECTORY = Path(__file__).resolve().parent
+BENCHMARK_START_TIME = datetime.now().strftime("%Y-%m-%d-%H:%M")
+
+HeliconeLockManager.write_custom_property("benchmark_start_time", BENCHMARK_START_TIME)
 
 (
     HOME_DIRECTORY,
     CONFIG_PATH,
     REGRESSION_TESTS_PATH,
-    INFO_TESTS_PATH,
+    REPORTS_PATH,
+    SUCCESS_RATE_PATH,
+    CHALLENGES_PATH,
 ) = calculate_dynamic_paths()
+BENCHMARK_GIT_COMMIT_SHA = get_git_commit_sha(HOME_DIRECTORY / ".." / "..")
+AGENT_GIT_COMMIT_SHA = get_git_commit_sha(HOME_DIRECTORY)
 
 
 @click.group()
 def cli() -> None:
     pass
 
 
 @cli.command()
 @click.option("--category", default=None, help="Specific category to run")
 @click.option("--test", default=None, help="Specific test to run")
 @click.option("--maintain", is_flag=True, help="Runs only regression tests")
 @click.option("--improve", is_flag=True, help="Run only non-regression tests")
 @click.option("--mock", is_flag=True, help="Run with mock")
+@click.option("--suite", default=None, help="Run a suite of related tests")
+@click.option(
+    "--no_dep",
+    is_flag=True,
+    help="Run without dependencies (can be useful for a suite run)",
+)
 @click.option("--nc", is_flag=True, help="Run without cutoff")
 def start(
-    category: str, test: str, maintain: bool, improve: bool, mock: bool, nc: bool
+    category: str,
+    test: str,
+    maintain: bool,
+    improve: bool,
+    mock: bool,
+    suite: str,
+    no_dep: bool,
+    nc: bool,
 ) -> int:
     """Start the benchmark tests. If a category flag is provided, run the categories with that mark."""
     # Check if configuration file exists and is not empty
 
     if maintain and improve:
         print(
             "Error: You can't use both --maintain and --improve at the same time. Please choose one."
         )
         return 1
 
-    if test and (category or maintain or improve):
+    if test and (category or maintain or improve or suite):
         print(
             "Error: If you're running a specific test make sure no other options are selected. Please just pass the --test."
         )
         return 1
 
-    print(CONFIG_PATH, os.path.exists(CONFIG_PATH), os.stat(CONFIG_PATH).st_size)
+    # TODO: test and ensure that this functionality works before removing
+    # change elif suite below if removing
+    if suite and (category or maintain or improve):
+        print(
+            "Error: If you're running a specific suite make sure no other options are selected. Please just pass the --suite."
+        )
+        return 1
+
+    if os.path.join("Auto-GPT-Benchmarks") in str(HOME_DIRECTORY) and not AGENT_NAME:
+        print(
+            "If you are running from the Auto-GPT-Benchmarks repo, you must have AGENT_NAME defined."
+        )
+        return 1
+
     if not os.path.exists(CONFIG_PATH) or os.stat(CONFIG_PATH).st_size == 0:
         config = {}
 
         config["workspace"] = click.prompt(
             "Please enter a new workspace path",
-            default=os.path.join(Path.home(), "workspace"),
-        )
-
-        config["entry_path"] = click.prompt(
-            "Please enter a the path to your run_specific_agent function implementation within the benchmarks folder",
-            default="agbenchmark/benchmarks.py",
-        )
-
-        config["cutoff"] = click.prompt(
-            "Please enter a hard cutoff runtime for your agent per test",
-            default="60",
+            default=os.path.join("workspace"),
+            show_default=True,
         )
 
         with open(CONFIG_PATH, "w") as f:
             json.dump(config, f)
     else:
         # If the configuration file exists and is not empty, load it
         with open(CONFIG_PATH, "r") as f:
             config = json.load(f)
 
-    os.environ["MOCK_TEST"] = "True" if mock else "False"
-
-    if not os.path.exists(REGRESSION_TESTS_PATH):
-        with open(REGRESSION_TESTS_PATH, "w"):
-            pass
-
-    if not os.path.exists(INFO_TESTS_PATH):
-        with open(INFO_TESTS_PATH, "w"):
-            pass
-
     print("Current configuration:")
     for key, value in config.items():
         print(f"{key}: {value}")
 
+    os.environ["MOCK_TEST"] = "True" if mock else "False"
+
     pytest_args = ["-vs"]
     if test:
         print("Running specific test:", test)
         pytest_args.extend(["-k", test, "--test"])
+    elif suite:
+        print("Running specific suite:", suite)
+        pytest_args.extend(["--suite"])
     else:
         if category:
-            pytest_args.extend(["-m", category])
+            pytest_args.extend(["-m", category, "--category"])
             print("Running tests of category:", category)
         else:
             print("Running all categories")
 
         if maintain:
             print("Running only regression tests")
             pytest_args.append("--maintain")
         elif improve:
             print("Running only non-regression tests")
             pytest_args.append("--improve")
 
     if mock:
         pytest_args.append("--mock")
 
+    if no_dep:
+        pytest_args.append("--no_dep")
     if nc:
         pytest_args.append("--nc")
 
     # when used as a library, the pytest directory to execute is in the CURRENT_DIRECTORY
     pytest_args.append(str(CURRENT_DIRECTORY))
 
     return sys.exit(pytest.main(pytest_args))
```

### Comparing `agbenchmark-0.0.2/agbenchmark/utils.py` & `agbenchmark-0.0.3/agbenchmark/utils/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,94 @@
 # radio charts, logs, helper functions for tests, anything else relevant.
-import glob
 import math
 import os
 import re
 import sys
 from datetime import datetime
 from pathlib import Path
-from typing import Any
+from typing import Any, Optional
 
+import git
 from dotenv import load_dotenv
 
 load_dotenv()
 
-from agbenchmark.challenges.define_task_types import DIFFICULTY_MAP, DifficultyLevel
+from agbenchmark.utils.data_types import DIFFICULTY_MAP, DifficultyLevel
 
 AGENT_NAME = os.getenv("AGENT_NAME")
-HOME_ENV = os.getenv("HOME_ENV")
-report_location = os.getenv("REPORT_LOCATION", None)
+REPORT_LOCATION = os.getenv("REPORT_LOCATION", None)
 
 
 def calculate_info_test_path(reports_path: Path) -> str:
-    if report_location:
-        reports_path = Path(os.getcwd()) / report_location
-
     command = sys.argv
 
     if not reports_path.exists():
         reports_path.mkdir(parents=True, exist_ok=True)
 
-    json_files = glob.glob(str(reports_path / "*.json"))
+    # Collect all directories in reports_path
+    all_items = os.listdir(str(reports_path))
+    dirs = [item for item in all_items if os.path.isdir(reports_path / item)]
 
     # Default naming scheme
-    file_count = len(json_files)
-    run_name = f"file{file_count + 1}_{datetime.now().strftime('%m-%d-%H-%M')}.json"
+    dir_count = len(dirs)
+    run_name = f"folder{dir_count + 1}_{datetime.now().strftime('%m-%d-%H-%M')}"
 
-    # # If "--test" is in command
+    test_index = None
+    test_arg = None
+    # Check command-line arguments
     if "--test" in command:
         test_index = command.index("--test")
-        try:
-            test_arg = command[test_index + 1]  # Argument after --test
-        except IndexError:
-            raise ValueError("Expected an argument after --test")
-
-        # Get all files that include the string that is the argument after --test
-        related_files = [f for f in json_files if test_arg in f]
-        related_file_count = len(related_files)
-
-        # Determine the prefix based on the existing files
-        if related_file_count == 0:
-            # Try to find the highest prefix number among all files, then increment it
-            all_prefix_numbers = []
-            for f in json_files:
-                try:
-                    number = float(Path(f).stem.split("_")[0])
-                except ValueError:
-                    print(f"File {f} is invalid.")
-                    continue
-
-                all_prefix_numbers.append(math.floor(number))
+    elif "--suite" in command:
+        test_index = command.index("--suite")
+    elif "--category" in command:
+        test_index = command.index("--category")
+    elif "--maintain" in command:
+        test_index = command.index("--maintain")
+        test_arg = "maintain"
+    elif "--improve" in command:
+        test_index = command.index("--improve")
+        test_arg = "improve"
+
+    if test_index:
+        if not test_arg:
+            test_arg = command[test_index + 1]
+
+        # collect related directories and their prefix numbers
+        related_dirs = []
+        prefix_numbers = []
 
-            max_prefix = max(all_prefix_numbers, default=0)
-            run_name = f"{max_prefix + 1}_{test_arg}.json"
+        for dir in dirs:
+            dir_parts = dir.split("_")
+            try:
+                prefix = float(dir_parts[0][6:])
+                test_name = "_".join(dir_parts[1:])
+                if test_arg == test_name:
+                    prefix_numbers.append(math.floor(prefix))
+                    related_dirs.append(test_name)
+            except:
+                pass
+
+        related_dir_count = len(related_dirs)
+
+        if related_dir_count == 0:
+            max_prefix = max(prefix_numbers, default=0)
+            run_name = f"folder{max_prefix + 1}_{test_arg}"
         else:
-            print(f"Found {related_file_count} files with '{test_arg}' in the name")
-            # Take the number from before the _ and add the .{number}
+            print(
+                f"Found {related_dir_count} directories with '{test_arg}' in the name"
+            )
+            prefix = max(prefix_numbers)
+            run_name = f"folder{prefix}.{related_dir_count}_{test_arg}"
+
+    new_dir_path = reports_path / run_name
 
-            prefix_str = Path(related_files[0]).stem.rsplit("_")[0].split(".")[0]
-            prefix = math.floor(float(prefix_str))
-            run_name = f"{prefix}.{related_file_count}_{test_arg}.json"
+    if not os.path.exists(new_dir_path):
+        os.makedirs(new_dir_path)
 
-    new_file_path = reports_path / run_name
-    return str(new_file_path)
+    return str(new_dir_path)
 
 
 def replace_backslash(value: Any) -> Any:
     if isinstance(value, str):
         return re.sub(
             r"\\+", "/", value
         )  # replace one or more backslashes with a forward slash
@@ -93,100 +107,181 @@
     total_count = len(last_results)
     if total_count == 0:
         return 0
     success_percentage = (success_count / total_count) * 100  # as a percentage
     return round(success_percentage, 2)
 
 
-def get_highest_success_difficulty(data: dict) -> str:
+def get_test_path(json_file: str | Path) -> str:
+    if isinstance(json_file, str):
+        json_file = Path(json_file)
+
+    # Find the index of "agbenchmark" in the path parts
+    try:
+        agbenchmark_index = json_file.parts.index("agbenchmark")
+    except ValueError:
+        raise ValueError("Invalid challenge location.")
+
+    # Create the path from "agbenchmark" onwards
+    challenge_location = Path(*json_file.parts[agbenchmark_index:])
+
+    formatted_location = replace_backslash(str(challenge_location))
+    if isinstance(formatted_location, str):
+        return formatted_location
+    else:
+        return str(challenge_location)
+
+
+def get_highest_success_difficulty(
+    data: dict, just_string: Optional[bool] = None
+) -> str:
     highest_difficulty = None
     highest_difficulty_level = 0
 
     for test_name, test_data in data.items():
-        if test_data["metrics"]["success"]:
-            # Replace 'medium' with 'intermediate' for this example
-            difficulty_str = test_data["metrics"]["difficulty"]
-
-            try:
-                difficulty_enum = DifficultyLevel[difficulty_str.lower()]
-                difficulty_level = DIFFICULTY_MAP[difficulty_enum]
-
-                if difficulty_level > highest_difficulty_level:
-                    highest_difficulty = difficulty_enum
-                    highest_difficulty_level = difficulty_level
-            except KeyError:
-                print(
-                    f"Unexpected difficulty level '{difficulty_str}' in test '{test_name}'"
-                )
+        try:
+            if test_data.get("tests", None):
+                highest_difficulty_str = test_data["metrics"]["highest_difficulty"]
+                try:
+                    highest_difficulty = DifficultyLevel[highest_difficulty_str]
+                    highest_difficulty_level = DIFFICULTY_MAP[highest_difficulty]
+                except KeyError:
+                    print(
+                        f"Unexpected difficulty level '{highest_difficulty_str}' in test '{test_name}'"
+                    )
+                    continue
+            else:
+                if test_data["metrics"]["success"]:
+                    difficulty_str = test_data["metrics"]["difficulty"]
+
+                    try:
+                        difficulty_enum = DifficultyLevel[difficulty_str.lower()]
+                        difficulty_level = DIFFICULTY_MAP[difficulty_enum]
+
+                        if difficulty_level > highest_difficulty_level:
+                            highest_difficulty = difficulty_enum
+                            highest_difficulty_level = difficulty_level
+                    except KeyError:
+                        print(
+                            f"Unexpected difficulty level '{difficulty_str}' in test '{test_name}'"
+                        )
+                        continue
+        except Exception:
+            print(f"Make sure you selected the right test, no reports were generated.")
+            break
 
     if highest_difficulty is not None:
         highest_difficulty_str = highest_difficulty.name  # convert enum to string
     else:
         highest_difficulty_str = ""
 
-    if highest_difficulty_level:
+    if highest_difficulty_level and not just_string:
         return f"{highest_difficulty_str}: {highest_difficulty_level}"
+    elif highest_difficulty_str:
+        return highest_difficulty_str
     return "No successful tests"
 
 
-def assign_paths(folder_path: Path) -> tuple[str, str, str]:
+def assign_paths(folder_path: Path) -> tuple[str, str, str, str, str]:
     CONFIG_PATH = str(folder_path / "config.json")
-    REGRESSION_TESTS_PATH = str(folder_path / "regression_tests.json")
 
-    if HOME_ENV == "ci" and AGENT_NAME:
-        INFO_TESTS_PATH = calculate_info_test_path(
-            Path(os.getcwd()) / "agbenchmark" / "reports" / AGENT_NAME
-        )
-    else:
-        INFO_TESTS_PATH = calculate_info_test_path(folder_path / "reports")
+    reports_location = folder_path / "reports"
+
+    # if the user has a locally defined challenges path that they've added tests to
+    CHALLENGES_PATH = str(folder_path / "challenges")
+    if not os.path.exists(CHALLENGES_PATH):
+        CHALLENGES_PATH = str(Path(__file__).parent.parent / "challenges")
 
-    return CONFIG_PATH, REGRESSION_TESTS_PATH, INFO_TESTS_PATH
+    if not os.path.exists(reports_location):
+        os.makedirs(reports_location)
 
+    # from the ci
+    if REPORT_LOCATION:
+        reports_location = Path.cwd() / REPORT_LOCATION
 
-def calculate_dynamic_paths() -> tuple[Path, str, str, str]:
+    REPORTS_PATH = calculate_info_test_path(reports_location)
+
+    REGRESSION_TESTS_PATH = str(reports_location / "regression_tests.json")
+
+    SUCCESS_RATE_PATH = str(reports_location / "success_rate.json")
+
+    return (
+        CONFIG_PATH,
+        REGRESSION_TESTS_PATH,
+        REPORTS_PATH,
+        SUCCESS_RATE_PATH,
+        CHALLENGES_PATH,
+    )
+
+
+def calculate_dynamic_paths() -> tuple[Path, str, str, str, str, str]:
     # the default home is where you're running from
     HOME_DIRECTORY = Path(os.getcwd())
     benchmarks_folder_path = HOME_DIRECTORY / "agbenchmark"
 
-    if AGENT_NAME and HOME_ENV == "ci":
-        if "/Auto-GPT-Benchmarks/agent" in str(HOME_DIRECTORY):
-            raise Exception("Must run from root of benchmark repo if HOME_ENV is ci")
-
-        # however if the env is local and the agent name is defined, we want to run that agent from the repo and then get the data in the internal agbenchmark directory
-        # this is for the ci/cd pipeline
-        benchmarks_folder_path = HOME_DIRECTORY / "agent" / AGENT_NAME / "agbenchmark"
-
-        CONFIG_PATH, REGRESSION_TESTS_PATH, INFO_TESTS_PATH = assign_paths(
-            benchmarks_folder_path
-        )
-
-        # we want to run the agent from the submodule
-        HOME_DIRECTORY = Path(os.getcwd()) / "agent" / AGENT_NAME
-
-    elif AGENT_NAME and not os.path.join("Auto-GPT-Benchmarks", "agent") in str(
+    if AGENT_NAME and not os.path.join("Auto-GPT-Benchmarks", "agent") in str(
         HOME_DIRECTORY
     ):
         # if the agent name is defined but the run is not from the agent repo, then home is the agent repo
         # used for development of both a benchmark and an agent
         HOME_DIRECTORY = Path(os.getcwd()) / "agent" / AGENT_NAME
         benchmarks_folder_path = HOME_DIRECTORY / "agbenchmark"
 
-        CONFIG_PATH, REGRESSION_TESTS_PATH, INFO_TESTS_PATH = assign_paths(
-            benchmarks_folder_path
-        )
-
+        (
+            CONFIG_PATH,
+            REGRESSION_TESTS_PATH,
+            REPORTS_PATH,
+            SUCCESS_RATE_PATH,
+            CHALLENGES_PATH,
+        ) = assign_paths(benchmarks_folder_path)
     else:
         # otherwise the default is when home is an agent (running agbenchmark from agent/agent_repo)
         # used when its just a pip install
-        CONFIG_PATH, REGRESSION_TESTS_PATH, INFO_TESTS_PATH = assign_paths(
-            benchmarks_folder_path
-        )
+        (
+            CONFIG_PATH,
+            REGRESSION_TESTS_PATH,
+            REPORTS_PATH,
+            SUCCESS_RATE_PATH,
+            CHALLENGES_PATH,
+        ) = assign_paths(benchmarks_folder_path)
 
     if not benchmarks_folder_path.exists():
         benchmarks_folder_path.mkdir(exist_ok=True)
 
+    if not os.path.exists(benchmarks_folder_path / "reports"):
+        os.makedirs(benchmarks_folder_path / "reports")
+
+    if not os.path.exists(REGRESSION_TESTS_PATH):
+        with open(REGRESSION_TESTS_PATH, "w"):
+            pass
+
+    if not os.path.exists(SUCCESS_RATE_PATH):
+        with open(SUCCESS_RATE_PATH, "w"):
+            pass
+
+    if not os.path.exists(Path(REPORTS_PATH) / "report.json"):
+        with open(Path(REPORTS_PATH) / "report.json", "w"):
+            pass
+
     return (
         HOME_DIRECTORY,
         CONFIG_PATH,
         REGRESSION_TESTS_PATH,
-        INFO_TESTS_PATH,
+        REPORTS_PATH,
+        SUCCESS_RATE_PATH,
+        CHALLENGES_PATH,
     )
+
+
+def get_git_commit_sha(directory: Path) -> Optional[str]:
+    try:
+        repo = git.Repo(directory)
+        remote_url = repo.remotes.origin.url
+        if remote_url.endswith(".git"):
+            remote_url = remote_url[:-4]
+        git_commit_sha = f"{remote_url}/tree/{repo.head.commit.hexsha}"
+
+        print(f"GIT_COMMIT_SHA: {git_commit_sha}")
+        return git_commit_sha
+    except Exception:
+        print(f"{directory} is not a git repository!")
+        return None
```

### Comparing `agbenchmark-0.0.2/pyproject.toml` & `agbenchmark-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 [tool.poetry]
 name = "agbenchmark"
-version = "0.0.2"
+version = "0.0.3"
 description = "Benchmarking the performance of agents far and wide, regardless of how they are set up and how they work"
 authors = ["Silen Naihin <silen.naihin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "agbenchmark"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytest = "^7.3.2"
 requests = "^2.31.0"
 openai = "^0.27.8"
 pydantic = "^1.10.9"
 pytest-depends = "^1.0.1"
-python-dotenv = "^0.21.0"
+python-dotenv = "^1.0.0"
 click = "^8.1.3"
 types-requests = "^2.31.0.1"
 pexpect = "^4.8.0"
 psutil = "^5.9.5"
+helicone = "^1.0.6"
+matplotlib = "^3.7.2"
+pandas = "^2.0.3"
+gitpython = "^3.1.32"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^3.9.2"
-mypy = "^0.910"
+mypy = "^1.01"
 isort = "^5.9.3"
 black = "22.3"
 autoflake = "^1.4"
 pandas = "^2.0.3"
 gspread = "^5.10.0"
 oauth2client = "^4.1.3"
 
@@ -41,15 +45,18 @@
     "tests", "agbenchmark",
 ]
 markers = [
     "retrieval",
     "interface",
     "code",
     "memory",
-    "iterate"
+    "iterate",
+    "adaptability",
+    "safety",
+    "content_gen"
 ]
 
 [tool.poetry.scripts]
 agbenchmark = "agbenchmark.start_benchmark:cli"
 
 [tool.black]
 line-length = 88
```

