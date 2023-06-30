# Comparing `tmp/data-inclusion-schema-0.8.0.tar.gz` & `tmp/data_inclusion_schema-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-inclusion-schema-0.8.0.tar", last modified: Wed Mar  8 10:44:41 2023, max compression
+gzip compressed data, was "data_inclusion_schema-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `data-inclusion-schema-0.8.0.tar` & `data_inclusion_schema-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     2422 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/README.md
--rw-r--r--   0        0        0     1276 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/__init__.py
--rw-r--r--   0        0        0     1352 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/__main__.py
--rw-r--r--   0        0        0     1217 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/base.py
--rw-r--r--   0        0        0      316 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/code_officiel_geographique.py
--rw-r--r--   0        0        0      912 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/frais.py
--rw-r--r--   0        0        0     7575 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/labels_nationaux.py
--rw-r--r--   0        0        0     4779 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/models.py
--rw-r--r--   0        0        0      264 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/modes_accueil.py
--rw-r--r--   0        0        0     1430 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/profils.py
--rw-r--r--   0        0        0    22946 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/thematiques.py
--rw-r--r--   0        0        0     1955 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/typologies_de_services.py
--rw-r--r--   0        0        0     7464 2023-03-08 10:44:28.649751 data-inclusion-schema-0.8.0/src/data_inclusion/schema/typologies_de_structures.py
--rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 data-inclusion-schema-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2422 2023-06-30 08:51:01.949597 data_inclusion_schema-0.9.0/README.md
+-rw-r--r--   0        0        0     1276 2023-06-30 08:51:01.949597 data_inclusion_schema-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/__init__.py
+-rw-r--r--   0        0        0     1526 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/__main__.py
+-rw-r--r--   0        0        0     1217 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/base.py
+-rw-r--r--   0        0        0      466 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/code_officiel_geographique.py
+-rw-r--r--   0        0        0      912 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/frais.py
+-rw-r--r--   0        0        0     7575 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/labels_nationaux.py
+-rw-r--r--   0        0        0     5153 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/models.py
+-rw-r--r--   0        0        0      264 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/modes_accueil.py
+-rw-r--r--   0        0        0     1446 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/modes_orientation.py
+-rw-r--r--   0        0        0     1687 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/profils.py
+-rw-r--r--   0        0        0    25488 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/thematiques.py
+-rw-r--r--   0        0        0     1955 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/typologies_de_services.py
+-rw-r--r--   0        0        0     7581 2023-06-30 08:51:01.953597 data_inclusion_schema-0.9.0/src/data_inclusion/schema/typologies_de_structures.py
+-rw-r--r--   0        0        0     3156 1970-01-01 00:00:00.000000 data_inclusion_schema-0.9.0/PKG-INFO
```

### Comparing `data-inclusion-schema-0.8.0/README.md` & `data_inclusion_schema-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `data-inclusion-schema-0.8.0/pyproject.toml` & `data_inclusion_schema-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "data-inclusion-schema"
-version = "0.8.0"
+version = "0.9.0"
 description = "Schéma de l'offre d'insertion"
 authors = [{ name = "data.inclusion", email = "data.inclusion@beta.gouv.fr" }]
 readme = "README.md"
 dynamic = []
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/__main__.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         ("typologies-de-structures.json", models.Typologie),
         ("labels-nationaux.json", models.LabelNational),
         ("thematiques.json", models.Thematique),
         ("typologies-de-services.json", models.TypologieService),
         ("frais.json", models.Frais),
         ("profils.json", models.Profil),
         ("modes-accueil.json", models.ModeAccueil),
+        ("modes-orientation-beneficiaire.json", models.ModeOrientationBeneficiaire),
+        ("modes-orientation-accompagnateur.json", models.ModeOrientationAccompagnateur),
     ]
 
     for filename, enum in enum_x_file_tuples_list:
         with (output_dir / "extra" / filename).open("w") as file:
             json.dump(
                 enum.as_dict_list(),
                 file,
```

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/base.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/base.py`

 * *Files identical despite different names*

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/frais.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/frais.py`

 * *Files identical despite different names*

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/labels_nationaux.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/labels_nationaux.py`

 * *Files identical despite different names*

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/models.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import pydantic
 from pydantic import BaseModel, EmailStr, Extra, HttpUrl, constr
 
 from data_inclusion.schema.code_officiel_geographique import TypeCOG
 from data_inclusion.schema.frais import Frais
 from data_inclusion.schema.labels_nationaux import LabelNational
 from data_inclusion.schema.modes_accueil import ModeAccueil
+from data_inclusion.schema.modes_orientation import (
+    ModeOrientationAccompagnateur,
+    ModeOrientationBeneficiaire,
+)
 from data_inclusion.schema.profils import Profil
 from data_inclusion.schema.thematiques import Thematique
 from data_inclusion.schema.typologies_de_services import TypologieService
 from data_inclusion.schema.typologies_de_structures import Typologie
 
 
 class Service(BaseModel):
@@ -46,18 +50,22 @@
     courriel: Optional[EmailStr]
     contact_public: Optional[bool]
     date_maj: Optional[date | datetime]
     modes_accueil: Optional[list[ModeAccueil]]
     zone_diffusion_type: Optional[TypeCOG]
     zone_diffusion_code: Optional[
         constr(regex=r"^\w{5}$")  # code commune
+        | constr(regex=r"^\d{9}$")  # code epci
         | constr(regex=r"^\w{2,3}$")  # code departement
         | constr(regex=r"^\d{2}$")  # code region
     ]
     zone_diffusion_nom: Optional[str]
+    contact_nom_prenom: Optional[str]
+    modes_orientation_beneficiaire: Optional[list[ModeOrientationBeneficiaire]]
+    modes_orientation_accompagnateur: Optional[list[ModeOrientationAccompagnateur]]
 
     class Config:
         extra = Extra.forbid
 
 
 class Structure(BaseModel):
     id: str
```

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/profils.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/profils.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,7 +56,17 @@
         "Le lieu propose des accompagnements réservés aux femmes.",
     )
     PERSONNES_EN_SITUATION_ILLETTRISME = (
         "personnes-en-situation-illettrisme",
         "Personnes en situation d’illettrisme",
         None,
     )
+    BENEFICIAIRE_RSA = (
+        "beneficiaire-rsa",
+        "Bénéficiaire du Revenu de Solidarité Active (RSA)",
+        None,
+    )
+    DEMANDEUR_EMPLOI = (
+        "demandeur-demploi",
+        "Demandeur ou demandeuse d’emploi",
+        None,
+    )
```

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/thematiques.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/thematiques.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,19 @@
         None,
     )
     ACCES_AUX_DROITS_ET_CITOYENNETE__ACCOMPAGNEMENT_JURIDIQUE = (
         "acces-aux-droits-et-citoyennete--accompagnement-juridique",
         "Accompagnement juridique",
         None,
     )
+    ACCES_AUX_DROITS_ET_CITOYENNETE__AIDE_AUX_VICTIMES = (
+        "acces-aux-droits-et-citoyennete--aide-aux-victimes",
+        "Aide aux victimes",
+        None,
+    )
     ACCES_AUX_DROITS_ET_CITOYENNETE__CONNAITRE_SES_DROITS = (
         "acces-aux-droits-et-citoyennete--connaitre-ses-droits",
         "Connaitre ses droits",
         None,
     )
     ACCES_AUX_DROITS_ET_CITOYENNETE__DEMANDEURS_DASILE_ET_NATURALISATION = (
         "acces-aux-droits-et-citoyennete--demandeurs-dasile-et-naturalisation",
@@ -64,14 +69,35 @@
             "accompagnement-social-et-professionnel-personnalise--"
             "parcours-d-insertion-socioprofessionnel"
         ),
         "Parcours d’insertion socio-professionnel",
         None,
     )
 
+    APPRENDRE_FRANCAIS = (
+        "apprendre-francais",
+        "Apprendre le Français",
+        None,
+    )
+    APPRENDRE_FRANCAIS__ACCOMPAGNEMENT_INSERTION_PRO = (
+        "apprendre-francais--accompagnement-insertion-pro",
+        "Accompagnement vers l’insertion professionnelle",
+        None,
+    )
+    APPRENDRE_FRANCAIS__COMMUNIQUER_VIE_TOUS_LES_JOURS = (
+        "apprendre-francais--communiquer-vie-tous-les-jours",
+        "Communiquer dans la vie de tous les jours",
+        None,
+    )
+    APPRENDRE_FRANCAIS__SUIVRE_FORMATION = (
+        "apprendre-francais--suivre-formation",
+        "Suivre une formation",
+        None,
+    )
+
     CHOISIR_UN_METIER = (
         "choisir-un-metier",
         "Choisir un métier",
         None,
     )
     CHOISIR_UN_METIER__IDENTIFIER_SES_POINTS_FORTS_ET_SES_COMPETENCES = (
         "choisir-un-metier--identifier-ses-points-forts-et-ses-competences",
@@ -283,14 +309,70 @@
             "handicap--"
             "gerer-le-depart-a-la-retraite-des-personnes-en-situation-de-handicap"
         ),
         "Gérer le départ à la retraite des personnes en situation de handicap",
         None,
     )
 
+    ILLETRISME = (
+        "illettrisme",
+        "Illettrisme",
+        None,
+    )
+    ILLETTRISME__ACCOMPAGNER_SCOLARITE = (
+        "illettrisme--accompagner-scolarite",
+        "Accompagner la scolarité d’un enfant",
+        None,
+    )
+    ILLETTRISME__AMELIORER_VOCABULAIRE = (
+        "illettrisme--ameliorer-vocabulaire",
+        "Améliorer un niveau de vocabulaire",
+        None,
+    )
+    ILLETTRISME__ETRE_AUTONOME = (
+        "illettrisme--etre-autonome",
+        "Être autonome dans la vie de tous les jours",
+        None,
+    )
+    ILLETTRISME__INFO_ACQUISITION_CONNAISSANCES = (
+        "illettrisme--info-acquisition-connaissances",
+        "Être informé(e) sur l’acquisition des compétences de base",
+        None,
+    )
+    ILLETTRISME__PERMIS_CONDUIRE = (
+        "illettrisme--permis-conduire",
+        "Passer le permis de conduire",
+        None,
+    )
+    ILLETTRISME__REPERER_SITUATION_ILLETTRISME = (
+        "illettrisme--reperer-situation-illettrisme",
+        "Repérer des situations d’illettrisme",
+        None,
+    )
+    ILLETTRISME__SURMONTER_TROUBLE_APPRENTISSAGE = (
+        "illettrisme--surmonter-trouble-apprentissage",
+        "Surmonter un trouble de l’apprentissage",
+        None,
+    )
+    ILLETTRISME__TROUVER_EMPLOI_FORMATION = (
+        "illettrisme--trouver-emploi-formation",
+        "Trouver un emploi ou une formation",
+        None,
+    )
+    ILLETTRISME__UTILISER_NUMERIQUE = (
+        "illettrisme--utiliser-numerique",
+        "Savoir utiliser les outils numériques",
+        None,
+    )
+    ILLETTRISME__VALIDER_CERTIFICATION_CLEA = (
+        "illettrisme--valider-certification-clea",
+        "Valider une certification Cléa",
+        None,
+    )
+
     LOGEMENT_HEBERGEMENT = (
         "logement-hebergement",
         "Logement et hébergement",
         None,
     )
     LOGEMENT_HEBERGEMENT__ETRE_ACCOMPAGNE_POUR_SE_LOGER = (
         "logement-hebergement--etre-accompagne-pour-se-loger",
```

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/typologies_de_services.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/typologies_de_services.py`

 * *Files identical despite different names*

### Comparing `data-inclusion-schema-0.8.0/src/data_inclusion/schema/typologies_de_structures.py` & `data_inclusion_schema-0.9.0/src/data_inclusion/schema/typologies_de_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,19 @@
         None,
     )
     Autre = (
         "Autre",
         "Autre",
         None,
     )
+    AVIP = (
+        "AVIP",
+        "Crèche À Vocation d’Insertion Professionnelle (AVIP)",
+        None,
+    )
     BIB = (
         "BIB",
         "Bibliothèque / Médiathèque",
         None,
     )
     CAARUD = (
         "CAARUD",
```

### Comparing `data-inclusion-schema-0.8.0/PKG-INFO` & `data_inclusion_schema-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-inclusion-schema
-Version: 0.8.0
+Version: 0.9.0
 Summary: Schéma de l'offre d'insertion
 Author-email: "data.inclusion" <data.inclusion@beta.gouv.fr>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pydantic[email]>=1.9.1,<2.0.0
 Requires-Dist: black==22.10.0 ; extra == "dev"
```

