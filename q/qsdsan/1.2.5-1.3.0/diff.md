# Comparing `tmp/qsdsan-1.2.5.tar.gz` & `tmp/qsdsan-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsdsan-1.2.5.tar", last modified: Tue Jan 31 23:14:11 2023, max compression
+gzip compressed data, was "qsdsan-1.3.0.tar", last modified: Fri Jun 30 20:19:46 2023, max compression
```

## Comparing `qsdsan-1.2.5.tar` & `qsdsan-1.3.0.tar`

### file list

```diff
@@ -1,164 +1,172 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.142684 qsdsan-1.2.5/
--rw-rw-rw-   0        0        0     1254 2022-10-08 14:20:28.000000 qsdsan-1.2.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     9932 2022-12-08 03:42:09.000000 qsdsan-1.2.5/CHANGELOG.rst
--rw-rw-rw-   0        0        0     5385 2022-10-08 14:20:28.000000 qsdsan-1.2.5/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0    16866 2023-01-25 01:09:07.000000 qsdsan-1.2.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1937 2022-10-08 14:20:28.000000 qsdsan-1.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      594 2022-10-08 14:20:28.000000 qsdsan-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0    11187 2023-01-31 23:14:11.142684 qsdsan-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     9842 2022-12-08 03:42:09.000000 qsdsan-1.2.5/README.rst
--rw-rw-rw-   0        0        0      475 2022-10-08 14:20:28.000000 qsdsan-1.2.5/pytest.ini
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.008278 qsdsan-1.2.5/qsdsan/
--rw-rw-rw-   0        0        0     2899 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/__init__.py
--rw-rw-rw-   0        0        0    31037 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/_component.py
--rw-rw-rw-   0        0        0    33186 2022-12-29 15:48:21.000000 qsdsan-1.2.5/qsdsan/_components.py
--rw-rw-rw-   0        0        0     8600 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/_construction.py
--rw-rw-rw-   0        0        0     5949 2023-01-31 02:18:30.000000 qsdsan-1.2.5/qsdsan/_equipment.py
--rw-rw-rw-   0        0        0    13906 2022-12-06 20:30:34.000000 qsdsan-1.2.5/qsdsan/_impact_indicator.py
--rw-rw-rw-   0        0        0    29724 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/_impact_item.py
--rw-rw-rw-   0        0        0    36996 2023-01-31 02:18:30.000000 qsdsan-1.2.5/qsdsan/_lca.py
--rw-rw-rw-   0        0        0    52298 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/_process.py
--rw-rw-rw-   0        0        0    24528 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/_sanstream.py
--rw-rw-rw-   0        0        0    27356 2023-01-31 22:52:29.000000 qsdsan-1.2.5/qsdsan/_sanunit.py
--rw-rw-rw-   0        0        0    20837 2023-01-31 22:52:29.000000 qsdsan-1.2.5/qsdsan/_tea.py
--rw-rw-rw-   0        0        0    11720 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/_transportation.py
--rw-rw-rw-   0        0        0    88937 2023-01-31 02:18:30.000000 qsdsan-1.2.5/qsdsan/_waste_stream.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.026996 qsdsan-1.2.5/qsdsan/data/
--rw-rw-rw-   0        0        0    13259 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/_adm1.xlsx
--rw-rw-rw-   0        0        0     7170 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/data/_components.tsv
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.031303 qsdsan-1.2.5/qsdsan/data/process_data/
--rw-rw-rw-   0        0        0     1334 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/process_data/_adm1.tsv
--rw-rw-rw-   0        0        0      822 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/process_data/_asm1.tsv
--rw-rw-rw-   0        0        0     2583 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/process_data/_asm2d.tsv
--rw-rw-rw-   0        0        0     1443 2023-01-04 22:10:35.000000 qsdsan-1.2.5/qsdsan/data/process_data/_pm2.tsv
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.041594 qsdsan-1.2.5/qsdsan/data/sanunit_data/
--rw-rw-rw-   0        0        0     1051 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_anaerobic_baffled_reactor.tsv
--rw-rw-rw-   0        0        0      923 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_anaerobic_digestion.tsv
--rw-rw-rw-   0        0        0     1043 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_anaerobic_lagoon.tsv
--rw-rw-rw-   0        0        0     2141 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_drying_bed.tsv
--rw-rw-rw-   0        0        0     2918 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_excretion.tsv
--rw-rw-rw-   0        0        0     1178 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_facultative_lagoon.tsv
--rw-rw-rw-   0        0        0   104004 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_inf_dry_2006.tsv
--rw-rw-rw-   0        0        0      793 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_liquid_treatment_bed.tsv
--rw-rw-rw-   0        0        0     1416 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_murt.tsv
--rw-rw-rw-   0        0        0     1691 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_pit_latrine.tsv
--rw-rw-rw-   0        0        0     1202 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_sedimentation_tank.tsv
--rw-rw-rw-   0        0        0     1077 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_septic_tank.csv
--rw-rw-rw-   0        0        0     1119 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_sludge_pasteurization.tsv
--rw-rw-rw-   0        0        0      553 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_sludge_separator.tsv
--rw-rw-rw-   0        0        0     1288 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_toilet.tsv
--rw-rw-rw-   0        0        0     1403 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/_uddt.tsv
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.052785 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/
--rw-rw-rw-   0        0        0     8043 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_carbonizer_base.tsv
--rw-rw-rw-   0        0        0     3980 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_controls.tsv
--rw-rw-rw-   0        0        0      495 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_grinder.tsv
--rw-rw-rw-   0        0        0     4120 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_hhx.tsv
--rw-rw-rw-   0        0        0     1164 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_hhx_dryer.tsv
--rw-rw-rw-   0        0        0      805 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_housing.tsv
--rw-rw-rw-   0        0        0     1605 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_ion_exchange.tsv
--rw-rw-rw-   0        0        0      804 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_ohx.tsv
--rw-rw-rw-   0        0        0     3053 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_pollution_control.tsv
--rw-rw-rw-   0        0        0      999 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_screw_press.tsv
--rw-rw-rw-   0        0        0      997 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_struvite_precipitation.tsv
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.060134 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/
--rw-rw-rw-   0        0        0      736 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_aerobic.tsv
--rw-rw-rw-   0        0        0      723 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_anaerobic.tsv
--rw-rw-rw-   0        0        0      678 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_anoxic.tsv
--rw-rw-rw-   0        0        0     1152 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_bio_cost.tsv
--rw-rw-rw-   0        0        0    14447 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_ecr.xlsx
--rw-rw-rw-   0        0        0     1284 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_mbr.tsv
--rw-rw-rw-   0        0        0    13527 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_primary.xlsx
--rw-rw-rw-   0        0        0      843 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_solar.tsv
--rw-rw-rw-   0        0        0      898 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_system.tsv
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.064189 qsdsan-1.2.5/qsdsan/data/sanunit_data/re/
--rw-rw-rw-   0        0        0     1025 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_ecr.csv
--rw-rw-rw-   0        0        0     1621 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_housing.csv
--rw-rw-rw-   0        0        0     3559 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_ion_exchange.csv
--rw-rw-rw-   0        0        0     1668 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_solar.csv
--rw-rw-rw-   0        0        0     3413 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_system.csv
--rw-rw-rw-   0        0        0     6847 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_ultrafiltration.csv
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.071986 qsdsan-1.2.5/qsdsan/equipments/
--rw-rw-rw-   0        0        0     1065 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/__init__.py
--rw-rw-rw-   0        0        0    10296 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/_aeration.py
--rw-rw-rw-   0        0        0     2328 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/_column.py
--rw-rw-rw-   0        0        0     3439 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/_electrode.py
--rw-rw-rw-   0        0        0     1512 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/_encapsulation.py
--rw-rw-rw-   0        0        0     1750 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/_machine.py
--rw-rw-rw-   0        0        0     4117 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/_membrane.py
--rw-rw-rw-   0        0        0     2071 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/_vacuum_pump.py
--rw-rw-rw-   0        0        0     2717 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/equipments/_vertical_mixer.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.078742 qsdsan-1.2.5/qsdsan/processes/
--rw-rw-rw-   0        0        0      870 2023-01-04 22:10:35.000000 qsdsan-1.2.5/qsdsan/processes/__init__.py
--rw-rw-rw-   0        0        0    30452 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/processes/_adm1.py
--rw-rw-rw-   0        0        0    11547 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/processes/_aeration.py
--rw-rw-rw-   0        0        0    11758 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/processes/_asm1.py
--rw-rw-rw-   0        0        0    30686 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/processes/_asm2d.py
--rw-rw-rw-   0        0        0    11867 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/processes/_decay.py
--rw-rw-rw-   0        0        0    11113 2023-01-07 18:39:59.000000 qsdsan-1.2.5/qsdsan/processes/_kinetic_reaction.py
--rw-rw-rw-   0        0        0    35864 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/processes/_pm2.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.117804 qsdsan-1.2.5/qsdsan/sanunits/
--rw-rw-rw-   0        0        0     4608 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/__init__.py
--rw-rw-rw-   0        0        0    13081 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_abstract.py
--rw-rw-rw-   0        0        0    26331 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_activated_sludge_process.py
--rw-rw-rw-   0        0        0    37663 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_anaerobic_reactors.py
--rw-rw-rw-   0        0        0    51946 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_biogenic_refinery.py
--rw-rw-rw-   0        0        0    19434 2023-01-02 21:25:34.000000 qsdsan-1.2.5/qsdsan/sanunits/_clarifier.py
--rw-rw-rw-   0        0        0    16379 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_combustion.py
--rw-rw-rw-   0        0        0     2301 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_compressor.py
--rw-rw-rw-   0        0        0     3461 2023-01-04 22:10:35.000000 qsdsan-1.2.5/qsdsan/sanunits/_crop_application.py
--rw-rw-rw-   0        0        0     1539 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_distillation.py
--rw-rw-rw-   0        0        0     9688 2023-01-31 22:52:29.000000 qsdsan-1.2.5/qsdsan/sanunits/_dynamic_influent.py
--rw-rw-rw-   0        0        0    24306 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_eco_san.py
--rw-rw-rw-   0        0        0     8160 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_electrochemical_cell.py
--rw-rw-rw-   0        0        0    11721 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/sanunits/_encapsulation_bioreactor.py
--rw-rw-rw-   0        0        0     9186 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/sanunits/_excretion.py
--rw-rw-rw-   0        0        0     1495 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_flash.py
--rw-rw-rw-   0        0        0    13432 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_heat_exchanging.py
--rw-rw-rw-   0        0        0    23530 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_hydroprocessing.py
--rw-rw-rw-   0        0        0    28246 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_hydrothermal.py
--rw-rw-rw-   0        0        0    21867 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/sanunits/_internal_circulation_rx.py
--rw-rw-rw-   0        0        0    33946 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_junction.py
--rw-rw-rw-   0        0        0     7964 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_lagoon.py
--rw-rw-rw-   0        0        0    47808 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/sanunits/_membrane_bioreactors.py
--rw-rw-rw-   0        0        0    12474 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_membrane_distillation.py
--rw-rw-rw-   0        0        0     3135 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/sanunits/_non_reactive.py
--rw-rw-rw-   0        0        0    26719 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/sanunits/_polishing_filter.py
--rw-rw-rw-   0        0        0    39311 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_pumping.py
--rw-rw-rw-   0        0        0     8954 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_reactor.py
--rw-rw-rw-   0        0        0    28231 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_reclaimer.py
--rw-rw-rw-   0        0        0     2146 2023-01-02 19:15:09.000000 qsdsan-1.2.5/qsdsan/sanunits/_screening.py
--rw-rw-rw-   0        0        0     6766 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_sedimentation.py
--rw-rw-rw-   0        0        0     8043 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_septic_tank.py
--rw-rw-rw-   0        0        0    13337 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_sludge_pasteurization.py
--rw-rw-rw-   0        0        0    18475 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_sludge_thickening.py
--rw-rw-rw-   0        0        0    25539 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/sanunits/_suspended_growth_bioreactor.py
--rw-rw-rw-   0        0        0     6416 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_tanks.py
--rw-rw-rw-   0        0        0    43871 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_toilets.py
--rw-rw-rw-   0        0        0    13518 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_treatment_beds.py
--rw-rw-rw-   0        0        0     6323 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/sanunits/_trucking.py
--rw-rw-rw-   0        0        0    63183 2022-12-06 20:30:34.000000 qsdsan-1.2.5/qsdsan/stats.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.141683 qsdsan-1.2.5/qsdsan/utils/
--rw-rw-rw-   0        0        0     1952 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/utils/__init__.py
--rw-rw-rw-   0        0        0    16262 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/utils/cod.py
--rw-rw-rw-   0        0        0     3884 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/utils/colors.py
--rw-rw-rw-   0        0        0     5484 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/utils/components.py
--rw-rw-rw-   0        0        0    20383 2022-12-06 20:30:34.000000 qsdsan-1.2.5/qsdsan/utils/construction.py
--rw-rw-rw-   0        0        0    10168 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/utils/doc_examples.py
--rw-rw-rw-   0        0        0     8011 2023-01-31 22:52:29.000000 qsdsan-1.2.5/qsdsan/utils/dynamics.py
--rw-rw-rw-   0        0        0     1134 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/utils/formatting.py
--rw-rw-rw-   0        0        0     3574 2023-01-25 01:09:07.000000 qsdsan-1.2.5/qsdsan/utils/loading.py
--rw-rw-rw-   0        0        0     6025 2023-01-07 15:40:42.000000 qsdsan-1.2.5/qsdsan/utils/misc.py
--rw-rw-rw-   0        0        0     8910 2023-01-24 23:01:04.000000 qsdsan-1.2.5/qsdsan/utils/model_eval.py
--rw-rw-rw-   0        0        0     6573 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/utils/parsing.py
--rw-rw-rw-   0        0        0     3914 2023-01-31 22:52:29.000000 qsdsan-1.2.5/qsdsan/utils/scope.py
--rw-rw-rw-   0        0        0      482 2022-10-08 14:20:28.000000 qsdsan-1.2.5/qsdsan/utils/units_definition.txt
--rw-rw-rw-   0        0        0     3764 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/utils/utilities.py
--rw-rw-rw-   0        0        0     1871 2022-12-08 03:42:09.000000 qsdsan-1.2.5/qsdsan/utils/wwt_design.py
-drwxrwxrwx   0        0        0        0 2023-01-31 23:14:11.025000 qsdsan-1.2.5/qsdsan.egg-info/
--rw-rw-rw-   0        0        0    11187 2023-01-31 23:14:10.000000 qsdsan-1.2.5/qsdsan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4927 2023-01-31 23:14:10.000000 qsdsan-1.2.5/qsdsan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 23:14:10.000000 qsdsan-1.2.5/qsdsan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-01-31 23:14:10.000000 qsdsan-1.2.5/qsdsan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-31 23:14:10.000000 qsdsan-1.2.5/qsdsan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 23:14:11.142684 qsdsan-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2592 2023-01-31 23:13:07.000000 qsdsan-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.893013 qsdsan-1.3.0/
+-rw-rw-rw-   0        0        0     1254 2022-10-08 14:20:28.000000 qsdsan-1.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0    10566 2023-06-30 20:16:21.000000 qsdsan-1.3.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     5385 2022-10-08 14:20:28.000000 qsdsan-1.3.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0    16866 2023-06-04 13:25:54.000000 qsdsan-1.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1937 2022-10-08 14:20:28.000000 qsdsan-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      594 2022-10-08 14:20:28.000000 qsdsan-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11187 2023-06-30 20:19:46.893013 qsdsan-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9842 2023-06-04 13:25:54.000000 qsdsan-1.3.0/README.rst
+-rw-rw-rw-   0        0        0      475 2022-10-08 14:20:28.000000 qsdsan-1.3.0/pytest.ini
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.740694 qsdsan-1.3.0/qsdsan/
+-rw-rw-rw-   0        0        0     2899 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/__init__.py
+-rw-rw-rw-   0        0        0    31037 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/_component.py
+-rw-rw-rw-   0        0        0    33186 2022-12-29 15:48:21.000000 qsdsan-1.3.0/qsdsan/_components.py
+-rw-rw-rw-   0        0        0     8600 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/_construction.py
+-rw-rw-rw-   0        0        0     5949 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/_equipment.py
+-rw-rw-rw-   0        0        0    13906 2022-12-06 20:30:34.000000 qsdsan-1.3.0/qsdsan/_impact_indicator.py
+-rw-rw-rw-   0        0        0    31286 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/_impact_item.py
+-rw-rw-rw-   0        0        0    37186 2023-06-14 16:11:00.000000 qsdsan-1.3.0/qsdsan/_lca.py
+-rw-rw-rw-   0        0        0    52298 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/_process.py
+-rw-rw-rw-   0        0        0    24528 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/_sanstream.py
+-rw-rw-rw-   0        0        0    27356 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/_sanunit.py
+-rw-rw-rw-   0        0        0    20837 2023-06-14 16:11:00.000000 qsdsan-1.3.0/qsdsan/_tea.py
+-rw-rw-rw-   0        0        0    11720 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/_transportation.py
+-rw-rw-rw-   0        0        0    88948 2023-06-14 16:11:00.000000 qsdsan-1.3.0/qsdsan/_waste_stream.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.772189 qsdsan-1.3.0/qsdsan/data/
+-rw-rw-rw-   0        0        0    13259 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/_adm1.xlsx
+-rw-rw-rw-   0        0        0     7170 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/data/_components.tsv
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.778931 qsdsan-1.3.0/qsdsan/data/process_data/
+-rw-rw-rw-   0        0        0     1334 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/process_data/_adm1.tsv
+-rw-rw-rw-   0        0        0      822 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/process_data/_asm1.tsv
+-rw-rw-rw-   0        0        0     2583 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/process_data/_asm2d.tsv
+-rw-rw-rw-   0        0        0     1443 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/data/process_data/_pm2.tsv
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.799018 qsdsan-1.3.0/qsdsan/data/sanunit_data/
+-rw-rw-rw-   0        0        0     1051 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_anaerobic_baffled_reactor.tsv
+-rw-rw-rw-   0        0        0      923 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_anaerobic_digestion.tsv
+-rw-rw-rw-   0        0        0     1043 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_anaerobic_lagoon.tsv
+-rw-rw-rw-   0        0        0     2141 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_drying_bed.tsv
+-rw-rw-rw-   0        0        0     2918 2023-03-03 02:59:10.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_excretion.tsv
+-rw-rw-rw-   0        0        0     1178 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_facultative_lagoon.tsv
+-rw-rw-rw-   0        0        0   104004 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_inf_dry_2006.tsv
+-rw-rw-rw-   0        0        0      793 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_liquid_treatment_bed.tsv
+-rw-rw-rw-   0        0        0     1416 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_murt.tsv
+-rw-rw-rw-   0        0        0     1691 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_pit_latrine.tsv
+-rw-rw-rw-   0        0        0     1202 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_sedimentation_tank.tsv
+-rw-rw-rw-   0        0        0     1077 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_septic_tank.csv
+-rw-rw-rw-   0        0        0     1119 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_sludge_pasteurization.tsv
+-rw-rw-rw-   0        0        0      553 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_sludge_separator.tsv
+-rw-rw-rw-   0        0        0     1288 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_toilet.tsv
+-rw-rw-rw-   0        0        0     1403 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/_uddt.tsv
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.808464 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/
+-rw-rw-rw-   0        0        0     8043 2023-03-03 20:43:01.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_carbonizer_base.tsv
+-rw-rw-rw-   0        0        0     3980 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_controls.tsv
+-rw-rw-rw-   0        0        0      495 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_grinder.tsv
+-rw-rw-rw-   0        0        0     4120 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_hhx.tsv
+-rw-rw-rw-   0        0        0     1164 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_hhx_dryer.tsv
+-rw-rw-rw-   0        0        0      805 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_housing.tsv
+-rw-rw-rw-   0        0        0     1605 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_ion_exchange.tsv
+-rw-rw-rw-   0        0        0      804 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_ohx.tsv
+-rw-rw-rw-   0        0        0     3053 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_pollution_control.tsv
+-rw-rw-rw-   0        0        0      999 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_screw_press.tsv
+-rw-rw-rw-   0        0        0      997 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_struvite_precipitation.tsv
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.816874 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/
+-rw-rw-rw-   0        0        0      736 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_aerobic.tsv
+-rw-rw-rw-   0        0        0      723 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_anaerobic.tsv
+-rw-rw-rw-   0        0        0      678 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_anoxic.tsv
+-rw-rw-rw-   0        0        0     1152 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_bio_cost.tsv
+-rw-rw-rw-   0        0        0    14447 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_ecr.xlsx
+-rw-rw-rw-   0        0        0     1284 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_mbr.tsv
+-rw-rw-rw-   0        0        0    13527 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_primary.xlsx
+-rw-rw-rw-   0        0        0      843 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_solar.tsv
+-rw-rw-rw-   0        0        0      898 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_system.tsv
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.821140 qsdsan-1.3.0/qsdsan/data/sanunit_data/re/
+-rw-rw-rw-   0        0        0     1025 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_ecr.csv
+-rw-rw-rw-   0        0        0     1621 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_housing.csv
+-rw-rw-rw-   0        0        0     3559 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_ion_exchange.csv
+-rw-rw-rw-   0        0        0     1668 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_solar.csv
+-rw-rw-rw-   0        0        0     3413 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_system.csv
+-rw-rw-rw-   0        0        0     6847 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_ultrafiltration.csv
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.828650 qsdsan-1.3.0/qsdsan/equipments/
+-rw-rw-rw-   0        0        0     1065 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/equipments/__init__.py
+-rw-rw-rw-   0        0        0    10296 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/equipments/_aeration.py
+-rw-rw-rw-   0        0        0     2328 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/equipments/_column.py
+-rw-rw-rw-   0        0        0     3551 2023-06-14 17:49:37.000000 qsdsan-1.3.0/qsdsan/equipments/_electrode.py
+-rw-rw-rw-   0        0        0     1512 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/equipments/_encapsulation.py
+-rw-rw-rw-   0        0        0     1750 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/equipments/_machine.py
+-rw-rw-rw-   0        0        0     4117 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/equipments/_membrane.py
+-rw-rw-rw-   0        0        0     2071 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/equipments/_vacuum_pump.py
+-rw-rw-rw-   0        0        0     2717 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/equipments/_vertical_mixer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.836804 qsdsan-1.3.0/qsdsan/processes/
+-rw-rw-rw-   0        0        0      870 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/processes/__init__.py
+-rw-rw-rw-   0        0        0    30452 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/processes/_adm1.py
+-rw-rw-rw-   0        0        0    11547 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/processes/_aeration.py
+-rw-rw-rw-   0        0        0    11758 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/processes/_asm1.py
+-rw-rw-rw-   0        0        0    30686 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/processes/_asm2d.py
+-rw-rw-rw-   0        0        0    11867 2022-12-08 03:42:09.000000 qsdsan-1.3.0/qsdsan/processes/_decay.py
+-rw-rw-rw-   0        0        0    11113 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/processes/_kinetic_reaction.py
+-rw-rw-rw-   0        0        0    35864 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/processes/_pm2.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.871770 qsdsan-1.3.0/qsdsan/sanunits/
+-rw-rw-rw-   0        0        0     4654 2023-06-14 17:49:37.000000 qsdsan-1.3.0/qsdsan/sanunits/__init__.py
+-rw-rw-rw-   0        0        0    13312 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_abstract.py
+-rw-rw-rw-   0        0        0    26331 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_activated_sludge_process.py
+-rw-rw-rw-   0        0        0    37859 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_anaerobic_reactors.py
+-rw-rw-rw-   0        0        0    51946 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_biogenic_refinery.py
+-rw-rw-rw-   0        0        0    19434 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/sanunits/_clarifier.py
+-rw-rw-rw-   0        0        0    16379 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_combustion.py
+-rw-rw-rw-   0        0        0     2301 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_compressor.py
+-rw-rw-rw-   0        0        0     3461 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_crop_application.py
+-rw-rw-rw-   0        0        0     1539 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_distillation.py
+-rw-rw-rw-   0        0        0     9688 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_dynamic_influent.py
+-rw-rw-rw-   0        0        0    24306 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_eco_san.py
+-rw-rw-rw-   0        0        0    12440 2023-06-14 17:49:37.000000 qsdsan-1.3.0/qsdsan/sanunits/_electrochemical_cell.py
+-rw-rw-rw-   0        0        0    11721 2023-06-11 13:23:17.000000 qsdsan-1.3.0/qsdsan/sanunits/_encapsulation_bioreactor.py
+-rw-rw-rw-   0        0        0     9186 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/sanunits/_excretion.py
+-rw-rw-rw-   0        0        0     1495 2023-06-30 19:52:25.000000 qsdsan-1.3.0/qsdsan/sanunits/_flash.py
+-rw-rw-rw-   0        0        0    13364 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_heat_exchanging.py
+-rw-rw-rw-   0        0        0    23526 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_hydroprocessing.py
+-rw-rw-rw-   0        0        0    28992 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_hydrothermal.py
+-rw-rw-rw-   0        0        0    21867 2022-12-08 03:42:09.000000 qsdsan-1.3.0/qsdsan/sanunits/_internal_circulation_rx.py
+-rw-rw-rw-   0        0        0    33946 2023-06-04 13:32:38.000000 qsdsan-1.3.0/qsdsan/sanunits/_junction.py
+-rw-rw-rw-   0        0        0     7964 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_lagoon.py
+-rw-rw-rw-   0        0        0    47808 2022-12-08 03:42:09.000000 qsdsan-1.3.0/qsdsan/sanunits/_membrane_bioreactors.py
+-rw-rw-rw-   0        0        0    12474 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_membrane_distillation.py
+-rw-rw-rw-   0        0        0     3135 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/sanunits/_non_reactive.py
+-rw-rw-rw-   0        0        0    26719 2022-12-08 03:42:09.000000 qsdsan-1.3.0/qsdsan/sanunits/_polishing_filter.py
+-rw-rw-rw-   0        0        0    39311 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_pumping.py
+-rw-rw-rw-   0        0        0     8954 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_reactor.py
+-rw-rw-rw-   0        0        0    28231 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_reclaimer.py
+-rw-rw-rw-   0        0        0     2146 2023-01-02 19:15:09.000000 qsdsan-1.3.0/qsdsan/sanunits/_screening.py
+-rw-rw-rw-   0        0        0     6766 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_sedimentation.py
+-rw-rw-rw-   0        0        0     8043 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_septic_tank.py
+-rw-rw-rw-   0        0        0    13337 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_sludge_pasteurization.py
+-rw-rw-rw-   0        0        0    18475 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_sludge_thickening.py
+-rw-rw-rw-   0        0        0    25539 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_suspended_growth_bioreactor.py
+-rw-rw-rw-   0        0        0     6416 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_tanks.py
+-rw-rw-rw-   0        0        0    43871 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_toilets.py
+-rw-rw-rw-   0        0        0    13518 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_treatment_beds.py
+-rw-rw-rw-   0        0        0     6323 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/sanunits/_trucking.py
+-rw-rw-rw-   0        0        0    63183 2022-12-06 20:30:34.000000 qsdsan-1.3.0/qsdsan/stats.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.885013 qsdsan-1.3.0/qsdsan/utils/
+-rw-rw-rw-   0        0        0     1952 2022-12-08 03:42:09.000000 qsdsan-1.3.0/qsdsan/utils/__init__.py
+-rw-rw-rw-   0        0        0    16262 2022-12-08 03:42:09.000000 qsdsan-1.3.0/qsdsan/utils/cod.py
+-rw-rw-rw-   0        0        0     3884 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/utils/colors.py
+-rw-rw-rw-   0        0        0     5484 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/utils/components.py
+-rw-rw-rw-   0        0        0    20383 2022-12-06 20:30:34.000000 qsdsan-1.3.0/qsdsan/utils/construction.py
+-rw-rw-rw-   0        0        0    10168 2022-12-08 03:42:09.000000 qsdsan-1.3.0/qsdsan/utils/doc_examples.py
+-rw-rw-rw-   0        0        0     8011 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/utils/dynamics.py
+-rw-rw-rw-   0        0        0     1134 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/utils/formatting.py
+-rw-rw-rw-   0        0        0     3574 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/utils/loading.py
+-rw-rw-rw-   0        0        0     6025 2023-05-22 15:23:34.000000 qsdsan-1.3.0/qsdsan/utils/misc.py
+-rw-rw-rw-   0        0        0     8910 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/utils/model_eval.py
+-rw-rw-rw-   0        0        0     6573 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/utils/parsing.py
+-rw-rw-rw-   0        0        0     3914 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/utils/scope.py
+-rw-rw-rw-   0        0        0      482 2022-10-08 14:20:28.000000 qsdsan-1.3.0/qsdsan/utils/units_definition.txt
+-rw-rw-rw-   0        0        0     3754 2023-06-14 16:11:00.000000 qsdsan-1.3.0/qsdsan/utils/utilities.py
+-rw-rw-rw-   0        0        0     2028 2023-06-04 13:25:54.000000 qsdsan-1.3.0/qsdsan/utils/wwt_design.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.762627 qsdsan-1.3.0/qsdsan.egg-info/
+-rw-rw-rw-   0        0        0    11187 2023-06-30 20:19:46.000000 qsdsan-1.3.0/qsdsan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5090 2023-06-30 20:19:46.000000 qsdsan-1.3.0/qsdsan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 20:19:46.000000 qsdsan-1.3.0/qsdsan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-06-30 20:19:46.000000 qsdsan-1.3.0/qsdsan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-30 20:19:46.000000 qsdsan-1.3.0/qsdsan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 20:19:46.893013 qsdsan-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2590 2023-06-30 20:18:13.000000 qsdsan-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 20:19:46.892015 qsdsan-1.3.0/tests/
+-rw-rw-rw-   0        0        0     6582 2023-06-30 20:06:24.000000 qsdsan-1.3.0/tests/test_bst_units.py
+-rw-rw-rw-   0        0        0     3533 2022-12-08 03:42:09.000000 qsdsan-1.3.0/tests/test_component.py
+-rw-rw-rw-   0        0        0     1308 2022-10-08 14:20:28.000000 qsdsan-1.3.0/tests/test_dyn_sys.py
+-rw-rw-rw-   0        0        0     2599 2023-06-14 16:11:00.000000 qsdsan-1.3.0/tests/test_exposan.py
+-rw-rw-rw-   0        0        0     5257 2022-10-08 14:20:28.000000 qsdsan-1.3.0/tests/test_process.py
+-rw-rw-rw-   0        0        0     2045 2023-06-04 13:25:54.000000 qsdsan-1.3.0/tests/test_sanunit.py
+-rw-rw-rw-   0        0        0     2288 2022-10-08 14:20:28.000000 qsdsan-1.3.0/tests/test_waste_stream.py
```

### Comparing `qsdsan-1.2.5/AUTHORS.rst` & `qsdsan-1.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/CHANGELOG.rst` & `qsdsan-1.3.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Change Log
 ==========
 
 This document records notable changes to `QSDsan <https://github.com/QSD-Group/QSDsan>`_. We aim to follow `Semantic Versioning <https://semver.org/>`_.
 
 
-Ongoing
--------
+`1.3.0`_
+--------
+- Enhance and use QSDsan's capacity for dynamic simulation for emerging and benchmark configurations (see EXPOsan METAB and PM2 (on the algae branch) modules).
+- New publications
+
+	- The paper introducing `DMsan <https://doi.org/10.1021/acsenvironau.2c00067>`_, the package developed for decision-making of sanitation and resource recovery technologies, is published in *ACS Environmental Au*!
+	- QSDsan was used to evaluate the sustainability of the `NEWgenerator <https://doi.org/10.1021/acsenvironau.3c00001>`_ system as in this paper on *ACS Environmental Au*!
+
 - New modules
 
 	- :class:`qsdsan.processes.KineticReaction`
 
 - ``QSDsan`` now has a `website <https://qsdsan.com/>`_ to host all of the resources!
 - ``QSDsan``'s `documentation <https://qsdsan.readthedocs.io/en/latest/index.html>`_ is getting a new look!
 - Add new units to enable dynamic simulation of systems with multiple process models. Check out :class:`qsdsan.sanunits.Junction`, :class:`qsdsan.sanunits.ADMtoASM`, :class:`qsdsan.sanunits.ASMtoADM` and their use in the `interface system demo <https://github.com/QSD-Group/EXPOsan/tree/main/exposan/interface>`_.
 - In `online testing <https://github.com/QSD-Group/QSDsan/actions>`_, we dropped the test for Python 3.8 and added Python 3.10. The main developing environment for QSDsan is 3.9.
 
 
 `1.2.0`_
 --------
 - The `QSDsan paper <https://www.doi.org/10.1039/d2ew00455k>`_ is accepted by *Environmental Science: Water Research & Technology*!
-- The first paper using QSDsan for the design of sanitation is accepted by `ACS Environmental Au <https://pubs.acs.org/doi/10.1021/acsenvironau.2c00022>`_! The Biogenic Refinery system described in this paper is also available in ``QSDsan``/``EXPOsan`` now.
+- The first paper using QSDsan for the design of sanitation is accepted by *ACS Environmental Au*! Read the `Biogenic Refinery <https://pubs.acs.org/doi/10.1021/acsenvironau.2c00022>`_ paper and check out the system module in ``QSDsan``/``EXPOsan``.
 - Added multiple systems (including their unit operations), check out the details on the `Developed System <https://qsdsan.readthedocs.io/en/latest/Developed_Systems.html>`_ page!
 
 	- Biogenic Refinery
 	- Eco-San
 	- Reclaimer
 
 - Added the anaerobic digestion model no. 1 (ADM1) process model and the unit :class:`qsdsan.sanunits.AnaerobicCSTR`, the corresponding `system <https://github.com/QSD-Group/EXPOsan/tree/main/exposan/adm>`_ can be found in EXPOsan.
@@ -175,14 +181,15 @@
 .. Other links
 .. _latest: https://qsdsan.readthedocs.io/en/latest
 .. _beta: https://qsdsan.readthedocs.io/en/beta
 .. _EXPOsan:  https://github.com/QSD-Group/exposan
 .. _Trimmer et al.: https://doi.org/10.1021/acs.est.0c03296
 
 .. Commit links
+.. _1.3.0: https://github.com/QSD-Group/QSDsan/releases/tag/v1.3.0
 .. _1.2.0: https://github.com/QSD-Group/QSDsan/releases/tag/v1.2.0
 .. _1.1.0: https://github.com/QSD-Group/QSDsan/releases/tag/v1.1.0
 .. _1.0.0: https://github.com/QSD-Group/QSDsan/releases/tag/v1.0.0
 .. _0.3.0: https://github.com/QSD-Group/QSDsan/releases/tag/v0.3.0
 .. _0.2.0: https://github.com/QSD-Group/QSDsan/commit/286943eb206ebd89f58e50b9fdd1bed486e894ae
 .. _0.1.0: https://github.com/QSD-Group/QSDsan/commit/1c3d11d9f72421c8b5dbdf6b537775ca35ec65c0
 .. _0.0.3: https://github.com/QSD-Group/QSDsan/commit/e20222caccc58d9ee414ca08d8ec55f3a44ffca7
```

### Comparing `qsdsan-1.2.5/CODE_OF_CONDUCT.md` & `qsdsan-1.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/CONTRIBUTING.rst` & `qsdsan-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/LICENSE.txt` & `qsdsan-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/MANIFEST.in` & `qsdsan-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/PKG-INFO` & `qsdsan-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsdsan
-Version: 1.2.5
+Version: 1.3.0
 Summary: Quantitative Sustainable Design for sanitation and resource recovery systems
 Home-page: https://github.com/QSD-Group/QSDsan
 Author: Quantitative Sustainable Design Group
 Author-email: quantitative.sustainable.design@gmail.com
 License: UIUC
 Project-URL: Homepage, https://qsdsan.com
 Project-URL: Documentation, https://qsdsan.readthedocs.io
```

### Comparing `qsdsan-1.2.5/README.rst` & `qsdsan-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/__init__.py` & `qsdsan-1.3.0/qsdsan/__init__.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_component.py` & `qsdsan-1.3.0/qsdsan/_component.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_components.py` & `qsdsan-1.3.0/qsdsan/_components.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_construction.py` & `qsdsan-1.3.0/qsdsan/_construction.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_equipment.py` & `qsdsan-1.3.0/qsdsan/_equipment.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_impact_indicator.py` & `qsdsan-1.3.0/qsdsan/_impact_indicator.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_impact_item.py` & `qsdsan-1.3.0/qsdsan/_impact_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -542,17 +542,21 @@
     Parameters
     ----------
     ID : str
         ID of the item. If no ID is provided but its `linked_stream` is provided,
         the ID will be set as ID of the `linked_stream` with a suffix '_item'
     linked_stream : :class:`SanStream`
         The associated :class:`SanStream` for environmental impact calculation.
+    functional_unit : str
+        Functional unit of the impact item. The default is 'kg'.
     source : :class:`StreamImpactItem`
         If provided, all attributions and properties of this
         :class:`StreamImpactItem` will be copied from the provided source.
+    flow_getter : callable|float|int
+        If none specified, default to `SanStream.F_mass`.
     indicator_CFs : kwargs
         ImpactIndicators and their characterization factors (CFs).
 
     Tip
     ---
     For environmental impacts associated with construction and transportation,
     use :class:`ImpactItem` instead.
@@ -619,17 +623,19 @@
     Source          : methane_item
     Price           : None USD
     ImpactIndicators:
                                Characterization factors
     GlobalWarming (kg CO2-eq)                        28
     '''
 
-    __slots__ = ('_ID', '_linked_stream', '_functional_unit', '_CFs', '_source')
+    __slots__ = ('_ID', '_linked_stream', '_functional_unit', 
+                 '_CFs', '_source', '_flow_getter')
 
-    def __init__(self, ID='', linked_stream=None, source=None, **indicator_CFs):
+    def __init__(self, ID='', linked_stream=None, functional_unit='kg', 
+                 source=None, flow_getter=None, **indicator_CFs):
         self._linked_stream = None
         self.linked_stream = linked_stream
 
         CF_dct = self._format_CF_vals(**indicator_CFs)
 
         price = linked_stream.price if linked_stream else 0.
         returned = self._register_with_consistency_check(
@@ -642,18 +648,20 @@
             ID = self.linked_stream.ID + '_item'
         self._ID = ID
 
         if source:
             self.source = source
         else:
             self._source = None
-            self._functional_unit = auom('kg')
+            self._functional_unit = auom(functional_unit)
+            # self._functional_unit = auom('kg')
             self._CFs = {}
+            self.flow_getter = flow_getter
             for indicator, (value, unit) in CF_dct.items():
-                self.add_indicator(indicator, value, unit)
+                self.add_indicator(indicator, value, unit)        
 
 
     def __repr__(self):
         return f'<StreamImpactItem: {self.ID}>'
 
 
     def show(self):
@@ -714,14 +722,40 @@
             stream.stream_impact_item = new
             if not new_ID:
                 new.ID = f'{stream.ID}_item'
 
         return new
 
     __copy__ = copy
+    
+    @property
+    def flow_getter(self):
+        '''[callable] A function taking a `SanStream` object and returns the 
+        flow [functional unit/hr] for impact calculation. If None specified, default to
+        `SanStream.F_mass`.'''
+        if not hasattr(self, '_flow_getter'):
+            try: return self.source._flow_getter
+            except: self.flow_getter = None
+        return self._flow_getter
+    @flow_getter.setter
+    def flow_getter(self, f):
+        if f is None:
+            self._flow_getter = lambda ws: ws.F_mass
+        else:
+            if callable(f):
+                nargs = f.__code__.co_argcount
+                if nargs != 1:
+                    raise ValueError('flow_getter must take exactly 1 positional argument,'
+                                     'which is expected to be a `SanStream` object')
+                self._flow_getter = f
+            elif isinstance(f, (float, int)):
+                self._flow_getter = lambda ws: f
+            else:
+                raise TypeError('flow_getter must be a callable, or a number, or None, '
+                                f'not {type(f)}')
 
     @property
     def source(self):
         '''
         [:class:`StreamImpactItem`] If provided, all attributions and properties of this
         :class:`StreamImpactItem` will be copied from the provided source.
         ID of the impact item can be provided instead of the object.
@@ -794,18 +828,18 @@
         the ID will be set as ID of the `linked_stream` with a suffix '_item'.
         '''
         return self._ID
     @ID.setter
     def ID(self, i):
         self._ID = i
 
-    @property
-    def functional_unit(self):
-        '''[str] Functional unit of the item, set to 'kg'.'''
-        return auom('kg')
+    # @property
+    # def functional_unit(self):
+    #     '''[str] Functional unit of the item, set to 'kg'.'''
+    #     return auom('kg')
 
     @property
     def price(self):
         '''[float] Price of the linked stream.'''
         if self.linked_stream:
             return self.linked_stream.price
         else:
```

### Comparing `qsdsan-1.2.5/qsdsan/_lca.py` & `qsdsan-1.3.0/qsdsan/_lca.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     Now we can look at the total impacts associate with this system.
 
     >>> lca.show() # doctest: +ELLIPSIS
     LCA: sys (lifetime 10 yr)
     ...
     >>> # Retrieve impacts associated with a specific indicator
     >>> lca.get_total_impacts()[GWP.ID] # doctest: +ELLIPSIS
-    349737807.9765445...
+    349737809...
     >>> # Or breakdowns of the different category
     >>> lca.get_impact_table('Construction') # doctest: +SKIP
     >>> # Below is for testing purpose, you do not need it
     >>> lca.get_impact_table('Construction').to_dict() # doctest: +ELLIPSIS
     {'Quantity': ...
     >>> lca.get_impact_table('Transportation').to_dict() # doctest: +ELLIPSIS
     {'Quantity': ...
@@ -188,25 +188,25 @@
     {'Mass [kg]': ...
     >>> lca.get_impact_table('Construction').to_dict() # doctest: +ELLIPSIS
     {'Quantity': ...
 
     You can also allocate the impact based on mass, energy, value, or a ratio you like
 
     >>> lca.get_allocated_impacts(sys.products, allocate_by='mass')['waste_brine']['FossilEnergyConsumption'] # doctest: +ELLIPSIS
-    46018518.870...
+    46018554...
     >>> lca.get_allocated_impacts(sys.products, allocate_by='energy')['alcohols']['GlobalWarming'] # doctest: +ELLIPSIS
-    11063009.556...
+    11063012...
     >>> alcohols.price = 5
     >>> waste_brine.price = 1
     >>> GWP_alcohols = lca.get_allocated_impacts(sys.products, allocate_by='value')['alcohols']['GlobalWarming']
     >>> GWP_brine = lca.get_allocated_impacts(sys.products, allocate_by='value')['waste_brine']['GlobalWarming']
     >>> GWP_alcohols + GWP_brine # doctest: +ELLIPSIS
-    5469807.9765...
+    5469809...
     >>> lca.get_total_impacts(exclude=sys.products)['GlobalWarming'] # doctest: +ELLIPSIS
-    5469807.9765...
+    5469809...
     >>> # Clear all registries for testing purpose
     >>> from qsdsan.utils import clear_lca_registries
     >>> clear_lca_registries()
 
     See Also
     --------
     `SanUnit and System <https://qsdsan.readthedocs.io/en/latest/tutorials/SanUnit_and_System.html>`_
@@ -285,15 +285,18 @@
         '''Add other :class:`ImpactItem` in LCA.'''
         if isinstance(item, str):
             item = ImpactItem.get_item(item)
         fu = item.functional_unit
         if not callable(f_quantity):
             f = lambda: f_quantity
         else:
-            f = f_quantity
+            nargs = f_quantity.__code__.co_argcount
+            if nargs == 0: f = f_quantity
+            else: f = lambda: f_quantity(self)
+            # f = f_quantity
         quantity = f()
         if unit and unit != fu:
             try:
                 quantity = auom(unit).convert(quantity, fu)
             except:
                 raise ValueError(f'Conversion of the given unit {unit} to '
                                  f'item functional unit {fu} is not supported.')
@@ -421,28 +424,29 @@
                 if j.stream_impact_item:
                     j = ws.stream_impact_item
                 else: continue
             else:
                 ws = j.linked_stream
 
             if ws in exclude: continue
-
+            
+            F_mass = j.flow_getter(ws)
             for m, n in j.CFs.items():
                 if kind in ('all', 'total', 'net'):
                     pass
                 elif kind in ('direct', 'direct_emission'):
                     n = max(n, 0)
                 elif kind == 'offset':
                     n = min(n, 0)
                 else:
                     raise ValueError('kind can only be "all", "direct_emission", or "offset", '
                                      f'not "{kind}".')
                 if m not in impacts.keys():
                     continue
-                impacts[m] += n*time*ws.F_mass
+                impacts[m] += n*time*F_mass
         return impacts
 
     def get_other_impacts(self, time=None, time_unit='hr'):
         '''
         Return all additional impacts from "other" :class:`ImpactItems` objects,
         based on defined quantity.
         '''
@@ -545,15 +549,15 @@
         '''Return total impacts with certain units, normalized to a certain time frame. '''
         if not isinstance(units, Iterable):
             units = (units,)
         constr = self.get_construction_impacts(units, time, time_unit)
         trans = self.get_transportation_impacts(units, time, time_unit)
         stream_items = set(i for i in
                        sum((tuple(unit.ins+unit.outs) for unit in units), ())
-                       if i.impact_item)
+                       if i.stream_impact_item)
 
         s = self.get_stream_impacts(stream_items=stream_items, exclude=exclude,
                                      time=time, time_unit=time_unit)
         other = self.get_other_impacts()
         tot = constr.copy()
         for m in tot.keys():
             tot[m] += trans[m] + s[m] + other[m]
@@ -650,15 +654,15 @@
             headings = ['Stream', 'Mass [kg]', *ind_head]
             item_dct = dict.fromkeys(headings)
             for key in item_dct.keys():
                 item_dct[key] = []
             for ws_item in self.stream_inventory:
                 ws = ws_item.linked_stream
                 item_dct['Stream'].append(ws.ID)
-                mass = ws.F_mass * time
+                mass = ws_item.flow_getter(ws) * time
                 item_dct['Mass [kg]'].append(mass)
                 for ind in self.indicators:
                     if ind.ID in ws_item.CFs.keys():
                         impact = ws_item.CFs[ind.ID]*mass
                         item_dct[f'{ind.ID} [{ind.unit}]'].append(impact)
                         item_dct[f'Category {ind.ID} Ratio'].append(impact/(tot[ind.ID]*time_ratio))
                     else:
```

### Comparing `qsdsan-1.2.5/qsdsan/_process.py` & `qsdsan-1.3.0/qsdsan/_process.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_sanstream.py` & `qsdsan-1.3.0/qsdsan/_sanstream.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_sanunit.py` & `qsdsan-1.3.0/qsdsan/_sanunit.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_tea.py` & `qsdsan-1.3.0/qsdsan/_tea.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     >>> tea = qs.TEA(system=sys, discount_rate=0.05, start_year=2021,
     ...              lifetime=10, uptime_ratio=0.9,
     ...              system_add_OPEX=0.03)
     >>> # Your results maybe slightly different depending on the version of
     >>> # QSDsan's dependent packages (e.g., thermo)
     >>> tea.show() # doctest: +ELLIPSIS
     TEA: sys
-    NPV  : -258,...
+    NPV  : -259,...
 
     See Also
     --------
     `SanUnit and System <https://qsdsan.readthedocs.io/en/latest/tutorials/SanUnit_and_System.html>`_
 
     `TEA and LCA <https://qsdsan.readthedocs.io/en/latest/tutorials/TEA_and_LCA.html>`_
     '''
```

### Comparing `qsdsan-1.2.5/qsdsan/_transportation.py` & `qsdsan-1.3.0/qsdsan/_transportation.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/_waste_stream.py` & `qsdsan-1.3.0/qsdsan/_waste_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,15 @@
         >>> ws.show()
         WasteStream: ws
          phase: 'l', T: 250 K, P: 101325 Pa
          flow (g/hr): H2O  1.8e+06
          WasteStream-specific properties:
           pH         : 7.0
          Component concentrations (mg/L):
-          H2O          1012485.4
+          H2O          992181.4
         >>> ws.price
         8.0
         '''
         # Missing stream
         if isinstance(stream, MissingStream):
             new = MissingWasteStream.__new__(MissingWasteStream)
             new.__init__(stream._source, stream._sink)
@@ -937,18 +937,18 @@
         >>> ws1 = WasteStream('ws1', Water=100, NaCl=1)
         >>> ws2 = ws1.proxy('ws2')
         >>> ws2.mol is ws1.mol
         True
         >>> # Note that concentration is always calculated (mass/vol) upon request,
         >>> # so `ws2.conc is ws1.conc` will return False
         >>> import numpy as np
-        >>> np.all(ws2.conc==ws1.conc)
+        >>> np.all(list(ws2.conc==ws1.conc))
         True
         >>> ws1.imol['Water'] = 10000
-        >>> np.all(ws2.conc==ws1.conc)
+        >>> np.all(list(ws2.conc==ws1.conc))
         True
         '''
         new = SanStream.proxy(self, ID=ID)
         for slot in _ws_specific_slots:
             if slot == '_scope': continue # see notes in `copy`
             value = getattr(self, slot)
             setattr(new, slot, value)
@@ -987,16 +987,16 @@
         WasteStream: ws
          phase: 'l', T: 298.15 K, P: 101325 Pa
          flow (g/hr): S_O2  1e+05
                       H2O   1e+05
          WasteStream-specific properties:
           pH         : 7.0
          Component concentrations (mg/L):
-          S_O2         303021.4
-          H2O          303021.4
+          S_O2         450614.6
+          H2O          450614.6
         '''
         SanStream.mix_from(self, others, **kwargs)
 
         for slot in _ws_specific_slots:
             if not hasattr(self, slot):
                 continue
             #!!! This needs reviewing, might not be good to calculate some
```

### Comparing `qsdsan-1.2.5/qsdsan/data/_adm1.xlsx` & `qsdsan-1.3.0/qsdsan/data/_adm1.xlsx`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/_components.tsv` & `qsdsan-1.3.0/qsdsan/data/_components.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/process_data/_adm1.tsv` & `qsdsan-1.3.0/qsdsan/data/process_data/_adm1.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/process_data/_asm1.tsv` & `qsdsan-1.3.0/qsdsan/data/process_data/_asm1.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/process_data/_asm2d.tsv` & `qsdsan-1.3.0/qsdsan/data/process_data/_asm2d.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/process_data/_pm2.tsv` & `qsdsan-1.3.0/qsdsan/data/process_data/_pm2.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_anaerobic_baffled_reactor.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_anaerobic_baffled_reactor.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_anaerobic_digestion.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_anaerobic_digestion.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_anaerobic_lagoon.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_anaerobic_lagoon.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_drying_bed.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_drying_bed.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_excretion.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_excretion.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_facultative_lagoon.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_facultative_lagoon.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_inf_dry_2006.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_inf_dry_2006.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_liquid_treatment_bed.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_liquid_treatment_bed.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_murt.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_murt.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_pit_latrine.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_pit_latrine.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_sedimentation_tank.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_sedimentation_tank.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_septic_tank.csv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_septic_tank.csv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_sludge_pasteurization.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_sludge_pasteurization.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_sludge_separator.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_sludge_separator.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_toilet.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_toilet.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/_uddt.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/_uddt.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_carbonizer_base.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_carbonizer_base.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_controls.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_controls.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_hhx.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_hhx.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_hhx_dryer.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_hhx_dryer.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_housing.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_housing.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_ion_exchange.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_ion_exchange.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_ohx.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_ohx.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_pollution_control.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_pollution_control.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_screw_press.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_screw_press.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/br/_br_struvite_precipitation.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/br/_br_struvite_precipitation.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_aerobic.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_aerobic.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_anaerobic.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_anaerobic.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_anoxic.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_anoxic.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_bio_cost.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_bio_cost.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_ecr.xlsx` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_ecr.xlsx`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_mbr.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_mbr.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_primary.xlsx` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_primary.xlsx`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_solar.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_solar.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/es/_es_system.tsv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/es/_es_system.tsv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_ecr.csv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_ecr.csv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_housing.csv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_housing.csv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_ion_exchange.csv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_ion_exchange.csv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_solar.csv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_solar.csv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_system.csv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_system.csv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/data/sanunit_data/re/_re_ultrafiltration.csv` & `qsdsan-1.3.0/qsdsan/data/sanunit_data/re/_re_ultrafiltration.csv`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/equipments/__init__.py` & `qsdsan-1.3.0/qsdsan/equipments/__init__.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/equipments/_aeration.py` & `qsdsan-1.3.0/qsdsan/equipments/_aeration.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/equipments/_column.py` & `qsdsan-1.3.0/qsdsan/equipments/_column.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/equipments/_electrode.py` & `qsdsan-1.3.0/qsdsan/equipments/_electrode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# modifying electrode script to include 'reference' option
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 '''
 QSDsan: Quantitative Sustainable Design for sanitation and resource recovery systems
 
 This module is developed by:
@@ -26,15 +27,15 @@
     Refer to the example in :class:`~.sanunits.ElectroChemCell` for how to use this class.
 
     Parameters
     ----------
     N : int
         Number of units of the given electrode.
     electrode_type : str
-        Type of the electrode, can only be "anode" or "cathode".
+        Type of the electrode, can only be "anode", "cathode" or "reference".
     material: str
         Material of the electrode.
     unit_cost: float
         Unit cost of the electrode, will use default cost (if available)
         if not provided.
     surface_area : float
         Surface area of the electrode in m2.
@@ -81,22 +82,22 @@
         return self._N
     @N.setter
     def N(self, i):
         self._N = int(i)
 
     @property
     def electrode_type(self):
-        '''[str] Type of the electrode, either "anode" or "cathode".'''
+        '''[str] Type of the electrode, either "anode", "cathode" or "reference".'''
         return self._electrode_type
     @electrode_type.setter
     def electrode_type(self, i):
-        if i.lower() in ('anode', 'cathode'):
+        if i.lower() in ('anode', 'cathode', 'reference'):
             self._electrode_type = i
         else:
-            raise ValueError(f'Electrode can only be "anode" or "cathode", not "{i}".')
+            raise ValueError(f'Electrode can only be "anode", "cathode" or "reference", not "{i}".')
 
     @property
     def unit_cost(self):
         '''[float] Cost of one electrode.'''
         if self._unit_cost:
             return self._unit_cost
         cost = self._default_unit_cost.get(self.material)
```

### Comparing `qsdsan-1.2.5/qsdsan/equipments/_encapsulation.py` & `qsdsan-1.3.0/qsdsan/equipments/_encapsulation.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/equipments/_machine.py` & `qsdsan-1.3.0/qsdsan/equipments/_machine.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/equipments/_membrane.py` & `qsdsan-1.3.0/qsdsan/equipments/_membrane.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/equipments/_vacuum_pump.py` & `qsdsan-1.3.0/qsdsan/equipments/_vacuum_pump.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/equipments/_vertical_mixer.py` & `qsdsan-1.3.0/qsdsan/equipments/_vertical_mixer.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/processes/__init__.py` & `qsdsan-1.3.0/qsdsan/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/processes/_adm1.py` & `qsdsan-1.3.0/qsdsan/processes/_adm1.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/processes/_aeration.py` & `qsdsan-1.3.0/qsdsan/processes/_aeration.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/processes/_asm1.py` & `qsdsan-1.3.0/qsdsan/processes/_asm1.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/processes/_asm2d.py` & `qsdsan-1.3.0/qsdsan/processes/_asm2d.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/processes/_decay.py` & `qsdsan-1.3.0/qsdsan/processes/_decay.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/processes/_kinetic_reaction.py` & `qsdsan-1.3.0/qsdsan/processes/_kinetic_reaction.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/processes/_pm2.py` & `qsdsan-1.3.0/qsdsan/processes/_pm2.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/__init__.py` & `qsdsan-1.3.0/qsdsan/sanunits/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     Tori Morgan <vlmorgan@illinois.edu>
     
     Shion Watabe <swatabe2@illinois.edu>
     
     Lane To <lane20@illinois.edu>
     
     Smiti Mittal <smitimittal@gmail.com>
+    
+    Anna Kogler <akogler@stanford.edu>
 
     Jianan Feng <jiananf2@illinois.edu>
 
 This module is under the University of Illinois/NCSA Open Source License.
 Please refer to https://github.com/QSD-Group/QSDsan/blob/main/LICENSE.txt
 for license details.
 '''
```

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_abstract.py` & `qsdsan-1.3.0/qsdsan/sanunits/_abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 https://github.com/BioSTEAMDevelopmentGroup/biosteam
 
 This module is under the University of Illinois/NCSA Open Source License.
 Please refer to https://github.com/QSD-Group/QSDsan/blob/main/LICENSE.txt
 for license details.
 '''
 
-import numpy as np
+import numpy as np, thermosteam as tmo
+from warnings import warn
 from collections.abc import Iterable
 from biosteam.units import (
     Mixer as BSTMixer,
     Splitter as BSTSplitter,
     FakeSplitter as BSTFakeSplitter,
     ReversedSplitter as BSTReversedSplitter,
     )
@@ -150,14 +151,17 @@
         SanUnit.__init__(self, ID, ins, outs, thermo, init_with)
         self.phase = phase
 
         
     def _run(self):
         influent = self.ins[0]
         effluent = self.outs[0]
+        if isinstance(influent, tmo.MultiStream): # issue a warning
+            warn(f'MultiStream {influent.ID} converted to Stream in {self.ID}')
+            influent.as_stream()
         effluent.copy_like(influent)
         effluent.phase = self.phase
         
     @property
     def phase(self):
         return self._phase
     @phase.setter
```

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_activated_sludge_process.py` & `qsdsan-1.3.0/qsdsan/sanunits/_activated_sludge_process.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_anaerobic_reactors.py` & `qsdsan-1.3.0/qsdsan/sanunits/_anaerobic_reactors.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,20 @@
     @property
     def fixed_headspace_P(self):
         '''Headspace total pressure [bar].'''
         return self._fixed_P_gas
     @fixed_headspace_P.setter
     def fixed_headspace_P(self, b):
         self._fixed_P_gas = bool(b)
-        
+    
+    def set_retention_efficacy(self, i):
+        if i < 0 or i > 1:
+            raise ValueError('retention efficacy must be within [0,1]')
+        self._f_retain = (self._f_retain > 0) * i
+    
     @property
     def state(self):
         '''The state of the anaerobic CSTR, including component concentrations [kg/m3],
         biogas concentrations in the headspace [M biogas], and liquid flow rate [m^3/d].'''
         if self._state is None: return None
         else:
             return dict(zip(self._state_keys, self._state))
```

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_biogenic_refinery.py` & `qsdsan-1.3.0/qsdsan/sanunits/_biogenic_refinery.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_clarifier.py` & `qsdsan-1.3.0/qsdsan/sanunits/_clarifier.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_combustion.py` & `qsdsan-1.3.0/qsdsan/sanunits/_combustion.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_compressor.py` & `qsdsan-1.3.0/qsdsan/sanunits/_compressor.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_crop_application.py` & `qsdsan-1.3.0/qsdsan/sanunits/_crop_application.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_distillation.py` & `qsdsan-1.3.0/qsdsan/sanunits/_distillation.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_dynamic_influent.py` & `qsdsan-1.3.0/qsdsan/sanunits/_dynamic_influent.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_eco_san.py` & `qsdsan-1.3.0/qsdsan/sanunits/_eco_san.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_encapsulation_bioreactor.py` & `qsdsan-1.3.0/qsdsan/sanunits/_encapsulation_bioreactor.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_excretion.py` & `qsdsan-1.3.0/qsdsan/sanunits/_excretion.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_flash.py` & `qsdsan-1.3.0/qsdsan/sanunits/_flash.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_heat_exchanging.py` & `qsdsan-1.3.0/qsdsan/sanunits/_heat_exchanging.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 https://github.com/BioSTEAMDevelopmentGroup/biosteam
 
 This module is under the University of Illinois/NCSA Open Source License.
 Please refer to https://github.com/QSD-Group/QSDsan/blob/main/LICENSE.txt
 for license details.
 '''
 
-import biosteam as bst
 from warnings import warn
 from math import ceil, pi
-from biosteam.units import HXprocess as HXP, HXutility as HXU
-from biosteam.units.facilities import HeatExchangerNetwork as HXN
+from biosteam import HeatExchangerNetwork as HXN, HXprocess as HXP, HXutility as HXU
 from biosteam.units.design_tools.specification_factors import material_densities_lb_per_ft3
 from biosteam.exceptions import bounds_warning, DesignWarning
 from biosteam.units.design_tools import flash_vessel_design
 from .. import SanUnit, Construction
 from ..utils import auom
 
 __all__ = ('HeatExchangerNetwork', 'HXprocess', 'HXutility',)
```

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_hydroprocessing.py` & `qsdsan-1.3.0/qsdsan/sanunits/_hydroprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,16 +168,16 @@
             hc_out.imass[name] = hydrocarbon_mass*ratio
         
         hc_out.imass['H2'] = heavy_oil.F_mass*self.hydrogen_rxned_to_heavy_oil*(self.hydrogen_excess - 1)
         
         hc_out.P = heavy_oil.P
         hc_out.T = self.HCrxn_T
         
-        hc_out.vle(T=hc_out.T, P=hc_out.P)
-        
+        # hc_out.vle(T=hc_out.T, P=hc_out.P)
+
         cmps = self.components
         C_in = 0
         total_num = len(list(cmps))
         for num in range(total_num):
             C_in += heavy_oil.imass[str(list(cmps)[num])]*list(cmps)[num].i_C
             
         C_out = self.hydrocarbon_C
@@ -426,15 +426,15 @@
         # use water to represent HT aqueous phase,
         # C and N can be calculated base on MB closure.
         
         ht_out.P = biocrude.P
         
         ht_out.T = self.HTrxn_T
         
-        ht_out.vle(T=ht_out.T, P=ht_out.P)
+        # ht_out.vle(T=ht_out.T, P=ht_out.P)
         
         if self.HTaqueous_C < -0.1*self.HTL.WWTP.sludge_C:
             raise Exception('carbon mass balance is out of +/- 10% for the whole system')
         # allow +/- 10% out of mass balance
         # should be no C in the aqueous phase, the calculation here is just for MB
         
         if self.HTaqueous_N < -0.1*self.HTL.WWTP.sludge_N:
```

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_hydrothermal.py` & `qsdsan-1.3.0/qsdsan/sanunits/_hydrothermal.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,15 +161,17 @@
         chg_out, catalyst_out = self.outs
         
         catalyst_in.imass['CHG_catalyst'] = chg_in.F_mass/self.WHSV/self.catalyst_lifetime
         catalyst_in.phase = 's'
         catalyst_out.copy_like(catalyst_in)
         # catalysts amount is quite low compared to the main stream, therefore do not consider
         # heating/cooling of catalysts
-            
+        
+        chg_out.phase='g'
+        
         cmps = self.components
         gas_C_ratio = 0
         for name, ratio in self.gas_composition.items():
             gas_C_ratio += ratio*cmps[name].i_C
             
         gas_mass = chg_in.imass['C']*self.gas_C_2_total_C/gas_C_ratio
         
@@ -177,15 +179,17 @@
             chg_out.imass[name] = gas_mass*ratio
                 
         chg_out.imass['H2O'] = chg_in.F_mass - gas_mass
         # all C, N, and P are accounted in H2O here, but will be calculated as properties.
         
         chg_out.T = self.cool_temp
         chg_out.P = self.pump_pressure
-        
+
+        # chg_out.vle(T=chg_out.T, P=chg_out.P)
+
     @property
     def CHGout_C(self):
         # not include carbon in gas phase
         return self.ins[0].imass['C']*(1 - self.gas_C_2_total_C)
     
     @property
     def CHGout_N(self):
@@ -508,36 +512,36 @@
                          _source.ins[0]._source
         
         dewatered_sludge_afdw = dewatered_sludge.imass['Sludge_lipid'] +\
                                 dewatered_sludge.imass['Sludge_protein'] +\
                                 dewatered_sludge.imass['Sludge_carbo']
         # just use afdw in revised MCA model, other places use dw
         
-        afdw_lipid_ratio = self.WWTP.sludge_afdw_lipid
-        afdw_protein_ratio = self.WWTP.sludge_afdw_protein
-        afdw_carbo_ratio = self.WWTP.sludge_afdw_carbo
+        self.afdw_lipid_ratio = self.WWTP.sludge_afdw_lipid
+        self.afdw_protein_ratio = self.WWTP.sludge_afdw_protein
+        self.afdw_carbo_ratio = self.WWTP.sludge_afdw_carbo
 
         # the following calculations are based on revised MCA model
-        biochar.imass['Biochar'] = 0.377*afdw_carbo_ratio*dewatered_sludge_afdw
+        biochar.imass['Biochar'] = 0.377*self.afdw_carbo_ratio*dewatered_sludge_afdw
         
-        HTLaqueous.imass['HTLaqueous'] = (0.481*afdw_protein_ratio +\
-                                          0.154*afdw_lipid_ratio)*\
+        HTLaqueous.imass['HTLaqueous'] = (0.481*self.afdw_protein_ratio +\
+                                          0.154*self.afdw_lipid_ratio)*\
                                           dewatered_sludge_afdw
         # HTLaqueous is TDS in aqueous phase
         # 0.377, 0.481, and 0.154 don't have uncertainties because they are calculated values
          
-        gas_mass = (self.protein_2_gas*afdw_protein_ratio + self.carbo_2_gas*afdw_carbo_ratio)*\
+        gas_mass = (self.protein_2_gas*self.afdw_protein_ratio + self.carbo_2_gas*self.afdw_carbo_ratio)*\
                        dewatered_sludge_afdw
                        
         for name, ratio in self.gas_composition.items():
             offgas.imass[name] = gas_mass*ratio
             
-        biocrude.imass['Biocrude'] = (self.protein_2_biocrude*afdw_protein_ratio +\
-                                      self.lipid_2_biocrude*afdw_lipid_ratio +\
-                                      self.carbo_2_biocrude*afdw_carbo_ratio)*\
+        biocrude.imass['Biocrude'] = (self.protein_2_biocrude*self.afdw_protein_ratio +\
+                                      self.lipid_2_biocrude*self.afdw_lipid_ratio +\
+                                      self.carbo_2_biocrude*self.afdw_carbo_ratio)*\
                                       dewatered_sludge_afdw
         biocrude.imass['H2O'] = biocrude.imass['Biocrude']/(1 -\
                                 self.biocrude_moisture_content) -\
                                 biocrude.imass['Biocrude']
                                 
         HTLaqueous.imass['H2O'] = dewatered_sludge.F_mass - biochar.F_mass -\
                                   biocrude.F_mass - gas_mass - HTLaqueous.imass['HTLaqueous']
@@ -549,14 +553,32 @@
         
         biochar.P = self.biochar_pre
         HTLaqueous.P = self.HTLaqueous_pre
         biocrude.P = self.biocrude_pre
         offgas.P = self.offgas_pre
         
         for stream in self.outs : stream.T = self.heat_exchanger.T
+        
+    @property
+    def biocrude_yield(self):
+        return self.protein_2_biocrude*self.afdw_protein_ratio +\
+               self.lipid_2_biocrude*self.afdw_lipid_ratio +\
+               self.carbo_2_biocrude*self.afdw_carbo_ratio
+
+    @property
+    def aqueous_yield(self):
+        return 0.481*self.afdw_protein_ratio + 0.154*self.afdw_lipid_ratio
+    
+    @property
+    def biochar_yield(self):
+        return 0.377*self.afdw_carbo_ratio
+    
+    @property
+    def gas_yield(self):
+        return self.protein_2_gas*self.afdw_protein_ratio + self.carbo_2_gas*self.afdw_carbo_ratio
 
     @property
     def biocrude_C_ratio(self):
         return (self.WWTP.AOSc*self.biocrude_C_slope + self.biocrude_C_intercept)/100 # [2]
     
     @property
     def biocrude_H_ratio(self):
@@ -632,16 +654,16 @@
         hx_ins0, hx_outs0 = hx.ins[0], hx.outs[0]
         hx_ins0.mix_from((self.outs[1], self.outs[2], self.outs[3]))
         hx_outs0.copy_like(hx_ins0)
         hx_ins0.T = self.ins[0].T # temperature before/after HTL are similar
         hx_outs0.T = hx.T
         hx_ins0.P = hx_outs0.P = self.outs[0].P # cooling before depressurized, heating after pressurized
         # in other words, both heating and cooling are performed under relatively high pressure
-        hx_ins0.vle(T=hx_ins0.T, P=hx_ins0.P)
-        hx_outs0.vle(T=hx_outs0.T, P=hx_outs0.P)
+        # hx_ins0.vle(T=hx_ins0.T, P=hx_ins0.P)
+        # hx_outs0.vle(T=hx_outs0.T, P=hx_outs0.P)
         hx.simulate_as_auxiliary_exchanger(ins=hx.ins, outs=hx.outs)
 
         self.P = self.ins[0].P
         Reactor._design(self)
         Design['Solid filter and separator weight'] = 0.2*Design['Weight']*Design['Number of reactors'] # assume stainless steel
         # based on [6], case D design table, the purchase price of solid filter and separator to
         # the purchase price of HTL reactor is around 0.2, therefore, assume the weight of solid filter
```

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_internal_circulation_rx.py` & `qsdsan-1.3.0/qsdsan/sanunits/_internal_circulation_rx.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_junction.py` & `qsdsan-1.3.0/qsdsan/sanunits/_junction.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_lagoon.py` & `qsdsan-1.3.0/qsdsan/sanunits/_lagoon.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_membrane_bioreactors.py` & `qsdsan-1.3.0/qsdsan/sanunits/_membrane_bioreactors.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_membrane_distillation.py` & `qsdsan-1.3.0/qsdsan/sanunits/_membrane_distillation.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_non_reactive.py` & `qsdsan-1.3.0/qsdsan/sanunits/_non_reactive.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_polishing_filter.py` & `qsdsan-1.3.0/qsdsan/sanunits/_polishing_filter.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_pumping.py` & `qsdsan-1.3.0/qsdsan/sanunits/_pumping.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_reactor.py` & `qsdsan-1.3.0/qsdsan/sanunits/_reactor.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_reclaimer.py` & `qsdsan-1.3.0/qsdsan/sanunits/_reclaimer.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_screening.py` & `qsdsan-1.3.0/qsdsan/sanunits/_screening.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_sedimentation.py` & `qsdsan-1.3.0/qsdsan/sanunits/_sedimentation.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_septic_tank.py` & `qsdsan-1.3.0/qsdsan/sanunits/_septic_tank.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_sludge_pasteurization.py` & `qsdsan-1.3.0/qsdsan/sanunits/_sludge_pasteurization.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_sludge_thickening.py` & `qsdsan-1.3.0/qsdsan/sanunits/_sludge_thickening.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_suspended_growth_bioreactor.py` & `qsdsan-1.3.0/qsdsan/sanunits/_suspended_growth_bioreactor.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_tanks.py` & `qsdsan-1.3.0/qsdsan/sanunits/_tanks.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_toilets.py` & `qsdsan-1.3.0/qsdsan/sanunits/_toilets.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_treatment_beds.py` & `qsdsan-1.3.0/qsdsan/sanunits/_treatment_beds.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/sanunits/_trucking.py` & `qsdsan-1.3.0/qsdsan/sanunits/_trucking.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/stats.py` & `qsdsan-1.3.0/qsdsan/stats.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/__init__.py` & `qsdsan-1.3.0/qsdsan/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/cod.py` & `qsdsan-1.3.0/qsdsan/utils/cod.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/colors.py` & `qsdsan-1.3.0/qsdsan/utils/colors.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/components.py` & `qsdsan-1.3.0/qsdsan/utils/components.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/construction.py` & `qsdsan-1.3.0/qsdsan/utils/construction.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/doc_examples.py` & `qsdsan-1.3.0/qsdsan/utils/doc_examples.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/dynamics.py` & `qsdsan-1.3.0/qsdsan/utils/dynamics.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/formatting.py` & `qsdsan-1.3.0/qsdsan/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/loading.py` & `qsdsan-1.3.0/qsdsan/utils/loading.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/misc.py` & `qsdsan-1.3.0/qsdsan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/model_eval.py` & `qsdsan-1.3.0/qsdsan/utils/model_eval.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/parsing.py` & `qsdsan-1.3.0/qsdsan/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/scope.py` & `qsdsan-1.3.0/qsdsan/utils/scope.py`

 * *Files identical despite different names*

### Comparing `qsdsan-1.2.5/qsdsan/utils/utilities.py` & `qsdsan-1.3.0/qsdsan/utils/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
     Examples
     --------
     >>> from qsdsan.utils import create_example_system, sum_system_utility
     >>> sys = create_example_system()
     >>> sys.simulate()
     >>> sum_system_utility(sys, utility='heating', result_unit='kJ/yr') # doctest: +ELLIPSIS
-    463359.875...
+    463479...
     >>> sum_system_utility(sys, utility='cooling', result_unit='GJ/yr') # doctest: +NUMBER
     0.0
     >>> # Exclude a certain unit
     >>> sum_system_utility(sys, utility='power') # doctest: +ELLIPSIS
-    0.9156667...
+    0.9157...
     >>> sum_system_utility(sys, utility='power', exclude_units=(sys.units[0],)) # doctest: +ELLIPSIS
-    0.6611597...
+    0.6612...
     '''
 
     hrs = operating_hours or getattr(system, 'operating_hours') or 1.
     utility = utility.lower()
     try: iter(exclude_units)
     except: exclude_units = (exclude_units,)
     units = [i for i in system.units if i not in exclude_units]
```

### Comparing `qsdsan-1.2.5/qsdsan/utils/wwt_design.py` & `qsdsan-1.3.0/qsdsan/utils/wwt_design.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 This module is under the University of Illinois/NCSA Open Source License.
 Please refer to https://github.com/QSD-Group/QSDsan/blob/main/LICENSE.txt
 for license details.
 '''
 
 __all__ = ('get_SRT',)
 
-def get_SRT(system, biomass_IDs, active_unit_IDs=None):
+def get_SRT(system, biomass_IDs, wastage=None, active_unit_IDs=None):
     """
     Estimate sludge residence time (SRT) of an activated sludge system.
 
     Parameters
     ----------
     system : obj
         The system whose SRT will be calculated for.
     biomass_IDs : tuple[str]
-        Component IDs of active biomass
+        Component IDs of active biomass.
+    wastage : iterable[:class:`WasteStream`]
+        Streams with wasted biomass.
     active_unit_IDs : tuple[str], optional
         IDs of activated sludge units. The default is None, meaning to include
         all units in the system.
 
     Returns
     -------
     [float] Estimated sludge residence time in days.
@@ -39,13 +41,14 @@
         [2] The units included in calculation must all have :func:`get_retained_mass`
         to calculate the retained biomass.
 
     Examples
     --------
     `bsm1 system <https://github.com/QSD-Group/EXPOsan/blob/main/exposan/bsm1/system.py>`_
     """
+    if wastage is None: wastage = [ws for ws in system.products if ws.phase in ('l','s')]
     waste = sum([ws.composite('solids', subgroup=biomass_IDs)*ws.F_vol*24 \
-                 for ws in system.products if ws.phase in ('l','s')])
+                 for ws in wastage])
     units = system.units if active_unit_IDs is None \
         else [u for u in system.units if u.ID in active_unit_IDs]
     retain = sum([u.get_retained_mass(biomass_IDs) for u in units if u.isdynamic])
     return retain/waste
```

### Comparing `qsdsan-1.2.5/qsdsan.egg-info/PKG-INFO` & `qsdsan-1.3.0/qsdsan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsdsan
-Version: 1.2.5
+Version: 1.3.0
 Summary: Quantitative Sustainable Design for sanitation and resource recovery systems
 Home-page: https://github.com/QSD-Group/QSDsan
 Author: Quantitative Sustainable Design Group
 Author-email: quantitative.sustainable.design@gmail.com
 License: UIUC
 Project-URL: Homepage, https://qsdsan.com
 Project-URL: Documentation, https://qsdsan.readthedocs.io
```

### Comparing `qsdsan-1.2.5/qsdsan.egg-info/SOURCES.txt` & `qsdsan-1.3.0/qsdsan.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -142,8 +142,15 @@
 qsdsan/utils/loading.py
 qsdsan/utils/misc.py
 qsdsan/utils/model_eval.py
 qsdsan/utils/parsing.py
 qsdsan/utils/scope.py
 qsdsan/utils/units_definition.txt
 qsdsan/utils/utilities.py
-qsdsan/utils/wwt_design.py
+qsdsan/utils/wwt_design.py
+tests/test_bst_units.py
+tests/test_component.py
+tests/test_dyn_sys.py
+tests/test_exposan.py
+tests/test_process.py
+tests/test_sanunit.py
+tests/test_waste_stream.py
```

### Comparing `qsdsan-1.2.5/setup.py` & `qsdsan-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 '''
 QSDsan: Quantitative Sustainable Design for sanitation and resource recovery systems
 
 This module is developed by:
+
     Yalin Li <mailto.yalin.li@gmail.com>
 
 This module is under the University of Illinois/NCSA Open Source License.
 Please refer to https://github.com/QSD-Group/QSDsan/blob/main/LICENSE.txt
 for license details.
 '''
 
 from setuptools import setup
 
 setup(
     name='qsdsan',
     packages=['qsdsan'],
-    version='1.2.5',
+    version='1.3.0',
     license='UIUC',
     author='Quantitative Sustainable Design Group',
     author_email='quantitative.sustainable.design@gmail.com',
     description='Quantitative Sustainable Design for sanitation and resource recovery systems',
     long_description=open('README.rst', encoding='utf-8').read(),
     url='https://github.com/QSD-Group/QSDsan',
     project_urls={
         'Homepage': 'https://qsdsan.com',
         'Documentation': 'https://qsdsan.readthedocs.io',
         'Repository': 'https://github.com/QSD-Group/QSDsan',
     },
     install_requires=[
-        'biosteam>=2.36.1',
-        'thermosteam>=0.32.0',
+        'biosteam>=2.37.4',
+        'thermosteam>=0.35.1',
         'matplotlib>=3.3.2',
         'pandas>=1.3.2',
         'SALib>=1.4.5',
         'scikit-learn',
         'scipy>=1.7.1',
         'seaborn',
         'sympy>=1.8',
     ],
-    package_data=
-        {'qsdsan': [
+    package_data={
+        'qsdsan': [
             'data/*',
             'data/process_data/*',
             'data/sanunit_data/*',
             'data/sanunit_data/br/*',
             'data/sanunit_data/es/*',
             'data/sanunit_data/re/*',
             'equipments/*',
             'processes/*',
             'sanunits/*',
             'utils/*',
-        ]},
+    ]},
     classifiers=[
         'License :: OSI Approved :: University of Illinois/NCSA Open Source License',
         'Environment :: Console',
         'Topic :: Education',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Mathematics',
```

