# Comparing `tmp/kgdata-4.0.1.tar.gz` & `tmp/kgdata-4.0.2.tar.gz`

## Comparing `kgdata-4.0.1.tar` & `kgdata-4.0.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 kgdata-4.0.1/Cargo.toml
--rw-r--r--   0     1001      123     1064 2023-07-27 05:41:42.000000 kgdata-4.0.1/LICENSE
--rw-r--r--   0     1001      123      839 2023-07-27 05:41:42.000000 kgdata-4.0.1/README.md
--rw-r--r--   0     1001      123    33142 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/conversions.rs
--rw-r--r--   0     1001      123     6414 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/db.rs
--rw-r--r--   0     1001      123      743 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/error.rs
--rw-r--r--   0     1001      123      581 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/lib.rs
--rw-r--r--   0     1001      123      527 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/models/class.rs
--rw-r--r--   0     1001      123     2254 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/models/entity.rs
--rw-r--r--   0     1001      123      245 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/models/entity_link.rs
--rw-r--r--   0     1001      123      426 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/models/entity_metadata.rs
--rw-r--r--   0     1001      123      545 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/models/mod.rs
--rw-r--r--   0     1001      123      648 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/models/multilingual.rs
--rw-r--r--   0     1001      123     3399 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/models/property.rs
--rw-r--r--   0     1001      123     5137 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/models/value.rs
--rw-r--r--   0     1001      123      952 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/pyo3helper/hashbrown.rs
--rw-r--r--   0     1001      123     4371 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/pyo3helper/macros/list.rs
--rw-r--r--   0     1001      123     5848 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/pyo3helper/macros/map.rs
--rw-r--r--   0     1001      123     6339 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/pyo3helper/macros/mod.rs
--rw-r--r--   0     1001      123     2133 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/pyo3helper/macros/set.rs
--rw-r--r--   0     1001      123      558 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/pyo3helper/mod.rs
--rw-r--r--   0     1001      123      805 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/pyo3helper/strview.rs
--rw-r--r--   0     1001      123       16 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/mod.rs
--rw-r--r--   0     1001      123     1280 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/class.rs
--rw-r--r--   0     1001      123      419 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/conversions.rs
--rw-r--r--   0     1001      123     3007 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/entity.rs
--rw-r--r--   0     1001      123     1133 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/entity_metadata.rs
--rw-r--r--   0     1001      123    10911 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/iterators.rs
--rw-r--r--   0     1001      123     1443 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/mod.rs
--rw-r--r--   0     1001      123     2433 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/multilingual.rs
--rw-r--r--   0     1001      123     1735 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/property.rs
--rw-r--r--   0     1001      123     8042 2023-07-27 05:41:42.000000 kgdata-4.0.1/src/python/models/value.rs
--rw-r--r--   0     1001      123     1558 2023-07-27 05:41:42.000000 kgdata-4.0.1/pyproject.toml
--rw-r--r--   0     1001      123    43877 2023-07-27 05:41:42.000000 kgdata-4.0.1/Cargo.lock
--rw-r--r--   0     1001      123    13715 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/spark.py
--rw-r--r--   0     1001      123        0 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/py.typed
--rw-r--r--   0     1001      123     2040 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/config.py
--rw-r--r--   0     1001      123       42 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/prelude.py
--rw-r--r--   0     1001      123     2908 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/misc.py
--rw-r--r--   0     1001      123        0 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/__init__.py
--rw-r--r--   0     1001      123     5053 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/wikiapi.py
--rw-r--r--   0     1001      123     1985 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/easy_tables_metadata.py
--rw-r--r--   0     1001      123     1584 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/html_articles.py
--rw-r--r--   0     1001      123     4428 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/linked_relational_tables.py
--rw-r--r--   0     1001      123     8222 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/easy_tables.py
--rw-r--r--   0     1001      123     1454 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/relational_tables.py
--rw-r--r--   0     1001      123     2911 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/articles.py
--rw-r--r--   0     1001      123     4167 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/grouped_articles.py
--rw-r--r--   0     1001      123        0 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/__init__.py
--rw-r--r--   0     1001      123     2600 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/html_tables.py
--rw-r--r--   0     1001      123     1726 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/datasets/__main__.py
--rw-r--r--   0     1001      123     1356 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/models/page_article.py
--rw-r--r--   0     1001      123     3721 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/models/linked_html_table.py
--rw-r--r--   0     1001      123       27 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/models/__init__.py
--rw-r--r--   0     1001      123     3470 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikipedia/models/html_article.py
--rw-r--r--   0     1001      123     2468 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/db.py
--rw-r--r--   0     1001      123     6683 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dataset.py
--rw-r--r--   0     1001      123     6623 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/extra_ent_db.py
--rw-r--r--   0     1001      123     1786 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/wikidata_prefixes.yml
--rw-r--r--   0     1001      123    10742 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/db.py
--rw-r--r--   0     1001      123     2686 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/config.py
--rw-r--r--   0     1001      123        0 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/__init__.py
--rw-r--r--   0     1001      123    16526 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/__main__.py
--rw-r--r--   0     1001      123     2969 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/property_ranges.py
--rw-r--r--   0     1001      123     1291 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/page_dump.py
--rw-r--r--   0     1001      123     1824 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/class_count.py
--rw-r--r--   0     1001      123     2897 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entity_ids.py
--rw-r--r--   0     1001      123     1608 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entity_types.py
--rw-r--r--   0     1001      123     2460 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entity_wikilinks.py
--rw-r--r--   0     1001      123     9132 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entity_pagerank.py
--rw-r--r--   0     1001      123     1206 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/wp2wd.py
--rw-r--r--   0     1001      123     1348 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entity_dump.py
--rw-r--r--   0     1001      123     1453 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entity_redirection_dump.py
--rw-r--r--   0     1001      123     1878 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/property_count.py
--rw-r--r--   0     1001      123      223 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/__init__.py
--rw-r--r--   0     1001      123     2439 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entity_metadata.py
--rw-r--r--   0     1001      123     5072 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/classes.py
--rw-r--r--   0     1001      123     1905 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/__main__.py
--rw-r--r--   0     1001      123     4686 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/properties.py
--rw-r--r--   0     1001      123     6002 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entity_redirections.py
--rw-r--r--   0     1001      123     8992 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/entities.py
--rw-r--r--   0     1001      123     2430 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/property_domains.py
--rw-r--r--   0     1001      123     3109 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/datasets/page_ids.py
--rw-r--r--   0     1001      123      639 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/wdentitylabel.py
--rw-r--r--   0     1001      123     1577 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/wdstatement.py
--rw-r--r--   0     1001      123     1921 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/wdclass.py
--rw-r--r--   0     1001      123      428 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/wdentitylink.py
--rw-r--r--   0     1001      123     1259 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/propertystats.py
--rw-r--r--   0     1001      123     1381 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/wdentitymetadata.py
--rw-r--r--   0     1001      123     1138 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/__init__.py
--rw-r--r--   0     1001      123     7559 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/wdvalue.py
--rw-r--r--   0     1001      123     4346 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/wdproperty.py
--rw-r--r--   0     1001      123     8231 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/wikidata/models/wdentity.py
--rw-r--r--   0     1001      123       27 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/core/__init__.pyi
--rw-r--r--   0     1001      123     6006 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/core/models.pyi
--rw-r--r--   0     1001      123     1385 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/core/base.pyi
--rw-r--r--   0     1001      123      417 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/table_tests.py
--rw-r--r--   0     1001      123     2602 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/db.py
--rw-r--r--   0     1001      123    13843 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/instances_extraction.py
--rw-r--r--   0     1001      123    12214 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/dbpediamodels.py
--rw-r--r--   0     1001      123     2834 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/config.py
--rw-r--r--   0     1001      123      138 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/prelude.py
--rw-r--r--   0     1001      123        0 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/__init__.py
--rw-r--r--   0     1001      123     2658 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/__main__.py
--rw-r--r--   0     1001      123     3908 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/wikilinks.py
--rw-r--r--   0     1001      123     1692 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/mapping_extractor_dump.py
--rw-r--r--   0     1001      123     2081 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/ontology_dump.py
--rw-r--r--   0     1001      123      222 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/__init__.py
--rw-r--r--   0     1001      123      595 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/page_id_dump.py
--rw-r--r--   0     1001      123      600 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/wikilink_dump.py
--rw-r--r--   0     1001      123     3207 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/classes.py
--rw-r--r--   0     1001      123     1419 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/__main__.py
--rw-r--r--   0     1001      123     5423 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/properties.py
--rw-r--r--   0     1001      123     1691 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/generic_extractor_dump.py
--rw-r--r--   0     1001      123     3601 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/entities.py
--rw-r--r--   0     1001      123     2034 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/page_ids.py
--rw-r--r--   0     1001      123     2045 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/datasets/redirection_dump.py
--rw-r--r--   0     1001      123    37449 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/dbpedia/table_extraction.py
--rw-r--r--   0     1001      123      364 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/config.py
--rw-r--r--   0     1001      123     6732 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/splitter.py
--rw-r--r--   0     1001      123        0 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/__init__.py
--rw-r--r--   0     1001      123     2404 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/models/ont_class.py
--rw-r--r--   0     1001      123     2813 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/models/ont_property.py
--rw-r--r--   0     1001      123        0 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/models/__init__.py
--rw-r--r--   0     1001      123     1930 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/models/entity.py
--rw-r--r--   0     1001      123     1829 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/models/multilingual.py
--rw-r--r--   0     1001      123     7492 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/misc/ntriples_parser.py
--rw-r--r--   0     1001      123     1733 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/misc/resource.py
--rw-r--r--   0     1001      123    18138 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/misc/download.py
--rw-r--r--   0     1001      123       43 2023-07-27 05:41:42.000000 kgdata-4.0.1/kgdata/misc/__init__.py
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 kgdata-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 kgdata-4.0.2/Cargo.toml
+-rw-r--r--   0     1001      123     1064 2023-08-04 06:01:58.000000 kgdata-4.0.2/LICENSE
+-rw-r--r--   0     1001      123      839 2023-08-04 06:01:58.000000 kgdata-4.0.2/README.md
+-rw-r--r--   0     1001      123    33142 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/conversions.rs
+-rw-r--r--   0     1001      123     6414 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/db.rs
+-rw-r--r--   0     1001      123      743 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/error.rs
+-rw-r--r--   0     1001      123      581 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/lib.rs
+-rw-r--r--   0     1001      123      527 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/models/class.rs
+-rw-r--r--   0     1001      123     2254 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/models/entity.rs
+-rw-r--r--   0     1001      123      245 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/models/entity_link.rs
+-rw-r--r--   0     1001      123      426 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/models/entity_metadata.rs
+-rw-r--r--   0     1001      123      545 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/models/mod.rs
+-rw-r--r--   0     1001      123      648 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/models/multilingual.rs
+-rw-r--r--   0     1001      123     3399 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/models/property.rs
+-rw-r--r--   0     1001      123     5137 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/models/value.rs
+-rw-r--r--   0     1001      123      952 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/pyo3helper/hashbrown.rs
+-rw-r--r--   0     1001      123     4371 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/pyo3helper/macros/list.rs
+-rw-r--r--   0     1001      123     5848 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/pyo3helper/macros/map.rs
+-rw-r--r--   0     1001      123     6339 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/pyo3helper/macros/mod.rs
+-rw-r--r--   0     1001      123     2133 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/pyo3helper/macros/set.rs
+-rw-r--r--   0     1001      123      558 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/pyo3helper/mod.rs
+-rw-r--r--   0     1001      123      805 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/pyo3helper/strview.rs
+-rw-r--r--   0     1001      123       16 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/mod.rs
+-rw-r--r--   0     1001      123     1280 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/class.rs
+-rw-r--r--   0     1001      123      419 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/conversions.rs
+-rw-r--r--   0     1001      123     3007 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/entity.rs
+-rw-r--r--   0     1001      123     1133 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/entity_metadata.rs
+-rw-r--r--   0     1001      123    10911 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/iterators.rs
+-rw-r--r--   0     1001      123     1443 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/mod.rs
+-rw-r--r--   0     1001      123     2433 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/multilingual.rs
+-rw-r--r--   0     1001      123     1735 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/property.rs
+-rw-r--r--   0     1001      123     8042 2023-08-04 06:01:58.000000 kgdata-4.0.2/src/python/models/value.rs
+-rw-r--r--   0     1001      123     1558 2023-08-04 06:01:58.000000 kgdata-4.0.2/pyproject.toml
+-rw-r--r--   0     1001      123    43877 2023-08-04 06:01:58.000000 kgdata-4.0.2/Cargo.lock
+-rw-r--r--   0     1001      123     6683 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dataset.py
+-rw-r--r--   0     1001      123     2404 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/models/ont_class.py
+-rw-r--r--   0     1001      123     1829 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/models/multilingual.py
+-rw-r--r--   0     1001      123     2813 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/models/ont_property.py
+-rw-r--r--   0     1001      123     1930 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/models/entity.py
+-rw-r--r--   0     1001      123        0 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/models/__init__.py
+-rw-r--r--   0     1001      123      417 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/table_tests.py
+-rw-r--r--   0     1001      123      138 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/prelude.py
+-rw-r--r--   0     1001      123    37449 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/table_extraction.py
+-rw-r--r--   0     1001      123    13843 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/instances_extraction.py
+-rw-r--r--   0     1001      123     2834 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/config.py
+-rw-r--r--   0     1001      123    12214 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/dbpediamodels.py
+-rw-r--r--   0     1001      123     2081 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/ontology_dump.py
+-rw-r--r--   0     1001      123     2045 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/redirection_dump.py
+-rw-r--r--   0     1001      123     3601 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/entities.py
+-rw-r--r--   0     1001      123     5423 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/properties.py
+-rw-r--r--   0     1001      123     1691 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/generic_extractor_dump.py
+-rw-r--r--   0     1001      123     3207 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/classes.py
+-rw-r--r--   0     1001      123      595 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/page_id_dump.py
+-rw-r--r--   0     1001      123      600 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/wikilink_dump.py
+-rw-r--r--   0     1001      123     1419 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/__main__.py
+-rw-r--r--   0     1001      123     3908 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/wikilinks.py
+-rw-r--r--   0     1001      123     2034 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/page_ids.py
+-rw-r--r--   0     1001      123     1692 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/mapping_extractor_dump.py
+-rw-r--r--   0     1001      123      222 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/datasets/__init__.py
+-rw-r--r--   0     1001      123     2658 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/__main__.py
+-rw-r--r--   0     1001      123     2602 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/db.py
+-rw-r--r--   0     1001      123        0 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/dbpedia/__init__.py
+-rw-r--r--   0     1001      123     4346 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/wdproperty.py
+-rw-r--r--   0     1001      123     1921 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/wdclass.py
+-rw-r--r--   0     1001      123     1577 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/wdstatement.py
+-rw-r--r--   0     1001      123      428 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/wdentitylink.py
+-rw-r--r--   0     1001      123     8231 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/wdentity.py
+-rw-r--r--   0     1001      123     7559 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/wdvalue.py
+-rw-r--r--   0     1001      123     1381 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/wdentitymetadata.py
+-rw-r--r--   0     1001      123     1259 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/propertystats.py
+-rw-r--r--   0     1001      123      639 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/wdentitylabel.py
+-rw-r--r--   0     1001      123     1138 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/models/__init__.py
+-rw-r--r--   0     1001      123     2686 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/config.py
+-rw-r--r--   0     1001      123     6623 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/extra_ent_db.py
+-rw-r--r--   0     1001      123     2969 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/property_ranges.py
+-rw-r--r--   0     1001      123     1348 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entity_dump.py
+-rw-r--r--   0     1001      123     8992 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entities.py
+-rw-r--r--   0     1001      123     4686 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/properties.py
+-rw-r--r--   0     1001      123     2460 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entity_wikilinks.py
+-rw-r--r--   0     1001      123     1206 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/wp2wd.py
+-rw-r--r--   0     1001      123     2430 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/property_domains.py
+-rw-r--r--   0     1001      123     1878 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/property_count.py
+-rw-r--r--   0     1001      123     2897 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entity_ids.py
+-rw-r--r--   0     1001      123     5072 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/classes.py
+-rw-r--r--   0     1001      123     1291 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/page_dump.py
+-rw-r--r--   0     1001      123     1824 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/class_count.py
+-rw-r--r--   0     1001      123     6002 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entity_redirections.py
+-rw-r--r--   0     1001      123     1905 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/__main__.py
+-rw-r--r--   0     1001      123     9132 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entity_pagerank.py
+-rw-r--r--   0     1001      123     1608 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entity_types.py
+-rw-r--r--   0     1001      123     2439 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entity_metadata.py
+-rw-r--r--   0     1001      123     1453 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/entity_redirection_dump.py
+-rw-r--r--   0     1001      123     3109 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/page_ids.py
+-rw-r--r--   0     1001      123      223 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/datasets/__init__.py
+-rw-r--r--   0     1001      123    16526 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/__main__.py
+-rw-r--r--   0     1001      123    10742 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/db.py
+-rw-r--r--   0     1001      123     1786 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/wikidata_prefixes.yml
+-rw-r--r--   0     1001      123        0 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikidata/__init__.py
+-rw-r--r--   0     1001      123      364 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/config.py
+-rw-r--r--   0     1001      123     6732 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/splitter.py
+-rw-r--r--   0     1001      123     6006 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/core/models.pyi
+-rw-r--r--   0     1001      123       27 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/core/__init__.pyi
+-rw-r--r--   0     1001      123     1385 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/core/base.pyi
+-rw-r--r--   0     1001      123    13715 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/spark.py
+-rw-r--r--   0     1001      123     2468 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/db.py
+-rw-r--r--   0     1001      123    18138 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/misc/download.py
+-rw-r--r--   0     1001      123     1733 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/misc/resource.py
+-rw-r--r--   0     1001      123     7492 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/misc/ntriples_parser.py
+-rw-r--r--   0     1001      123       43 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/misc/__init__.py
+-rw-r--r--   0     1001      123        0 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/__init__.py
+-rw-r--r--   0     1001      123        0 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/py.typed
+-rw-r--r--   0     1001      123       42 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/prelude.py
+-rw-r--r--   0     1001      123     3721 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/models/linked_html_table.py
+-rw-r--r--   0     1001      123     3542 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/models/html_article.py
+-rw-r--r--   0     1001      123     1356 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/models/page_article.py
+-rw-r--r--   0     1001      123       27 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/models/__init__.py
+-rw-r--r--   0     1001      123     2040 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/config.py
+-rw-r--r--   0     1001      123     2908 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/misc.py
+-rw-r--r--   0     1001      123     5053 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/wikiapi.py
+-rw-r--r--   0     1001      123     4167 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/grouped_articles.py
+-rw-r--r--   0     1001      123     2600 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/html_tables.py
+-rw-r--r--   0     1001      123     1454 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/relational_tables.py
+-rw-r--r--   0     1001      123     4428 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/linked_relational_tables.py
+-rw-r--r--   0     1001      123     1726 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/__main__.py
+-rw-r--r--   0     1001      123     8222 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/easy_tables.py
+-rw-r--r--   0     1001      123     1985 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/easy_tables_metadata.py
+-rw-r--r--   0     1001      123     2911 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/articles.py
+-rw-r--r--   0     1001      123     1584 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/html_articles.py
+-rw-r--r--   0     1001      123      224 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/datasets/__init__.py
+-rw-r--r--   0     1001      123        0 2023-08-04 06:01:58.000000 kgdata-4.0.2/kgdata/wikipedia/__init__.py
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 kgdata-4.0.2/PKG-INFO
```

### Comparing `kgdata-4.0.1/Cargo.toml` & `kgdata-4.0.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/LICENSE` & `kgdata-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/README.md` & `kgdata-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/conversions.rs` & `kgdata-4.0.2/src/conversions.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/db.rs` & `kgdata-4.0.2/src/db.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/error.rs` & `kgdata-4.0.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/lib.rs` & `kgdata-4.0.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/models/class.rs` & `kgdata-4.0.2/src/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/models/entity.rs` & `kgdata-4.0.2/src/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/models/mod.rs` & `kgdata-4.0.2/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/models/multilingual.rs` & `kgdata-4.0.2/src/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/models/property.rs` & `kgdata-4.0.2/src/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/models/value.rs` & `kgdata-4.0.2/src/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/pyo3helper/hashbrown.rs` & `kgdata-4.0.2/src/pyo3helper/hashbrown.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/pyo3helper/macros/list.rs` & `kgdata-4.0.2/src/pyo3helper/macros/list.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/pyo3helper/macros/map.rs` & `kgdata-4.0.2/src/pyo3helper/macros/map.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/pyo3helper/macros/mod.rs` & `kgdata-4.0.2/src/pyo3helper/macros/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/pyo3helper/macros/set.rs` & `kgdata-4.0.2/src/pyo3helper/macros/set.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/pyo3helper/mod.rs` & `kgdata-4.0.2/src/pyo3helper/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/pyo3helper/strview.rs` & `kgdata-4.0.2/src/pyo3helper/strview.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/python/models/class.rs` & `kgdata-4.0.2/src/python/models/class.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/python/models/entity.rs` & `kgdata-4.0.2/src/python/models/entity.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/python/models/entity_metadata.rs` & `kgdata-4.0.2/src/python/models/entity_metadata.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/python/models/iterators.rs` & `kgdata-4.0.2/src/python/models/iterators.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/python/models/mod.rs` & `kgdata-4.0.2/src/python/models/mod.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/python/models/multilingual.rs` & `kgdata-4.0.2/src/python/models/multilingual.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/python/models/property.rs` & `kgdata-4.0.2/src/python/models/property.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/src/python/models/value.rs` & `kgdata-4.0.2/src/python/models/value.rs`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/pyproject.toml` & `kgdata-4.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kgdata"
-version = "4.0.1"
+version = "4.0.2"
 description = "Library to process dumps of knowledge graphs (Wikipedia, DBpedia, Wikidata)"
 readme = "README.md"
 authors = [{ name = "Binh Vu", email = "binh@toan2.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `kgdata-4.0.1/Cargo.lock` & `kgdata-4.0.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/spark.py` & `kgdata-4.0.2/kgdata/spark.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/config.py` & `kgdata-4.0.2/kgdata/wikipedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/misc.py` & `kgdata-4.0.2/kgdata/wikipedia/misc.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/wikiapi.py` & `kgdata-4.0.2/kgdata/wikipedia/wikiapi.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/easy_tables_metadata.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/easy_tables_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/html_articles.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/html_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/linked_relational_tables.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/linked_relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/easy_tables.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/easy_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/relational_tables.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/relational_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/articles.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/grouped_articles.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/grouped_articles.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/html_tables.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/html_tables.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/datasets/__main__.py` & `kgdata-4.0.2/kgdata/wikipedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/models/page_article.py` & `kgdata-4.0.2/kgdata/wikipedia/models/page_article.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/models/linked_html_table.py` & `kgdata-4.0.2/kgdata/wikipedia/models/linked_html_table.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikipedia/models/html_article.py` & `kgdata-4.0.2/kgdata/wikipedia/models/html_article.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from dataclasses import dataclass
 from typing import List, Literal, Optional
 
 
 @dataclass
 class HTMLArticle:
     """Model of the HTML page article from Wikipedia HTML Dumps."""
@@ -37,15 +38,15 @@
 
     # list of wikipedia pages that redirect to this page
     redirects: List[NameAndURL]
 
     # the parsed html
     html: str
 
-    # the wikitext
+    # the wikitext -- empty if there is no wikitext
     wikitext: str
 
     @staticmethod
     def from_dump_dict(o: dict) -> HTMLArticle:
         additional_entities = []
         for ent in o.get("additional_entities", []):
             assert len(ent) == 3
@@ -63,23 +64,24 @@
             lang=o["in_language"]["identifier"],
             wdentity=o["main_entity"]["identifier"] if "main_entity" in o else None,
             additional_entities=additional_entities,
             is_part_of=o["is_part_of"]["identifier"],
             categories=[
                 NameAndURL(name=x["name"], url=x["url"])
                 for x in o.get("categories", [])
+                if len(x) > 0
             ],
             templates=[
                 NameAndURL(name=x["name"], url=x["url"]) for x in o.get("templates", [])
             ],
             redirects=[
                 NameAndURL(name=x["name"], url=x["url"]) for x in o.get("redirects", [])
             ],
             html=o["article_body"]["html"],
-            wikitext=o["article_body"]["wikitext"],
+            wikitext=o["article_body"].get("wikitext", ""),
         )
 
     def to_dict(self) -> dict:
         return {
             "name": self.name,
             "page_id": self.page_id,
             "date_modified": self.date_modified,
```

### Comparing `kgdata-4.0.1/kgdata/db.py` & `kgdata-4.0.2/kgdata/db.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dataset.py` & `kgdata-4.0.2/kgdata/dataset.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/extra_ent_db.py` & `kgdata-4.0.2/kgdata/wikidata/extra_ent_db.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/wikidata_prefixes.yml` & `kgdata-4.0.2/kgdata/wikidata/wikidata_prefixes.yml`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/db.py` & `kgdata-4.0.2/kgdata/wikidata/db.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/config.py` & `kgdata-4.0.2/kgdata/wikidata/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/__main__.py` & `kgdata-4.0.2/kgdata/wikidata/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/property_ranges.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/property_ranges.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/page_dump.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/page_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/class_count.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/class_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entity_ids.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entity_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entity_types.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entity_types.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entity_wikilinks.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entity_wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entity_pagerank.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entity_pagerank.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/wp2wd.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/wp2wd.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entity_dump.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entity_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entity_redirection_dump.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entity_redirection_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/property_count.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/property_count.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entity_metadata.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entity_metadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/classes.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/__main__.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/properties.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entity_redirections.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entity_redirections.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/entities.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/property_domains.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/property_domains.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/datasets/page_ids.py` & `kgdata-4.0.2/kgdata/wikidata/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/wdentitylabel.py` & `kgdata-4.0.2/kgdata/wikidata/models/wdentitylabel.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/wdstatement.py` & `kgdata-4.0.2/kgdata/wikidata/models/wdstatement.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/wdclass.py` & `kgdata-4.0.2/kgdata/wikidata/models/wdclass.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/propertystats.py` & `kgdata-4.0.2/kgdata/wikidata/models/propertystats.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/wdentitymetadata.py` & `kgdata-4.0.2/kgdata/wikidata/models/wdentitymetadata.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/__init__.py` & `kgdata-4.0.2/kgdata/wikidata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/wdvalue.py` & `kgdata-4.0.2/kgdata/wikidata/models/wdvalue.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/wdproperty.py` & `kgdata-4.0.2/kgdata/wikidata/models/wdproperty.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/wikidata/models/wdentity.py` & `kgdata-4.0.2/kgdata/wikidata/models/wdentity.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/core/models.pyi` & `kgdata-4.0.2/kgdata/core/models.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/core/base.pyi` & `kgdata-4.0.2/kgdata/core/base.pyi`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/db.py` & `kgdata-4.0.2/kgdata/dbpedia/db.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/instances_extraction.py` & `kgdata-4.0.2/kgdata/dbpedia/instances_extraction.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/dbpediamodels.py` & `kgdata-4.0.2/kgdata/dbpedia/dbpediamodels.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/config.py` & `kgdata-4.0.2/kgdata/dbpedia/config.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/__main__.py` & `kgdata-4.0.2/kgdata/dbpedia/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/wikilinks.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/wikilinks.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/mapping_extractor_dump.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/mapping_extractor_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/ontology_dump.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/ontology_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/page_id_dump.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/page_id_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/wikilink_dump.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/wikilink_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/classes.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/__main__.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/properties.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/properties.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/generic_extractor_dump.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/generic_extractor_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/entities.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/page_ids.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/page_ids.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/datasets/redirection_dump.py` & `kgdata-4.0.2/kgdata/dbpedia/datasets/redirection_dump.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/dbpedia/table_extraction.py` & `kgdata-4.0.2/kgdata/dbpedia/table_extraction.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/splitter.py` & `kgdata-4.0.2/kgdata/splitter.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/models/ont_class.py` & `kgdata-4.0.2/kgdata/models/ont_class.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/models/ont_property.py` & `kgdata-4.0.2/kgdata/models/ont_property.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/models/entity.py` & `kgdata-4.0.2/kgdata/models/entity.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/models/multilingual.py` & `kgdata-4.0.2/kgdata/models/multilingual.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/misc/ntriples_parser.py` & `kgdata-4.0.2/kgdata/misc/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/misc/resource.py` & `kgdata-4.0.2/kgdata/misc/resource.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/kgdata/misc/download.py` & `kgdata-4.0.2/kgdata/misc/download.py`

 * *Files identical despite different names*

### Comparing `kgdata-4.0.1/PKG-INFO` & `kgdata-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgdata
-Version: 4.0.1
+Version: 4.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: orjson >=3.9.0, <4.0.0
 Requires-Dist: tqdm >=4.64.0, <5.0.0
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: loguru >=0.6.0, <0.7.0
 Requires-Dist: rdflib >=6.1.1, <7.0.0
```

