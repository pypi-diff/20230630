# Comparing `tmp/feedancy-0.0.3.tar.gz` & `tmp/feedancy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.3.tar", max compression
+gzip compressed data, was "feedancy-0.0.4.tar", max compression
```

## Comparing `feedancy-0.0.3.tar` & `feedancy-0.0.4.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0       37 2023-06-05 13:45:57.561946 feedancy-0.0.3/README.md
--rw-r--r--   0        0        0      203 2023-06-30 13:04:55.017686 feedancy-0.0.3/feedancy/MANIFEST.in
--rw-r--r--   0        0        0      615 2023-06-30 13:04:55.013686 feedancy-0.0.3/feedancy/README.md
--rw-r--r--   0        0        0      126 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 13:04:54.917685 feedancy-0.0.3/feedancy/feedancy/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 13:04:54.917685 feedancy-0.0.3/feedancy/feedancy/apis/api/__init__.py
--rw-r--r--   0        0        0    13072 2023-06-30 13:04:54.921685 feedancy-0.0.3/feedancy/feedancy/apis/api/api.py
--rw-r--r--   0        0        0      896 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py
--rw-r--r--   0        0        0      820 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py
--rw-r--r--   0        0        0      853 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py
--rw-r--r--   0        0        0      908 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py
--rw-r--r--   0        0        0      863 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_create.py
--rw-r--r--   0        0        0      810 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_destroy.py
--rw-r--r--   0        0        0      830 2023-06-30 13:04:54.937685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_retrieve.py
--rw-r--r--   0        0        0      885 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py
--rw-r--r--   0        0        0      917 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_update.py
--rw-r--r--   0        0        0     1258 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_create.py
--rw-r--r--   0        0        0      813 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_destroy.py
--rw-r--r--   0        0        0     1222 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_retrieve.py
--rw-r--r--   0        0        0     1277 2023-06-30 13:04:54.941685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py
--rw-r--r--   0        0        0     1312 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_update.py
--rw-r--r--   0        0        0      899 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_create.py
--rw-r--r--   0        0        0      817 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py
--rw-r--r--   0        0        0      859 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_update.py
--rw-r--r--   0        0        0      935 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_create.py
--rw-r--r--   0        0        0      813 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_destroy.py
--rw-r--r--   0        0        0      899 2023-06-30 13:04:54.945685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py
--rw-r--r--   0        0        0      954 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_update.py
--rw-r--r--   0        0        0      876 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_create.py
--rw-r--r--   0        0        0      813 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_destroy.py
--rw-r--r--   0        0        0      840 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_retrieve.py
--rw-r--r--   0        0        0      895 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py
--rw-r--r--   0        0        0      930 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_update.py
--rw-r--r--   0        0        0      881 2023-06-30 13:04:54.953685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_create.py
--rw-r--r--   0        0        0      814 2023-06-30 13:04:54.953685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_destroy.py
--rw-r--r--   0        0        0      844 2023-06-30 13:04:54.949685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py
--rw-r--r--   0        0        0      899 2023-06-30 13:04:54.953685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py
--rw-r--r--   0        0        0      935 2023-06-30 13:04:54.953685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_update.py
--rw-r--r--   0        0        0     1922 2023-06-30 13:04:54.961685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_create.py
--rw-r--r--   0        0        0     1941 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_destroy.py
--rw-r--r--   0        0        0     1883 2023-06-30 13:04:54.957685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py
--rw-r--r--   0        0        0     1938 2023-06-30 13:04:54.961685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py
--rw-r--r--   0        0        0     1976 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_update.py
--rw-r--r--   0        0        0      917 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py
--rw-r--r--   0        0        0      820 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py
--rw-r--r--   0        0        0      874 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py
--rw-r--r--   0        0        0      929 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py
--rw-r--r--   0        0        0      935 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py
--rw-r--r--   0        0        0      823 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py
--rw-r--r--   0        0        0      889 2023-06-30 13:04:54.965685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
--rw-r--r--   0        0        0      944 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
--rw-r--r--   0        0        0      989 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py
--rw-r--r--   0        0        0      923 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py
--rw-r--r--   0        0        0      821 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py
--rw-r--r--   0        0        0      879 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py
--rw-r--r--   0        0        0      934 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
--rw-r--r--   0        0        0      977 2023-06-30 13:04:54.969685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py
--rw-r--r--   0        0        0     1627 2023-06-30 13:04:54.973685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py
--rw-r--r--   0        0        0      814 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py
--rw-r--r--   0        0        0     1590 2023-06-30 13:04:54.973685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py
--rw-r--r--   0        0        0     1645 2023-06-30 13:04:54.973685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
--rw-r--r--   0        0        0     1681 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py
--rw-r--r--   0        0        0      874 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_create.py
--rw-r--r--   0        0        0      812 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_destroy.py
--rw-r--r--   0        0        0      839 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_retrieve.py
--rw-r--r--   0        0        0      894 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py
--rw-r--r--   0        0        0      928 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_update.py
--rw-r--r--   0        0        0      988 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_create.py
--rw-r--r--   0        0        0      812 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_destroy.py
--rw-r--r--   0        0        0      953 2023-06-30 13:04:54.977686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py
--rw-r--r--   0        0        0     1008 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py
--rw-r--r--   0        0        0     1042 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_update.py
--rw-r--r--   0        0        0      966 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
--rw-r--r--   0        0        0      827 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
--rw-r--r--   0        0        0      916 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
--rw-r--r--   0        0        0      971 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
--rw-r--r--   0        0        0     1020 2023-06-30 13:04:54.981685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
--rw-r--r--   0        0        0      896 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py
--rw-r--r--   0        0        0      820 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py
--rw-r--r--   0        0        0      890 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
--rw-r--r--   0        0        0      945 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
--rw-r--r--   0        0        0      950 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py
--rw-r--r--   0        0        0      851 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_create.py
--rw-r--r--   0        0        0      811 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_destroy.py
--rw-r--r--   0        0        0      817 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py
--rw-r--r--   0        0        0      872 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py
--rw-r--r--   0        0        0      905 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_update.py
--rw-r--r--   0        0        0      856 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_create.py
--rw-r--r--   0        0        0      812 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_destroy.py
--rw-r--r--   0        0        0      821 2023-06-30 13:04:54.985685 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_retrieve.py
--rw-r--r--   0        0        0      876 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py
--rw-r--r--   0        0        0      910 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_update.py
--rw-r--r--   0        0        0      886 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py
--rw-r--r--   0        0        0      818 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py
--rw-r--r--   0        0        0      845 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
--rw-r--r--   0        0        0      900 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
--rw-r--r--   0        0        0      940 2023-06-30 13:04:54.989686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py
--rw-r--r--   0        0        0     2046 2023-06-30 13:04:54.993686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_create.py
--rw-r--r--   0        0        0     2068 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py
--rw-r--r--   0        0        0     3236 2023-06-30 13:04:54.993686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_list.py
--rw-r--r--   0        0        0     2065 2023-06-30 13:04:54.997686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py
--rw-r--r--   0        0        0     2100 2023-06-30 13:04:54.997686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancy_update.py
--rw-r--r--   0        0        0      899 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py
--rw-r--r--   0        0        0      817 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py
--rw-r--r--   0        0        0      859 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py
--rw-r--r--   0        0        0      914 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
--rw-r--r--   0        0        0      953 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py
--rw-r--r--   0        0        0      917 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py
--rw-r--r--   0        0        0      820 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py
--rw-r--r--   0        0        0      874 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
--rw-r--r--   0        0        0      929 2023-06-30 13:04:55.001686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
--rw-r--r--   0        0        0      971 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py
--rw-r--r--   0        0        0      905 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py
--rw-r--r--   0        0        0      818 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py
--rw-r--r--   0        0        0      864 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
--rw-r--r--   0        0        0      919 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
--rw-r--r--   0        0        0      959 2023-06-30 13:04:55.005686 feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py
--rw-r--r--   0        0        0      658 2023-06-30 13:04:55.009686 feedancy-0.0.3/feedancy/feedancy/client.py
--rw-r--r--   0        0        0     1000 2023-06-30 13:04:55.017686 feedancy-0.0.3/feedancy/setup.py
--rw-r--r--   0        0        0      936 2023-06-30 13:12:14.929610 feedancy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 feedancy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-06-05 13:45:57.561946 feedancy-0.0.4/README.md
+-rw-r--r--   0        0        0      203 2023-06-30 13:29:02.155745 feedancy-0.0.4/feedancy/MANIFEST.in
+-rw-r--r--   0        0        0      615 2023-06-30 13:29:02.151745 feedancy-0.0.4/feedancy/README.md
+-rw-r--r--   0        0        0      126 2023-06-30 13:29:02.143744 feedancy-0.0.4/feedancy/feedancy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:29:02.091741 feedancy-0.0.4/feedancy/feedancy/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:29:02.091741 feedancy-0.0.4/feedancy/feedancy/apis/api/__init__.py
+-rw-r--r--   0        0        0    13072 2023-06-30 13:29:02.095742 feedancy-0.0.4/feedancy/feedancy/apis/api/api.py
+-rw-r--r--   0        0        0      763 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py
+-rw-r--r--   0        0        0      762 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py
+-rw-r--r--   0        0        0      753 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_create.py
+-rw-r--r--   0        0        0      810 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_destroy.py
+-rw-r--r--   0        0        0      752 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_retrieve.py
+-rw-r--r--   0        0        0      807 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py
+-rw-r--r--   0        0        0      807 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_update.py
+-rw-r--r--   0        0        0      756 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_destroy.py
+-rw-r--r--   0        0        0      755 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_retrieve.py
+-rw-r--r--   0        0        0      810 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py
+-rw-r--r--   0        0        0      810 2023-06-30 13:29:02.107742 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_update.py
+-rw-r--r--   0        0        0      760 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_create.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py
+-rw-r--r--   0        0        0      759 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py
+-rw-r--r--   0        0        0      814 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py
+-rw-r--r--   0        0        0      814 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_update.py
+-rw-r--r--   0        0        0      756 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_contact_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_contact_destroy.py
+-rw-r--r--   0        0        0      755 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py
+-rw-r--r--   0        0        0      810 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py
+-rw-r--r--   0        0        0      810 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_contact_update.py
+-rw-r--r--   0        0        0      756 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_create.py
+-rw-r--r--   0        0        0      813 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_destroy.py
+-rw-r--r--   0        0        0      755 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_retrieve.py
+-rw-r--r--   0        0        0      810 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py
+-rw-r--r--   0        0        0      810 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_update.py
+-rw-r--r--   0        0        0      757 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_create.py
+-rw-r--r--   0        0        0      814 2023-06-30 13:29:02.115743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_destroy.py
+-rw-r--r--   0        0        0      756 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py
+-rw-r--r--   0        0        0      811 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py
+-rw-r--r--   0        0        0      811 2023-06-30 13:29:02.111743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_update.py
+-rw-r--r--   0        0        0      759 2023-06-30 13:29:02.115743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_create.py
+-rw-r--r--   0        0        0     1941 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_destroy.py
+-rw-r--r--   0        0        0      758 2023-06-30 13:29:02.115743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py
+-rw-r--r--   0        0        0     1938 2023-06-30 13:29:02.115743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py
+-rw-r--r--   0        0        0     1976 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_update.py
+-rw-r--r--   0        0        0      763 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py
+-rw-r--r--   0        0        0      762 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py
+-rw-r--r--   0        0        0      766 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py
+-rw-r--r--   0        0        0      823 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py
+-rw-r--r--   0        0        0      765 2023-06-30 13:29:02.119743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py
+-rw-r--r--   0        0        0      764 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py
+-rw-r--r--   0        0        0      821 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py
+-rw-r--r--   0        0        0      763 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py
+-rw-r--r--   0        0        0      818 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py
+-rw-r--r--   0        0        0      818 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py
+-rw-r--r--   0        0        0      757 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py
+-rw-r--r--   0        0        0      814 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py
+-rw-r--r--   0        0        0      756 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve.py
+-rw-r--r--   0        0        0      811 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py
+-rw-r--r--   0        0        0      811 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py
+-rw-r--r--   0        0        0      755 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_region_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_region_destroy.py
+-rw-r--r--   0        0        0      754 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_region_retrieve.py
+-rw-r--r--   0        0        0      809 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py
+-rw-r--r--   0        0        0      809 2023-06-30 13:29:02.123743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_region_update.py
+-rw-r--r--   0        0        0      755 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_destroy.py
+-rw-r--r--   0        0        0      754 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py
+-rw-r--r--   0        0        0      809 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py
+-rw-r--r--   0        0        0      809 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_update.py
+-rw-r--r--   0        0        0      770 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py
+-rw-r--r--   0        0        0      827 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py
+-rw-r--r--   0        0        0      769 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py
+-rw-r--r--   0        0        0      824 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      824 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py
+-rw-r--r--   0        0        0      763 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py
+-rw-r--r--   0        0        0      762 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py
+-rw-r--r--   0        0        0      754 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_create.py
+-rw-r--r--   0        0        0      811 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_destroy.py
+-rw-r--r--   0        0        0      753 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py
+-rw-r--r--   0        0        0      808 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py
+-rw-r--r--   0        0        0      808 2023-06-30 13:29:02.127743 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_update.py
+-rw-r--r--   0        0        0      755 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_source_create.py
+-rw-r--r--   0        0        0      812 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_source_destroy.py
+-rw-r--r--   0        0        0      754 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_source_retrieve.py
+-rw-r--r--   0        0        0      809 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py
+-rw-r--r--   0        0        0      809 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_source_update.py
+-rw-r--r--   0        0        0      761 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py
+-rw-r--r--   0        0        0      818 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py
+-rw-r--r--   0        0        0      760 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py
+-rw-r--r--   0        0        0      815 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py
+-rw-r--r--   0        0        0      815 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py
+-rw-r--r--   0        0        0     2046 2023-06-30 13:29:02.135744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_create.py
+-rw-r--r--   0        0        0     2068 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py
+-rw-r--r--   0        0        0     3236 2023-06-30 13:29:02.131744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_list.py
+-rw-r--r--   0        0        0     2065 2023-06-30 13:29:02.135744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py
+-rw-r--r--   0        0        0     2100 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_update.py
+-rw-r--r--   0        0        0      760 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py
+-rw-r--r--   0        0        0      759 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py
+-rw-r--r--   0        0        0      814 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py
+-rw-r--r--   0        0        0      814 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py
+-rw-r--r--   0        0        0      763 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py
+-rw-r--r--   0        0        0      820 2023-06-30 13:29:02.143744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py
+-rw-r--r--   0        0        0      762 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py
+-rw-r--r--   0        0        0      817 2023-06-30 13:29:02.139744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py
+-rw-r--r--   0        0        0      761 2023-06-30 13:29:02.143744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py
+-rw-r--r--   0        0        0      818 2023-06-30 13:29:02.143744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py
+-rw-r--r--   0        0        0      760 2023-06-30 13:29:02.143744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py
+-rw-r--r--   0        0        0      815 2023-06-30 13:29:02.143744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve_2.py
+-rw-r--r--   0        0        0      815 2023-06-30 13:29:02.143744 feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py
+-rw-r--r--   0        0        0      658 2023-06-30 13:29:02.147745 feedancy-0.0.4/feedancy/feedancy/client.py
+-rw-r--r--   0        0        0     1000 2023-06-30 13:29:02.151745 feedancy-0.0.4/feedancy/setup.py
+-rw-r--r--   0        0        0      936 2023-06-30 13:28:36.882275 feedancy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 feedancy-0.0.4/PKG-INFO
```

### Comparing `feedancy-0.0.3/feedancy/README.md` & `feedancy-0.0.4/feedancy/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_region_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,45 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class ActivitySphere(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: ActivitySphere,
 
+    id: str,
 
-) -> ActivitySphere:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/activitysphere/".format(
+        method="PUT",
+        path="/api/v1/region/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": ActivitySphere,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,31 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class ActivitySphere(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> ActivitySphere:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/activitysphere/".format(
+        method="POST",
+        path="/api/v1/country/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": ActivitySphere,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,35 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class ActivitySphere(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> ActivitySphere:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/activitysphere/{id}/".format(
-            
-                id=id,
+        path="/api/v1/internship/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -41,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": ActivitySphere,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,49 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class ActivitySphere(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: ActivitySphere,
-
 
     id: str,
 
-) -> ActivitySphere:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/activitysphere/{id}/".format(
+        path="/api/v1/skill/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": ActivitySphere,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_create.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class City(BaseModel):
-    name: str 
-    region: int 
-
 def make_request(self: BaseApi,
 
-    __request__: City,
-
 
-) -> City:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/api/v1/city/".format(
+        path="/api/v1/skill/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class City(BaseModel):
-    id: int 
-    name: str 
-    region: int 
-
 def make_request(self: BaseApi,
 
 
-) -> City:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/city/".format(
+        method="POST",
+        path="/api/v1/internshipcity/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_retrieve_2.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,25 +5,20 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class City(BaseModel):
-    id: int 
-    name: str 
-    region: int 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> City:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_city_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class City(BaseModel):
-    name: str 
-    region: int 
-
 def make_request(self: BaseApi,
 
-    __request__: City,
-
 
     id: str,
 
-) -> City:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/city/{id}/".format(
+        path="/api/v1/internshipcontact/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": City,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_update.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,38 +5,53 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Company(BaseModel):
-    description: typing.Optional[typing.Union[str, None]]  = None
-    is_accredited: typing.Optional[typing.Union[bool, None]]  = None
-    link: typing.Optional[typing.Union[str, None]]  = None
-    logo: typing.Optional[typing.Union[str, None]]  = None
+class Internship(BaseModel):
+    company: typing.Optional[typing.Union[int, None]]  = None
+    duration: typing.Optional[typing.Union[int, None]]  = None
+    external_id: str 
+    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
+    has_test_task: typing.Optional[typing.Union[bool, None]]  = None
+    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    link: str 
     name: str 
-    size: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
-    sphere: typing.Optional[typing.Union[int, None]]  = None
+    publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    raw_description: typing.Optional[typing.Union[str, None]]  = None
+    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    requirement: typing.Optional[typing.Union[str, None]]  = None
+    responsibility: typing.Optional[typing.Union[str, None]]  = None
+    salary: typing.Optional[typing.Union[int, None]]  = None
+    source: int 
+    test_task_link: typing.Optional[typing.Union[str, None]]  = None
+    work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
-    __request__: Company,
+    __request__: Internship,
 
 
-) -> Company:
+    id: str,
+
+) -> Internship:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/company/".format(
+        method="PUT",
+        path="/api/v1/internship/{id}/".format(
+            
+                id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -44,12 +59,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Company,
+                "application/json": Internship,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_create.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,54 +5,63 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Company(BaseModel):
-    description: typing.Optional[typing.Union[str, None]]  = None
-    id: int 
-    is_accredited: typing.Optional[typing.Union[bool, None]]  = None
-    link: typing.Optional[typing.Union[str, None]]  = None
-    logo: typing.Optional[typing.Union[str, None]]  = None
+class Vacancy(BaseModel):
+    company: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    external_id: str 
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
+    has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
+    has_test_task: typing.Optional[typing.Union[bool, None]]  = None
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
+    link: str 
     name: str 
-    size: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
-    sphere: typing.Optional[typing.Union[int, None]]  = None
+    publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
+    raw_description: typing.Optional[typing.Union[str, None]]  = None
+    requirement: typing.Optional[typing.Union[str, None]]  = None
+    responsibility: typing.Optional[typing.Union[str, None]]  = None
+    salary: typing.Optional[typing.Union[int, None]]  = None
+    source: int 
+    test_task_link: typing.Optional[typing.Union[str, None]]  = None
+    work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
+    __request__: Vacancy,
 
-    id: str,
 
-) -> Company:
+) -> Vacancy:
     
 
     
-    body = None
+    body = __request__
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/company/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/vacancy/".format(
             
         ),
-        content_type=None,
+        content_type="application/json",
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Company,
+                "application/json": Vacancy,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class CompanyCity(BaseModel):
-    city: int 
-    company: int 
-
 def make_request(self: BaseApi,
 
-    __request__: CompanyCity,
-
 
-) -> CompanyCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/companycity/".format(
+        method="GET",
+        path="/api/v1/activitysphere/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": CompanyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_retrieve.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,18 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class CompanyCity(BaseModel):
-    city: int 
-    company: int 
-    id: int 
-
 def make_request(self: BaseApi,
 
 
-) -> CompanyCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": CompanyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class CompanyCity(BaseModel):
-    city: int 
-    company: int 
-    id: int 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> CompanyCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/companycity/{id}/".format(
+        method="PUT",
+        path="/api/v1/country/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": CompanyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_companycity_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,50 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class CompanyCity(BaseModel):
-    city: int 
-    company: int 
-
 def make_request(self: BaseApi,
 
-    __request__: CompanyCity,
-
 
-    id: str,
-
-) -> CompanyCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/companycity/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/activitysphere/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": CompanyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,47 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Contact(BaseModel):
-    data: str 
-    name: typing.Optional[typing.Union[str, None]]  = None
-    type: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Contact,
 
+    id: str,
 
-) -> Contact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/contact/".format(
+        method="DELETE",
+        path="/api/v1/vacancycity/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "200": {
+        "204": {
             
-                "application/json": Contact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_contact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Contact(BaseModel):
-    data: str 
-    id: int 
-    name: typing.Optional[typing.Union[str, None]]  = None
-    type: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Contact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/contact/".format(
+        method="POST",
+        path="/api/v1/searchkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -39,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Contact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_retrieve_2.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,35 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Contact(BaseModel):
-    data: str 
-    id: int 
-    name: typing.Optional[typing.Union[str, None]]  = None
-    type: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Contact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/contact/{id}/".format(
+        path="/api/v1/company/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -43,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Contact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_contact_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,51 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Contact(BaseModel):
-    data: str 
-    name: typing.Optional[typing.Union[str, None]]  = None
-    type: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Contact,
-
 
     id: str,
 
-) -> Contact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/contact/{id}/".format(
+        path="/api/v1/vacancycity/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Contact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_source_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Country(BaseModel):
-    code: str 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Country,
-
 
-) -> Country:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/api/v1/country/".format(
+        path="/api/v1/source/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,18 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Country(BaseModel):
-    code: str 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Country:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Country(BaseModel):
-    code: str 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> Country:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/country/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/jobmixin/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_country_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,50 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Country(BaseModel):
-    code: str 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Country,
-
 
-    id: str,
-
-) -> Country:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/country/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/vacancyskill/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Country,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_create.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Currency(BaseModel):
-    code: str 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Currency,
-
 
-) -> Currency:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/api/v1/currency/".format(
+        path="/api/v1/companycity/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Currency,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Currency(BaseModel):
-    code: str 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Currency:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/currency/".format(
+        method="POST",
+        path="/api/v1/internshipskill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Currency,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_create.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Currency(BaseModel):
-    code: str 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> Currency:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/currency/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/city/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Currency,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_currency_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_create.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,50 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Currency(BaseModel):
-    code: str 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Currency,
-
 
-    id: str,
-
-) -> Currency:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/currency/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/salary/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Currency,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class Internship(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
     duration: typing.Optional[typing.Union[int, None]]  = None
     external_id: str 
     has_employment: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
+    id: int 
     is_paid: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
     recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
@@ -27,30 +28,32 @@
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
-    __request__: Internship,
 
+    id: str,
 
 ) -> Internship:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/internship/".format(
+        method="GET",
+        path="/api/v1/internship/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internship_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_retrieve.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,48 +5,53 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Internship(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
-    duration: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
-    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     id: int 
-    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
-    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
 
-) -> Internship:
+    id: str,
+
+) -> Vacancy:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/internship/".format(
+        path="/api/v1/vacancy/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -54,12 +59,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Internship,
+                "application/json": Vacancy,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_destroy.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,50 +5,51 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Internship(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
-    duration: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
-    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
     id: int 
-    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
-    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Internship:
+) -> Vacancy:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/internship/{id}/".format(
+        method="DELETE",
+        path="/api/v1/vacancy/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -58,12 +59,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Internship,
+                "application/json": Vacancy,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internship_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,51 +5,52 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Internship(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
-    duration: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
-    has_employment: typing.Optional[typing.Union[bool, None]]  = None
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
-    is_paid: typing.Optional[typing.Union[bool, None]]  = None
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
-    recruitment_end_date: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
 def make_request(self: BaseApi,
 
-    __request__: Internship,
+    __request__: Vacancy,
 
 
     id: str,
 
-) -> Internship:
+) -> Vacancy:
     
 
     
     body = __request__
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/internship/{id}/".format(
+        path="/api/v1/vacancy/{id}/".format(
             
                 id=id,
             
         ),
         content_type="application/json",
         body=body,
         headers=self._only_provided({
@@ -59,12 +60,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Internship,
+                "application/json": Vacancy,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipCity(BaseModel):
-    city: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipCity,
 
+    id: str,
 
-) -> InternshipCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/internshipcity/".format(
+        method="PUT",
+        path="/api/v1/searchkeywords/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipCity(BaseModel):
-    city: int 
-    id: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
 
-) -> InternshipCity:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/internshipcity/".format(
+        path="/api/v1/internshipskill/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipCity(BaseModel):
-    city: int 
-    id: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> InternshipCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/internshipcity/{id}/".format(
-            
-                id=id,
+        path="/api/v1/internshipskill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipCity(BaseModel):
-    city: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipCity,
-
 
     id: str,
 
-) -> InternshipCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
         path="/api/v1/internshipcity/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipContact(BaseModel):
-    contact: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipContact,
-
 
-) -> InternshipContact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
+        method="GET",
         path="/api/v1/internshipcontact/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_contact_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipContact(BaseModel):
-    contact: int 
-    id: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
 
-) -> InternshipContact:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/internshipcontact/".format(
+        method="PUT",
+        path="/api/v1/contact/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcontact_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipContact(BaseModel):
-    contact: int 
-    id: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> InternshipContact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/internshipcontact/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/internshipcontact/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipcontact_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipContact(BaseModel):
-    contact: int 
-    internship: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipContact,
-
 
     id: str,
 
-) -> InternshipContact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/internshipcontact/{id}/".format(
+        path="/api/v1/internshipskill/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_retrieve_2.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipSkill(BaseModel):
-    internship: int 
-    skill: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipSkill,
 
+    id: str,
 
-) -> InternshipSkill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/internshipskill/".format(
+        method="GET",
+        path="/api/v1/jobmixin/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipSkill(BaseModel):
-    id: int 
-    internship: int 
-    skill: int 
-
 def make_request(self: BaseApi,
 
 
-) -> InternshipSkill:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/internshipskill/".format(
+        method="PUT",
+        path="/api/v1/activitysphere/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipSkill(BaseModel):
-    id: int 
-    internship: int 
-    skill: int 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> InternshipSkill:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/internshipskill/{id}/".format(
+        path="/api/v1/skill/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_internshipskill_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class InternshipSkill(BaseModel):
-    internship: int 
-    skill: int 
-
 def make_request(self: BaseApi,
 
-    __request__: InternshipSkill,
-
 
     id: str,
 
-) -> InternshipSkill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/internshipskill/{id}/".format(
+        path="/api/v1/city/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": InternshipSkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancy_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,58 +5,108 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class JobMixin(BaseModel):
+class Vacancy(BaseModel):
     company: typing.Optional[typing.Union[int, None]]  = None
+    contract_type: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    employment_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
+    experience: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
     external_id: str 
+    has_insurance: typing.Optional[typing.Union[bool, None]]  = None
     has_portfolio: typing.Optional[typing.Union[bool, None]]  = None
     has_test_task: typing.Optional[typing.Union[bool, None]]  = None
+    id: int 
+    is_relocation_required: typing.Optional[typing.Union[bool, None]]  = None
     link: str 
     name: str 
     publicated_at: typing.Optional[typing.Union[datetime.datetime, None]]  = None
     raw_description: typing.Optional[typing.Union[str, None]]  = None
     requirement: typing.Optional[typing.Union[str, None]]  = None
     responsibility: typing.Optional[typing.Union[str, None]]  = None
     salary: typing.Optional[typing.Union[int, None]]  = None
     source: int 
     test_task_link: typing.Optional[typing.Union[str, None]]  = None
     work_format: typing.Optional[typing.Union[typing.Union[str, str, str], None]]  = None
 
+class PaginatedVacancyList(BaseModel):
+    count: typing.Optional[int]  = None
+    next: typing.Optional[typing.Union[str, None]]  = None
+    previous: typing.Optional[typing.Union[str, None]]  = None
+    results: typing.Optional[typing.List[Vacancy]]  = None
+
 def make_request(self: BaseApi,
 
-    __request__: JobMixin,
 
+    activity_sphere: str = ...,
+
+    company_size: str = ...,
+
+    employment_format: str = ...,
+
+    has_insurance: bool = ...,
+
+    is_accredited: bool = ...,
+
+    is_relocation_required: bool = ...,
+
+    page: int = ...,
+
+    relocation_is_required: bool = ...,
+
+    search: str = ...,
+
+    work_format: str = ...,
 
-) -> JobMixin:
+) -> PaginatedVacancyList:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/jobmixin/".format(
+        method="GET",
+        path="/api/v1/vacancy/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
+                "activity_sphere": activity_sphere,
+            
+                "company_size": company_size,
+            
+                "employment_format": employment_format,
+            
+                "has_insurance": has_insurance,
+            
+                "is_accredited": is_accredited,
+            
+                "is_relocation_required": is_relocation_required,
+            
+                "page": page,
+            
+                "relocation_is_required": relocation_is_required,
+            
+                "search": search,
+            
+                "work_format": work_format,
+            
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": JobMixin,
+                "application/json": PaginatedVacancyList,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Region(BaseModel):
-    country: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Region,
-
 
-) -> Region:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
-        path="/api/v1/region/".format(
+        path="/api/v1/currency/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_region_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_country_retrieve_2.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Region(BaseModel):
-    country: int 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Region:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/region/".format(
+        path="/api/v1/country/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_region_retrieve.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Region(BaseModel):
-    country: int 
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> Region:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/region/{id}/".format(
-            
-                id=id,
+        path="/api/v1/region/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_region_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,50 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Region(BaseModel):
-    country: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Region,
-
 
-    id: str,
-
-) -> Region:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/region/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/vacancycity/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Region,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,47 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Salary(BaseModel):
-    currency: int 
-    max_value: typing.Optional[typing.Union[int, None]]  = None
-    min_value: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
-    __request__: Salary,
 
+    id: str,
 
-) -> Salary:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/salary/".format(
+        method="PUT",
+        path="/api/v1/vacancycontact/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Salary,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve_2.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Salary(BaseModel):
-    currency: int 
-    id: int 
-    max_value: typing.Optional[typing.Union[int, None]]  = None
-    min_value: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
 
-) -> Salary:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/salary/".format(
+        path="/api/v1/internshipcity/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -39,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Salary,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,34 +5,28 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Salary(BaseModel):
-    currency: int 
-    id: int 
-    max_value: typing.Optional[typing.Union[int, None]]  = None
-    min_value: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Salary:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
+        method="PUT",
         path="/api/v1/salary/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
@@ -43,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Salary,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_salary_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,51 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Salary(BaseModel):
-    currency: int 
-    max_value: typing.Optional[typing.Union[int, None]]  = None
-    min_value: typing.Optional[typing.Union[int, None]]  = None
-
 def make_request(self: BaseApi,
 
-    __request__: Salary,
-
 
     id: str,
 
-) -> Salary:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/salary/{id}/".format(
+        path="/api/v1/vacancyskill/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Salary,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_internshipcity_retrieve.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class SearchAndStopKeywords(BaseModel):
-    search_keywords: int 
-    stop_keywords: int 
-
 def make_request(self: BaseApi,
 
-    __request__: SearchAndStopKeywords,
-
 
-) -> SearchAndStopKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/searchandstopkeywords/".format(
+        method="GET",
+        path="/api/v1/internshipcity/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchAndStopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class SearchAndStopKeywords(BaseModel):
-    id: int 
-    search_keywords: int 
-    stop_keywords: int 
-
 def make_request(self: BaseApi,
 
 
-) -> SearchAndStopKeywords:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/searchandstopkeywords/".format(
+        path="/api/v1/source/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchAndStopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_create.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class SearchAndStopKeywords(BaseModel):
-    id: int 
-    search_keywords: int 
-    stop_keywords: int 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> SearchAndStopKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/searchandstopkeywords/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/company/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchAndStopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,50 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class SearchAndStopKeywords(BaseModel):
-    search_keywords: int 
-    stop_keywords: int 
-
 def make_request(self: BaseApi,
 
-    __request__: SearchAndStopKeywords,
-
 
     id: str,
 
-) -> SearchAndStopKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="PUT",
-        path="/api/v1/searchandstopkeywords/{id}/".format(
+        path="/api/v1/stopkeywords/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchAndStopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,45 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class SearchKeywords(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: SearchKeywords,
-
 
-) -> SearchKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
+        method="GET",
         path="/api/v1/searchkeywords/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_activitysphere_retrieve_2.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class SearchKeywords(BaseModel):
-    id: int 
-    name: str 
-    stop_keywords: typing.List[int] 
-
 def make_request(self: BaseApi,
 
 
-) -> SearchKeywords:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/searchkeywords/".format(
+        path="/api/v1/activitysphere/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchkeywords_retrieve_2.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,20 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class SearchKeywords(BaseModel):
-    id: int 
-    name: str 
-    stop_keywords: typing.List[int] 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> SearchKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_searchkeywords_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_city_retrieve.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,49 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class SearchKeywords(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: SearchKeywords,
-
 
-    id: str,
-
-) -> SearchKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/searchkeywords/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/city/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": SearchKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_retrieve_2.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,45 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Skill(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Skill,
 
+    id: str,
 
-) -> Skill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/skill/".format(
+        method="GET",
+        path="/api/v1/companycity/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_salary_retrieve.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,31 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Skill(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Skill:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/skill/".format(
+        path="/api/v1/salary/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_companycity_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,33 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Skill(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> Skill:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/skill/{id}/".format(
+        method="PUT",
+        path="/api/v1/companycity/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -41,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_skill_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,49 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Skill(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Skill,
-
 
     id: str,
 
-) -> Skill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/skill/{id}/".format(
+        method="GET",
+        path="/api/v1/vacancycity/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Skill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_update.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,45 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Source(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Source,
 
+    id: str,
 
-) -> Source:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/source/".format(
+        method="PUT",
+        path="/api/v1/company/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_source_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_jobmixin_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Source(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> Source:
+    id: str,
+
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/source/".format(
+        method="PUT",
+        path="/api/v1/jobmixin/{id}/".format(
+            
+                id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,35 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Source(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> Source:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/source/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/vacancycontact/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -41,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_source_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,49 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class Source(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: Source,
-
 
     id: str,
 
-) -> Source:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/source/{id}/".format(
+        method="GET",
+        path="/api/v1/vacancycontact/{id}/".format(
             
                 id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": Source,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_retrieve.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,45 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class StopKeywords(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: StopKeywords,
-
 
-) -> StopKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/stopkeywords/".format(
+        method="GET",
+        path="/api/v1/currency/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_skill_retrieve.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,31 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class StopKeywords(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-) -> StopKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/stopkeywords/".format(
+        path="/api/v1/skill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -37,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_retrieve.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,35 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class StopKeywords(BaseModel):
-    id: int 
-    name: str 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> StopKeywords:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/stopkeywords/{id}/".format(
-            
-                id=id,
+        path="/api/v1/vacancyskill/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -41,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_stopkeywords_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,49 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class StopKeywords(BaseModel):
-    name: str 
-
 def make_request(self: BaseApi,
 
-    __request__: StopKeywords,
-
 
-    id: str,
-
-) -> StopKeywords:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/stopkeywords/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/vacancycontact/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": StopKeywords,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycity_create.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyCity(BaseModel):
-    city: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancyCity,
-
 
-) -> VacancyCity:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
         method="POST",
         path="/api/v1/vacancycity/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,41 +8,37 @@
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
 def make_request(self: BaseApi,
 
 
-    id: str,
-
 ) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="DELETE",
-        path="/api/v1/vacancycity/{id}/".format(
-            
-                id=id,
+        method="POST",
+        path="/api/v1/stopkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
-        "204": {
+        "200": {
             
                 "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_contact_retrieve.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyCity(BaseModel):
-    city: int 
-    id: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
 
-) -> VacancyCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/vacancycity/".format(
+        path="/api/v1/contact/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycity_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_currency_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyCity(BaseModel):
-    city: int 
-    id: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
 
     id: str,
 
-) -> VacancyCity:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/vacancycity/{id}/".format(
+        method="PUT",
+        path="/api/v1/currency/{id}/".format(
             
                 id=id,
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
@@ -42,12 +37,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyCity,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_company_retrieve.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancyContact,
-
 
-) -> VacancyContact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/vacancycontact/".format(
+        method="GET",
+        path="/api/v1/company/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancycontact_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
-    id: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
 
-) -> VacancyContact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
-        method="GET",
-        path="/api/v1/vacancycontact/".format(
+        method="POST",
+        path="/api/v1/searchandstopkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -38,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_retrieve_2.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_stopkeywords_retrieve.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,36 +5,27 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
-    id: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
 
-    id: str,
-
-) -> VacancyContact:
+) -> None:
     
 
     
     body = None
     
 
     m = ApiRequest(
         method="GET",
-        path="/api/v1/vacancycontact/{id}/".format(
-            
-                id=id,
+        path="/api/v1/stopkeywords/".format(
             
         ),
         content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
@@ -42,12 +33,12 @@
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancycontact_update.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_retrieve.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,50 +5,40 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancyContact(BaseModel):
-    contact: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancyContact,
-
 
-    id: str,
-
-) -> VacancyContact:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="PUT",
-        path="/api/v1/vacancycontact/{id}/".format(
-            
-                id=id,
+        method="GET",
+        path="/api/v1/searchandstopkeywords/".format(
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancyContact,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_create.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_searchandstopkeywords_update.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 import typing
 
 from pydantic import BaseModel
 
 from feedancy.lib.base import BaseApi
 from feedancy.lib.request import ApiRequest
 from feedancy.lib import json
-class VacancySkill(BaseModel):
-    skill: int 
-    vacancy: int 
-
 def make_request(self: BaseApi,
 
-    __request__: VacancySkill,
 
+    id: str,
 
-) -> VacancySkill:
+) -> None:
     
 
     
-    body = __request__
+    body = None
     
 
     m = ApiRequest(
-        method="POST",
-        path="/api/v1/vacancyskill/".format(
+        method="PUT",
+        path="/api/v1/searchandstopkeywords/{id}/".format(
+            
+                id=id,
             
         ),
-        content_type="application/json",
+        content_type=None,
         body=body,
         headers=self._only_provided({
         }),
         query_params=self._only_provided({
         }),
         cookies=self._only_provided({
         }),
     )
     return self.make_request({
     
         "200": {
             
-                "application/json": VacancySkill,
+                "default": None,
             
         },
     
     }, m)
```

### Comparing `feedancy-0.0.3/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py` & `feedancy-0.0.4/feedancy/feedancy/apis/api/api_v1_vacancyskill_destroy.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/feedancy/client.py` & `feedancy-0.0.4/feedancy/feedancy/client.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/feedancy/setup.py` & `feedancy-0.0.4/feedancy/setup.py`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.3/pyproject.toml` & `feedancy-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy"
-version = "0.0.3"
+version = "0.0.4"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `feedancy-0.0.3/PKG-INFO` & `feedancy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.0.3
+Version: 0.0.4
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

