# Comparing `tmp/db_plugins-4.2.7.tar.gz` & `tmp/db_plugins-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_plugins-4.2.7.tar", max compression
+gzip compressed data, was "db_plugins-5.1.0.tar", max compression
```

## Comparing `db_plugins-4.2.7.tar` & `db_plugins-5.1.0.tar`

### file list

```diff
@@ -1,26 +1,23 @@
--rw-r--r--   0        0        0     7495 2023-08-01 16:04:00.788536 db_plugins-4.2.7/README.rst
--rw-r--r--   0        0        0       22 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/cli/__init__.py
--rw-r--r--   0        0        0     2498 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/cli/manage.py
--rw-r--r--   0        0        0       40 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/__init__.py
--rw-r--r--   0        0        0    11334 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/generic.py
--rw-r--r--   0        0        0        0 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/mongo/__init__.py
--rw-r--r--   0        0        0     4157 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/mongo/connection.py
--rw-r--r--   0        0        0        0 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/mongo/helpers/__init__.py
--rw-r--r--   0        0        0     2619 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/mongo/helpers/update_probs.py
--rw-r--r--   0        0        0      166 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/mongo/initialization.py
--rw-r--r--   0        0        0     6294 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/mongo/models.py
--rw-r--r--   0        0        0     2047 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/mongo/orm.py
--rw-r--r--   0        0        0    10174 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/mongo/query.py
--rw-r--r--   0        0        0        0 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/__init__.py
--rw-r--r--   0        0        0     2020 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/alembic.ini
--rw-r--r--   0        0        0     5757 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/connection.py
--rw-r--r--   0        0        0     1294 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/initialization.py
--rw-r--r--   0        0        0       38 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/migrations/README
--rw-r--r--   0        0        0     2472 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/migrations/env.py
--rw-r--r--   0        0        0      494 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/migrations/script.py.mako
--rwxr-xr-x   0        0        0    13925 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/models.py
--rw-r--r--   0        0        0     6916 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/query.py
--rw-r--r--   0        0        0      422 2023-08-01 16:04:00.788536 db_plugins-4.2.7/db_plugins/db/sql/serializers.py
--rw-r--r--   0        0        0      607 2023-08-01 16:04:00.796536 db_plugins-4.2.7/pyproject.toml
--rw-r--r--   0        0        0     8134 1970-01-01 00:00:00.000000 db_plugins-4.2.7/PKG-INFO
+-rw-r--r--   0        0        0     3482 2023-08-04 21:20:37.737435 db_plugins-5.1.0/README.rst
+-rw-r--r--   0        0        0        0 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/cli/__init__.py
+-rw-r--r--   0        0        0     2498 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/cli/manage.py
+-rw-r--r--   0        0        0       40 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/__init__.py
+-rw-r--r--   0        0        0     2012 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/generic.py
+-rw-r--r--   0        0        0        0 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/mongo/__init__.py
+-rw-r--r--   0        0        0     2748 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/mongo/_connection.py
+-rw-r--r--   0        0        0        0 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/mongo/helpers/__init__.py
+-rw-r--r--   0        0        0     2534 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/mongo/helpers/update_probs.py
+-rw-r--r--   0        0        0      234 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/mongo/initialization.py
+-rw-r--r--   0        0        0     6294 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/mongo/models.py
+-rw-r--r--   0        0        0     2047 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/mongo/orm.py
+-rw-r--r--   0        0        0        0 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/sql/__init__.py
+-rw-r--r--   0        0        0     1193 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/sql/_connection.py
+-rw-r--r--   0        0        0     2020 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/sql/alembic.ini
+-rw-r--r--   0        0        0      930 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/sql/initialization.py
+-rw-r--r--   0        0        0       38 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/sql/migrations/README
+-rw-r--r--   0        0        0     2472 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/sql/migrations/env.py
+-rw-r--r--   0        0        0      494 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/sql/migrations/script.py.mako
+-rwxr-xr-x   0        0        0    12920 2023-08-04 21:20:37.737435 db_plugins-5.1.0/db_plugins/db/sql/models.py
+-rw-r--r--   0        0        0      567 2023-08-04 21:20:37.737435 db_plugins-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4072 1970-01-01 00:00:00.000000 db_plugins-5.1.0/PKG-INFO
```

### Comparing `db_plugins-4.2.7/db_plugins/cli/manage.py` & `db_plugins-5.1.0/db_plugins/cli/manage.py`

 * *Files identical despite different names*

### Comparing `db_plugins-4.2.7/db_plugins/db/mongo/connection.py` & `db_plugins-5.1.0/db_plugins/db/mongo/_connection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 from collections import UserDict
-
 from pymongo import MongoClient
-
-from .query import MongoQuery
-from ..generic import DatabaseConnection, DatabaseCreator
 from .orm import ModelMetaClass
 
 
 class _MongoConfig(UserDict):
     """Special dictionary used to parse configuration dictionaries for mongodb.
 
     The required keys are described in `REQUIRED_KEYS`, but can come with any
@@ -38,31 +34,18 @@
         """Converts keys from (case-insensitive) `snake_case` to `lowerCamelCase`"""
         klist = [
             w.lower() if i == 0 else w.title() for i, w in enumerate(key.split("_"))
         ]
         super().__setitem__("".join(klist), value)
 
 
-class MongoConnection(DatabaseConnection):
-    def __init__(self, config=None):
-        self.config = config
-        self.client = None
-        self.database = None
-
-    @property
-    def config(self):
-        return self.__config
-
-    @config.setter
-    def config(self, config):
-        self.__config = config if config is None else _MongoConfig(config)
-
-    def connect(self, config=None):
+class MongoConnection:
+    def __init__(self, config):
         """
-        Establishes connection to a database and initializes a session.
+        Establishes connection to a database.
 
         Parameters
         ----------
         config : dict
             Database configuration. For example:
 
             .. code-block:: python
@@ -73,51 +56,25 @@
                     "PASSWORD": "pwd",
                     "PORT": 27017, # mongo typically runs on port 27017.
                                    # Notice that we use an int here.
                     "DATABASE": "database",
                     "AUTH_SOURCE": "admin" # could be admin or the same as DATABASE
                 }
         """
-        if config is not None:
-            self.config = config
-        self.client = self.client or MongoClient(**self.config)
+        self.config = config
+        self.client = MongoClient(**self.config)
         self.database = self.client[self.config.db_name]
         ModelMetaClass.set_database(self.config.db_name)
 
+    @property
+    def config(self):
+        return self.__config
+
+    @config.setter
+    def config(self, config):
+        self.__config = config if config is None else _MongoConfig(config)
+
     def create_db(self):
         ModelMetaClass.metadata.create_all(self.client, self.config.db_name)
 
     def drop_db(self):
         ModelMetaClass.metadata.drop_all(self.client, self.config.db_name)
-
-    def query(self, model=None, name=None):
-        """Create a BaseQuery object that allows you to query the database using
-        the PyMongo Collection API, or using the BaseQuery methods
-        like ``get_or_create``.
-
-        Parameters
-        ----------
-        model : Type[BaseModel]
-            Model class to create the query for
-        name : str
-            Name of collection to use
-
-        Examples
-        --------
-        .. code-block:: python
-
-            # Using PyMongo API through collection attribute
-            db_conn.query(
-                name='my_collection',
-            ).collection.find({'hello': 'world'})
-            # Using db-plugins
-            # These two statements are equivalent
-            db_conn.query(model=Object).get_or_create(filter_by=filters)
-            db_conn.query().get_or_create(model=Object, filter_by=filters)
-        """
-        return MongoQuery(self.database, model=model, name=name)
-
-
-class MongoDatabaseCreator(DatabaseCreator):
-    @classmethod
-    def create_database(cls) -> MongoConnection:
-        return MongoConnection()
```

### Comparing `db_plugins-4.2.7/db_plugins/db/mongo/helpers/update_probs.py` & `db_plugins-5.1.0/db_plugins/db/mongo/helpers/update_probs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from db_plugins.db.mongo.connection import MongoConnection
 from pymongo import UpdateOne
+from pymongo.database import Database
 
 """
 Helper function to create or update the probabilities for an object
 """
 
 
-def get_probabilities(connection: MongoConnection, aids: list):
-    probabilities = connection.database["object"].find(
+def get_probabilities(database: Database, aids: list):
+    probabilities = database["object"].find(
         {"_id": {"$in": aids}}, {"probabilities": True}
     )
     return {item["_id"]: item["probabilities"] for item in probabilities}
 
 
 def get_db_operations(
     classifier: str,
@@ -53,44 +53,44 @@
         {"_id": aid}, {"$set": {"probabilities": object_probabilities}}
     )
 
     return operation
 
 
 def create_or_update_probabilities(
-    connection: MongoConnection,
+    database: Database,
     classifier: str,
     version: str,
     aid: str,
     probabilities: dict,
 ):
-    object_probs = get_probabilities(connection, [aid])
+    object_probs = get_probabilities(database, [aid])
 
-    connection.database["object"].bulk_write(
+    database["object"].bulk_write(
         [get_db_operations(classifier, version, aid, object_probs[aid], probabilities)],
         ordered=False,
     )
 
 
 def create_or_update_probabilities_bulk(
-    connection: MongoConnection,
+    database: Database,
     classifier: str,
     version: str,
     aids: list,
     probabilities: list,
 ):
     """
     Bulk update using the actual bulk object of pymongo
     """
     db_operations = []
 
     # no warrants that probs will have the same aid order
-    object_probabilities = get_probabilities(connection, aids)
+    object_probabilities = get_probabilities(database, aids)
 
     for aid, probs in zip(aids, probabilities):
         db_operations.append(
             get_db_operations(
                 classifier, version, aid, object_probabilities[aid], probs
             )
         )
 
-    connection.database["object"].bulk_write(db_operations, ordered=False)
+    database["object"].bulk_write(db_operations, ordered=False)
```

### Comparing `db_plugins-4.2.7/db_plugins/db/mongo/models.py` & `db_plugins-5.1.0/db_plugins/db/mongo/models.py`

 * *Files identical despite different names*

### Comparing `db_plugins-4.2.7/db_plugins/db/mongo/orm.py` & `db_plugins-5.1.0/db_plugins/db/mongo/orm.py`

 * *Files identical despite different names*

### Comparing `db_plugins-4.2.7/db_plugins/db/sql/alembic.ini` & `db_plugins-5.1.0/db_plugins/db/sql/alembic.ini`

 * *Files identical despite different names*

### Comparing `db_plugins-4.2.7/db_plugins/db/sql/migrations/env.py` & `db_plugins-5.1.0/db_plugins/db/sql/migrations/env.py`

 * *Files identical despite different names*

### Comparing `db_plugins-4.2.7/db_plugins/db/sql/models.py` & `db_plugins-5.1.0/db_plugins/db/sql/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Float,
     Boolean,
     ARRAY,
     Index,
     DateTime,
     ForeignKeyConstraint,
 )
-from sqlalchemy.orm import relationship
-from .. import generic
 
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import DeclarativeBase
 
-Base = declarative_base()
+
+class Base(DeclarativeBase):
+    pass
 
 
 class Commons:
     def __getitem__(self, field):
         return self.__dict__[field]
 
 
-class Step(Base, generic.AbstractStep):
+class Step(Base):
     __tablename__ = "step"
 
     step_id = Column(String, primary_key=True)
     name = Column(String, nullable=False)
     version = Column(String, nullable=False)
     comments = Column(String, nullable=False)
     date = Column(DateTime, nullable=False)
 
 
-class Object(Base, generic.AbstractObject):
+class Object(Base):
     __tablename__ = "object"
 
     oid = Column(String, primary_key=True)
     ndethist = Column(Integer)
     ncovhist = Column(Integer)
     mjdstarthist = Column(Float(precision=53))
     mjdendhist = Column(Float(precision=53))
@@ -65,30 +65,14 @@
         Index("ix_object_firstmjd", "firstmjd", postgresql_using="btree"),
         Index("ix_object_g_r_max", "g_r_max", postgresql_using="btree"),
         Index("ix_object_g_r_mean_corr", "g_r_mean_corr", postgresql_using="btree"),
         Index("ix_object_meanra", "meanra", postgresql_using="btree"),
         Index("ix_object_meandec", "meandec", postgresql_using="btree"),
     )
 
-    # xmatches = relationship("Xmatch")
-    magstats = relationship("MagStats", uselist=True)
-    non_detections = relationship("NonDetection", order_by="NonDetection.mjd")
-    detections = relationship("Detection", order_by="Detection.mjd")
-    features = relationship("Feature")
-    probabilities = relationship(
-        "Probability", uselist=True, order_by="Probability.classifier_name"
-    )
-
-    def get_lightcurve(self):
-        """Get the lightcurve of the object."""
-        return {
-            "detections": self.detections,
-            "non_detections": self.non_detections,
-        }
-
     def __repr__(self):
         return "<Object(oid='%s')>" % (self.oid)
 
 
 class Taxonomy(Base):
     __tablename__ = "taxonomy"
     classifier_name = Column(String, primary_key=True)
@@ -177,15 +161,15 @@
 
     __table_args__ = (
         Index("ix_allwise_dec", "dec", postgresql_using="btree"),
         Index("ix_allwise_ra", "ra", postgresql_using="btree"),
     )
 
 
-class MagStats(Base, generic.AbstractMagnitudeStatistics):
+class MagStats(Base):
     __tablename__ = "magstat"
 
     oid = Column(String, ForeignKey("object.oid"), primary_key=True)
     fid = Column(Integer, primary_key=True)
     stellar = Column(Boolean, nullable=False)
     corrected = Column(Boolean, nullable=False)
     ndet = Column(Integer, nullable=False)
@@ -222,25 +206,25 @@
         Index("ix_magstats_magfirst", "magfirst", postgresql_using="btree"),
         Index("ix_magstats_ndet", "ndet", postgresql_using="btree"),
         Index("ix_magstats_maglast", "maglast", postgresql_using="btree"),
         Index("ix_magstats_oid", "oid", postgresql_using="hash"),
     )
 
 
-class NonDetection(Base, generic.AbstractNonDetection, Commons):
+class NonDetection(Base, Commons):
     __tablename__ = "non_detection"
 
     oid = Column(String, ForeignKey("object.oid"), primary_key=True)
     fid = Column(Integer, primary_key=True)
     mjd = Column(Float(precision=53), primary_key=True)
     diffmaglim = Column(Float)
     __table_args__ = (Index("ix_non_detection_oid", "oid", postgresql_using="hash"),)
 
 
-class Detection(Base, generic.AbstractDetection, Commons):
+class Detection(Base, Commons):
     __tablename__ = "detection"
 
     candid = Column(BigInteger, primary_key=True)
     oid = Column(String, ForeignKey("object.oid"), primary_key=True)
     mjd = Column(Float(precision=53), nullable=False)
     fid = Column(Integer, nullable=False)
     pid = Column(Float, nullable=False)
@@ -268,25 +252,23 @@
     dubious = Column(Boolean, nullable=False)
     parent_candid = Column(BigInteger)
     has_stamp = Column(Boolean, nullable=False)
     step_id_corr = Column(String, nullable=False)
 
     __table_args__ = (Index("ix_ndetection_oid", "oid", postgresql_using="hash"),)
 
-    dataquality = relationship("Dataquality")
-
     def __repr__(self):
         return "<Detection(candid='%i', fid='%i', oid='%s')>" % (
             self.candid,
             self.fid,
             self.oid,
         )
 
 
-class Dataquality(Base, generic.AbstractDataquality):
+class Dataquality(Base):
     __tablename__ = "dataquality"
 
     candid = Column(BigInteger, primary_key=True)
     oid = Column(String, primary_key=True)
     fid = Column(Integer, nullable=False)
     xpos = Column(Float)
     ypos = Column(Float)
@@ -320,42 +302,42 @@
 
     __table_args__ = (
         ForeignKeyConstraint([candid, oid], [Detection.candid, Detection.oid]),
         {},
     )
 
 
-class Gaia_ztf(Base, generic.AbstractGaia_ztf):
+class Gaia_ztf(Base):
     __tablename__ = "gaia_ztf"
 
     oid = Column(String, ForeignKey("object.oid"), primary_key=True)
     candid = Column(BigInteger, nullable=False)
     neargaia = Column(Float)
     neargaiabright = Column(Float)
     maggaia = Column(Float)
     maggaiabright = Column(Float)
     unique1 = Column(Boolean, nullable=False)
 
 
-class Ss_ztf(Base, generic.AbstractSs_ztf):
+class Ss_ztf(Base):
     __tablename__ = "ss_ztf"
 
     oid = Column(String, ForeignKey("object.oid"), primary_key=True)
     candid = Column(BigInteger, nullable=False)
     ssdistnr = Column(Float)
     ssmagnr = Column(Float)
     ssnamenr = Column(String)
 
     __table_args__ = (
         Index("ix_ss_ztf_candid", "candid", postgresql_using="btree"),
         Index("ix_ss_ztf_ssnamenr", "ssnamenr", postgresql_using="btree"),
     )
 
 
-class Ps1_ztf(Base, generic.AbstractPs1_ztf):
+class Ps1_ztf(Base):
     __tablename__ = "ps1_ztf"
 
     oid = Column(String, ForeignKey("object.oid"), primary_key=True)
     candid = Column(BigInteger, primary_key=True)
     objectidps1 = Column(Float)
     sgmag1 = Column(Float)
     srmag1 = Column(Float)
@@ -379,15 +361,15 @@
     distpsnr3 = Column(Float)
     nmtchps = Column(Integer, nullable=False)
     unique1 = Column(Boolean, nullable=False)
     unique2 = Column(Boolean, nullable=False)
     unique3 = Column(Boolean, nullable=False)
 
 
-class Reference(Base, generic.AbstractReference):
+class Reference(Base):
     __tablename__ = "reference"
 
     oid = Column(String, ForeignKey("object.oid"), primary_key=True)
     rfid = Column(BigInteger, primary_key=True)
     candid = Column(BigInteger, nullable=False)
     fid = Column(Integer, nullable=False)
     rcid = Column(Integer)
@@ -401,15 +383,15 @@
     mjdstartref = Column(Float(precision=53), nullable=False)
     mjdendref = Column(Float(precision=53), nullable=False)
     nframesref = Column(Integer, nullable=False)
 
     __table_args__ = (Index("ix_reference_fid", "fid", postgresql_using="btree"),)
 
 
-class Pipeline(Base, generic.AbstractPipeline):
+class Pipeline(Base):
     __tablename__ = "pipeline"
 
     pipeline_id = Column(String, primary_key=True)
     step_id_corr = Column(String)
     step_id_feat = Column(String)
     step_id_clf = Column(String)
     step_id_out = Column(String)
```

