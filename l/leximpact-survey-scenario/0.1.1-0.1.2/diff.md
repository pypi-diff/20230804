# Comparing `tmp/leximpact_survey_scenario-0.1.1.tar.gz` & `tmp/leximpact_survey_scenario-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leximpact_survey_scenario-0.1.1.tar", max compression
+gzip compressed data, was "leximpact_survey_scenario-0.1.2.tar", max compression
```

## Comparing `leximpact_survey_scenario-0.1.1.tar` & `leximpact_survey_scenario-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/LICENSE
--rw-r--r--   0        0        0      102 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/README.md
--rw-r--r--   0        0        0       54 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/__init__.py
--rw-r--r--   0        0        0    10764 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/leximpact_survey_scenario.py
--rw-r--r--   0        0        0     6539 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/leximpact_tax_and_benefit_system.py
--rw-r--r--   0        0        0       23 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/__init__.py
--rw-r--r--   0        0        0    17584 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/helpers_survey_scenario.py
--rw-r--r--   0        0        0     9021 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/inflation_calibration_values.py
--rw-r--r--   0        0        0     5233 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/inflator.py
--rw-r--r--   0        0        0     1561 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/leximpact_comparator.py
--rw-r--r--   0        0        0     9040 2023-07-17 11:12:26.577678 leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/plot.py
--rw-r--r--   0        0        0     1599 2023-07-17 11:12:26.581678 leximpact_survey_scenario-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 leximpact_survey_scenario-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-08-03 08:38:38.445347 leximpact_survey_scenario-0.1.2/LICENSE
+-rw-r--r--   0        0        0      102 2023-08-03 08:38:38.449347 leximpact_survey_scenario-0.1.2/README.md
+-rw-r--r--   0        0        0       54 2023-08-03 08:38:38.449347 leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/__init__.py
+-rw-r--r--   0        0        0    10894 2023-08-04 09:03:46.599109 leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/leximpact_survey_scenario.py
+-rw-r--r--   0        0        0     7662 2023-08-04 09:03:46.599109 leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/leximpact_tax_and_benefit_system.py
+-rw-r--r--   0        0        0       23 2023-08-03 08:38:38.449347 leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/__init__.py
+-rw-r--r--   0        0        0    17560 2023-08-04 09:03:46.603109 leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/helpers_survey_scenario.py
+-rw-r--r--   0        0        0     9034 2023-08-04 09:03:46.603109 leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/inflation_calibration_values.py
+-rw-r--r--   0        0        0     5237 2023-08-04 09:03:46.603109 leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/inflator.py
+-rw-r--r--   0        0        0     9040 2023-08-03 08:38:38.449347 leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/plot.py
+-rw-r--r--   0        0        0     1599 2023-08-04 09:03:46.611109 leximpact_survey_scenario-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 leximpact_survey_scenario-0.1.2/PKG-INFO
```

### Comparing `leximpact_survey_scenario-0.1.1/LICENSE` & `leximpact_survey_scenario-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/leximpact_survey_scenario.py` & `leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/leximpact_survey_scenario.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,41 +48,41 @@
 
 class LeximpactErfsSurveyScenario(ErfsFprSurveyScenario):
     """Survey scenario spécialisé pour l'ERFS-FPR utilisée par Leximpact."""
 
     def __init__(
         self,
         config_dirpath: str = default_config_files_directory,
-        annee_erfs: int = 2019,
+        annee_donnees: int = 2019,
         final_year: int = 2023,
         rebuild_input_data: bool = False,
         # rebuild_input_data est un paramètre hérité de survey_manager.
         init_from_data: bool = True,
         baseline_tax_benefit_system: Optional[TaxBenefitSystem] = None,
         tax_benefit_system_plf: Optional[TaxBenefitSystem] = None,
         data: Any = None,
         collection: str = "leximpact",
         survey_name: str = None,
     ):
         """Crée un `LeximpactErfsSurveyScenario`.
 
-        :param annee_erfs:                  L'année des données de l'enquête.
+        :param annee_donnees:               L'année des données utilisées en input.
         :param rebuild_input_data:          Si l'on doit formatter les données (raw) ou pas.
         :param init_from_data:              Si on veut suspendre l'initialisation automatique par les données
         :param tax_benefit_system:          Le `TaxBenefitSystem` déjà réformé.
         :param baseline_tax_benefit_system: Le `TaxBenefitSystem` au droit courant.
         :param data:                        Les données de l'enquête.
         :param reform:                      Reform OpenFisca.
         :param collection:                  Collection à lire.
         :param survey_name:                 Nom de l'enquête.
         """
 
-        super().__init__(annee_erfs)
+        super().__init__(annee_donnees)
         self.collection = collection
-        self.annee_erfs = int(annee_erfs)
+        self.annee_donnees = int(annee_donnees)
         self.final_year = int(final_year)
         self.config_dirpath = config_dirpath
         self.config_files_directory = config_dirpath
 
         self._set_used_as_input_variables()
         # non_neutralizable_variables hérite d'une liste de variables d'ErfsFprSurveyScenario
         self.non_neutralizable_variables += self.used_as_input_variables
@@ -96,15 +96,15 @@
 
         self.set_tax_benefit_systems(
             tax_benefit_system=tax_benefit_system_plf,
             baseline_tax_benefit_system=baseline_tax_benefit_system,
         )
 
         if survey_name is None:
-            survey_name = f"{collection}_{annee_erfs}"
+            survey_name = f"{collection}_{annee_donnees}"
 
         # ## Création de la base de données sur les périodes voulues
         # S'il n'y a pas de données, on sait où les trouver.
         if data is None:
             # List of years available
             years_available = []
             print(
@@ -116,28 +116,28 @@
             survey = survey_collection.get_survey(survey_name)
             for table_name, _ in survey.tables.items():
                 if table_name[-4:].isnumeric():
                     years_available.append(int(table_name[-4:]))
             years_available = list(set(years_available))
 
             # List of years to create
-            years = [year for year in range(self.annee_erfs, self.final_year + 1)]
+            years = [year for year in range(self.annee_donnees, self.final_year + 1)]
 
             print(f"{years_available=} vs {years=}")
 
             data = {"input_data_table_by_entity_by_period": {}, "survey": survey_name}
             current_year = None
 
             for year in years:
                 if data["input_data_table_by_entity_by_period"].get(year) is None:
                     data["input_data_table_by_entity_by_period"][year] = {}
                 if year in years_available:
                     data_year = year
                 else:
-                    data_year = self.annee_erfs
+                    data_year = self.annee_donnees
                     print(f"WARNING: no data for {year}, will took {data_year}")
                 for table_name, _ in survey.tables.items():
                     current_year = table_name[-4:]
                     if current_year.isnumeric():
                         current_year = int(current_year)
                         entity = table_name[:-5]
                         if current_year == data_year:
@@ -164,41 +164,41 @@
             self.final_year - 1,
             self.final_year,
         ]:
             inflator_by_variable.update(
                 {
                     inflation_year: inflation_coefs(
                         self.used_as_input_variables,
-                        str(self.annee_erfs),
+                        str(self.annee_donnees),
                         str(inflation_year),
                     )
                 }
             )
         for var in self.used_as_input_variables:
             if var in simulation.tax_benefit_system.variables:
                 array_var = self.calculate_variable(
-                    var, period=self.annee_erfs, use_baseline=True
+                    var, period=self.annee_donnees, use_baseline=True
                 )
                 for inflation_year in [
                     self.final_year - 2,
                     self.final_year - 1,
                     self.final_year,
                 ]:
                     if var in inflator_by_variable[inflation_year].keys():
                         inflated_array = (
                             array_var.copy() * inflator_by_variable[inflation_year][var]
                         )
                     elif (var in ["date_naissance"]) & (
-                        self.final_year > self.annee_erfs
+                        self.final_year > self.annee_donnees
                     ):
                         inflated_array = [
                             np.datetime64(
                                 (
                                     np.datetime64(date, "Y")
-                                    + (self.final_year - self.annee_erfs)
+                                    + (self.final_year - self.annee_donnees)
                                 ),
                                 "D",
                             )
                             for date in array_var
                         ]
                     else:
                         inflated_array = array_var.copy()
@@ -258,20 +258,25 @@
             # TODO comme ci dessus pour les variables d'indentifiant
             "noindiv",  # source : ERFS-FPR
             "quifoy",
             "quifam",
             "quimen",
         ]
 
-        specific_variables = ["taux_capacite_travail", "taux_incapacite"]
+        variables_imputation_erfs = [
+            "taux_capacite_travail",
+            "taux_incapacite",
+            "caseP",
+            "caseT",
+        ]
 
         leximpact_variables = (
             wprms
             + variables_to_keep_or_to_calculate
             + ids
             + roles
             + future_monte_carlo_variables
-            + specific_variables
+            + variables_imputation_erfs
         )
         self.used_as_input_variables = list(
             set(self.used_as_input_variables + leximpact_variables)
         )
```

### Comparing `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/leximpact_tax_and_benefit_system.py` & `leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/leximpact_tax_and_benefit_system.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 import numpy as np
 from openfisca_core import reforms
-
 from openfisca_france_data import france_data_tax_benefit_system
 from openfisca_france_data.model.base import (
     ETERNITY,
     YEAR,
     Individu,
     Menage,
     FoyerFiscal,
@@ -147,26 +146,55 @@
                 Impôt après imputation des réductions d'impôt
                 """
                 ip_net = foyer_fiscal("ip_net", period)
                 reductions = foyer_fiscal("reductions", period)
 
                 return np.maximum(0, ip_net - reductions)
 
+        class reduction_effective(Variable):
+            value_type = float
+            entity = FoyerFiscal
+            label = "Impôt après imputation des réductions d'impôt"
+            definition_period = YEAR
+
+            def formula(foyer_fiscal, period):
+                """
+                Impôt après imputation des réductions d'impôt
+                """
+                ip_net = foyer_fiscal("ip_net", period)
+                reductions = foyer_fiscal("reductions", period)
+
+                return np.where(ip_net - reductions >= 0, reductions, ip_net)
+
+        class impot_revenu_total(Variable):
+            value_type = float
+            entity = FoyerFiscal
+            label = "Impôt sur le revenu avec la partie pfu"
+            definition_period = YEAR
+
+            def formula(foyer_fiscal, period):
+                irpp = foyer_fiscal("irpp_economique", period)
+                pfu = foyer_fiscal("prelevement_forfaitaire_unique_ir", period)
+
+                return irpp + pfu
+
         variables = [
             quimen,
             quifam,
             quifoy,
             idmen,
             idmen_original,
             idfam,
             idfoy,
             menage_id,
             famille_id,
             foyer_fiscal_id,
             noindiv,
+            impot_revenu_total,
+            reduction_effective,
         ]
 
         # Adaptation de variables du fait des variables de revenus du capital imputées
         updated_variables = [
             iaidrdi,
             plus_values_prelevement_forfaitaire_unique_ir,
             rfr_plus_values_hors_rni,
@@ -183,9 +211,11 @@
         for neutralized_variable in neutralized_variables:
             log.info(f"Neutralizing {neutralized_variable}")
             if self.get_variable(neutralized_variable):
                 self.neutralize_variable(neutralized_variable)
         for updated_variable in updated_variables:
             self.update_variable(updated_variable)
 
+        self.neutralize_variable("taxe_habitation")
+
 
 leximpact_tbs = leximpact_tbs_extension(france_data_tax_benefit_system)
```

### Comparing `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/helpers_survey_scenario.py` & `leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/helpers_survey_scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from leximpact_aggregates.aggregate import AggregateManager
 from decouple import config
 
 
 tc = unittest.TestCase()
 
 # Import des années
-annee_erfs = config("YEAR_ERFS")
 annee_pote = config("YEAR_POTE")
 annee_de_calcul = config("YEAR_COMPUTATION")
 aggregates_path = config("AGREGATS_PATH")
 
 dico_var = {
     "entity_list": {"individu", "menage", "famille", "foyer_fiscal"},
     "individu": {
@@ -550,34 +549,34 @@
         var_name,
     )
 
     return quantiles, frontieres_var
 
 
 def generate_title(
-    var_name, annee_erfs, annee_pote, title_suffix, log=False, cal=False
+    var_name, annee_donnees, annee_pote, title_suffix, log=False, cal=False
 ):
     """Génère un titre adapté pour les différents plots issus de la calibration"""
     # Avec ou sans calibration
     if cal is False:
         title = (
             "Comparaison des distributions de "
             + var_name
             + "\n ERFS "
-            + annee_erfs
+            + annee_donnees
             + " (en rouge) et  POTE  "
             + annee_pote
             + " (en bleu) "
         )
     else:
         title = (
             "Calibration de la distribution de "
             + var_name
             + "\n ERFS "
-            + annee_erfs
+            + annee_donnees
             + " (en rouge), calibration (en vert) et  POTE  "
             + annee_pote
             + " (en bleu) "
         )
 
     # Details
     title = title + title_suffix
```

### Comparing `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/inflation_calibration_values.py` & `leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/inflation_calibration_values.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 # Regression linéaire pour estimer les salaires des années futures
 def projection_salaires(yearf):
     yearf = int(yearf)
     salaires_annuels = total_annuel_salaires.copy()
 
     last_known = int(list(total_annuel_salaires.keys())[-1])
-    print(
-        "Attention, les années au-dessus de ",
-        last_known,
-        " sont estimées par régression linéaire",
-    )
+    # print(
+    #    "Attention, les années au-dessus de ",
+    #    last_known,
+    #    " sont estimées par régression linéaire",
+    # )
 
     # Linear Regression
     # X = np.array([int(i) for i in range(len(inflation_sal.values()))]).reshape(-1, 1)
     X = np.array([int(i) for i in total_annuel_salaires.keys()]).reshape(-1, 1)
     Y = np.array([float(i) for i in total_annuel_salaires.values()]).reshape(-1, 1)
 
     model = LinearRegression().fit(X, Y)
@@ -94,15 +94,15 @@
 # REVALORISATION DES RETRAITES
 def inflator_retraite(startp, endp):
     startp = int(startp)
     endp = int(endp)
     # Calcul du taux d'inflation des retraites sur plusieurs années
     adjrate_ret = 1
     for year in range(startp, endp):
-        print(year)
+        # print(year)
         rateinfla = revalorisation_retraite[str(year)]
         adjrate_ret = adjrate_ret * (1 + rateinfla / 100)  # Car on a les données en %
     # print("Taux d'ajustement de revalorisation des retraites: ", adjrate_ret)
 
     return adjrate_ret
 
 
@@ -208,15 +208,15 @@
         "revenus_capitaux_prelevement_forfaitaire_unique_ir",
         "rente_viagere_titre_onereux_net",
         "revenu_categoriel_foncier",
         "assiette_csg_plus_values",
         "reductions",
         "credits_impot",
     ]
-    adjrate_sal = inflator_smpt(startp, endp)
+    adjrate_sal = inflator_salarial(startp, endp)
 
     # Variables indexées sur l'indice des prix à la consommation
     cols_type_idc = [
         "revenus_capitaux_prelevement_liberatoire",
         "revenus_capitaux_prelevement_bareme",
         "revenus_capitaux_prelevement_forfaitaire_unique_ir",
         "rente_viagere_titre_onereux_net",
```

### Comparing `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/inflator.py` & `leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/inflator.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     "2014": 674_188_954_200,
     "2015": 683_665_874_000,
     "2016": 695_665_787_000,
     "2017": 713_523_524_000,
     "2018": 738_077_177_000,
     "2019": 743_500_200_000,  # Sur le nouveau site
     "2020": 758_741_700_000,  # Sur le nouveau site
-    "2021": 758_741_700_000 * 1.023,
-    "2022": 758_741_700_000 * 1.023 * 1.031,
-    "2023": 758_741_700_000 * 1.023 * 1.031 * 1.033,
+    "2021": 789_033_000_000,
+    "2022": 789_033_000_000 * 1.057,  # à changer
+    "2023": 789_033_000_000 * 1.057 * 1.038,  # à changer
 }
 
 # Création de la liste des taux d'inflation (en %)
 # Données issues du PLF - 'Chiffres clés' (=inflation hors tabac = prix à la consommation)
 inflation_idc = {
     "2017": 1.0,
     "2018": 1.6,
```

### Comparing `leximpact_survey_scenario-0.1.1/leximpact_survey_scenario/scenario_tools/plot.py` & `leximpact_survey_scenario-0.1.2/leximpact_survey_scenario/scenario_tools/plot.py`

 * *Files identical despite different names*

### Comparing `leximpact_survey_scenario-0.1.1/pyproject.toml` & `leximpact_survey_scenario-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leximpact-survey-scenario"
-version = "0.1.1"
+version = "0.1.2"
 description = "OpenFisca Survey Scenario for LexImpact"
 authors = ["LexImapct"]
 license = "LGPLv3"
 readme = "README.md"
 packages = [{include = "leximpact_survey_scenario"}]
 
 [tool.poetry.dependencies]
```

### Comparing `leximpact_survey_scenario-0.1.1/PKG-INFO` & `leximpact_survey_scenario-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leximpact-survey-scenario
-Version: 0.1.1
+Version: 0.1.2
 Summary: OpenFisca Survey Scenario for LexImpact
 License: LGPLv3
 Author: LexImapct
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

