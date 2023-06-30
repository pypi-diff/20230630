# Comparing `tmp/feedancy-0.0.0.tar.gz` & `tmp/feedancy-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.0.tar", max compression
+gzip compressed data, was "feedancy-0.0.1.tar", max compression
```

## Comparing `feedancy-0.0.0.tar` & `feedancy-0.0.1.tar`

### file list

```diff
@@ -1,123 +1,126 @@
--rw-r--r--   0        0        0      615 2023-06-29 16:42:07.944019 feedancy-0.0.0/README.md
--rw-r--r--   0        0        0      126 2023-06-29 16:42:07.936019 feedancy-0.0.0/feedancy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 16:42:07.884018 feedancy-0.0.0/feedancy/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 16:42:07.884018 feedancy-0.0.0/feedancy/apis/api/__init__.py
--rw-r--r--   0        0        0    13072 2023-06-29 16:42:07.884018 feedancy-0.0.0/feedancy/apis/api/api.py
--rw-r--r--   0        0        0      763 2023-06-29 16:42:07.896018 feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_create.py
--rw-r--r--   0        0        0      820 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_destroy.py
--rw-r--r--   0        0        0      762 2023-06-29 16:42:07.896018 feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_retrieve.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_update.py
--rw-r--r--   0        0        0      753 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_city_create.py
--rw-r--r--   0        0        0      810 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_city_destroy.py
--rw-r--r--   0        0        0      752 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_city_retrieve.py
--rw-r--r--   0        0        0      807 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_city_retrieve_2.py
--rw-r--r--   0        0        0      807 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_city_update.py
--rw-r--r--   0        0        0      756 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_company_create.py
--rw-r--r--   0        0        0      813 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_company_destroy.py
--rw-r--r--   0        0        0      755 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_company_retrieve.py
--rw-r--r--   0        0        0      810 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_company_retrieve_2.py
--rw-r--r--   0        0        0      810 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_company_update.py
--rw-r--r--   0        0        0      760 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_create.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_destroy.py
--rw-r--r--   0        0        0      759 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_retrieve.py
--rw-r--r--   0        0        0      814 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_retrieve_2.py
--rw-r--r--   0        0        0      814 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_update.py
--rw-r--r--   0        0        0      756 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_contact_create.py
--rw-r--r--   0        0        0      813 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_contact_destroy.py
--rw-r--r--   0        0        0      755 2023-06-29 16:42:07.900018 feedancy-0.0.0/feedancy/apis/api/api_v1_contact_retrieve.py
--rw-r--r--   0        0        0      810 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_contact_retrieve_2.py
--rw-r--r--   0        0        0      810 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_contact_update.py
--rw-r--r--   0        0        0      756 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_country_create.py
--rw-r--r--   0        0        0      813 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_country_destroy.py
--rw-r--r--   0        0        0      755 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_country_retrieve.py
--rw-r--r--   0        0        0      810 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_country_retrieve_2.py
--rw-r--r--   0        0        0      810 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_country_update.py
--rw-r--r--   0        0        0      757 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_currency_create.py
--rw-r--r--   0        0        0      814 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_currency_destroy.py
--rw-r--r--   0        0        0      756 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_currency_retrieve.py
--rw-r--r--   0        0        0      811 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_currency_retrieve_2.py
--rw-r--r--   0        0        0      811 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_currency_update.py
--rw-r--r--   0        0        0      759 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_internship_create.py
--rw-r--r--   0        0        0     1941 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internship_destroy.py
--rw-r--r--   0        0        0      758 2023-06-29 16:42:07.904018 feedancy-0.0.0/feedancy/apis/api/api_v1_internship_retrieve.py
--rw-r--r--   0        0        0     1938 2023-06-29 16:42:07.908018 feedancy-0.0.0/feedancy/apis/api/api_v1_internship_retrieve_2.py
--rw-r--r--   0        0        0     1976 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internship_update.py
--rw-r--r--   0        0        0      763 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_create.py
--rw-r--r--   0        0        0      820 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_destroy.py
--rw-r--r--   0        0        0      762 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_retrieve.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_update.py
--rw-r--r--   0        0        0      766 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_create.py
--rw-r--r--   0        0        0      823 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_destroy.py
--rw-r--r--   0        0        0      765 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
--rw-r--r--   0        0        0      820 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0      820 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_update.py
--rw-r--r--   0        0        0      764 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_create.py
--rw-r--r--   0        0        0      821 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_destroy.py
--rw-r--r--   0        0        0      763 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_retrieve.py
--rw-r--r--   0        0        0      818 2023-06-29 16:42:07.912018 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      818 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_update.py
--rw-r--r--   0        0        0      757 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_create.py
--rw-r--r--   0        0        0      814 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_destroy.py
--rw-r--r--   0        0        0      756 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_retrieve.py
--rw-r--r--   0        0        0      811 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
--rw-r--r--   0        0        0      811 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_update.py
--rw-r--r--   0        0        0      755 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_region_create.py
--rw-r--r--   0        0        0      812 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_region_destroy.py
--rw-r--r--   0        0        0      754 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_region_retrieve.py
--rw-r--r--   0        0        0      809 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_region_retrieve_2.py
--rw-r--r--   0        0        0      809 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_region_update.py
--rw-r--r--   0        0        0      755 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_salary_create.py
--rw-r--r--   0        0        0      812 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_salary_destroy.py
--rw-r--r--   0        0        0      754 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_salary_retrieve.py
--rw-r--r--   0        0        0      809 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_salary_retrieve_2.py
--rw-r--r--   0        0        0      809 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_salary_update.py
--rw-r--r--   0        0        0      770 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
--rw-r--r--   0        0        0      827 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      769 2023-06-29 16:42:07.916019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      824 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      824 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
--rw-r--r--   0        0        0      763 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_create.py
--rw-r--r--   0        0        0      820 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_destroy.py
--rw-r--r--   0        0        0      762 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_update.py
--rw-r--r--   0        0        0      754 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_skill_create.py
--rw-r--r--   0        0        0      811 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_skill_destroy.py
--rw-r--r--   0        0        0      753 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_skill_retrieve.py
--rw-r--r--   0        0        0      808 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_skill_retrieve_2.py
--rw-r--r--   0        0        0      808 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_skill_update.py
--rw-r--r--   0        0        0      755 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_source_create.py
--rw-r--r--   0        0        0      812 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_source_destroy.py
--rw-r--r--   0        0        0      754 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_source_retrieve.py
--rw-r--r--   0        0        0      809 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_source_retrieve_2.py
--rw-r--r--   0        0        0      809 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_source_update.py
--rw-r--r--   0        0        0      761 2023-06-29 16:42:07.924019 feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_create.py
--rw-r--r--   0        0        0      818 2023-06-29 16:42:07.924019 feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_destroy.py
--rw-r--r--   0        0        0      760 2023-06-29 16:42:07.920019 feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
--rw-r--r--   0        0        0      815 2023-06-29 16:42:07.924019 feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      815 2023-06-29 16:42:07.924019 feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_update.py
--rw-r--r--   0        0        0     2046 2023-06-29 16:42:07.928019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_create.py
--rw-r--r--   0        0        0     2068 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_destroy.py
--rw-r--r--   0        0        0     3236 2023-06-29 16:42:07.924019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_list.py
--rw-r--r--   0        0        0     2065 2023-06-29 16:42:07.928019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_retrieve.py
--rw-r--r--   0        0        0     2100 2023-06-29 16:42:07.928019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_update.py
--rw-r--r--   0        0        0      760 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_create.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_destroy.py
--rw-r--r--   0        0        0      759 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_retrieve.py
--rw-r--r--   0        0        0      814 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      814 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_update.py
--rw-r--r--   0        0        0      763 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_create.py
--rw-r--r--   0        0        0      820 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_destroy.py
--rw-r--r--   0        0        0      762 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0      817 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_update.py
--rw-r--r--   0        0        0      761 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_create.py
--rw-r--r--   0        0        0      818 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_destroy.py
--rw-r--r--   0        0        0      760 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
--rw-r--r--   0        0        0      815 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      815 2023-06-29 16:42:07.932019 feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_update.py
--rw-r--r--   0        0        0      658 2023-06-29 16:42:07.940019 feedancy-0.0.0/feedancy/client.py
--rw-r--r--   0        0        0      640 2023-06-30 11:41:56.940365 feedancy-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 feedancy-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-06-05 13:45:57.561946 feedancy-0.0.1/README.md
+-rw-r--r--   0        0        0      203 2023-06-30 12:17:19.873899 feedancy-0.0.1/feedancy/MANIFEST.in
+-rw-r--r--   0        0        0      615 2023-06-30 12:17:19.873899 feedancy-0.0.1/feedancy/README.md
+-rw-r--r--   0        0        0      126 2023-06-30 12:17:19.865899 feedancy-0.0.1/feedancy/feedancy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 12:17:19.805898 feedancy-0.0.1/feedancy/feedancy/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 12:17:19.805898 feedancy-0.0.1/feedancy/feedancy/apis/api/__init__.py
+-rw-r--r--   0        0        0    13072 2023-06-30 12:17:19.809898 feedancy-0.0.1/feedancy/feedancy/apis/api/api.py
+-rw-r--r--   0        0        0      763 2023-06-30 12:17:19.821898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py
+-rw-r--r--   0        0        0      762 2023-06-30 12:17:19.821898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py
+-rw-r--r--   0        0        0      753 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_create.py
+-rw-r--r--   0        0        0      810 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_destroy.py
+-rw-r--r--   0        0        0      752 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_retrieve.py
+-rw-r--r--   0        0        0      807 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py
+-rw-r--r--   0        0        0      807 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_update.py
+-rw-r--r--   0        0        0      756 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_destroy.py
+-rw-r--r--   0        0        0      755 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_retrieve.py
+-rw-r--r--   0        0        0      810 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py
+-rw-r--r--   0        0        0      810 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_update.py
+-rw-r--r--   0        0        0      760 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_create.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py
+-rw-r--r--   0        0        0      759 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py
+-rw-r--r--   0        0        0      814 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py
+-rw-r--r--   0        0        0      814 2023-06-30 12:17:19.825898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_update.py
+-rw-r--r--   0        0        0      756 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_destroy.py
+-rw-r--r--   0        0        0      755 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py
+-rw-r--r--   0        0        0      810 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py
+-rw-r--r--   0        0        0      810 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_update.py
+-rw-r--r--   0        0        0      756 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_destroy.py
+-rw-r--r--   0        0        0      755 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_retrieve.py
+-rw-r--r--   0        0        0      810 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py
+-rw-r--r--   0        0        0      810 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_update.py
+-rw-r--r--   0        0        0      757 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_create.py
+-rw-r--r--   0        0        0      814 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_destroy.py
+-rw-r--r--   0        0        0      756 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py
+-rw-r--r--   0        0        0      811 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py
+-rw-r--r--   0        0        0      811 2023-06-30 12:17:19.829898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_update.py
+-rw-r--r--   0        0        0      759 2023-06-30 12:17:19.833898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_create.py
+-rw-r--r--   0        0        0     1941 2023-06-30 12:17:19.837898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_destroy.py
+-rw-r--r--   0        0        0      758 2023-06-30 12:17:19.833898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py
+-rw-r--r--   0        0        0     1938 2023-06-30 12:17:19.833898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py
+-rw-r--r--   0        0        0     1976 2023-06-30 12:17:19.837898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_update.py
+-rw-r--r--   0        0        0      763 2023-06-30 12:17:19.837898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py
+-rw-r--r--   0        0        0      762 2023-06-30 12:17:19.837898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.837898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.837898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py
+-rw-r--r--   0        0        0      766 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py
+-rw-r--r--   0        0        0      823 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py
+-rw-r--r--   0        0        0      765 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
+-rw-r--r--   0        0        0      820 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
+-rw-r--r--   0        0        0      820 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py
+-rw-r--r--   0        0        0      764 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py
+-rw-r--r--   0        0        0      821 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py
+-rw-r--r--   0        0        0      763 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py
+-rw-r--r--   0        0        0      818 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
+-rw-r--r--   0        0        0      818 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py
+-rw-r--r--   0        0        0      757 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py
+-rw-r--r--   0        0        0      814 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py
+-rw-r--r--   0        0        0      756 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py
+-rw-r--r--   0        0        0      811 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
+-rw-r--r--   0        0        0      811 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py
+-rw-r--r--   0        0        0      755 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_destroy.py
+-rw-r--r--   0        0        0      754 2023-06-30 12:17:19.841898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_retrieve.py
+-rw-r--r--   0        0        0      809 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py
+-rw-r--r--   0        0        0      809 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_update.py
+-rw-r--r--   0        0        0      755 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_destroy.py
+-rw-r--r--   0        0        0      754 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py
+-rw-r--r--   0        0        0      809 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py
+-rw-r--r--   0        0        0      809 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_update.py
+-rw-r--r--   0        0        0      770 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
+-rw-r--r--   0        0        0      827 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
+-rw-r--r--   0        0        0      769 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
+-rw-r--r--   0        0        0      824 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      824 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
+-rw-r--r--   0        0        0      763 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py
+-rw-r--r--   0        0        0      762 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.845898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py
+-rw-r--r--   0        0        0      754 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_create.py
+-rw-r--r--   0        0        0      811 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_destroy.py
+-rw-r--r--   0        0        0      753 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py
+-rw-r--r--   0        0        0      808 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py
+-rw-r--r--   0        0        0      808 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_update.py
+-rw-r--r--   0        0        0      755 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_destroy.py
+-rw-r--r--   0        0        0      754 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_retrieve.py
+-rw-r--r--   0        0        0      809 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py
+-rw-r--r--   0        0        0      809 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_update.py
+-rw-r--r--   0        0        0      761 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py
+-rw-r--r--   0        0        0      818 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py
+-rw-r--r--   0        0        0      760 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
+-rw-r--r--   0        0        0      815 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      815 2023-06-30 12:17:19.849898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py
+-rw-r--r--   0        0        0     2046 2023-06-30 12:17:19.857899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_create.py
+-rw-r--r--   0        0        0     2068 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py
+-rw-r--r--   0        0        0     3236 2023-06-30 12:17:19.853898 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_list.py
+-rw-r--r--   0        0        0     2065 2023-06-30 12:17:19.857899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py
+-rw-r--r--   0        0        0     2100 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_update.py
+-rw-r--r--   0        0        0      760 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py
+-rw-r--r--   0        0        0      759 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py
+-rw-r--r--   0        0        0      814 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
+-rw-r--r--   0        0        0      814 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py
+-rw-r--r--   0        0        0      763 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py
+-rw-r--r--   0        0        0      762 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
+-rw-r--r--   0        0        0      817 2023-06-30 12:17:19.861899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py
+-rw-r--r--   0        0        0      761 2023-06-30 12:17:19.865899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py
+-rw-r--r--   0        0        0      818 2023-06-30 12:17:19.865899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py
+-rw-r--r--   0        0        0      760 2023-06-30 12:17:19.865899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
+-rw-r--r--   0        0        0      815 2023-06-30 12:17:19.865899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
+-rw-r--r--   0        0        0      815 2023-06-30 12:17:19.865899 feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py
+-rw-r--r--   0        0        0      658 2023-06-30 12:17:19.869899 feedancy-0.0.1/feedancy/feedancy/client.py
+-rw-r--r--   0        0        0     1000 2023-06-30 12:17:19.873899 feedancy-0.0.1/feedancy/setup.py
+-rw-r--r--   0        0        0      937 2023-06-30 12:18:41.302353 feedancy-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 feedancy-0.0.1/PKG-INFO
```

### Comparing `feedancy-0.0.0/README.md` & `feedancy-0.0.1/feedancy/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_activitysphere_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_city_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_city_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_city_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_city_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_city_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_city_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_company_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_company_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_company_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_company_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_company_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_company_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_companycity_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_companycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_contact_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_contact_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_contact_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_contact_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_contact_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_contact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_country_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_country_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_country_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_country_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_country_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_country_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_currency_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_currency_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_currency_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_currency_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_currency_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_currency_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internship_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internship_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internship_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internship_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internship_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internship_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcity_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipcontact_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_internshipskill_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_jobmixin_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_region_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_region_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_region_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_region_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_region_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_region_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_salary_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_salary_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_salary_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_salary_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_salary_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_salary_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchandstopkeywords_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_searchkeywords_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_skill_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_skill_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_skill_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_skill_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_skill_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_skill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_source_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_source_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_source_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_source_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_source_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_source_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_stopkeywords_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_list.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_list.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancy_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancy_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycity_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancycontact_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_create.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_destroy.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_retrieve.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/apis/api/api_v1_vacancyskill_update.py` & `feedancy-0.0.1/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/feedancy/client.py` & `feedancy-0.0.1/feedancy/feedancy/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.0/pyproject.toml` & `feedancy-0.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,29 @@
+[tool.black]
+line-length = 79
+target-version = ['py38', 'py39']
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.eggs    # exclude a few common directories in the
+  | \.git     # root of Black repositories
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+)/
+'''
+
 [tool.poetry]
 name = "feedancy"
-version = "0.0.0"
+version = "0.0.1"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
@@ -21,8 +40,8 @@
 pydantic = ">=1.10.8"
 requests = ">=2.31"
 bs4 = ">=0.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

