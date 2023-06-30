# Comparing `tmp/scinumtools-1.5.4.tar.gz` & `tmp/scinumtools-1.5.5.tar.gz`

## Comparing `scinumtools-1.5.4.tar` & `scinumtools-1.5.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.4/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.5.4/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.5.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/units/BaseUnitsClass.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/units/DimensionsClass.py
--rw-r--r--   0        0        0    11114 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/units/RatioClass.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/units/UnitClass.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.5.4/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/README.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/cached_data.npy
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/pyproject.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/requirements.txt
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/test_data.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/test_math.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/test_physics.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/test_stats.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/test_struct.py
--rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/test_units.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/data/ImageClass.py
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/data/PlottingClass.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/math/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/math/solver/AtomClass.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/math/solver/ExpressionClass.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/math/solver/OperatorClass.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/math/solver/SolverClass.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/math/solver/TokensClass.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/math/solver/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/phys/ConstantsClass.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/phys/__init__.py
--rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/phys/units/QuantityClass.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/phys/units/UnitConverters.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/phys/units/UnitList.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/phys/units/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.5.4/tests/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.5.4/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.5.4/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.5.4/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.5/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.5.5/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.5.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/BaseUnitsClass.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/DimensionsClass.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/FractionClass.py
+-rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/UnitClass.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.5.5/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/cached_data.npy
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/pyproject.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/requirements.txt
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_data.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_math.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_physics.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_stats.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_struct.py
+-rw-r--r--   0        0        0    10619 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/test_units.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/data/ImageClass.py
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/__init__.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/AtomClass.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/ExpressionClass.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/OperatorClass.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/SolverClass.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/TokensClass.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/math/solver/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/ConstantsClass.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/__init__.py
+-rw-r--r--   0        0        0     9181 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/units/QuantityClass.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/units/UnitConverters.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/units/UnitList.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/phys/units/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.5.5/tests/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 scinumtools-1.5.5/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.5.5/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.5.5/PKG-INFO
```

### Comparing `scinumtools-1.5.4/.github/workflows/python-publish.yml` & `scinumtools-1.5.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/data/CachingClass.py` & `scinumtools-1.5.5/src/scinumtools/data/CachingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/data/ImageClass.py` & `scinumtools-1.5.5/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.5.5/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.5.5/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.5.5/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.5.5/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.5.5/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.5.5/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.5.5/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/phys/units/BaseUnitsClass.py` & `scinumtools-1.5.5/src/scinumtools/phys/units/BaseUnitsClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 from dataclasses import dataclass, field, fields
-from .RatioClass import Ratio
+from .FractionClass import Fraction
 
 @dataclass
 class BaseUnits:
 
     baseunits: dict = field(default_factory=dict)
     symbol: str = ':'
 
     def __post_init__(self):
         for unit,exp in self.baseunits.items():
-            if not isinstance(exp, Ratio):
-                self.baseunits[unit] = Ratio(exp)
+            if not isinstance(exp, Fraction):
+                self.baseunits[unit] = Fraction(exp)
         # remove zero dimensions
         for unit in list(self.baseunits.keys()):
             if self.baseunits[unit].num==0:
                 del self.baseunits[unit]
 
     def __str__(self):
         baseunits = []
@@ -43,18 +43,18 @@
     
     def __sub__(self, other):
         baseunits = dict(self.baseunits)
         for unit,exp in other.baseunits.items():
             baseunits[unit] = baseunits[unit]-exp if unit in baseunits else -exp
         return BaseUnits(baseunits)
 
-    def __mul__(self, power):
+    def __mul__(self, other):
         baseunits = dict(self.baseunits)
         for unit,exp in self.baseunits.items():
-            baseunits[unit] *= power
+            baseunits[unit] *= other
         return BaseUnits(baseunits)
 
     def __truediv__(self, div):
         baseunits = dict(self.baseunits)
         for unit,exp in self.baseunits.items():
             baseunits[unit] /= div
         return BaseUnits(baseunits)
```

### Comparing `scinumtools-1.5.4/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.5.5/src/scinumtools/phys/units/QuantityClass.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ...structs.ParameterClass import ParameterDict
 from ...math.solver import ExpressionSolver, AtomBase, OperatorPar, OperatorMul, OperatorTruediv
 from .UnitList import *
 from .UnitConverters import *
 from .DimensionsClass import Dimensions
 from .BaseUnitsClass import BaseUnits
-from .RatioClass import Ratio
+from .FractionClass import Fraction
 
 class Quantity:
     prefixes: dict            # list of prefixes 
     unitlist: dict            # list of units
     
     magnitude: float          # quantity magnitude
     dimensions: Dimensions    # quantity dimensions
@@ -135,16 +135,22 @@
 
     def __truediv__(self, other):
         return self._truediv(self, other)
     
     def __rtruediv__(self, other):
         return self._truediv(other, self)
     
-    def __pow__(self, power):
-        magnitude = self.magnitude**power
+    def __pow__(self, power: Union[float,int,tuple,Fraction]):
+        if isinstance(power, tuple):
+            exp = power[0]/power[1]
+        elif isinstance(power, Fraction):
+            exp = power.num/power.den
+        else:
+            exp = power
+        magnitude = self.magnitude**exp
         dimensions = self.dimensions*power
         baseunits = self.baseunits*power
         return Quantity(magnitude, dimensions, baseunits)
 
     def __neg__(self):
         return Quantity(-self.magnitude, self.dimensions, self.baseunits)
     
@@ -179,15 +185,21 @@
         if baseunits:
             return f"Quantity({magnitude:s} {baseunits})"
         else:
             return f"Quantity({magnitude:s})"
 
     def __array__(self):
         return np.array(self.magnitude)
-
+    
+    def __array_prepare__(self, array, context=None):
+        if context:
+            if context[0] in [np.sin, np.cos, np.tan]:
+                array = np.array(context[1][0].to('rad'))
+        return array
+    
     def __array_wrap__(self, out_arr, context=None):
         if out_arr.ndim==0:
             out_arr = float(out_arr)
         dimensions = self.dimensions
         baseunits = self.baseunits
         if context:
             if context[0]==np.sqrt:
@@ -195,29 +207,32 @@
                 baseunits /= 2
             elif context[0]==np.cbrt:
                 dimensions /= 3
                 baseunits /= 3
             elif context[0]==np.power:
                 dimensions *= context[1][1]
                 baseunits *= context[1][1]
+            elif context[0] in [np.sin, np.cos, np.tan]:
+                dimensions = Dimensions()
+                baseunits = BaseUnits()
         return Quantity(out_arr, dimensions, baseunits)
     
     def _atom_parser(self, string=None):
         # parse number
         m = re.match(r'^[-]?([0-9.]+)(e([0-9+-]+)|)$', str(string))
         if m:
             magnitude = float(string)
             return Quantity(magnitude)
         # parse unit
         string_bak = string
         exp, base, prefix = '', '', ''
         symbol, string = string[-1], ' '+string[:-1]
         # parse exponent
         while len(string):
-            if not re.match('^[0-9'+Ratio.symbol+'+-]{1}$', symbol):
+            if not re.match('^[0-9'+Fraction.symbol+'+-]{1}$', symbol):
                 break
             exp = symbol+exp
             symbol, string = string[-1], string[:-1]
         # parse unit symbol
         unitkeys = self.unitlist.keys()
         while len(string):
             nbase = len(base)+1
@@ -239,33 +254,34 @@
                 break
         if prefix:
             if prefix not in self.prefixes.keys():
                 raise Exception(f"Unknown unit prefix:", string_bak)
             magnitude *= self.prefixes[prefix].magnitude
             unitid = f"{prefix:s}{BaseUnits.symbol}{unitid}"
         # apply exponent
-        if exp and Ratio.symbol in exp:
-            exp = exp.split(Ratio.symbol)
-            exprat = Ratio(int(exp[0]), int(exp[1]))
+        if exp and Fraction.symbol in exp:
+            exp = exp.split(Fraction.symbol)
+            exprat = Fraction(int(exp[0]), int(exp[1]))
             magnitude = magnitude**(int(exp[0])/int(exp[1]))
             dimensions = [exprat*dim for dim in dimensions]
             baseunits = {unitid: exprat}
         elif exp:
             exp = int(exp)
             magnitude = magnitude**exp
             dimensions = [dim*exp for dim in dimensions]
             baseunits = {unitid: exp}            
         else:
             baseunits = {unitid: 1}
         return Quantity(magnitude, dimensions, baseunits)
     
-    def value(self):
-        baseunits = self.baseunits.expression()
-        if baseunits:
-            unit = self/Quantity(1,baseunits)
+    def value(self, expression=None):
+        if not expression:
+            expression = self.baseunits.expression()
+        if expression:
+            unit = self/Quantity(1,expression)
             return unit.magnitude
         else:
             return self.magnitude
 
     def units(self):
         return self.baseunits.expression()
```

### Comparing `scinumtools-1.5.4/src/scinumtools/phys/units/UnitClass.py` & `scinumtools-1.5.5/src/scinumtools/phys/units/UnitClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.5.5/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.5.5/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.5.5/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.5.5/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.5.5/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/cached_data.npy` & `scinumtools-1.5.5/tests/cached_data.npy`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/pyproject.toml` & `scinumtools-1.5.5/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/test_data.py` & `scinumtools-1.5.5/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/test_math.py` & `scinumtools-1.5.5/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/test_stats.py` & `scinumtools-1.5.5/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/test_struct.py` & `scinumtools-1.5.5/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/test_units.py` & `scinumtools-1.5.5/tests/test_units.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 
 from scinumtools.structs import ParameterDict
 from scinumtools.phys.units.UnitList import UnitStandard, UnitPrefixes
 from scinumtools.phys.units import *
 
 def test_quantity():
     
-    assert str(Quantity(123e2)) == "Quantity(1.230e+04)"
+    assert str(Quantity(123e2))         == "Quantity(1.230e+04)"
+    q = Quantity(123e2, 'km/s')
+    assert str(q) == "Quantity(1.230e+04 km*s-1)"
+    assert str(q.value()) == "12300.0"
+    assert str(q.value('m/s')) == "12300000.0"
+    assert str(q.units()) == "km*s-1"
     
     result = "Quantity(1.230e+04 m*s2:3)"
     assert str(Quantity(123e2, [1,0,(2,3),0,0,0,0,0] ))    == result
     assert str(Quantity(123e2, Dimensions(m=1, s=(2,3)) )) == result
 
     result = "Quantity(1.230e+04 J2*kg2:3)"
     assert str(Quantity(123e2, {'J': 2, 'kg':(2,3)} )) == result
@@ -23,30 +28,33 @@
 
     result = "Quantity(2.460e+04 m)"
     assert str(Quantity(123e2, Quantity(2, 'm'))) == result
     assert str(Quantity(123e2, 2*Unit('m'))) == result
     
 def test_units():
 
-    assert str(Unit('m'))         == "Quantity(1.000e+00 m)"
-    assert str(Unit('kg*m2*s-2')) == "Quantity(1.000e+00 kg*m2*s-2)"
-    
-    unit = Unit()
-    assert str(unit.m)      == "Quantity(1.000e+00 m)"
-    assert str(2*unit.kJ)   == "Quantity(2.000e+00 kJ)"
+    assert str(Unit('m'))                   == "Quantity(1.000e+00 m)"
+    assert str(Unit('kg*m2*s-2'))           == "Quantity(1.000e+00 kg*m2*s-2)"
+                                            
+    unit = Unit()                           
+    assert str(unit.m)                      == "Quantity(1.000e+00 m)"
+    assert str(2*unit.kJ)                   == "Quantity(2.000e+00 kJ)"
     assert str(unit.kg*unit.m**2/unit.s**2) == "Quantity(1.000e+00 kg*m2*s-2)"
-    assert str(unit.J.to('erg')) == "Quantity(1.000e+07 erg)"
+    assert str(unit.J.to('erg'))            == "Quantity(1.000e+07 erg)"
+    assert str(unit.m**(2,3))               == "Quantity(1.000e+00 m2:3)"
+    assert str(unit.m**Fraction(2,3))       == "Quantity(1.000e+00 m2:3)"
+    assert str((9*unit.m)**(1,2))           == "Quantity(3.000e+00 m1:2)"
 
 def test_constants():
 
     assert str(Constant('c')) == "Quantity(1.000e+00 [c])"
 
     const = Constant()
-    assert str(const.c)   == "Quantity(1.000e+00 [c])"
-    assert str(const.m_e) == "Quantity(1.000e+00 [m_e])"
+    assert str(const.c)       == "Quantity(1.000e+00 [c])"
+    assert str(const.m_e)     == "Quantity(1.000e+00 [m_e])"
     
 def test_dimensions():
 
     # Test simplification
     dims = Dimensions(m=(5,-2), g=3, s=1, cd=(-0,3), K=(34,1), rad=(18,12))
     assert str(dims) == "Dimensions(m=-5:2 g=3 s=1 K=34 rad=3:2)"
 
@@ -61,14 +69,35 @@
 
     # Test values
     value = [3, (3,2), 0, 0, 0, 0, 0, 0]
     dims = Dimensions(*value)
     assert str(dims) == "Dimensions(m=3 g=3:2)" 
     assert dims.value() == value
     assert dims.value(dtype=dict) == {'m': 3, 'g':(3,2)}
+
+def test_fractions():
+
+    # Test initialization
+    assert str(Fraction(2))   == "2"
+    assert str(Fraction(0,3)) == "0"
+    assert str(Fraction(1,3)) == "1:3"
+
+    # Test arithmetics
+    assert str(Fraction(1,3)+3)             == "10:3"
+    assert str(Fraction(1,3)+(3,2))         == "11:6"
+    assert str(Fraction(1,3)+Fraction(3,2)) == "11:6"
+    assert str(Fraction(1,3)-3)             == "-8:3"
+    assert str(Fraction(1,3)-(3,2))         == "-7:6"
+    assert str(Fraction(1,3)-Fraction(3,2)) == "-7:6"
+    assert str(Fraction(1,3)*3)             == "1"
+    assert str(Fraction(1,3)*(3,2))         == "1:2"
+    assert str(Fraction(1,3)*Fraction(3,2)) == "1:2"
+    assert str(Fraction(1,3)/3)             == "1:9"
+    assert str(Fraction(1,3)/(3,2))         == "2:9"
+    assert str(Fraction(1,3)/Fraction(3,2)) == "2:9"
     
 def test_base_units():
 
     # Test simplification
     bu = BaseUnits({'g':(3,2), 'km': 3, '[m_p]': (3,1)})
     assert str(bu) == "BaseUnits(g=3:2 km=3 [m_p]=3)"
 
@@ -175,23 +204,24 @@
 
     # Test unit conversion on arrays
     assert str(Quantity([1,2,3], 'm').to('km')) == "Quantity([0.001 0.002 0.003] km)"
 
 def test_numpy():
     
     # Test numpy functions
-    assert str(np.sqrt(Quantity(4, 'm2')))  == "Quantity(2.000e+00 m)"
-    assert str(np.sqrt(Quantity([4, 9, 16], 'm2')))  == "Quantity([2. 3. 4.] m)"
-    assert str(np.sqrt(Quantity([4, 9, 16], 'm3')))  == "Quantity([2. 3. 4.] m3:2)"
-    assert str(np.sqrt(Quantity([4, 9, 16], 'm-3')))  == "Quantity([2. 3. 4.] m-3:2)"
+    assert str(np.sqrt(Quantity(4, 'm2')))             == "Quantity(2.000e+00 m)"
+    assert str(np.sqrt(Quantity([4, 9, 16], 'm2')))    == "Quantity([2. 3. 4.] m)"
+    assert str(np.sqrt(Quantity([4, 9, 16], 'm3')))    == "Quantity([2. 3. 4.] m3:2)"
+    assert str(np.sqrt(Quantity([4, 9, 16], 'm-3')))   == "Quantity([2. 3. 4.] m-3:2)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm2:3')))  == "Quantity([2. 3. 4.] m1:3)"
     assert str(np.sqrt(Quantity([4, 9, 16], 'm2:3*g3:5*s5')))  == "Quantity([2. 3. 4.] m1:3*g3:10*s5:2)"
-    assert str(np.cbrt(Quantity([8, 27, 64], 'm3'))) == "Quantity([2. 3. 4.] m)"
-    assert str(np.power(Quantity([2, 3, 4], 'm'),3)) == "Quantity([ 8. 27. 64.] m3)"
-
+    assert str(np.cbrt(Quantity([8, 27, 64], 'm3')))   == "Quantity([2. 3. 4.] m)"
+    assert str(np.power(Quantity([2, 3, 4], 'm'),3))   == "Quantity([ 8. 27. 64.] m3)"
+    assert str(np.sin(Quantity([45, 60], "deg")))      == "Quantity([0.707 0.866])"
+    
 def test_operation_sides():
     
     p = Quantity([2,3,4], 'm')
     q = Quantity([5,6,7], 'm')
     assert p+q == q+p
     assert p-q == -(q-p)
     assert q*2 == 2*q
@@ -223,10 +253,10 @@
     assert str(Quantity(23,'degR').to('K'))       == "Quantity(1.278e+01 K)"
     assert str(Quantity(23,'degR').to('Cel'))     == "Quantity(-2.604e+02 Cel)"
     assert str(Quantity(23,'degR').to('degF'))    == "Quantity(-4.367e+02 degF)"
     assert str(Quantity(2300,'Cel').to('kK'))     == "Quantity(2.573e+00 kK)"
     
 def test_inversion():
 
-    assert str(Quantity(23, 'Hz').to('s'))     == "Quantity(4.348e-02 s)"
-    assert str(Quantity(34, 'Ohm').to('S'))    == "Quantity(2.941e-02 S)"
-    assert str(Quantity(102, 'J').to('erg-1')) == "Quantity(9.804e-10 erg-1)"
+    assert str(Quantity(23, 'Hz').to('s'))        == "Quantity(4.348e-02 s)"
+    assert str(Quantity(34, 'Ohm').to('S'))       == "Quantity(2.941e-02 S)"
+    assert str(Quantity(102, 'J').to('erg-1'))    == "Quantity(9.804e-10 erg-1)"
```

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/data/ImageClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/data/ImageClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/data/PlottingClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/data/PlottingClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/math/solver/AtomClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/math/solver/AtomClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/math/solver/ExpressionClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/math/solver/ExpressionClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/math/solver/OperatorClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/math/solver/OperatorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/math/solver/SolverClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/math/solver/SolverClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/math/solver/TokensClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/math/solver/TokensClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/phys/ConstantsClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/phys/ConstantsClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/phys/units/QuantityClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/phys/units/QuantityClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/phys/units/UnitConverters.py` & `scinumtools-1.5.5/tests/src/scinumtools/phys/units/UnitConverters.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/phys/units/UnitList.py` & `scinumtools-1.5.5/tests/src/scinumtools/phys/units/UnitList.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/tests/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.5.5/tests/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/.gitignore` & `scinumtools-1.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.5.4/pyproject.toml` & `scinumtools-1.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.5.4"
+version = "1.5.5"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.5.4/PKG-INFO` & `scinumtools-1.5.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.5.4
+Version: 1.5.5
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

