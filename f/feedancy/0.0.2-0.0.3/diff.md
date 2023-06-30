# Comparing `tmp/feedancy-0.0.2.tar.gz` & `tmp/feedancy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.2.tar", max compression
+gzip compressed data, was "feedancy-0.0.3.tar", max compression
```

## Comparing `feedancy-0.0.2.tar` & `feedancy-0.0.3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0       37 2023-06-05 13:45:57.561946 feedancy-0.0.2/README.md
--rw-r--r--   0        0        0      203 2023-06-30 13:04:55.017686 feedancy-0.0.2/feedancy/MANIFEST.in
--rw-r--r--   0        0        0      615 2023-06-30 13:04:55.013686 feedancy-0.0.2/feedancy/README.md
--rw-r--r--   0        0        0      126 2023-06-30 13:04:55.005686 feedancy-0.0.2/feedancy/feedancy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 13:04:54.917685 feedancy-0.0.2/feedancy/feedancy/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 13:04:54.917685 feedancy-0.0.2/feedancy/feedancy/apis/api/__init__.py
--rw-r--r--   0        0        0    13072 2023-06-30 13:04:54.921685 feedancy-0.0.2/feedancy/feedancy/apis/api/api.py
--rw-r--r--   0        0        0      896 2023-06-30 13:04:54.937685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py
--rw-r--r--   0        0        0      820 2023-06-30 13:04:54.937685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py
--rw-r--r--   0        0        0      853 2023-06-30 13:04:54.937685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py
--rw-r--r--   0        0        0      908 2023-06-30 13:04:54.937685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-06-30 13:04:54.937685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py
--rw-r--r--   0        0        0      863 2023-06-30 13:04:54.937685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_create.py
--rw-r--r--   0        0        0      810 2023-06-30 13:04:54.941685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_destroy.py
--rw-r--r--   0        0        0      830 2023-06-30 13:04:54.937685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_retrieve.py
--rw-r--r--   0        0        0      885 2023-06-30 13:04:54.941685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py
--rw-r--r--   0        0        0      917 2023-06-30 13:04:54.941685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_update.py
--rw-r--r--   0        0        0     1258 2023-06-30 13:04:54.941685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_create.py
--rw-r--r--   0        0        0      813 2023-06-30 13:04:54.945685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_destroy.py
--rw-r--r--   0        0        0     1222 2023-06-30 13:04:54.941685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_retrieve.py
--rw-r--r--   0        0        0     1277 2023-06-30 13:04:54.941685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py
--rw-r--r--   0        0        0     1312 2023-06-30 13:04:54.945685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_update.py
--rw-r--r--   0        0        0      899 2023-06-30 13:04:54.945685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_create.py
--rw-r--r--   0        0        0      817 2023-06-30 13:04:54.945685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py
--rw-r--r--   0        0        0      859 2023-06-30 13:04:54.945685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-06-30 13:04:54.945685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-06-30 13:04:54.945685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_update.py
--rw-r--r--   0        0        0      935 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_create.py
--rw-r--r--   0        0        0      813 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_destroy.py
--rw-r--r--   0        0        0      899 2023-06-30 13:04:54.945685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py
--rw-r--r--   0        0        0      954 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_update.py
--rw-r--r--   0        0        0      876 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_create.py
--rw-r--r--   0        0        0      813 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_destroy.py
--rw-r--r--   0        0        0      840 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_retrieve.py
--rw-r--r--   0        0        0      895 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py
--rw-r--r--   0        0        0      930 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_update.py
--rw-r--r--   0        0        0      881 2023-06-30 13:04:54.953685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_create.py
--rw-r--r--   0        0        0      814 2023-06-30 13:04:54.953685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_destroy.py
--rw-r--r--   0        0        0      844 2023-06-30 13:04:54.949685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py
--rw-r--r--   0        0        0      899 2023-06-30 13:04:54.953685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py
--rw-r--r--   0        0        0      935 2023-06-30 13:04:54.953685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_update.py
--rw-r--r--   0        0        0     1922 2023-06-30 13:04:54.961685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_create.py
--rw-r--r--   0        0        0     1941 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_destroy.py
--rw-r--r--   0        0        0     1883 2023-06-30 13:04:54.957685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py
--rw-r--r--   0        0        0     1938 2023-06-30 13:04:54.961685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py
--rw-r--r--   0        0        0     1976 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_update.py
--rw-r--r--   0        0        0      917 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py
--rw-r--r--   0        0        0      820 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py
--rw-r--r--   0        0        0      874 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py
--rw-r--r--   0        0        0      929 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py
--rw-r--r--   0        0        0      935 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py
--rw-r--r--   0        0        0      823 2023-06-30 13:04:54.969685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py
--rw-r--r--   0        0        0      889 2023-06-30 13:04:54.965685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
--rw-r--r--   0        0        0      944 2023-06-30 13:04:54.969685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-06-30 13:04:54.969685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py
--rw-r--r--   0        0        0      923 2023-06-30 13:04:54.969685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py
--rw-r--r--   0        0        0      821 2023-06-30 13:04:54.969685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py
--rw-r--r--   0        0        0      879 2023-06-30 13:04:54.969685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py
--rw-r--r--   0        0        0      934 2023-06-30 13:04:54.969685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      977 2023-06-30 13:04:54.969685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py
--rw-r--r--   0        0        0     1627 2023-06-30 13:04:54.973685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py
--rw-r--r--   0        0        0      814 2023-06-30 13:04:54.977686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py
--rw-r--r--   0        0        0     1590 2023-06-30 13:04:54.973685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py
--rw-r--r--   0        0        0     1645 2023-06-30 13:04:54.973685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
--rw-r--r--   0        0        0     1681 2023-06-30 13:04:54.977686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py
--rw-r--r--   0        0        0      874 2023-06-30 13:04:54.977686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_create.py
--rw-r--r--   0        0        0      812 2023-06-30 13:04:54.977686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_destroy.py
--rw-r--r--   0        0        0      839 2023-06-30 13:04:54.977686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_retrieve.py
--rw-r--r--   0        0        0      894 2023-06-30 13:04:54.977686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py
--rw-r--r--   0        0        0      928 2023-06-30 13:04:54.977686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_update.py
--rw-r--r--   0        0        0      988 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_create.py
--rw-r--r--   0        0        0      812 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_destroy.py
--rw-r--r--   0        0        0      953 2023-06-30 13:04:54.977686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py
--rw-r--r--   0        0        0     1008 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py
--rw-r--r--   0        0        0     1042 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_update.py
--rw-r--r--   0        0        0      966 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
--rw-r--r--   0        0        0      827 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      916 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      971 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0     1020 2023-06-30 13:04:54.981685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
--rw-r--r--   0        0        0      896 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py
--rw-r--r--   0        0        0      820 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py
--rw-r--r--   0        0        0      890 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
--rw-r--r--   0        0        0      945 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py
--rw-r--r--   0        0        0      851 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_create.py
--rw-r--r--   0        0        0      811 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_destroy.py
--rw-r--r--   0        0        0      817 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py
--rw-r--r--   0        0        0      872 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py
--rw-r--r--   0        0        0      905 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_update.py
--rw-r--r--   0        0        0      856 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_create.py
--rw-r--r--   0        0        0      812 2023-06-30 13:04:54.989686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_destroy.py
--rw-r--r--   0        0        0      821 2023-06-30 13:04:54.985685 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_retrieve.py
--rw-r--r--   0        0        0      876 2023-06-30 13:04:54.989686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py
--rw-r--r--   0        0        0      910 2023-06-30 13:04:54.989686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_update.py
--rw-r--r--   0        0        0      886 2023-06-30 13:04:54.989686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py
--rw-r--r--   0        0        0      818 2023-06-30 13:04:54.989686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py
--rw-r--r--   0        0        0      845 2023-06-30 13:04:54.989686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
--rw-r--r--   0        0        0      900 2023-06-30 13:04:54.989686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      940 2023-06-30 13:04:54.989686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py
--rw-r--r--   0        0        0     2046 2023-06-30 13:04:54.993686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_create.py
--rw-r--r--   0        0        0     2068 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py
--rw-r--r--   0        0        0     3236 2023-06-30 13:04:54.993686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_list.py
--rw-r--r--   0        0        0     2065 2023-06-30 13:04:54.997686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py
--rw-r--r--   0        0        0     2100 2023-06-30 13:04:54.997686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_update.py
--rw-r--r--   0        0        0      899 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py
--rw-r--r--   0        0        0      817 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py
--rw-r--r--   0        0        0      859 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py
--rw-r--r--   0        0        0      917 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py
--rw-r--r--   0        0        0      820 2023-06-30 13:04:55.005686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py
--rw-r--r--   0        0        0      874 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
--rw-r--r--   0        0        0      929 2023-06-30 13:04:55.001686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-06-30 13:04:55.005686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py
--rw-r--r--   0        0        0      905 2023-06-30 13:04:55.005686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py
--rw-r--r--   0        0        0      818 2023-06-30 13:04:55.005686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py
--rw-r--r--   0        0        0      864 2023-06-30 13:04:55.005686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
--rw-r--r--   0        0        0      919 2023-06-30 13:04:55.005686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      959 2023-06-30 13:04:55.005686 feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py
--rw-r--r--   0        0        0      658 2023-06-30 13:04:55.009686 feedancy-0.0.2/feedancy/feedancy/client.py
--rw-r--r--   0        0        0     1000 2023-06-30 13:04:55.017686 feedancy-0.0.2/feedancy/setup.py
--rw-r--r--   0        0        0      937 2023-06-30 13:05:07.181779 feedancy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 feedancy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-06-05 13:45:57.561946 feedancy-0.0.3/README.md
+-rw-r--r--   0        0        0      203 2023-06-30 13:04:55.017686 feedancy-0.0.3/feedancy/MANIFEST.in
+-rw-r--r--   0        0        0      615 2023-06-30 13:04:55.013686 feedancy-0.0.3/feedancy/README.md
+-rw-r--r--   0        0        0      126 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:04:54.917685 feedancy-0.0.3/feedancy/feedancy/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:04:54.917685 feedancy-0.0.3/feedancy/feedancy/apis/api/__init__.py
+-rw-r--r--   0        0        0    13072 2023-06-30 13:04:54.921685 feedancy-0.0.3/feedancy/feedancy/apis/api/api.py
+-rw-r--r--   0        0        0      896 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py
+-rw-r--r--   0        0        0      853 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py
+-rw-r--r--   0        0        0      908 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
+-rw-r--r--   0        0        0      950 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py
+-rw-r--r--   0        0        0      863 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_create.py
+-rw-r--r--   0        0        0      810 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_destroy.py
+-rw-r--r--   0        0        0      830 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_retrieve.py
+-rw-r--r--   0        0        0      885 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py
+-rw-r--r--   0        0        0      917 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_update.py
+-rw-r--r--   0        0        0     1258 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_destroy.py
+-rw-r--r--   0        0        0     1222 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_retrieve.py
+-rw-r--r--   0        0        0     1277 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py
+-rw-r--r--   0        0        0     1312 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_update.py
+-rw-r--r--   0        0        0      899 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_create.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py
+-rw-r--r--   0        0        0      859 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py
+-rw-r--r--   0        0        0      914 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py
+-rw-r--r--   0        0        0      953 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_update.py
+-rw-r--r--   0        0        0      935 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_destroy.py
+-rw-r--r--   0        0        0      899 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py
+-rw-r--r--   0        0        0      954 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py
+-rw-r--r--   0        0        0      989 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_update.py
+-rw-r--r--   0        0        0      876 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_destroy.py
+-rw-r--r--   0        0        0      840 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_retrieve.py
+-rw-r--r--   0        0        0      895 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py
+-rw-r--r--   0        0        0      930 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_update.py
+-rw-r--r--   0        0        0      881 2023-06-30 13:04:54.953685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_create.py
+-rw-r--r--   0        0        0      814 2023-06-30 13:04:54.953685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_destroy.py
+-rw-r--r--   0        0        0      844 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py
+-rw-r--r--   0        0        0      899 2023-06-30 13:04:54.953685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py
+-rw-r--r--   0        0        0      935 2023-06-30 13:04:54.953685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_update.py
+-rw-r--r--   0        0        0     1922 2023-06-30 13:04:54.961685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_create.py
+-rw-r--r--   0        0        0     1941 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_destroy.py
+-rw-r--r--   0        0        0     1883 2023-06-30 13:04:54.957685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py
+-rw-r--r--   0        0        0     1938 2023-06-30 13:04:54.961685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py
+-rw-r--r--   0        0        0     1976 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_update.py
+-rw-r--r--   0        0        0      917 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py
+-rw-r--r--   0        0        0      874 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py
+-rw-r--r--   0        0        0      929 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
+-rw-r--r--   0        0        0      971 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py
+-rw-r--r--   0        0        0      935 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py
+-rw-r--r--   0        0        0      823 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py
+-rw-r--r--   0        0        0      889 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
+-rw-r--r--   0        0        0      944 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
+-rw-r--r--   0        0        0      989 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py
+-rw-r--r--   0        0        0      923 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py
+-rw-r--r--   0        0        0      821 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py
+-rw-r--r--   0        0        0      879 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py
+-rw-r--r--   0        0        0      934 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
+-rw-r--r--   0        0        0      977 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py
+-rw-r--r--   0        0        0     1627 2023-06-30 13:04:54.973685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py
+-rw-r--r--   0        0        0      814 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py
+-rw-r--r--   0        0        0     1590 2023-06-30 13:04:54.973685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py
+-rw-r--r--   0        0        0     1645 2023-06-30 13:04:54.973685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
+-rw-r--r--   0        0        0     1681 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py
+-rw-r--r--   0        0        0      874 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_destroy.py
+-rw-r--r--   0        0        0      839 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_retrieve.py
+-rw-r--r--   0        0        0      894 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py
+-rw-r--r--   0        0        0      928 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_update.py
+-rw-r--r--   0        0        0      988 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_destroy.py
+-rw-r--r--   0        0        0      953 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py
+-rw-r--r--   0        0        0     1008 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py
+-rw-r--r--   0        0        0     1042 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_update.py
+-rw-r--r--   0        0        0      966 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
+-rw-r--r--   0        0        0      827 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
+-rw-r--r--   0        0        0      916 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
+-rw-r--r--   0        0        0      971 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0     1020 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
+-rw-r--r--   0        0        0      896 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py
+-rw-r--r--   0        0        0      890 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
+-rw-r--r--   0        0        0      945 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      950 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py
+-rw-r--r--   0        0        0      851 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_create.py
+-rw-r--r--   0        0        0      811 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_destroy.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py
+-rw-r--r--   0        0        0      872 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py
+-rw-r--r--   0        0        0      905 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_update.py
+-rw-r--r--   0        0        0      856 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_destroy.py
+-rw-r--r--   0        0        0      821 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_retrieve.py
+-rw-r--r--   0        0        0      876 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py
+-rw-r--r--   0        0        0      910 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_update.py
+-rw-r--r--   0        0        0      886 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py
+-rw-r--r--   0        0        0      818 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py
+-rw-r--r--   0        0        0      845 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
+-rw-r--r--   0        0        0      900 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      940 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py
+-rw-r--r--   0        0        0     2046 2023-06-30 13:04:54.993686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_create.py
+-rw-r--r--   0        0        0     2068 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py
+-rw-r--r--   0        0        0     3236 2023-06-30 13:04:54.993686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_list.py
+-rw-r--r--   0        0        0     2065 2023-06-30 13:04:54.997686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py
+-rw-r--r--   0        0        0     2100 2023-06-30 13:04:54.997686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_update.py
+-rw-r--r--   0        0        0      899 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py
+-rw-r--r--   0        0        0      859 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py
+-rw-r--r--   0        0        0      914 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
+-rw-r--r--   0        0        0      953 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py
+-rw-r--r--   0        0        0      917 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py
+-rw-r--r--   0        0        0      874 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
+-rw-r--r--   0        0        0      929 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
+-rw-r--r--   0        0        0      971 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py
+-rw-r--r--   0        0        0      905 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py
+-rw-r--r--   0        0        0      818 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py
+-rw-r--r--   0        0        0      864 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
+-rw-r--r--   0        0        0      919 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
+-rw-r--r--   0        0        0      959 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py
+-rw-r--r--   0        0        0      658 2023-06-30 13:04:55.009686 feedancy-0.0.3/feedancy/feedancy/client.py
+-rw-r--r--   0        0        0     1000 2023-06-30 13:04:55.017686 feedancy-0.0.3/feedancy/setup.py
+-rw-r--r--   0        0        0      936 2023-06-30 13:12:14.929610 feedancy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 feedancy-0.0.3/PKG-INFO
```

### Comparing `feedancy-0.0.2/feedancy/README.md` & `feedancy-0.0.3/feedancy/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_city_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_company_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_companycity_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_contact_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_country_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_currency_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internship_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_region_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_salary_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_skill_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_source_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_list.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_list.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancy_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py` & `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/feedancy/client.py` & `feedancy-0.0.3/feedancy/feedancy/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/feedancy/setup.py` & `feedancy-0.0.3/feedancy/setup.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.2/pyproject.toml` & `feedancy-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,26 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy"
-version = "0.0.2"
+version = "0.0.3"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.8"
 djangorestframework = ">=3.14.0"
 Django = ">=4"
 gunicorn = ">=20.1.0"
 psycopg2-binary = ">=2.9.6"
 Pillow = ">=9.5.0"
 django-filter = ">=23.2"
 pydantic = ">=1.10.8"
```

### Comparing `feedancy-0.0.2/PKG-INFO` & `feedancy-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.0.2
+Version: 0.0.3
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=4)
 Requires-Dist: Pillow (>=9.5.0)
 Requires-Dist: bs4 (>=0.0.1)
 Requires-Dist: django-filter (>=23.2)
 Requires-Dist: djangorestframework (>=3.14.0)
```

