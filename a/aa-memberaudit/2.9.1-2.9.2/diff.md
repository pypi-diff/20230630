# Comparing `tmp/aa_memberaudit-2.9.1.tar.gz` & `tmp/aa_memberaudit-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_memberaudit-2.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_memberaudit-2.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_memberaudit-2.9.1.tar` & `aa_memberaudit-2.9.2.tar`

### file list

```diff
@@ -1,241 +1,241 @@
--rw-r--r--   0        0        0     1070 2020-12-07 16:50:18.594218 aa_memberaudit-2.9.1/LICENSE
--rw-r--r--   0        0        0     5782 2023-05-08 12:02:59.444605 aa_memberaudit-2.9.1/README.md
--rw-r--r--   0        0        0      240 2023-06-20 12:20:45.235100 aa_memberaudit-2.9.1/memberaudit/__init__.py
--rw-r--r--   0        0        0    24333 2023-06-20 12:20:45.235100 aa_memberaudit-2.9.1/memberaudit/admin.py
--rw-r--r--   0        0        0     4548 2023-06-18 14:40:14.289539 aa_memberaudit-2.9.1/memberaudit/app_settings.py
--rw-r--r--   0        0        0      407 2023-06-18 19:47:02.522598 aa_memberaudit-2.9.1/memberaudit/apps.py
--rw-r--r--   0        0        0     1251 2023-06-18 19:47:02.522598 aa_memberaudit-2.9.1/memberaudit/auth_hooks.py
--rw-r--r--   0        0        0     1271 2023-06-18 14:40:14.289539 aa_memberaudit-2.9.1/memberaudit/checks.py
--rw-r--r--   0        0        0     1704 2023-06-18 14:40:14.293539 aa_memberaudit-2.9.1/memberaudit/constants.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.002082 aa_memberaudit-2.9.1/memberaudit/core/__init__.py
--rw-r--r--   0        0        0    11526 2023-06-19 16:16:36.734579 aa_memberaudit-2.9.1/memberaudit/core/data_exporters.py
--rw-r--r--   0        0        0    19456 2023-06-18 16:38:29.684085 aa_memberaudit-2.9.1/memberaudit/core/eft_parser.py
--rw-r--r--   0        0        0     5563 2023-06-20 12:20:45.235100 aa_memberaudit-2.9.1/memberaudit/core/fittings.py
--rw-r--r--   0        0        0     2244 2023-06-18 14:40:14.293539 aa_memberaudit-2.9.1/memberaudit/core/skill_plans.py
--rw-r--r--   0        0        0     5362 2023-06-20 12:20:45.235100 aa_memberaudit-2.9.1/memberaudit/core/skills.py
--rw-r--r--   0        0        0     3159 2023-06-16 09:54:37.516799 aa_memberaudit-2.9.1/memberaudit/core/xml_converter.py
--rw-r--r--   0        0        0     2430 2023-06-18 14:40:14.293539 aa_memberaudit-2.9.1/memberaudit/decorators.py
--rw-r--r--   0        0        0     3740 2023-06-18 14:40:14.293539 aa_memberaudit-2.9.1/memberaudit/forms.py
--rw-r--r--   0        0        0     1820 2023-06-18 19:20:57.381084 aa_memberaudit-2.9.1/memberaudit/helpers.py
--rw-r--r--   0        0        0      384 2023-04-25 19:10:30.704306 aa_memberaudit-2.9.1/memberaudit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43105 2023-06-15 19:47:27.818479 aa_memberaudit-2.9.1/memberaudit/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    43046 2023-06-15 19:47:27.818479 aa_memberaudit-2.9.1/memberaudit/locale/django.pot
--rw-r--r--   0        0        0    43093 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2023-04-19 20:05:21.889406 aa_memberaudit-2.9.1/memberaudit/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43093 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      450 2023-04-25 19:10:30.708306 aa_memberaudit-2.9.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43171 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      438 2023-04-25 19:10:30.712306 aa_memberaudit-2.9.1/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43159 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-04-25 19:10:30.712306 aa_memberaudit-2.9.1/memberaudit/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43100 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43112 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26859 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.1/memberaudit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    54952 2023-06-15 19:47:27.822479 aa_memberaudit-2.9.1/memberaudit/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      609 2023-04-25 19:10:30.716307 aa_memberaudit-2.9.1/memberaudit/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43330 2023-06-15 19:47:27.826479 aa_memberaudit-2.9.1/memberaudit/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2023-04-19 20:05:21.917406 aa_memberaudit-2.9.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43086 2023-06-15 19:47:27.826479 aa_memberaudit-2.9.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      102 2020-11-24 21:31:34.925680 aa_memberaudit-2.9.1/memberaudit/management/commands/__init__.py
--rw-r--r--   0        0        0     1443 2023-06-18 19:47:02.526598 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_data_export.py
--rw-r--r--   0        0        0     1374 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_load_eve.py
--rw-r--r--   0        0        0     3859 2023-06-16 09:54:37.520799 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-r--r--   0        0        0      740 2023-06-16 09:54:37.524799 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_stats.py
--rw-r--r--   0        0        0     1941 2023-06-16 09:54:37.524799 aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_update_characters.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.006082 aa_memberaudit-2.9.1/memberaudit/managers/__init__.py
--rw-r--r--   0        0        0    13017 2023-06-18 16:38:29.684085 aa_memberaudit-2.9.1/memberaudit/managers/character.py
--rw-r--r--   0        0        0    26850 2023-06-20 12:20:45.239100 aa_memberaudit-2.9.1/memberaudit/managers/character_sections_1.py
--rw-r--r--   0        0        0    29910 2023-06-20 12:20:45.239100 aa_memberaudit-2.9.1/memberaudit/managers/character_sections_2.py
--rw-r--r--   0        0        0    25043 2023-06-19 16:16:36.738579 aa_memberaudit-2.9.1/memberaudit/managers/character_sections_3.py
--rw-r--r--   0        0        0    24472 2023-06-18 16:38:29.684085 aa_memberaudit-2.9.1/memberaudit/managers/general.py
--rw-r--r--   0        0        0    65995 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.1/memberaudit/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     3444 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.1/memberaudit/migrations/0002_add_mining_ledger.py
--rw-r--r--   0        0        0     1478 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.1/memberaudit/migrations/0003_add_notify_permission.py
--rw-r--r--   0        0        0      513 2023-02-24 17:11:11.385592 aa_memberaudit-2.9.1/memberaudit/migrations/0004_character_is_disabled.py
--rw-r--r--   0        0        0     3819 2023-03-22 20:57:15.506894 aa_memberaudit-2.9.1/memberaudit/migrations/0005_add_fw_stats.py
--rw-r--r--   0        0        0     5969 2023-04-16 16:03:49.361835 aa_memberaudit-2.9.1/memberaudit/migrations/0006_add_localizations.py
--rw-r--r--   0        0        0     2129 2023-04-19 20:05:21.917406 aa_memberaudit-2.9.1/memberaudit/migrations/0007_add_localization_2.py
--rw-r--r--   0        0        0     2727 2023-06-15 13:23:00.558207 aa_memberaudit-2.9.1/memberaudit/migrations/0008_improve_skill_sets.py
--rw-r--r--   0        0        0     3274 2023-06-15 21:43:52.147759 aa_memberaudit-2.9.1/memberaudit/migrations/0009_add_planetary_industry.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.006082 aa_memberaudit-2.9.1/memberaudit/migrations/__init__.py
--rw-r--r--   0        0        0     1117 2023-06-18 15:15:28.267801 aa_memberaudit-2.9.1/memberaudit/models/__init__.py
--rw-r--r--   0        0        0    15243 2023-06-18 16:38:29.688085 aa_memberaudit-2.9.1/memberaudit/models/character_sections_1.py
--rw-r--r--   0        0        0    13506 2023-06-18 15:15:28.267801 aa_memberaudit-2.9.1/memberaudit/models/character_sections_2.py
--rw-r--r--   0        0        0    13923 2023-06-18 15:15:28.271801 aa_memberaudit-2.9.1/memberaudit/models/character_sections_3.py
--rw-r--r--   0        0        0    26983 2023-06-20 12:20:45.247100 aa_memberaudit-2.9.1/memberaudit/models/characters.py
--rw-r--r--   0        0        0      108 2021-01-17 22:43:01.025805 aa_memberaudit-2.9.1/memberaudit/models/constants.py
--rw-r--r--   0        0        0    17213 2023-06-18 16:38:29.688085 aa_memberaudit-2.9.1/memberaudit/models/general.py
--rw-r--r--   0        0        0      299 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/providers.py
--rw-r--r--   0        0        0      542 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/signals.py
--rw-r--r--   0        0        0      191 2023-02-24 14:11:29.027672 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/admin.css
--rw-r--r--   0        0        0      174 2022-02-09 21:55:36.823364 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_finder.css
--rw-r--r--   0        0        0     5736 2023-06-15 20:13:14.507685 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_viewer.css
--rw-r--r--   0        0        0     2540 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_viewer.min.css
--rw-r--r--   0        0        0       94 2022-11-27 20:20:23.212674 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/data_export.css
--rw-r--r--   0        0        0     1538 2021-05-04 21:32:43.714694 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/global.css
--rw-r--r--   0        0        0      646 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/global.min.css
--rw-r--r--   0        0        0     4331 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/launcher.css
--rw-r--r--   0        0        0     2765 2021-01-29 15:59:17.153310 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/launcher.min.css
--rw-r--r--   0        0        0     1363 2021-02-16 17:03:36.468870 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/memberaudit.css
--rw-r--r--   0        0        0      617 2021-02-16 17:03:36.468870 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-r--r--   0        0        0      611 2021-02-17 10:40:00.762093 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/reports.css
--rw-r--r--   0        0        0    43262 2020-10-26 16:42:17.713201 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-10-26 16:42:17.713201 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     1862 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/charisma.png
--rw-r--r--   0        0        0      694 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/eve-prism.png
--rw-r--r--   0        0        0      220 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/evelogo.png
--rw-r--r--   0        0        0      595 2020-11-03 21:09:40.510944 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/evesearch.png
--rw-r--r--   0        0        0     1966 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/intelligence.png
--rw-r--r--   0        0        0     1809 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/memory.png
--rw-r--r--   0        0        0     1803 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/perception.png
--rw-r--r--   0        0        0     1782 2021-02-23 10:36:55.530247 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/willpower.png
--rw-r--r--   0        0        0      259 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/zkillboard.png
--rw-r--r--   0        0        0     5573 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3908 2022-04-01 19:33:31.239451 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2022-04-01 19:48:30.310949 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2020-10-22 17:18:29.995572 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0    69950 2020-10-28 14:46:25.711812 aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-r--r--   0        0        0   881821 2023-02-16 19:01:05.384001 aa_memberaudit-2.9.1/memberaudit/swagger.json
--rw-r--r--   0        0        0    40513 2023-06-20 12:20:45.247100 aa_memberaudit-2.9.1/memberaudit/tasks.py
--rw-r--r--   0        0        0      687 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
--rw-r--r--   0        0        0      488 2022-09-02 18:40:08.749489 aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-r--r--   0        0        0      848 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
--rw-r--r--   0        0        0      367 2020-12-07 00:53:01.652277 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/base.html
--rw-r--r--   0        0        0     4801 2023-04-25 19:10:30.720306 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/character_finder.html
--rw-r--r--   0        0        0    29413 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/character_viewer.html
--rw-r--r--   0        0        0     2932 2023-04-25 19:10:30.720306 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/data_export.html
--rw-r--r--   0        0        0     8515 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/launcher.html
--rw-r--r--   0        0        0     1238 2021-01-29 15:52:00.995855 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-r--r--   0        0        0     4307 2022-04-01 19:33:31.243451 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-r--r--   0        0        0     1713 2021-02-18 07:41:27.336226 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-r--r--   0        0        0     1246 2020-11-01 21:48:51.676098 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-r--r--   0        0        0     8075 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-r--r--   0        0        0      658 2023-04-16 16:03:49.365835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-r--r--   0        0        0     1375 2022-02-09 21:55:36.827364 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-r--r--   0        0        0      382 2023-04-16 16:03:49.369835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-r--r--   0        0        0     3880 2022-04-01 19:33:31.243451 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
--rw-r--r--   0        0        0     9005 2023-06-15 11:31:30.596583 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-r--r--   0        0        0     1451 2023-04-16 16:03:49.369835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-r--r--   0        0        0      637 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
--rw-r--r--   0        0        0     1256 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-r--r--   0        0        0      560 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-r--r--   0        0        0     2604 2021-02-23 15:40:36.322996 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-r--r--   0        0        0      314 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-r--r--   0        0        0      848 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-r--r--   0        0        0      960 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-r--r--   0        0        0      582 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-r--r--   0        0        0      894 2020-12-14 23:31:49.226782 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-r--r--   0        0        0      549 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-r--r--   0        0        0     2786 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-r--r--   0        0        0      563 2023-06-15 19:47:27.834479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-r--r--   0        0        0      721 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-r--r--   0        0        0      148 2020-11-09 19:29:14.885373 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-r--r--   0        0        0      611 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-r--r--   0        0        0     2878 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-r--r--   0        0        0      779 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-r--r--   0        0        0      885 2023-06-16 09:54:37.528799 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html
--rw-r--r--   0        0        0      669 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-r--r--   0        0        0      882 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-r--r--   0        0        0      592 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-r--r--   0        0        0      907 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-r--r--   0        0        0      916 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-r--r--   0        0        0     3941 2023-06-15 19:47:27.838479 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-r--r--   0        0        0     2674 2022-01-23 15:08:18.156059 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/menu.html
--rw-r--r--   0        0        0      292 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
--rw-r--r--   0        0        0      684 2023-04-16 16:03:49.373835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-r--r--   0        0        0      760 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-r--r--   0        0        0      775 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-r--r--   0        0        0      691 2021-02-16 15:13:05.236586 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-r--r--   0        0        0      709 2023-04-16 16:03:49.377835 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-r--r--   0        0        0     9420 2022-04-01 19:56:47.910687 aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/reports.html
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/templatetags/__init__.py
--rw-r--r--   0        0        0      355 2023-06-18 16:38:29.688085 aa_memberaudit-2.9.1/memberaudit/templatetags/memberaudit.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/tests/core/__init__.py
--rw-r--r--   0        0        0     6350 2023-06-16 09:54:37.532799 aa_memberaudit-2.9.1/memberaudit/tests/core/test_core_xml_converter.py
--rw-r--r--   0        0        0    12725 2023-06-18 19:47:02.526598 aa_memberaudit-2.9.1/memberaudit/tests/core/test_data_exporters.py
--rw-r--r--   0        0        0    22366 2023-06-16 09:54:37.532799 aa_memberaudit-2.9.1/memberaudit/tests/core/test_eft_parser.py
--rw-r--r--   0        0        0     6371 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.1/memberaudit/tests/core/test_fittings.py
--rw-r--r--   0        0        0     4082 2022-09-03 21:36:22.049912 aa_memberaudit-2.9.1/memberaudit/tests/core/test_skill_plans.py
--rw-r--r--   0        0        0     2458 2023-06-16 09:54:37.536799 aa_memberaudit-2.9.1/memberaudit/tests/core/test_skills.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/tests/managers/__init__.py
--rw-r--r--   0        0        0    18357 2023-02-24 14:11:29.027672 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character.py
--rw-r--r--   0        0        0    30687 2023-06-20 12:20:45.247100 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_1.py
--rw-r--r--   0        0        0    37493 2023-06-19 14:17:29.534236 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_2.py
--rw-r--r--   0        0        0    24751 2023-06-19 16:16:36.742579 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_3.py
--rw-r--r--   0        0        0    46675 2023-06-17 19:32:02.157925 aa_memberaudit-2.9.1/memberaudit/tests/managers/test_general.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.018082 aa_memberaudit-2.9.1/memberaudit/tests/models/__init__.py
--rw-r--r--   0        0        0     2963 2023-06-18 15:15:28.271801 aa_memberaudit-2.9.1/memberaudit/tests/models/test_character_sections.py
--rw-r--r--   0        0        0    36073 2023-06-18 15:15:28.271801 aa_memberaudit-2.9.1/memberaudit/tests/models/test_characters_1.py
--rw-r--r--   0        0        0    23158 2023-06-20 12:20:45.247100 aa_memberaudit-2.9.1/memberaudit/tests/models/test_characters_2.py
--rw-r--r--   0        0        0    10969 2023-06-16 19:39:55.468632 aa_memberaudit-2.9.1/memberaudit/tests/models/test_general.py
--rw-r--r--   0        0        0    15428 2023-06-15 13:23:00.558207 aa_memberaudit-2.9.1/memberaudit/tests/test_admin.py
--rw-r--r--   0        0        0     1807 2023-02-24 17:52:57.675286 aa_memberaudit-2.9.1/memberaudit/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1314 2023-03-22 16:51:39.514903 aa_memberaudit-2.9.1/memberaudit/tests/test_checks.py
--rw-r--r--   0        0        0     3487 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.1/memberaudit/tests/test_commands.py
--rw-r--r--   0        0        0     4119 2023-06-17 19:32:02.161924 aa_memberaudit-2.9.1/memberaudit/tests/test_decorators.py
--rw-r--r--   0        0        0      900 2023-06-16 09:54:37.540799 aa_memberaudit-2.9.1/memberaudit/tests/test_factories.py
--rw-r--r--   0        0        0     3516 2022-09-03 16:21:19.096009 aa_memberaudit-2.9.1/memberaudit/tests/test_forms.py
--rw-r--r--   0        0        0     1476 2023-06-18 19:20:57.381084 aa_memberaudit-2.9.1/memberaudit/tests/test_helpers.py
--rw-r--r--   0        0        0    15643 2023-06-18 13:31:57.369928 aa_memberaudit-2.9.1/memberaudit/tests/test_integration.py
--rw-r--r--   0        0        0     1215 2022-03-05 14:47:06.220060 aa_memberaudit-2.9.1/memberaudit/tests/test_signals.py
--rw-r--r--   0        0        0    38340 2023-06-19 16:16:36.742579 aa_memberaudit-2.9.1/memberaudit/tests/test_tasks.py
--rw-r--r--   0        0        0      968 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/test_templatetags.py
--rw-r--r--   0        0        0     3822 2023-06-16 19:39:55.468632 aa_memberaudit-2.9.1/memberaudit/tests/test_utils.py
--rw-r--r--   0        0        0      267 2020-10-22 17:18:30.011572 aa_memberaudit-2.9.1/memberaudit/tests/testdata/__init__.py
--rw-r--r--   0        0        0     4432 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0     4350 2022-02-10 22:57:31.960297 aa_memberaudit-2.9.1/memberaudit/tests/testdata/entities.json
--rw-r--r--   0        0        0     5298 2023-06-19 21:45:47.103045 aa_memberaudit-2.9.1/memberaudit/tests/testdata/esi_client_stub.py
--rw-r--r--   0        0        0    41017 2023-06-15 19:47:27.842479 aa_memberaudit-2.9.1/memberaudit/tests/testdata/esi_testdata.json
--rw-r--r--   0        0        0  1225856 2023-06-15 19:47:27.862479 aa_memberaudit-2.9.1/memberaudit/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    13508 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/factories.py
--rw-r--r--   0        0        0      799 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-r--r--   0        0        0      889 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-r--r--   0        0        0      231 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-r--r--   0        0        0      503 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-r--r--   0        0        0      193 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-r--r--   0        0        0      377 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-r--r--   0        0        0      293 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-r--r--   0        0        0       96 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-r--r--   0        0        0      583 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-r--r--   0        0        0      432 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-r--r--   0        0        0      700 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-r--r--   0        0        0      459 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-r--r--   0        0        0      332 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-r--r--   0        0        0      410 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-r--r--   0        0        0      460 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-r--r--   0        0        0      455 2023-05-08 11:52:50.156096 aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
--rw-r--r--   0        0        0     4268 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/generate_character.py
--rw-r--r--   0        0        0     3859 2022-01-20 23:34:01.558036 aa_memberaudit-2.9.1/memberaudit/tests/testdata/generate_doctrines.py
--rw-r--r--   0        0        0     3680 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_entities.py
--rw-r--r--   0        0        0      478 2023-06-18 16:38:29.692085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0     1188 2022-02-10 21:29:55.833941 aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_locations.py
--rw-r--r--   0        0        0     1097 2022-04-01 19:33:31.251451 aa_memberaudit-2.9.1/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-r--r--   0        0        0      838 2023-06-18 16:38:29.696085 aa_memberaudit-2.9.1/memberaudit/tests/testdata/profiler_toolbox.py
--rw-r--r--   0        0        0     5744 2023-06-20 12:20:45.251100 aa_memberaudit-2.9.1/memberaudit/tests/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.022082 aa_memberaudit-2.9.1/memberaudit/tests/views/__init__.py
--rw-r--r--   0        0        0     9299 2023-06-15 13:23:00.562207 aa_memberaudit-2.9.1/memberaudit/tests/views/test_admin.py
--rw-r--r--   0        0        0     7089 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_finder.py
--rw-r--r--   0        0        0    32680 2023-03-22 21:45:48.968406 aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_viewer_1.py
--rw-r--r--   0        0        0    24561 2023-06-15 19:47:27.866479 aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_viewer_2.py
--rw-r--r--   0        0        0    14594 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/views/test_characters.py
--rw-r--r--   0        0        0     4101 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/views/test_data_export.py
--rw-r--r--   0        0        0    16249 2023-06-16 09:54:37.544799 aa_memberaudit-2.9.1/memberaudit/tests/views/test_reports.py
--rw-r--r--   0        0        0      710 2023-06-16 19:39:55.468632 aa_memberaudit-2.9.1/memberaudit/tools/clear_celery_once_locks.py
--rw-r--r--   0        0        0     3051 2022-10-21 18:07:26.108963 aa_memberaudit-2.9.1/memberaudit/tools/drop_tables.sql
--rw-r--r--   0        0        0      329 2020-12-16 22:00:54.319925 aa_memberaudit-2.9.1/memberaudit/tools/total_size.sql
--rw-r--r--   0        0        0     7242 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/urls.py
--rw-r--r--   0        0        0     2367 2023-06-18 16:38:29.696085 aa_memberaudit-2.9.1/memberaudit/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 11:55:38.022082 aa_memberaudit-2.9.1/memberaudit/views/__init__.py
--rw-r--r--   0        0        0     1539 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/views/_common.py
--rw-r--r--   0        0        0     3510 2023-06-18 14:40:14.297539 aa_memberaudit-2.9.1/memberaudit/views/admin.py
--rw-r--r--   0        0        0    12637 2023-06-18 16:38:29.696085 aa_memberaudit-2.9.1/memberaudit/views/character_finder.py
--rw-r--r--   0        0        0    24043 2023-06-18 19:20:57.385084 aa_memberaudit-2.9.1/memberaudit/views/character_viewer_1.py
--rw-r--r--   0        0        0    24241 2023-06-20 12:20:45.251100 aa_memberaudit-2.9.1/memberaudit/views/character_viewer_2.py
--rw-r--r--   0        0        0     8029 2023-06-18 16:38:29.700085 aa_memberaudit-2.9.1/memberaudit/views/characters.py
--rw-r--r--   0        0        0     2222 2023-06-18 14:40:14.301539 aa_memberaudit-2.9.1/memberaudit/views/data_export.py
--rw-r--r--   0        0        0    13139 2023-06-20 12:20:45.251100 aa_memberaudit-2.9.1/memberaudit/views/reports.py
--rw-r--r--   0        0        0     2278 2023-06-19 21:45:47.107045 aa_memberaudit-2.9.1/pyproject.toml
--rw-r--r--   0        0        0     7367 1970-01-01 00:00:00.000000 aa_memberaudit-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-23 12:09:49.027656 aa_memberaudit-2.9.2/LICENSE
+-rw-r--r--   0        0        0     5782 2023-06-23 12:09:49.027656 aa_memberaudit-2.9.2/README.md
+-rw-r--r--   0        0        0      240 2023-06-30 12:57:32.000784 aa_memberaudit-2.9.2/memberaudit/__init__.py
+-rw-r--r--   0        0        0    24333 2023-06-23 12:09:49.035656 aa_memberaudit-2.9.2/memberaudit/admin.py
+-rw-r--r--   0        0        0     4548 2023-06-23 12:09:49.035656 aa_memberaudit-2.9.2/memberaudit/app_settings.py
+-rw-r--r--   0        0        0      407 2023-06-23 12:09:49.035656 aa_memberaudit-2.9.2/memberaudit/apps.py
+-rw-r--r--   0        0        0     1251 2023-06-23 12:09:49.035656 aa_memberaudit-2.9.2/memberaudit/auth_hooks.py
+-rw-r--r--   0        0        0     1271 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/checks.py
+-rw-r--r--   0        0        0     1704 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/constants.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.428699 aa_memberaudit-2.9.2/memberaudit/core/__init__.py
+-rw-r--r--   0        0        0    11526 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/data_exporters.py
+-rw-r--r--   0        0        0    19456 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/eft_parser.py
+-rw-r--r--   0        0        0     5563 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/fittings.py
+-rw-r--r--   0        0        0     2244 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/skill_plans.py
+-rw-r--r--   0        0        0     5362 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/skills.py
+-rw-r--r--   0        0        0     3159 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/core/xml_converter.py
+-rw-r--r--   0        0        0     2430 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/decorators.py
+-rw-r--r--   0        0        0     3740 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/forms.py
+-rw-r--r--   0        0        0     1820 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/helpers.py
+-rw-r--r--   0        0        0      384 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43105 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    43046 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/django.pot
+-rw-r--r--   0        0        0    43093 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43093 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43171 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43159 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43100 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43112 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26859 2023-06-23 12:09:49.039656 aa_memberaudit-2.9.2/memberaudit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    54952 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43330 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43086 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_data_export.py
+-rw-r--r--   0        0        0     1374 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-r--r--   0        0        0     3859 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-r--r--   0        0        0      740 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_stats.py
+-rw-r--r--   0        0        0     1941 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_update_characters.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.428699 aa_memberaudit-2.9.2/memberaudit/managers/__init__.py
+-rw-r--r--   0        0        0    13017 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/character.py
+-rw-r--r--   0        0        0    26850 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/character_sections_1.py
+-rw-r--r--   0        0        0    29910 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/character_sections_2.py
+-rw-r--r--   0        0        0    25043 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/character_sections_3.py
+-rw-r--r--   0        0        0    24472 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/managers/general.py
+-rw-r--r--   0        0        0    65995 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     3444 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     1478 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0003_add_notify_permission.py
+-rw-r--r--   0        0        0      513 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0004_character_is_disabled.py
+-rw-r--r--   0        0        0     3819 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0005_add_fw_stats.py
+-rw-r--r--   0        0        0     5969 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0006_add_localizations.py
+-rw-r--r--   0        0        0     2129 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0007_add_localization_2.py
+-rw-r--r--   0        0        0     2727 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0008_improve_skill_sets.py
+-rw-r--r--   0        0        0     3274 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/migrations/0009_add_planetary_industry.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.428699 aa_memberaudit-2.9.2/memberaudit/migrations/__init__.py
+-rw-r--r--   0        0        0     1117 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/models/__init__.py
+-rw-r--r--   0        0        0    15243 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/models/character_sections_1.py
+-rw-r--r--   0        0        0    13506 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/models/character_sections_2.py
+-rw-r--r--   0        0        0    13923 2023-06-23 12:09:49.043656 aa_memberaudit-2.9.2/memberaudit/models/character_sections_3.py
+-rw-r--r--   0        0        0    26983 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/models/characters.py
+-rw-r--r--   0        0        0      108 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/models/constants.py
+-rw-r--r--   0        0        0    17213 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/models/general.py
+-rw-r--r--   0        0        0      299 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/providers.py
+-rw-r--r--   0        0        0      542 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/signals.py
+-rw-r--r--   0        0        0      191 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/admin.css
+-rw-r--r--   0        0        0      174 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_finder.css
+-rw-r--r--   0        0        0     5736 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-r--r--   0        0        0     2540 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_viewer.min.css
+-rw-r--r--   0        0        0       94 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/data_export.css
+-rw-r--r--   0        0        0     1538 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/global.css
+-rw-r--r--   0        0        0      646 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/global.min.css
+-rw-r--r--   0        0        0     4331 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/launcher.css
+-rw-r--r--   0        0        0     2765 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-r--r--   0        0        0     1363 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-r--r--   0        0        0      617 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-r--r--   0        0        0      611 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/reports.css
+-rw-r--r--   0        0        0    43262 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     1862 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/charisma.png
+-rw-r--r--   0        0        0      694 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-r--r--   0        0        0      220 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/evelogo.png
+-rw-r--r--   0        0        0      595 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/evesearch.png
+-rw-r--r--   0        0        0     1966 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/intelligence.png
+-rw-r--r--   0        0        0     1809 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/memory.png
+-rw-r--r--   0        0        0     1803 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/perception.png
+-rw-r--r--   0        0        0     1782 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/willpower.png
+-rw-r--r--   0        0        0      259 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/zkillboard.png
+-rw-r--r--   0        0        0     5573 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3908 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0    69950 2023-06-23 12:09:49.047656 aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0   881821 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/swagger.json
+-rw-r--r--   0        0        0    40513 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/tasks.py
+-rw-r--r--   0        0        0      687 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+-rw-r--r--   0        0        0      488 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-r--r--   0        0        0      848 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+-rw-r--r--   0        0        0      367 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/base.html
+-rw-r--r--   0        0        0     4801 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/character_finder.html
+-rw-r--r--   0        0        0    29413 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/character_viewer.html
+-rw-r--r--   0        0        0     2932 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/data_export.html
+-rw-r--r--   0        0        0     8515 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/launcher.html
+-rw-r--r--   0        0        0     1238 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-r--r--   0        0        0     4307 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-r--r--   0        0        0     1713 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-r--r--   0        0        0     1246 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-r--r--   0        0        0     8075 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-r--r--   0        0        0      658 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-r--r--   0        0        0     1375 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-r--r--   0        0        0      382 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-r--r--   0        0        0     3880 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+-rw-r--r--   0        0        0     9005 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-r--r--   0        0        0     1451 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-r--r--   0        0        0      637 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+-rw-r--r--   0        0        0     1256 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-r--r--   0        0        0      560 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-r--r--   0        0        0     2604 2023-06-23 12:09:49.051656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-r--r--   0        0        0      314 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-r--r--   0        0        0      848 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-r--r--   0        0        0      960 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-r--r--   0        0        0      582 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-r--r--   0        0        0      894 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-r--r--   0        0        0      549 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-r--r--   0        0        0     2786 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-r--r--   0        0        0      563 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-r--r--   0        0        0      721 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-r--r--   0        0        0      148 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-r--r--   0        0        0      611 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-r--r--   0        0        0     2878 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-r--r--   0        0        0      779 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-r--r--   0        0        0      885 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html
+-rw-r--r--   0        0        0      669 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-r--r--   0        0        0      882 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-r--r--   0        0        0      592 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-r--r--   0        0        0      907 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-r--r--   0        0        0      916 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-r--r--   0        0        0     3941 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-r--r--   0        0        0     2674 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/menu.html
+-rw-r--r--   0        0        0      292 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
+-rw-r--r--   0        0        0      684 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-r--r--   0        0        0      760 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-r--r--   0        0        0      775 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-r--r--   0        0        0      691 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-r--r--   0        0        0      709 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-r--r--   0        0        0     9420 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/reports.html
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/templatetags/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/templatetags/memberaudit.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/tests/core/__init__.py
+-rw-r--r--   0        0        0     6350 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_core_xml_converter.py
+-rw-r--r--   0        0        0    12725 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_data_exporters.py
+-rw-r--r--   0        0        0    22366 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_eft_parser.py
+-rw-r--r--   0        0        0     6371 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_fittings.py
+-rw-r--r--   0        0        0     4082 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_skill_plans.py
+-rw-r--r--   0        0        0     2458 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/core/test_skills.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/tests/managers/__init__.py
+-rw-r--r--   0        0        0    18357 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character.py
+-rw-r--r--   0        0        0    30687 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_1.py
+-rw-r--r--   0        0        0    37493 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_2.py
+-rw-r--r--   0        0        0    24751 2023-06-23 12:09:49.055656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_3.py
+-rw-r--r--   0        0        0    46675 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/managers/test_general.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.436699 aa_memberaudit-2.9.2/memberaudit/tests/models/__init__.py
+-rw-r--r--   0        0        0     2963 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/models/test_character_sections.py
+-rw-r--r--   0        0        0    36073 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/models/test_characters_1.py
+-rw-r--r--   0        0        0    23158 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/models/test_characters_2.py
+-rw-r--r--   0        0        0    10969 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/models/test_general.py
+-rw-r--r--   0        0        0    15428 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_admin.py
+-rw-r--r--   0        0        0     1807 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1314 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_checks.py
+-rw-r--r--   0        0        0     3487 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_commands.py
+-rw-r--r--   0        0        0     4119 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_decorators.py
+-rw-r--r--   0        0        0      900 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_factories.py
+-rw-r--r--   0        0        0     3516 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_forms.py
+-rw-r--r--   0        0        0     1476 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_helpers.py
+-rw-r--r--   0        0        0    15643 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_integration.py
+-rw-r--r--   0        0        0     1215 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_signals.py
+-rw-r--r--   0        0        0    38340 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_tasks.py
+-rw-r--r--   0        0        0      968 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3822 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/test_utils.py
+-rw-r--r--   0        0        0      267 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     4432 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0     4350 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/entities.json
+-rw-r--r--   0        0        0     5298 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0    41017 2023-06-23 12:09:49.059656 aa_memberaudit-2.9.2/memberaudit/tests/testdata/esi_testdata.json
+-rw-r--r--   0        0        0  1225856 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    13508 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/factories.py
+-rw-r--r--   0        0        0      799 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-r--r--   0        0        0      889 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-r--r--   0        0        0      231 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-r--r--   0        0        0      503 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-r--r--   0        0        0      193 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-r--r--   0        0        0      377 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-r--r--   0        0        0      293 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-r--r--   0        0        0       96 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-r--r--   0        0        0      583 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-r--r--   0        0        0      432 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-r--r--   0        0        0      700 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-r--r--   0        0        0      459 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-r--r--   0        0        0      332 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-r--r--   0        0        0      410 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-r--r--   0        0        0      460 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-r--r--   0        0        0      455 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
+-rw-r--r--   0        0        0     4268 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/generate_character.py
+-rw-r--r--   0        0        0     3859 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/generate_doctrines.py
+-rw-r--r--   0        0        0     3680 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_entities.py
+-rw-r--r--   0        0        0      478 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0     1188 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_locations.py
+-rw-r--r--   0        0        0     1097 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-r--r--   0        0        0      838 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-r--r--   0        0        0     5744 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.440699 aa_memberaudit-2.9.2/memberaudit/tests/views/__init__.py
+-rw-r--r--   0        0        0     9299 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_admin.py
+-rw-r--r--   0        0        0     7089 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_finder.py
+-rw-r--r--   0        0        0    32680 2023-06-23 12:09:49.063655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_viewer_1.py
+-rw-r--r--   0        0        0    24561 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_viewer_2.py
+-rw-r--r--   0        0        0    14594 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_characters.py
+-rw-r--r--   0        0        0     4101 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_data_export.py
+-rw-r--r--   0        0        0    16249 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tests/views/test_reports.py
+-rw-r--r--   0        0        0      710 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0     3051 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tools/drop_tables.sql
+-rw-r--r--   0        0        0      329 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/tools/total_size.sql
+-rw-r--r--   0        0        0     7242 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/urls.py
+-rw-r--r--   0        0        0     2367 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 13:31:50.440699 aa_memberaudit-2.9.2/memberaudit/views/__init__.py
+-rw-r--r--   0        0        0     1539 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/_common.py
+-rw-r--r--   0        0        0     3510 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/admin.py
+-rw-r--r--   0        0        0    12637 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/character_finder.py
+-rw-r--r--   0        0        0    24043 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/character_viewer_1.py
+-rw-r--r--   0        0        0    24147 2023-06-30 12:57:32.000784 aa_memberaudit-2.9.2/memberaudit/views/character_viewer_2.py
+-rw-r--r--   0        0        0     8029 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/characters.py
+-rw-r--r--   0        0        0     2222 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/data_export.py
+-rw-r--r--   0        0        0    13139 2023-06-23 12:09:49.067655 aa_memberaudit-2.9.2/memberaudit/views/reports.py
+-rw-r--r--   0        0        0     2285 2023-06-30 12:57:32.000784 aa_memberaudit-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7374 1970-01-01 00:00:00.000000 aa_memberaudit-2.9.2/PKG-INFO
```

### Comparing `aa_memberaudit-2.9.1/LICENSE` & `aa_memberaudit-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/README.md` & `aa_memberaudit-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/admin.py` & `aa_memberaudit-2.9.2/memberaudit/admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/app_settings.py` & `aa_memberaudit-2.9.2/memberaudit/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/auth_hooks.py` & `aa_memberaudit-2.9.2/memberaudit/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/checks.py` & `aa_memberaudit-2.9.2/memberaudit/checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/constants.py` & `aa_memberaudit-2.9.2/memberaudit/constants.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.9.2/memberaudit/core/data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.9.2/memberaudit/core/eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/core/fittings.py` & `aa_memberaudit-2.9.2/memberaudit/core/fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.9.2/memberaudit/core/skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/core/skills.py` & `aa_memberaudit-2.9.2/memberaudit/core/skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.9.2/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/decorators.py` & `aa_memberaudit-2.9.2/memberaudit/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/forms.py` & `aa_memberaudit-2.9.2/memberaudit/forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/helpers.py` & `aa_memberaudit-2.9.2/memberaudit/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/de/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/django.pot` & `aa_memberaudit-2.9.2/memberaudit/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/en/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/es/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/it_IT/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/ja/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/ru/LC_MESSAGES/django.mo` & `aa_memberaudit-2.9.2/memberaudit/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/ru/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/uk/LC_MESSAGES/django.mo` & `aa_memberaudit-2.9.2/memberaudit/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/uk/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.2/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.9.2/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/managers/character.py` & `aa_memberaudit-2.9.2/memberaudit/managers/character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/managers/character_sections_1.py` & `aa_memberaudit-2.9.2/memberaudit/managers/character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/managers/character_sections_2.py` & `aa_memberaudit-2.9.2/memberaudit/managers/character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/managers/character_sections_3.py` & `aa_memberaudit-2.9.2/memberaudit/managers/character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/managers/general.py` & `aa_memberaudit-2.9.2/memberaudit/managers/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0006_add_localizations.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0006_add_localizations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0007_add_localization_2.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0007_add_localization_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0008_improve_skill_sets.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0008_improve_skill_sets.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/migrations/0009_add_planetary_industry.py` & `aa_memberaudit-2.9.2/memberaudit/migrations/0009_add_planetary_industry.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/models/__init__.py` & `aa_memberaudit-2.9.2/memberaudit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/models/character_sections_1.py` & `aa_memberaudit-2.9.2/memberaudit/models/character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/models/character_sections_2.py` & `aa_memberaudit-2.9.2/memberaudit/models/character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/models/character_sections_3.py` & `aa_memberaudit-2.9.2/memberaudit/models/character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/models/characters.py` & `aa_memberaudit-2.9.2/memberaudit/models/characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/models/general.py` & `aa_memberaudit-2.9.2/memberaudit/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/signals.py` & `aa_memberaudit-2.9.2/memberaudit/signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/character_viewer.min.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/character_viewer.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.9.2/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/swagger.json` & `aa_memberaudit-2.9.2/memberaudit/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tasks.py` & `aa_memberaudit-2.9.2/memberaudit/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.9.2/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/character_finder.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/data_export.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/launcher.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/partials/solar_system.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/partials/solar_system.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.9.2/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.9.2/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.9.2/memberaudit/tests/core/test_data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.9.2/memberaudit/tests/core/test_eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/core/test_fittings.py` & `aa_memberaudit-2.9.2/memberaudit/tests/core/test_fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.9.2/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.9.2/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_1.py` & `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_2.py` & `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_character_sections_3.py` & `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.9.2/memberaudit/tests/managers/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/models/test_character_sections.py` & `aa_memberaudit-2.9.2/memberaudit/tests/models/test_character_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/models/test_characters_1.py` & `aa_memberaudit-2.9.2/memberaudit/tests/models/test_characters_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/models/test_characters_2.py` & `aa_memberaudit-2.9.2/memberaudit/tests/models/test_characters_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.9.2/memberaudit/tests/models/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_decorators.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/test_utils.py` & `aa_memberaudit-2.9.2/memberaudit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/generate_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.9.2/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/utils.py` & `aa_memberaudit-2.9.2/memberaudit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.9.2/memberaudit/tests/views/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.9.2/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.9.2/memberaudit/tests/views/test_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.9.2/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.9.2/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tools/clear_celery_once_locks.py` & `aa_memberaudit-2.9.2/memberaudit/tools/clear_celery_once_locks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/tools/drop_tables.sql` & `aa_memberaudit-2.9.2/memberaudit/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/urls.py` & `aa_memberaudit-2.9.2/memberaudit/urls.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/utils.py` & `aa_memberaudit-2.9.2/memberaudit/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/views/_common.py` & `aa_memberaudit-2.9.2/memberaudit/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/views/admin.py` & `aa_memberaudit-2.9.2/memberaudit/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/views/character_finder.py` & `aa_memberaudit-2.9.2/memberaudit/views/character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.9.2/memberaudit/views/character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.9.2/memberaudit/views/character_viewer_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Character viewer views (2/2)."""
 
 import datetime as dt
 from typing import Optional
 
 import humanize
-from humanize import naturaltime
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Prefetch
 from django.http import HttpResponse, HttpResponseNotFound, JsonResponse
 from django.shortcuts import get_object_or_404, render
 from django.urls import reverse
 from django.utils.html import format_html
-from django.utils.timezone import now
 from django.utils.translation import gettext, gettext_lazy
 from eveuniverse.core import eveimageserver
 from eveuniverse.models import EveType
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 from app_utils.views import (
@@ -259,30 +257,29 @@
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_planets_data(
     request, character_pk: int, character: Character
 ) -> JsonResponse:
     data = []
-    my_now = now()
     for planet in character.planets.select_related(
         "eve_planet",
         "eve_planet__eve_type",
         "eve_planet__eve_solar_system",
         "eve_planet__eve_solar_system__eve_constellation__eve_region",
     ):
         planet: CharacterPlanet
         eve_solar_system = planet.eve_planet.eve_solar_system
         solar_system_html = eve_solar_system_to_html(
             eve_solar_system, show_region=False
         )
         last_update_html = format_html(
             '<span title="{}">{}</span>',
             planet.last_update_at.strftime(DATETIME_FORMAT),
-            naturaltime(planet.last_update_at, when=my_now),
+            humanize.naturaltime(planet.last_update_at),
         )
         data.append(
             {
                 "id": planet.pk,
                 "last_update": {
                     "display": last_update_html,
                     "sort": planet.last_update_at.isoformat(),
```

### Comparing `aa_memberaudit-2.9.1/memberaudit/views/characters.py` & `aa_memberaudit-2.9.2/memberaudit/views/characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/views/data_export.py` & `aa_memberaudit-2.9.2/memberaudit/views/data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/memberaudit/views/reports.py` & `aa_memberaudit-2.9.2/memberaudit/views/reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.1/pyproject.toml` & `aa_memberaudit-2.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ]
 dependencies = [
     "allianceauth-app-utils>=1.18.1",
     "allianceauth>=3",
     "bleach",
     "dj-datatables-view",
     "django-eveuniverse>=1.2",
-    "humanize",
+    "humanize>=4.7.0",
     "unidecode",
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/ErikKalkoken/aa-memberaudit"
 Documentation = "https://aa-memberaudit.readthedocs.io/en/latest/"
 Source = "https://gitlab.com/ErikKalkoken/aa-memberaudit"
```

### Comparing `aa_memberaudit-2.9.1/PKG-INFO` & `aa_memberaudit-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit
-Version: 2.9.1
+Version: 2.9.2
 Summary: "An Alliance Auth app that provides full access to Eve characters
 Keywords: allianceauth,eveonline,memberaudit
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>, Peter Pfeufer <develop@ppfeufer.de>, Rebecca Murphy <rebecca@rcmurphy.me>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,15 +20,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: allianceauth-app-utils>=1.18.1
 Requires-Dist: allianceauth>=3
 Requires-Dist: bleach
 Requires-Dist: dj-datatables-view
 Requires-Dist: django-eveuniverse>=1.2
-Requires-Dist: humanize
+Requires-Dist: humanize>=4.7.0
 Requires-Dist: unidecode
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://aa-memberaudit.readthedocs.io/en/latest/
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-memberaudit
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-memberaudit
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/issues
```

