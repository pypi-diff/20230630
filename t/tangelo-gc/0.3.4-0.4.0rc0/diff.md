# Comparing `tmp/tangelo-gc-0.3.4.tar.gz` & `tmp/tangelo-gc-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tangelo-gc-0.3.4.tar", last modified: Tue Feb 21 06:48:31 2023, max compression
+gzip compressed data, was "tangelo-gc-0.4.0rc0.tar", last modified: Thu Jun 29 23:16:01 2023, max compression
```

## Comparing `tangelo-gc-0.3.4.tar` & `tangelo-gc-0.4.0rc0.tar`

### file list

```diff
@@ -1,294 +1,315 @@
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.248364 tangelo-gc-0.3.4/
--rwxrwxr-x   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/LICENSE
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      437 2023-02-21 06:48:31.248364 tangelo-gc-0.3.4/PKG-INFO
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10749 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/README.rst
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       38 2023-02-21 06:48:31.248364 tangelo-gc-0.3.4/setup.cfg
--rwxrwxr-x   0 valentin  (1000) valentin  (1000)      992 2022-08-08 22:09:06.000000 tangelo-gc-0.3.4/setup.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.196365 tangelo-gc-0.3.4/tangelo/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      723 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      735 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/_version.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.196365 tangelo-gc-0.3.4/tangelo/algorithms/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      772 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.196365 tangelo-gc-0.3.4/tangelo/algorithms/classical/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      704 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/classical/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4025 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/classical/ccsd_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5297 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/classical/fci_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2998 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/classical/semi_empirical_solver.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.200365 tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3095 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/test_ccsd_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2415 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/test_fci_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1559 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/test_semi_empirical_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2120 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/electronic_structure_solver.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.200365 tangelo-gc-0.3.4/tangelo/algorithms/projective/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      633 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/projective/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    15100 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/projective/quantum_imaginary_time.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.200365 tangelo-gc-0.3.4/tangelo/algorithms/projective/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/projective/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6064 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/projective/tests/test_qite.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.200365 tangelo-gc-0.3.4/tangelo/algorithms/variational/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      898 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    16264 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/adapt_vqe_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    15314 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/iqcc_ilc_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    14663 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/iqcc_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    15090 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/sa_oo_vqe_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    12034 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/sa_vqe_solver.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.200365 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5362 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_adapt_vqe_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3574 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_iqcc_ilc_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4033 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_iqcc_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2765 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_sa_oo_vqe_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10330 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_sa_vqe_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2251 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_tetris_adapt_vqe_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    27088 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_vqe_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2934 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/tetris_adapt_vqe_solver.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    35754 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/algorithms/variational/vqe_solver.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.204365 tangelo-gc-0.3.4/tangelo/helpers/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      642 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/helpers/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2118 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/helpers/math.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3444 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/helpers/utils.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.204365 tangelo-gc-0.3.4/tangelo/linq/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      868 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    17173 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/circuit.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8185 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/gate.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.204365 tangelo-gc-0.3.4/tangelo/linq/helpers/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      635 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/helpers/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.204365 tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      656 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2387 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/measurement_basis.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10280 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/statevector.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.204365 tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3208 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/tests/test_statevector.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.204365 tangelo-gc-0.3.4/tangelo/linq/helpers/operators/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      611 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/helpers/operators/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1724 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/helpers/operators/operators.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.204365 tangelo-gc-0.3.4/tangelo/linq/noisy_simulation/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      614 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/noisy_simulation/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5051 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/noisy_simulation/noise_models.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2268 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/qdk_template.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.208365 tangelo-gc-0.3.4/tangelo/linq/qpu_connection/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      731 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/qpu_connection/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7428 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/qpu_connection/ibm_connection.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9539 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/qpu_connection/ionq_connection.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6696 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/qpu_connection/qemist_cloud_connection.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      909 2022-08-08 22:09:06.000000 tangelo-gc-0.3.4/tangelo/linq/qpu_connection/qpu_connection.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2834 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/simulator.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.208365 tangelo-gc-0.3.4/tangelo/linq/target/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1082 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/target/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    34551 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/target/backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10660 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/target/target_cirq.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4596 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/target/target_qdk.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10355 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/target/target_qiskit.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10224 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/target/target_qulacs.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.208365 tangelo-gc-0.3.4/tangelo/linq/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    13001 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/test_circuits.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5896 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/test_gates.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3947 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/test_ibm_connection.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3178 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/test_ionq_connection.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    29605 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/test_simulator.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    13134 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/test_simulator_noisy.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    22583 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/test_translator_circuit.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9527 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/tests/test_translator_qubitop.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.212365 tangelo-gc-0.3.4/tangelo/linq/translator/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2105 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2281 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/qdk_template.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6366 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_braket.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3364 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_circuit.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8722 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_cirq.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5314 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_json_ionq.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6952 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_openqasm.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5753 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_pennylane.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7344 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_projectq.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6259 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_qdk.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9179 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_qiskit.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3528 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_qubitop.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10008 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/linq/translator/translate_qulacs.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5144 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/molecule_library.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.212365 tangelo-gc-0.3.4/tangelo/problem_decomposition/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      779 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.212365 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      639 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.216365 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1381 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5947 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2656 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_fragment.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3761 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_onerdm.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9468 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_orbitals.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4895 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_scf.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4378 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_scf_guess.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    33524 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10556 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/fragment.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.216365 tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      743 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9960 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/iao_localization.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1197 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/meta_lowdin_localization.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1252 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/nao_localization.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.216365 tangelo-gc-0.3.4/tangelo/problem_decomposition/incremental/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/incremental/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    17448 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/incremental/mifno_helper.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.216365 tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      638 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.216365 tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/_helpers/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/_helpers/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2410 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/_helpers/capping_groups.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    12039 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/_helpers/helper_classes.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5728 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/oniom_problem_decomposition.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      863 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/problem_decomposition.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.216365 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.220365 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10908 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2814 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet_fragment.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5347 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet_oneshot_loop.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2876 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet_orbitals.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3466 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet_vqe.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2716 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_osdmet.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.220365 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4272 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/test_capping.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6868 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/test_oniom.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6129 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/test_oniom_quantum.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.220365 tangelo-gc-0.3.4/tangelo/toolboxes/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.228365 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      943 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    21631 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_general_unitary_cc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2198 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_hea_circuit.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9590 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_qubit_cc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    14250 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_qubit_ilc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9849 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_qubit_mf.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    16155 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_unitary_cc_openshell.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3645 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_unitary_cc_paired.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4442 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_unitary_majorana_cc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7277 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/adapt_ansatz.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1709 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/ansatz.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    21303 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/ansatz_utils.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6132 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/fermionic_operators.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7772 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/hea.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    14088 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/ilc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6397 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/penalty_terms.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8521 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/puccd.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    14565 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/qcc.py
--rwxrwxr-x   0 valentin  (1000) valentin  (1000)    12343 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/qmf.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8542 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/rucc.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.228365 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2131 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_adapt_ansatz.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    16627 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_ansatz_util.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    11680 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_fermionic_operators.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5816 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_general_unitary_cc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4746 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_hea.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8408 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_ilc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    13153 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_penalty_terms.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2596 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_puccd.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7868 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_qcc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5980 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_qmf.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3394 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_rucc.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3747 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_uccgd.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6253 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_uccsd.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5452 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_upccgsd.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2439 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_variational_circuit.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5082 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_vsqs.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9051 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/uccgd.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    13909 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/uccsd.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10165 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/upccgsd.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3378 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/variational_circuit.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    12711 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/vsqs.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.232365 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      638 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7032 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/diagonal_coulomb.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3673 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/discrete_clock.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3854 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/grid_circuits.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    17697 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/lcu.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5839 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/multiproduct.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    12208 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/qsp.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.232365 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2214 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_diagonal_coulomb.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5892 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_discrete_clock.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3498 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_grid.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8640 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_lcu.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5092 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_mp.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5015 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_qsp.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.232365 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1045 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.236364 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      598 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8043 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/adaptive.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6221 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/classical_shadows.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10453 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/derandomized.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9000 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/randomized.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2387 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/estimate_measurements.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5618 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/qubit_terms_grouping.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.236364 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4398 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_adaptive_classical_shadows.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3730 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4767 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_measurements.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6846 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4894 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.236364 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2082 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/coefficients.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7500 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/frozen_orbitals.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    32258 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/molecule.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    12433 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/rdms.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.240364 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1465 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/test_coefficients.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5531 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6432 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/test_molecule.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6949 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/test_rdms.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.240364 tangelo-gc-0.3.4/tangelo/toolboxes/operators/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      844 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    16328 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/multiformoperator.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    13823 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/operators.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4539 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/taper_qubits.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.240364 tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4595 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/test_multiformoperator.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7776 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/test_operators.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6052 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/test_taper_qubits.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4174 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/test_z2_tapering.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7085 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/operators/z2_tapering.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.240364 tangelo-gc-0.3.4/tangelo/toolboxes/optimizers/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      619 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/optimizers/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3333 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/optimizers/rotosolve.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.240364 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      860 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2191 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/bootstrapping.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     6517 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/extrapolation.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8963 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/histogram.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3071 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/mc_weeny_rdm_purification.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5516 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/post_selection.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.244364 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3048 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/test_extrapolation.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7088 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/test_histogram.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2387 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2298 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/test_post_selection.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.244364 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      772 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2383 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2986 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/hcb.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     8073 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/jkmn.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2025 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/jordan_wigner.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7502 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/mapping_transform.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7336 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/statevector_mapping.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10494 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.244364 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      585 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2779 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    10280 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2175 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     7966 2023-02-21 06:46:16.000000 tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2023-02-21 06:48:31.248364 tangelo-gc-0.3.4/tangelo_gc.egg-info/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      437 2023-02-21 06:48:31.000000 tangelo-gc-0.3.4/tangelo_gc.egg-info/PKG-INFO
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    12093 2023-02-21 06:48:31.000000 tangelo-gc-0.3.4/tangelo_gc.egg-info/SOURCES.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)        1 2023-02-21 06:48:31.000000 tangelo-gc-0.3.4/tangelo_gc.egg-info/dependency_links.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       43 2023-02-21 06:48:31.000000 tangelo-gc-0.3.4/tangelo_gc.egg-info/requires.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)        8 2023-02-21 06:48:31.000000 tangelo-gc-0.3.4/tangelo_gc.egg-info/top_level.txt
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.500423 tangelo-gc-0.4.0rc0/
+-rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/LICENSE
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      440 2023-06-29 23:16:01.500288 tangelo-gc-0.4.0rc0/PKG-INFO
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11203 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/README.rst
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)       38 2023-06-29 23:16:01.500464 tangelo-gc-0.4.0rc0/setup.cfg
+-rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)      913 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/setup.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.453415 tangelo-gc-0.4.0rc0/tangelo/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      723 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      738 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/_version.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.454028 tangelo-gc-0.4.0rc0/tangelo/algorithms/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      783 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.454998 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      738 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13884 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/ccsd_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14155 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/fci_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14715 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/mp2_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3088 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/semi_empirical_solver.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.455737 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3613 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_ccsd_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3012 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_fci_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4247 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_mp2_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1617 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_semi_empirical_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2120 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/electronic_structure_solver.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.456014 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      633 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15369 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/quantum_imaginary_time.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.456297 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6064 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/test_qite.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.457956 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      898 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17441 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/adapt_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15567 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/iqcc_ilc_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14915 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/iqcc_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15440 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/sa_oo_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12679 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/sa_vqe_solver.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.459513 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7445 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_adapt_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3574 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_iqcc_ilc_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4033 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_iqcc_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2765 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_sa_oo_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11665 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_sa_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2251 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_tetris_adapt_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    29311 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2934 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tetris_adapt_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    36829 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/vqe_solver.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.459996 tangelo-gc-0.4.0rc0/tangelo/helpers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      642 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/helpers/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2873 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/helpers/math.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3762 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/helpers/utils.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.460804 tangelo-gc-0.4.0rc0/tangelo/linq/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      937 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    19075 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8982 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/gate.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.461041 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      635 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.461613 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      656 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3914 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/clifford_circuits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/measurement_basis.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10280 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/statevector.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.462114 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1871 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/test_clifford_circuits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3208 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/test_statevector.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.462396 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      611 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1724 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/operators.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.462670 tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      614 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5051 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/noise_models.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2268 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qdk_template.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.463601 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      779 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6112 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/braket_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7428 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/ibm_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9539 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/ionq_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6696 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/qemist_cloud_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      909 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/qpu_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2578 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/simulator.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.465070 tangelo-gc-0.4.0rc0/tangelo/linq/target/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1239 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    37084 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/backend.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12794 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_cirq.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4596 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qdk.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12428 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qiskit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11780 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qulacs.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7657 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_stim.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5024 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_sympy.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.467267 tangelo-gc-0.4.0rc0/tangelo/linq/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2799 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_braket_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14256 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_circuits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7437 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_gates.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3962 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_ibm_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3194 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_ionq_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    32240 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_simulator.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13817 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_simulator_noisy.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3246 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_symbolic_simulator.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    25603 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4278 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_perf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8362 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_qubitop.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.470031 tangelo-gc-0.4.0rc0/tangelo/linq/translator/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2015 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2281 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/qdk_template.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5896 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_braket.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3575 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8285 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_cirq.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4770 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_json_ionq.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5552 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_openqasm.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5753 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_pennylane.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6133 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_projectq.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5692 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qdk.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8706 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qiskit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3668 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qubitop.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9287 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qulacs.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5677 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_stim.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7610 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_sympy.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5310 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/molecule_library.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.470375 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      779 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.471223 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      639 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.472249 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1381 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6636 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2656 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_fragment.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3761 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_onerdm.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9799 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_orbitals.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4936 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4378 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf_guess.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    36407 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10607 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/fragment.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.472850 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      743 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10061 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/iao_localization.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1200 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/meta_lowdin_localization.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1255 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/nao_localization.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.473160 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17513 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/mifno_helper.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.473525 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      638 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.474084 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2410 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/capping_groups.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12174 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/helper_classes.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5725 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/oniom_problem_decomposition.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      863 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/problem_decomposition.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.474267 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.475694 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11803 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2814 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_fragment.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5347 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_oneshot_loop.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2876 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_orbitals.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3466 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_vqe.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2602 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_osdmet.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.476490 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4272 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_capping.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6868 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_oniom.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6129 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_oniom_quantum.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.476682 tangelo-gc-0.4.0rc0/tangelo/toolboxes/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.481540 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      943 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    21631 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_general_unitary_cc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2198 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_hea_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9590 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_cc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14250 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_ilc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9849 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_mf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16155 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_cc_openshell.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3645 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_cc_paired.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4442 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_majorana_cc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7277 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/adapt_ansatz.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1709 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ansatz.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    21208 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ansatz_utils.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6132 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/fermionic_operators.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7772 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/hea.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14088 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ilc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6397 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/penalty_terms.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8521 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/puccd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14565 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/qcc.py
+-rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)    12343 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/qmf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8542 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/rucc.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.484571 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2131 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_adapt_ansatz.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16763 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_ansatz_util.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11680 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_fermionic_operators.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5816 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_general_unitary_cc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4746 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_hea.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8408 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_ilc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13153 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_penalty_terms.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2596 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_puccd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7868 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_qcc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5980 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_qmf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3394 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_rucc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3747 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_uccgd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6253 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_uccsd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5452 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_upccgsd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2439 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_variational_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5312 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_vsqs.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9103 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/uccgd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14028 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/uccsd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10165 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/upccgsd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3378 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/variational_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12665 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/vsqs.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.485757 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      638 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7032 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/diagonal_coulomb.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3673 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/discrete_clock.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3854 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/grid_circuits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17697 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/lcu.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5839 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/multiproduct.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12208 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/qsp.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.488126 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2212 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_diagonal_coulomb.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5828 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_discrete_clock.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3412 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_grid.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8725 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_lcu.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5207 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_mp.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5038 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_qsp.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.488686 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1045 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.489535 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      598 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8043 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/adaptive.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6221 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/classical_shadows.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10453 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/derandomized.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9000 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/randomized.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/estimate_measurements.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5618 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/qubit_terms_grouping.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.490492 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4398 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_adaptive_classical_shadows.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3730 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4794 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_measurements.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6905 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4894 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.491846 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      876 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2082 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/coefficients.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7488 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/frozen_orbitals.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4598 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10238 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver_psi4.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12003 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver_pyscf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    26948 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/molecule.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    19213 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/rdms.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.493229 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1465 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_coefficients.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5531 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8616 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_molecule.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4069 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_nopyscf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4432 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_psi4.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9120 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_rdms.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.494166 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      844 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16328 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/multiformoperator.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14593 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/operators.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4539 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/taper_qubits.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.495062 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4595 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_multiformoperator.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7869 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_operators.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6052 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_taper_qubits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4744 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_trim_trivial_qubits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4174 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_z2_tapering.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6442 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/trim_trivial_qubits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7085 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/z2_tapering.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.495363 tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      619 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3333 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/rotosolve.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.496297 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      860 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2191 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/bootstrapping.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6517 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/extrapolation.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8963 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/histogram.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3071 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/mc_weeny_rdm_purification.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5535 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/post_selection.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.497070 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3048 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_extrapolation.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7088 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_histogram.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2298 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_post_selection.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.498544 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      813 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2383 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8432 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/combinatorial.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2986 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/hcb.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8073 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/jkmn.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2025 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/jordan_wigner.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7502 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/mapping_transform.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7350 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/statevector_mapping.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10494 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.499472 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2779 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4635 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_combinatorial.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10280 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2175 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7972 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.500109 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      440 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/PKG-INFO
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13175 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/SOURCES.txt
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)        1 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/dependency_links.txt
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)       26 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/requires.txt
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)        8 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/top_level.txt
```

### Comparing `tangelo-gc-0.3.4/LICENSE` & `tangelo-gc-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/README.rst` & `tangelo-gc-0.4.0rc0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -92,78 +92,62 @@
 
 If the installation of a dependency fails and the reason is not obvious, we suggest installing that dependency
 separately with ``pip``\ , before trying again.
 
 With Docker
 ^^^^^^^^^^^
 
-Use our Docker file to deploy Tangelo in a Linux environment, either retrieved from pip or mounted locally.
-Comment / uncomment the relevant sections of the Dockerfile to control installation and dependencies.
+Use our Docker file to deploy Tangelo in a Linux environment, either retrieved from pip or mounted locally. Comment / uncomment the relevant sections of the Dockerfile to control installation and dependencies.
 
 "No install" notebook method
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-A good alternative for users that simply want to quickly get a working environment ready, especially for quick tests, demos, tutorials.
-Check out the tutorial section below to see how services such as Google Colab may help you circumvent local installation challenges or go beyond the limitations of your personal computer if you feel short of compute power or memory.
+Check out the tutorial section below to see how services such as Google Colab, Binder or JupyterLab may help you circumvent local installation challenges or go beyond the compute capabilities of your laptop.
 
+Optional dependencies: Quantum Simulators
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Optional dependencies
-^^^^^^^^^^^^^^^^^^^^^
+Tangelo enables users to target various backends. In particular, it integrates quantum circuit simulators such as ``qulacs``\ , ``qiskit``\ , ``cirq`` or ``qdk``. We leave it to you to install the packages of your choice, and refer to their own documentation. Most packages can be installed through pip or conda in a straightforward way.
 
-Tangelo enables users to target various backends. In particular, it integrates quantum circuit simulators such as
-``qulacs``\ , ``qiskit``\ , ``cirq`` or ``qdk``. We leave it to you to install the packages of your choice, and refer to their own documentation.
-Most packages can be installed through pip in a straightforward way:
 
-.. code-block::
+Optional dependencies: Classical Quantum Chemistry Packages
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-   pip install qulacs
-   pip install qiskit
-   pip install cirq
-   ...
+Tangelo can be used without having a classical quantum chemistry package installed but many algorithms, by default, depend on one being installed. The two quantum chemistry packages that are natively supported are `PySCF <https://pyscf.org/>`_ and `Psi4 <https://psicode.org/>`_.
 
-Depending on your OS and environment, some of these packages may be more challenging to install. For installing Microsoft's QDK
-or any issue regarding the above packages, please check their respective documentation.
+You are also welcome to provide your own interface to a quantum chemistry package of your choice by defining a subclass of `IntegralSolver <https://github.com/goodchemistryco/Tangelo/blob/develop/tangelo/toolboxes/molecular_computation/integral_solver.py>`_. An example of this can be found in `this test <https://github.com/goodchemistryco/Tangelo/blob/develop/tangelo/toolboxes/molecular_computation/tests/test_molecule.py#L167>`_.
 
 
 Quick note for Windows users
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Our installation instructions will work on Linux and MacOS systems. If you are using Windows, we recommend
-you install the `Windows Linux Subsystem <https://docs.microsoft.com/en-us/windows/wsl/install>`_, which allows you
-to run Ubuntu as an application. Once it has been installed, you can type ``explorer.exe`` in your Ubuntu terminal to
-drag and drop files between your Windows and Linux environment.
-
-Here are a few essentials to install inside a brand new Ubuntu environment, before trying to install Tangelo:
+Depending on your OS and environment, some of the optional packages may be more challenging to install. If you are using Windows, we recommend you install the `Windows Linux Subsystem <https://docs.microsoft.com/en-us/windows/wsl/install>`_, which allows you to run Ubuntu as an application. Once it has been installed, you can type ``explorer.exe`` in your Ubuntu terminal to drag and drop files between your Windows and Linux environment. Here are a few essentials to install inside a brand new Ubuntu environment, before trying to install Tangelo:
 
 .. code-block::
 
    sudo apt update && sudo apt upgrade
    sudo apt-get install python3-dev
    sudo apt-get install python3-venv
    sudo apt-get install cmake unzip
 
 
 Optional: environment variables
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Some environment variables can impact performance (ex: using GPU for quantum circuit simulation, or changing
-the number of CPU threads used) or are used to connect to web services providing access to some compute backends.
+Some environment variables can impact performance (ex: using GPU for quantum circuit simulation, or changing the number of CPU threads used) or are used to connect to web services providing access to some compute backends.
 
-See the list of relevant environment variables and their use in ``env_var.sh``. In order for these variables to be set to
-the desired values in your environment, you can run this shell script in Linux with the following command line:
-``source env_var.sh`` (you may need to set execution permissions with ``chmod +x set_env_var.sh`` first), or you can set
-them in whatever way your OS supports it, or even inside your python script using the ``os`` package.
+See the list of relevant environment variables and their use in ``env_var.sh``. In order for these variables to be set to the desired values in your environment, you can run this shell script in Linux with the following command line:
+``source env_var.sh`` (you may need to set execution permissions with ``chmod +x set_env_var.sh`` first), or you can set them in whatever way your OS supports it, or even inside your python script using the ``os`` package.
 
 Tutorials and examples
 ----------------------
 
 We have a `dedicated repository <https://github.com/goodchemistryco/Tangelo-Examples>`_ for examples and tutorials !
 
-We wrote a number of them, and tried to provide material that doesn't just explain how to use the software, but provides insights into the complex topics of chemistry, quantum computing, and digs into the challenges we encountered in our previous hardware experiments.
-Nothing prevents users from contributing and showcasing what they have been doing with Tangelo.
+We wrote a number of them, and tried to provide material that doesn't just explain how to use the software, but provides insights into the complex topics of chemistry, quantum computing, and digs into the challenges we encountered in our previous hardware experiments. Nothing prevents users from contributing and showcasing what they have been doing with Tangelo.
 
 You can visualize notebooks directly on Github, most of them have been pre-run.
 If you'd like to be able to run them locally, we suggest you use `Jupyter notebooks inside a virtual environment <https://janakiev.com/blog/jupyter-virtual-envs/>`_.
 
 - Install Jupyter and ipykernel in your environment:
 .. code-block::
 
@@ -177,16 +161,15 @@
 Jupyter notebooks can also be displayed and executed in the cloud, with services such as Google Colab. This removes the constraint of building a local development envrionement, and enables users to run interactive notebooks on machines that may provide a better configuration than their own (more RAM, compute power, access to GPUs...). This may come in handy for users who want to get started quickly, especially for quick tests, demos and tutorials.
 
 Check out our `tutorials <./TUTORIALS.rst>`_ file for more details.
 
 Tests
 -----
 
-Unit tests can be found in the ``tests`` folders, located in the various toolboxes they are related to. To automatically
-find and run all tests (assuming you are in the ``tangelo`` subfolder that contains the code of the package):
+Unit tests can be found in the ``tests`` folders, located in the various toolboxes they are related to. To automatically find and run all tests (assuming you are in the ``tangelo`` subfolder that contains the code of the package):
 
 .. code-block::
 
    python -m unittest
 
 
 Contributions
@@ -194,16 +177,15 @@
 
 Thank you very much for considering contributing to this project; we'd love to have you on board !
 You do not need to be a seasoned software developer or expert in your field to make contributions to this project: it will take various kinds of people and backgrounds to tackle the challenges that await us.
 
 However we need some guidelines and processes to ensure that we build something of quality for the community. We describe them in the `contributions <./CONTRIBUTIONS.rst>`_ file.
 There are many ways you can contribute, but in case you're considering contributing to the codebase: don't be scared of the infamous pull request process ! It can feel intimidating, but we've had a few researchers or high-schoolers go through their first one and... they came back for more ! Mostly.
 
-You can use the `Issue tab <https://github.com/goodchemistryco/Tangelo/issues>`_ to open a bug report or feature request.
-If you're not sure, starting a discussion in the `Discussion tab <https://github.com/goodchemistryco/Tangelo/discussions>`_ is a good start: we'll figure it out from there.
+You can use the `Issue tab <https://github.com/goodchemistryco/Tangelo/issues>`_ to open a bug report or feature request. If you're not sure, starting a discussion in the `Discussion tab <https://github.com/goodchemistryco/Tangelo/discussions>`_ is a good start: we'll figure it out from there.
 
 By joining the Tangelo community and sharing your ideas and developments, you are creating an opportunity for us to learn and grow together, and take ideas to the finish line and beyond.
 
 Citations
 ---------
 
 If you use Tangelo in your research, please cite:
```

### Comparing `tangelo-gc-0.3.4/setup.py` & `tangelo-gc-0.4.0rc0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import setuptools
 import sys
 import subprocess
+import os
 
 
 def install(package):
     subprocess.check_call([sys.executable, "-m", "pip", "install", package])
 
+
 with open("tangelo/_version.py") as f:
     version = f.readlines()[-1].split()[-1].strip("\"'")
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 install('wheel')
-install('pyscf')
-install('git+https://github.com/pyscf/semiempirical')
 
 description = "Maintained by Good Chemistry Company, focusing on the development of end-to-end materials simulation workflows on quantum computers."
 
 setuptools.setup(
     name="tangelo-gc",
     author="The Tangelo developers",
     version=version,
     description=description,
     long_description=description,
-    #long_description_content_type=description,
+    # long_description_content_type=description,
     url="https://github.com/goodchemistryco/Tangelo",
     packages=setuptools.find_packages(),
     test_suite="tangelo",
     setup_requires=['h5py'],
-    install_requires=['h5py', 'bitarray', 'openfermion', 'openfermionpyscf']
+    install_requires=['h5py', 'bitarray', 'openfermion']
 )
```

### Comparing `tangelo-gc-0.3.4/tangelo/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/_version.py` & `tangelo-gc-0.4.0rc0/tangelo/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Define version number here. It is read in setup.py, and bumped automatically
 when using the new release Github action. """
-__version__ = "0.3.4"
+__version__ = "0.4.0.RC"
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .variational import BuiltInAnsatze, VQESolver, ADAPTSolver, SA_VQESolver, SA_OO_Solver
-from .classical import FCISolver, CCSDSolver, MINDO3Solver
+from .classical import FCISolver, CCSDSolver, MINDO3Solver, MP2Solver
 from .projective import QITESolver
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/classical/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .fci_solver import FCISolver
-from .ccsd_solver import CCSDSolver
-from .semi_empirical_solver import MINDO3Solver
+from .operators import *
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/classical/semi_empirical_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/semi_empirical_solver.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 Here are the semi-empirical method(s) implemented:
     - MINDO3
 """
 
 from tangelo.helpers.utils import is_package_installed
 from tangelo.algorithms.electronic_structure_solver import ElectronicStructureSolver
+from tangelo.toolboxes.molecular_computation.integral_solver_pyscf import mol_to_pyscf
 
 
 class MINDO3Solver(ElectronicStructureSolver):
     """Uses the MINDO3 method to solve the electronic structure problem, through
     pyscf. Only the restricted (RMINDO3) flavor is implemented.
 
     Args:
@@ -58,15 +59,15 @@
         """Perform the simulation (energy calculation) for the molecule.
 
         Returns:
             float: RMINDO3 energy.
         """
         from pyscf.semiempirical import mindo3
 
-        solver = mindo3.RMINDO3(self.molecule.to_pyscf()).run(verbose=0)
+        solver = mindo3.RMINDO3(mol_to_pyscf(self.molecule)).run(verbose=0)
         total_energy = solver.e_tot
 
         return total_energy
 
     def get_rdm(self):
         """Method must be defined (ElectronicStructureSolver). For
         semi-empirical methods, it is not relevant nor defined.
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/test_ccsd_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_ccsd_solver.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,73 +10,83 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
-from tangelo.algorithms.classical.ccsd_solver import CCSDSolver
-from tangelo.molecule_library import mol_H2_321g, mol_Be_321g, mol_H4_sto3g_uhf_a1_frozen
+from tangelo import SecondQuantizedMolecule
+from tangelo.algorithms.classical.ccsd_solver import CCSDSolver, default_ccsd_solver
+from tangelo.molecule_library import mol_H2_321g, mol_Be_321g, mol_H4_sto3g_uhf_a1_frozen, xyz_H4
 
 
-# TODO: Can we test the get_rdm method on H2 ? How do we get our reference? Whole matrix or its properties?
 class CCSDSolverTest(unittest.TestCase):
 
     def test_ccsd_h2(self):
         """Test CCSDSolver against result from reference implementation."""
 
         solver = CCSDSolver(mol_H2_321g)
         energy = solver.simulate()
 
-        self.assertAlmostEqual(energy, -1.1478300596229851, places=6)
+        self.assertAlmostEqual(energy, -1.1478300, places=5)
 
+    @unittest.skipIf("pyscf" != default_ccsd_solver, "Test Skipped: Only functions for pyscf \n")
     def test_ccsd_h4_uhf_a1_frozen(self):
-        """Test CCSDSolver against result from reference implementation."""
+        """Test CCSDSolver against result from reference implementation for single alpha frozen orbital and rdms returned."""
 
         solver = CCSDSolver(mol_H4_sto3g_uhf_a1_frozen)
         energy = solver.simulate()
 
         self.assertAlmostEqual(energy, -1.95831052, places=6)
 
         one_rdms, two_rdms = solver.get_rdm()
 
         self.assertAlmostEqual(mol_H4_sto3g_uhf_a1_frozen.energy_from_rdms(one_rdms, two_rdms), -1.95831052, places=6)
 
+    def test_ccsd_h4_uhf_different_alpha_beta_frozen(self):
+        """Test energy for case when different but equal number of alpha/beta orbitals are frozen."""
+
+        mol = SecondQuantizedMolecule(xyz_H4, q=0, spin=0, basis="3-21g", frozen_orbitals=[[2, 3, 4, 5], [2, 3, 6, 5]], symmetry=False, uhf=True)
+        solver = CCSDSolver(mol)
+        energy = solver.simulate()
+
+        self.assertAlmostEqual(energy, -2.0409800, places=5)
+
     def test_ccsd_be(self):
         """Test CCSDSolver against result from reference implementation."""
 
         solver = CCSDSolver(mol_Be_321g)
         energy = solver.simulate()
 
-        self.assertAlmostEqual(energy, -14.531416589890926, places=6)
+        self.assertAlmostEqual(energy, -14.531416, places=5)
 
     def test_ccsd_be_frozen_core(self):
         """ Test CCSDSolver against result from reference implementation, with
         no mean-field provided as input. Frozen core is considered.
         """
 
         mol_Be_321g_freeze1 = mol_Be_321g.freeze_mos(1, inplace=False)
 
         solver = CCSDSolver(mol_Be_321g_freeze1)
         energy = solver.simulate()
 
-        self.assertAlmostEqual(energy, -14.530687987160581, places=6)
+        self.assertAlmostEqual(energy, -14.5306879, places=5)
 
     def test_ccsd_be_as_two_levels(self):
         """ Test CCSDSolver against result from reference implementation, with
         no mean-field provided as input. This atom is reduced to an HOMO-LUMO
         problem.
         """
 
         mol_Be_321g_freeze_list = mol_Be_321g.freeze_mos([0, 3, 4, 5, 6, 7, 8], inplace=False)
 
         solver = CCSDSolver(mol_Be_321g_freeze_list)
         energy = solver.simulate()
 
-        self.assertAlmostEqual(energy, -14.498104489160106, places=6)
+        self.assertAlmostEqual(energy, -14.498104, places=5)
 
     def test_ccsd_get_rdm_without_simulate(self):
         """Test that the runtime error is raised when user calls get RDM without
         first running a simulation.
         """
 
         solver = CCSDSolver(mol_H2_321g)
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/test_fci_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/electronic_structure_solver.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,63 +8,54 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import unittest
-
-from tangelo.algorithms import FCISolver
-from tangelo.molecule_library import mol_H2_321g, mol_Be_321g, mol_H4_cation_sto3g
-
-
-# TODO: Can we test the get_rdm method on H2 ? How do we get our reference? Whole matrix or its properties?
-class FCISolverTest(unittest.TestCase):
-
-    def test_fci_h2(self):
-        """Test FCISolver against result from reference implementation (H2)."""
-
-        solver = FCISolver(mol_H2_321g)
-        energy = solver.simulate()
-
-        self.assertAlmostEqual(energy, -1.1478300596229851, places=6)
-
-    def test_fci_be(self):
-        """Test FCISolver against result from reference implementation (Be)."""
-
-        solver = FCISolver(mol_Be_321g)
-        energy = solver.simulate()
-
-        self.assertAlmostEqual(energy, -14.531444379108095, places=6)
-
-    def test_fci_get_rdm_without_simulate(self):
-        """Test that the runtime error is raised when user calls get RDM without
-        first running a simulation.
+"""Abstract class defining a common interface to all electronic structure
+solvers, in order to have consistency and ensure compatibility with higher-level
+workflows that can use them, such as problem decomposition methods.
+"""
+
+import abc
+
+
+class ElectronicStructureSolver(abc.ABC):
+    """Sets interface for objects that perform energy estimation of a molecule.
+
+    Specifics vary between concrete implementations, but common to all of them
+    is that after `simulate` is called, the right internal state is set for the
+    class so that `get_rdm` can return reduced density matrices for the last run
+    simulation.
+    """
+
+    def __init__(self, molecule):
+        """Performs the simulation for a molecule. The mean field is calculated
+        automatically.
+
+        Args:
+            molecule (SecondQuantizedMolecule): The molecule on which to perform the
+                simulation.
         """
+        pass
 
-        solver = FCISolver(mol_H2_321g)
-        self.assertRaises(RuntimeError, solver.get_rdm)
-
-    def test_fci_openshell(self):
-        """Test that the fci implementation for an openshell molecule is working properly"""
-
-        solver = FCISolver(mol_H4_cation_sto3g)
-        energy = solver.simulate()
+    @abc.abstractmethod
+    def simulate(self):
+        """Performs the simulation for a molecule."""
+        pass
+
+    @abc.abstractmethod
+    def get_rdm(self):
+        """Returns the RDM for the previous simulation.
+        In a concrete implementation, the `simulate` function would set the
+        necessary internal state for the class so that this function can return
+        the reduced density matrix.
+
+        Returns:
+            numpy.array: One-particle RDM.
+            numpy.array: Two-particle RDM.
 
-        self.assertAlmostEqual(energy, -1.6419373, places=6)
-
-    def test_fci_be_frozen_core(self):
-        """ Test FCISolver against result from reference implementation, with no mean-field provided as input.
-            Frozen core is considered.
+        Raises:
+            RuntimeError: If no simulation has been run.
         """
-
-        mol_Be_321g_freeze1 = mol_Be_321g.freeze_mos(1, inplace=False)
-
-        solver = FCISolver(mol_Be_321g_freeze1)
-        energy = solver.simulate()
-
-        self.assertAlmostEqual(energy, -14.530687987160581, places=6)
-
-
-if __name__ == "__main__":
-    unittest.main()
+        pass
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/classical/tests/test_semi_empirical_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_semi_empirical_solver.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 from tangelo.helpers.utils import is_package_installed
 from tangelo.molecule_library import mol_pyridine
 
 
 class SemiEmpiricalSolverTest(unittest.TestCase):
 
-    @unittest.skipIf(not is_package_installed("pyscf.semiempirical"), "Test Skipped: pyscf.semiempirical module not available \n")
+    @unittest.skipIf(not is_package_installed("pyscf") or not is_package_installed("pyscf.semiempirical"),
+                     "Test Skipped: pyscf.semiempirical module not available \n")
     def test_mindo3_energy(self):
         """Test MINDO3Solver with pyridine. Validated with:
             - MINDO/3-derived geometries and energies of alkylpyridines and the
             related N-methylpyridinium cations. Jeffrey I. Seeman,
             John C. Schug, and Jimmy W. Viers
             The Journal of Organic Chemistry 1983 48 (14), 2399-2407
             DOI: 10.1021/jo00162a021.
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/projective/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/projective/quantum_imaginary_time.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/quantum_imaginary_time.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Module that defines the Quantum Imaginary Time Algorithm (QITE)
 """
+from typing import Union, Callable, List
 from copy import copy
 import math
 
 from openfermion import FermionOperator as ofFermionOperator
 import numpy as np
 
+from tangelo import SecondQuantizedMolecule
 from tangelo.toolboxes.ansatz_generator.ansatz_utils import trotterize
 from tangelo.toolboxes.operators.operators import FermionOperator, QubitOperator
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.ansatz_generator._general_unitary_cc import uccgsd_generator as uccgsd_pool
 from tangelo.toolboxes.operators import qubitop_to_qubitham
 from tangelo.toolboxes.qubit_mappings.statevector_mapping import get_reference_circuit
 from tangelo.linq import Circuit, get_backend
@@ -51,36 +53,33 @@
         backend_options (dict): Backend options for the underlying QITE propagation
         verbose (bool): Flag for verbosity of QITE.
      """
 
     def __init__(self, opt_dict):
 
         default_backend_options = {"target": None, "n_shots": None, "noise_model": None}
-        default_options = {"molecule": None,
-                           "dt": 0.5, "max_cycles": 100,
-                           "min_de": 1.e-7,
-                           "pool": uccgsd_pool,
-                           "pool_args": None,
-                           "frozen_orbitals": "frozen_core",
-                           "qubit_mapping": "jw",
-                           "qubit_hamiltonian": None,
-                           "up_then_down": False,
-                           "n_spinorbitals": None,
-                           "n_electrons": None,
-                           "backend_options": default_backend_options,
-                           "verbose": True}
-
-        # Initialize with default values
-        self.__dict__ = default_options
-        # Overwrite default values with user-provided ones, if they correspond to a valid keyword
-        for k, v in opt_dict.items():
-            if k in default_options:
-                setattr(self, k, v)
-            else:
-                raise KeyError(f"Keyword :: {k}, not available in {self.__class__.__name__}")
+
+        copt_dict = opt_dict.copy()
+        self.molecule: SecondQuantizedMolecule = copt_dict.pop("molecule", None)
+        self.dt: float = copt_dict.pop("dt", 0.5)
+        self.max_cycles: int = copt_dict.pop("max_cycles", 100)
+        self.min_de: float = copt_dict.pop("min_de", 1.e-7)
+        self.pool: Callable[..., Union[List[QubitOperator], List[FermionOperator]]] = copt_dict.pop("pool", uccgsd_pool)
+        self.pool_args: dict = copt_dict.pop("pool_args", None)
+        self.frozen_orbitals: Union[str, List] = copt_dict.pop("frozen_orbitals", "frozen_core")
+        self.qubit_mapping: str = copt_dict.pop("qubit_mapping", "jw")
+        self.qubit_hamiltonian: QubitOperator = copt_dict.pop("qubit_hamiltonian", None)
+        self.up_then_down: bool = copt_dict.pop("up_then_down", False)
+        self.n_spinorbitals: int = copt_dict.pop("n_spinorbitals", None)
+        self.n_electrons: int = copt_dict.pop("n_electrons", None)
+        self.backend_options: dict = copt_dict.pop("backend_options", default_backend_options)
+        self.verbose: bool = copt_dict.pop("verbose", True)
+
+        if len(copt_dict) > 0:
+            raise KeyError(f"The following keywords are not supported in {self.__class__.__name__}: \n {copt_dict.keys()}")
 
         # Raise error/warnings if input is not as expected. Only a single input
         # must be provided to avoid conflicts.
         if not (bool(self.molecule) ^ bool(self.qubit_hamiltonian)):
             raise ValueError("A molecule OR qubit Hamiltonian object must be provided when instantiating "
                              f"{self.__class__.__name__}.")
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/projective/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/projective/tests/test_qite.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/test_qite.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/adapt_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/adapt_vqe_solver.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,19 +24,21 @@
     An adaptive variational algorithm for exact molecular simulations on a
     quantum computer.
     Nat Commun 10, 3007 (2019). https://doi.org/10.1038/s41467-019-10988-2.
 """
 
 import math
 import warnings
+from typing import Optional, Union, List, Callable
 
 from scipy.optimize import minimize
 from openfermion import commutator
 from openfermion import FermionOperator as ofFermionOperator
 
+from tangelo import SecondQuantizedMolecule
 from tangelo.toolboxes.operators.operators import FermionOperator, QubitOperator
 from tangelo.toolboxes.ansatz_generator.adapt_ansatz import ADAPTAnsatz
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.ansatz_generator._general_unitary_cc import uccgsd_generator as uccgsd_pool
 from tangelo.linq import Circuit, Gate
 from tangelo.algorithms.variational.vqe_solver import VQESolver
 
@@ -47,62 +49,65 @@
     energy.
 
     Attributes:
         molecule (SecondQuantizedMolecule): The molecular system.
         tol (float): Maximum gradient allowed for a particular operator  before
             convergence.
         max_cycles (int): Maximum number of iterations for ADAPT.
-        pool (func): Function that returns a list of FermionOperator. Each
+        pool (func): Function that returns a list of FermionOperator or QubitOperator. Each
             element represents excitation/operator that has an effect of the
             total energy.
         pool_args (dict) : The arguments for the pool function. Will be unpacked in
             function call as pool(**pool_args)
         qubit_mapping (str): One of the supported qubit mapping identifiers.
         qubit_hamiltonian (QubitOperator-like): Self-explanatory.
         up_then_down (bool): Spin orbitals ordering.
         n_spinorbitals (int): Self-explanatory.
         n_electrons (int): Self-explanatory.
+        spin (int): The spin of the system (# alpha - # beta electrons)
         optimizer (func): Optimization function for VQE minimization.
         backend_options (dict): Backend options for the underlying VQE object.
+        simulate_options (dict): Options for fine-control of the simulator backend, including desired measurement results, etc.
         verbose (bool): Flag for verbosity of VQE.
         deflation_circuits (list[Circuit]): Deflation circuits to add an
             orthogonalization penalty with.
         deflation_coeff (float): The coefficient of the deflation.
+        projective_circuit (Circuit): A terminal circuit that projects into the correct space, always added to
+            the end of the ansatz circuit.
         ref_state (array or Circuit): The reference configuration to use. Replaces HF state
      """
 
     def __init__(self, opt_dict):
 
         default_backend_options = {"target": None, "n_shots": None, "noise_model": None}
-        default_options = {"molecule": None,
-                           "tol": 1e-3, "max_cycles": 15,
-                           "pool": uccgsd_pool,
-                           "pool_args": None,
-                           "qubit_mapping": "jw",
-                           "qubit_hamiltonian": None,
-                           "up_then_down": False,
-                           "n_spinorbitals": None,
-                           "n_electrons": None,
-                           "spin": None,
-                           "optimizer": self.LBFGSB_optimizer,
-                           "backend_options": default_backend_options,
-                           "verbose": False,
-                           "ref_state": None,
-                           "deflation_circuits": list(),
-                           "deflation_coeff": 1}
-
-        # Initialize with default values
-        self.__dict__ = default_options
-        # Overwrite default values with user-provided ones, if they correspond to a valid keyword
-        for k, v in opt_dict.items():
-            if k in default_options:
-                setattr(self, k, v)
-            else:
-                # TODO Raise a warning instead, that variable will not be used unless user made mods to code
-                raise KeyError(f"Keyword :: {k}, not available in {self.__class__.__name__}")
+
+        copt_dict = opt_dict.copy()
+
+        self.molecule: Optional[SecondQuantizedMolecule] = copt_dict.pop("molecule", None)
+        self.tol: float = copt_dict.pop("tol", 1e-3)
+        self.max_cycles: int = copt_dict.pop("max_cycles", 15)
+        self.pool: Callable[..., Union[List[QubitOperator], List[FermionOperator]]] = copt_dict.pop("pool", uccgsd_pool)
+        self.pool_args: dict = copt_dict.pop("pool_args", None)
+        self.qubit_mapping: str = copt_dict.pop("qubit_mapping", "jw")
+        self.optimizer = copt_dict.pop("optimizer", self.LBFGSB_optimizer)
+        self.backend_options: dict = copt_dict.pop("backend_options", default_backend_options)
+        self.simulate_options: dict = copt_dict.pop("simulate_options", dict())
+        self.deflation_circuits: Optional[List[Circuit]] = copt_dict.pop("deflation_circuits", list())
+        self.deflation_coeff: float = copt_dict.pop("deflation_coeff", 1.)
+        self.up_then_down: bool = copt_dict.pop("up_then_down", False)
+        self.spin: int = copt_dict.pop("spin", 0)
+        self.qubit_hamiltonian: QubitOperator = copt_dict.pop("qubit_hamiltonian", None)
+        self.verbose: bool = copt_dict.pop("verbose", False)
+        self.projective_circuit: Circuit = copt_dict.pop("projective_circuit", None)
+        self.ref_state: Optional[Union[list, Circuit]] = copt_dict.pop("ref_state", None)
+        self.n_spinorbitals: Union[None, int] = copt_dict.pop("n_spinorbitals", None)
+        self.n_electrons: Union[None, int] = copt_dict.pop("n_electrons", None)
+
+        if len(copt_dict) > 0:
+            raise KeyError(f"The following keywords are not supported in {self.__class__.__name__}: \n {copt_dict.keys()}")
 
         # Raise error/warnings if input is not as expected. Only a single input
         # must be provided to avoid conflicts.
         if not (bool(self.molecule) ^ bool(self.qubit_hamiltonian)):
             raise ValueError(f"A molecule OR qubit Hamiltonian object must be provided when instantiating {self.__class__.__name__}.")
 
         self.ansatz = None
@@ -156,16 +161,18 @@
         self.ansatz = ADAPTAnsatz(self.n_spinorbitals, self.n_electrons, self.spin, ansatz_options)
 
         # Build underlying VQE solver. Options remain consistent throughout the ADAPT cycles.
         self.vqe_options = {"qubit_hamiltonian": self.qubit_hamiltonian,
                             "ansatz": self.ansatz,
                             "optimizer": self.optimizer,
                             "backend_options": self.backend_options,
+                            "simulate_options": self.simulate_options,
                             "deflation_circuits": self.deflation_circuits,
                             "deflation_coeff": self.deflation_coeff,
+                            "projective_circuit": self.projective_circuit,
                             "ref_state": self.ref_state
                             }
 
         self.vqe_solver = VQESolver(self.vqe_options)
 
         # Circuits without variational parameter raise a warning in VQESolver.
         warnings.filterwarnings("ignore", message="No variational gate found in the circuit.")
@@ -183,18 +190,18 @@
             else:
                 raise KeyError('pool_args must be defined if using own pool function')
 
         # Check if pool function returns a QubitOperator or FermionOperator and populate variables
         pool_list = self.pool(**self.pool_args)
 
         # Only a qubit operator is provided with a FermionOperator pool.
-        if not (self.n_spinorbitals and self.n_electrons and self.spin is not None):
+        if not (self.n_spinorbitals and self.n_electrons and isinstance(self.spin, int)):
             raise ValueError("Expecting the number of spin-orbitals (n_spinorbitals), "
-                "the number of electrons (n_electrons) and the spin (spin) with "
-                "a qubit_hamiltonian when working with a pool of fermion operators.")
+                             "the number of electrons (n_electrons) and the spin (spin) with "
+                             "a qubit_hamiltonian when working with a pool of fermion operators.")
 
         if isinstance(pool_list[0], QubitOperator):
             self.pool_type = 'qubit'
             self.pool_operators = pool_list
         elif isinstance(pool_list[0], (FermionOperator, ofFermionOperator)):
             self.pool_type = 'fermion'
             self.fermionic_operators = pool_list
@@ -228,14 +235,16 @@
         while self.iteration < self.max_cycles:
             self.iteration += 1
             if self.verbose:
                 print(f"Iteration {self.iteration} of ADAPT-VQE.")
 
             full_circuit = (self.vqe_solver.ansatz.circuit if self.ref_state is None else
                             self.vqe_solver.reference_circuit + self.vqe_solver.ansatz.circuit)
+            if self.projective_circuit:
+                full_circuit += self.projective_circuit
             gradients = self.compute_gradients(full_circuit, backend=self.vqe_solver.backend)
             pool_select = self.choose_operator(gradients, tolerance=self.tol)
 
             # If pool selection returns an operator that changes the energy by
             # more than self.tol. Else, the loop is complete and the energy is
             # considered as converged.
             if pool_select:
@@ -276,23 +285,23 @@
             circuit (tangelo.linq.Circuit): Circuit for measuring each commutator.
             backend (tangelo.linq.Backend): Backend to compute expectation values.
 
        Returns:
             list of float: Operator gradients.
         """
 
-        gradient = [abs(backend.get_expectation_value(element, circuit)) for element in self.pool_commutators]
+        gradient = [abs(backend.get_expectation_value(element, circuit, **self.simulate_options)) for element in self.pool_commutators]
         for deflate_circuit in self.deflation_circuits:
             for i, pool_op in enumerate(self.pool_operators):
                 op_circuit = Circuit([Gate(op[1], op[0]) for tuple in pool_op.terms for op in tuple])
                 pool_over = deflate_circuit.inverse() + op_circuit + circuit
-                f_dict, _ = backend.simulate(pool_over)
+                f_dict, _ = backend.simulate(pool_over, **self.simulate_options)
                 grad = f_dict.get("0"*self.vqe_solver.ansatz.circuit.width, 0)
                 pool_over = deflate_circuit.inverse() + circuit
-                f_dict, _ = backend.simulate(pool_over)
+                f_dict, _ = backend.simulate(pool_over, **self.simulate_options)
                 gradient[i] += self.deflation_coeff * grad * f_dict.get("0"*self.vqe_solver.ansatz.circuit.width, 0)
 
         return gradient
 
     def choose_operator(self, gradients, tolerance=1e-3):
         """Choose next operator to add according to the ADAPT-VQE algorithm.
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/iqcc_ilc_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/iqcc_ilc_solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,19 +25,22 @@
 that occurs when QCC generators are used.
 Refs:
     1. R. A. Lang, I. G. Ryabinkin, and A. F. Izmaylov.
         arXiv:2002.05701v1, 2020, 1–10.
     2. R. A. Lang, I. G. Ryabinkin, and A. F. Izmaylov.
         J. Chem. Theory Comput. 2021, 17, 1, 66–78.
 """
+from typing import List, Union, Optional
 
+from tangelo import SecondQuantizedMolecule
+from tangelo.algorithms.variational.vqe_solver import VQESolver
 from tangelo.linq import get_backend
+from tangelo.toolboxes.operators import QubitOperator
 from tangelo.toolboxes.ansatz_generator.ilc import ILC
 from tangelo.toolboxes.ansatz_generator.qcc import QCC
-from tangelo.algorithms.variational.vqe_solver import VQESolver
 from tangelo.toolboxes.ansatz_generator._qubit_ilc import ilc_op_dress
 
 
 class iQCC_ILC_solver:
     """The iQCC-ILC-VQE solver class combines the both the ILC and ILC ansatze
     Classes with the VQESolver class to perform an iterative and variational
     procedure to compute the total iQCC-ILC energy for a given Hamiltonian.
@@ -79,36 +82,32 @@
             Default, 1.59e-3 Hartree.
         verbose (bool): Flag for verbosity. Default, False.
      """
 
     def __init__(self, opt_dict):
 
         default_backend_options = {"target": None, "n_shots": None, "noise_model": None}
-        default_options = {"molecule": None,
-                           "qubit_mapping": "jw",
-                           "up_then_down": False,
-                           "initial_var_params": None,
-                           "backend_options": default_backend_options,
-                           "penalty_terms": None,
-                           "ilc_ansatz_options": dict(),
-                           "qcc_ansatz_options": dict(),
-                           "qubit_hamiltonian": None,
-                           "max_ilc_iter": 3,
-                           "compress_qubit_ham": False,
-                           "compress_eps": 1.59e-3,
-                           "verbose": False}
-
-        # Initialize with default values
-        self.__dict__ = default_options
-        # Overwrite default values with user-provided ones, if they correspond to a valid keyword
-        for param, val in opt_dict.items():
-            if param in default_options:
-                setattr(self, param, val)
-            else:
-                raise KeyError(f"The keyword {param} is not available in self.__class__.__name__.")
+
+        copt_dict = opt_dict.copy()
+        self.molecule: SecondQuantizedMolecule = copt_dict.pop("molecule", None)
+        self.qubit_mapping: str = copt_dict.pop("qubit_mapping", "jw")
+        self.up_then_down: str = copt_dict.pop("up_then_down", False)
+        self.initial_var_params: Union[List, str] = copt_dict.pop("initial_var_params", None)
+        self.backend_options: dict = copt_dict.pop("backend_options", default_backend_options)
+        self.penalty_terms: Optional[dict] = copt_dict.pop("penalty_terms", None)
+        self.ilc_ansatz_options: dict = copt_dict.pop("ilc_ansatz_options", dict())
+        self.qcc_ansatz_options: dict = copt_dict.pop("qcc_ansatz_options", dict())
+        self.qubit_hamiltonian: QubitOperator = copt_dict.pop("qubit_hamiltonian", None)
+        self.max_ilc_iter: int = copt_dict.pop("max_ilc_iter", 3)
+        self.compress_qubit_ham: bool = copt_dict.pop("compress_qubit_ham", False)
+        self.compress_eps: float = copt_dict.pop("compress_eps", 1.59e-3)
+        self.verbose: bool = copt_dict.pop("verbose", False)
+
+        if len(copt_dict) > 0:
+            raise KeyError(f"The following keywords are not supported in {self.__class__.__name__}: \n {copt_dict.keys()}")
 
         if not self.molecule and not self.qubit_hamiltonian:
             raise ValueError("An instance of SecondQuantizedMolecule or QubitOperator "
                              "is required for initializing self.__class__.__name__.")
 
         # initialize variables and lists to store useful data from each ILC-VQE iteration
         self.energies = []
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/iqcc_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/iqcc_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,19 @@
 exponential growth of the number of terms.
 
 Refs:
     1. I. G. Ryabinkin, R. A. Lang, S. N. Genin, and A. F. Izmaylov.
         J. Chem. Theory Comput. 2020, 16, 2, 1055–1063.
 """
 
+from typing import Union
+
+from tangelo import SecondQuantizedMolecule
 from tangelo.linq import get_backend
+from tangelo.toolboxes.operators import QubitOperator
 from tangelo.toolboxes.ansatz_generator.qcc import QCC
 from tangelo.algorithms.variational.vqe_solver import VQESolver, BuiltInAnsatze
 from tangelo.toolboxes.ansatz_generator._qubit_cc import qcc_op_dress
 
 
 class iQCC_solver:
     """The iQCC-VQE solver class combines the QCC ansatz and VQESolver classes
@@ -87,37 +91,33 @@
             Default, 1.59e-3 Hartree.
         verbose (bool): Flag for verbosity. Default, False.
      """
 
     def __init__(self, opt_dict):
 
         default_backend_options = {"target": None, "n_shots": None, "noise_model": None}
-        default_options = {"molecule": None,
-                           "qubit_mapping": "jw",
-                           "up_then_down": False,
-                           "initial_var_params": None,
-                           "backend_options": default_backend_options,
-                           "penalty_terms": None,
-                           "ansatz_options": dict(),
-                           "qubit_hamiltonian": None,
-                           "deqcc_thresh": 1e-5,
-                           "max_iqcc_iter": 100,
-                           "max_iqcc_retries": 10,
-                           "compress_qubit_ham": False,
-                           "compress_eps": 1.59e-3,
-                           "verbose": False}
-
-        # Initialize with default values
-        self.__dict__ = default_options
-        # Overwrite default values with user-provided ones, if they correspond to a valid keyword
-        for param, val in opt_dict.items():
-            if param in default_options:
-                setattr(self, param, val)
-            else:
-                raise KeyError(f"Keyword {param} not available in self.__class__.__name__.")
+
+        copt_dict = opt_dict.copy()
+        self.molecule: SecondQuantizedMolecule = copt_dict.pop("molecule", None)
+        self.qubit_mapping: str = copt_dict.pop("qubit_mapping", "jw")
+        self.up_then_down: bool = copt_dict.pop("up_then_down", False)
+        self.initial_var_params: Union[str, list] = copt_dict.pop("initial_var_params", None)
+        self.backend_options: dict = copt_dict.pop("backend_options", default_backend_options)
+        self.penalty_terms: dict = copt_dict.pop("penalty_terms", None)
+        self.ansatz_options: dict = copt_dict.pop("ansatz_options", dict())
+        self.qubit_hamiltonian: QubitOperator = copt_dict.pop("qubit_hamiltonian", None)
+        self.deqcc_thresh: float = copt_dict.pop("deqcc_thresh", 1e-5)
+        self.max_iqcc_iter: int = copt_dict.pop("max_iqcc_iter", 100)
+        self.max_iqcc_retries: int = copt_dict.pop("max_iqcc_retries", 10)
+        self.compress_qubit_ham: bool = copt_dict.pop("compress_qubit_ham", False)
+        self.compress_eps: float = copt_dict.pop("compress_eps", 1.59e-3)
+        self.verbose: bool = copt_dict.pop("verbose", False)
+
+        if len(copt_dict) > 0:
+            raise KeyError(f"The following keywords are not supported in {self.__class__.__name__}: \n {copt_dict.keys()}")
 
         if not self.molecule:
             raise ValueError(f"An instance of SecondQuantizedMolecule is required for initializing {self.__class__.__name__}.")
 
         # initialize variables and lists to store useful data from each iQCC-VQE iteration
         self.energies = []
         self.iteration = 0
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/sa_oo_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/sa_oo_vqe_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,21 +45,24 @@
         n_oo_per_iter (int): Number of orbital optimization Newton-Raphson steps per SA-OO-VQE iteration
         molecule (SecondQuantizedMolecule) : the molecular system.
         qubit_mapping (str) : one of the supported qubit mapping identifiers.
         ansatz (Ansatze) : one of the supported ansatze.
         optimizer (function handle): a function defining the classical optimizer and its behavior.
         initial_var_params (str or array-like) : initial value for the classical optimizer.
         backend_options (dict): parameters to build the underlying compute backend (simulator, etc).
+        simulate_options (dict): Options for fine-control of the simulator backend, including desired measurement results, etc.
         penalty_terms (dict): parameters for penalty terms to append to target qubit Hamiltonian (see penalty_terms
             for more details).
         ansatz_options (dict): parameters for the given ansatz (see given ansatz file for details).
         up_then_down (bool): change basis ordering putting all spin up orbitals first, followed by all spin down.
             Default, False has alternating spin up/down ordering.
         qubit_hamiltonian (QubitOperator-like): Self-explanatory.
         verbose (bool): Flag for VQE verbosity.
+        projective_circuit (Circuit): A terminal circuit that projects into the correct space, always added to
+            the end of the ansatz circuit.
         ref_states (list): The vector occupations of the reference configurations
         weights (array): The weights of the occupations
      """
 
     def __init__(self, opt_dict: dict):
 
         oo_options = {"tol": 1e-3,
@@ -75,16 +78,17 @@
             if k in oo_options:
                 oo_options[k] = opt_dict_sa_vqe.pop(k)
 
         # Initialization of SA_VQESOLVER will check if spurious dictionary items are present
         super().__init__(opt_dict_sa_vqe)
 
         # Add oo_options to attributes
-        for k, v in oo_options.items():
-            setattr(self, k, v)
+        self.tol: float = oo_options["tol"]
+        self.max_cycles: int = oo_options["max_cycles"]
+        self.n_oo_per_iter: int = oo_options["n_oo_per_iter"]
 
         self.n_ref_states = len(self.ref_states)
 
         self.converged = False
         self.iteration = 0
         self.energies = list()
         # vqe_energies could include a penalty term contribution so will be different from energies calculated using rdms
@@ -106,15 +110,15 @@
             if self.verbose:
                 print(f"The State-Averaged VQE energy for iteration {iter} is: {energy_new}")
             if iter > 0 and abs(energy_new-self.energies[-1]) < self.tol:
                 self.energies.append(energy_new)
                 break
             for _ in range(self.n_oo_per_iter):
                 u_mat = self.generate_oo_unitary()
-                self.molecule.mean_field.mo_coeff = self.molecule.mean_field.mo_coeff @ u_mat
+                self.molecule.mo_coeff = self.molecule.mo_coeff @ u_mat
             self.energies.append(self.energy_from_rdms())
             if self.verbose:
                 print(f"The State-Averaged Orbital Optimized energy for iteration {iter} is: {self.energies[-1]}")
             self.build()
 
     def energy_from_rdms(self):
         "Calculate energy from rdms generated from SA_VQESolver"
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/sa_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/sa_vqe_solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 [1] Saad Yalouz, Bruno Senjean, Jakob Gunther, Francesco Buda, Thomas E. O'Brien, Lucas Visscher, "A state-averaged
 orbital-optimized hybrid quantum-classical algorithm for a democratic description of ground and excited states",
 2021, Quantum Sci. Technol. 6 024004
 [2] Ken M Nakanishi, Kosuke Mitarai, Keisuke Fujii, "Subspace-search variational quantum eigensolver for excited states",
 Phys. Rev. Research 1, 033062 (2019)
 """
 
+from typing import List, Union, Type
+
 import numpy as np
 
 from tangelo.linq import get_backend, Circuit
 from tangelo.toolboxes.qubit_mappings import statevector_mapping
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.ansatz_generator.penalty_terms import combined_penalty
 from tangelo.algorithms.variational import BuiltInAnsatze, VQESolver
@@ -50,23 +52,26 @@
     Attributes:
         molecule (SecondQuantizedMolecule) : the molecular system.
         qubit_mapping (str) : one of the supported qubit mapping identifiers.
         ansatz (Ansatze) : one of the supported ansatze.
         optimizer (function handle): a function defining the classical optimizer and its behavior.
         initial_var_params (str or array-like) : initial value for the classical optimizer.
         backend_options (dict): parameters to build the underlying compute backend (simulator, etc).
+        simulate_options (dict): Options for fine-control of the simulator backend, including desired measurement results, etc.
         penalty_terms (dict): parameters for penalty terms to append to target qubit Hamiltonian (see penalty_terms
             for more details).
         deflation_circuits (list[Circuit]): Deflation circuits to add an orthogonalization penalty with.
         deflation_coeff (float): The coefficient of the deflation.
         ansatz_options (dict): parameters for the given ansatz (see given ansatz file for details).
         up_then_down (bool): change basis ordering putting all spin up orbitals first, followed by all spin down.
             Default, False has alternating spin up/down ordering.
         qubit_hamiltonian (QubitOperator-like): Self-explanatory.
         verbose (bool): Flag for VQE verbosity.
+        projective_circuit (Circuit): A terminal circuit that projects into the correct space, always added to
+            the end of the ansatz circuit.
         ref_states (list): The vector occupations of the reference configurations or the reference circuits.
         weights (array): The weights of the occupations
     """
 
     def __init__(self, opt_dict):
 
         sa_vqe_options = {"ref_states": None, "weights": None, "ansatz": BuiltInAnsatze.UCCGD}
@@ -79,16 +84,17 @@
 
         # Initialization of VQESolver will check if spurious dictionary items are present
         super().__init__(opt_dict_vqe)
 
         self.builtin_ansatze = set([BuiltInAnsatze.UpCCGSD, BuiltInAnsatze.UCCGD, BuiltInAnsatze.HEA, BuiltInAnsatze.UCCSD])
 
         # Add sa_vqe_options to attributes
-        for k, v in sa_vqe_options.items():
-            setattr(self, k, v)
+        self.ref_states: Union[List[int], np.ndarray] = sa_vqe_options["ref_states"]
+        self.weights: Union[List[float], np.ndarray] = sa_vqe_options["weights"]
+        self.ansatz: Type[agen.Ansatz] = sa_vqe_options["ansatz"]
 
         if self.ref_states is None:
             raise ValueError(f"ref_states must be provided when instantiating {self.__class__.__name__}")
 
         self.n_states = len(self.ref_states)
         if self.weights is None:
             self.weights = np.ones(self.n_states)/self.n_states
@@ -191,17 +197,19 @@
         """
 
         # Update variational parameters, compute energy using the hardware backend
         self.ansatz.update_var_params(var_params)
         energy = 0
         self.state_energies = list()
         for i, reference_circuit in enumerate(self.reference_circuits):
-            state_energy = self.backend.get_expectation_value(self.qubit_hamiltonian, reference_circuit + self.ansatz.circuit)
+            full_circ = (reference_circuit + self.ansatz.circuit + self.projective_circuit if self.projective_circuit
+                         else reference_circuit + self.ansatz.circuit)
+            state_energy = self.backend.get_expectation_value(self.qubit_hamiltonian, full_circ, **self.simulate_options)
             for circ in self.deflation_circuits:
-                f_dict, _ = self.backend.simulate(circ + self.ansatz.circuit.inverse() + reference_circuit.inverse())
+                f_dict, _ = self.backend.simulate(circ + full_circ.inverse(), **self.simulate_options)
                 state_energy += self.deflation_coeff * f_dict.get("0"*self.ansatz.circuit.width, 0)
             energy += state_energy*self.weights[i]
             self.state_energies.append(state_energy)
 
         if self.verbose:
             print(f"\tEnergy = {energy:.7f} ")
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_adapt_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_adapt_vqe_solver.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,26 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
-from tangelo.algorithms.variational import ADAPTSolver
+import numpy as np
+
 from tangelo.molecule_library import mol_H2_sto3g, xyz_H4
+from tangelo.linq import Circuit, Gate
+from tangelo.algorithms.variational import ADAPTSolver
+from tangelo.toolboxes.ansatz_generator.fermionic_operators import spinz_operator
+from tangelo.toolboxes.ansatz_generator.ansatz_utils import trotterize, get_qft_circuit
+from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.ansatz_generator._unitary_majorana_cc import get_majorana_uccgsd_pool, get_majorana_uccsd_pool
 from tangelo.toolboxes.molecular_computation.molecule import SecondQuantizedMolecule
 
 
 class ADAPTSolverTest(unittest.TestCase):
 
     def test_build_adapt(self):
         """Try instantiating ADAPTSolver with basic input."""
 
-        opt_dict = {"molecule": mol_H2_sto3g, "max_cycles": 15}
+        opt_dict = {"molecule": mol_H2_sto3g, "max_cycles": 15, "spin": 0}
         adapt_solver = ADAPTSolver(opt_dict)
         adapt_solver.build()
 
     def test_single_cycle_adapt(self):
         """Try instantiating ADAPTSolver with basic input. The fermionic term
         ordering has been taken from the reference below (original paper for
         ADAPT-VQE).
@@ -57,24 +63,24 @@
         self.assertEqual(adapt_solver.get_resources(), resources)
 
     def test_multiple_cycle_adapt_majorana_pool(self):
         """Solve H4 with one frozen orbital with ADAPTSolver using 4 cycles and operators chosen
         from a Majorana UCCGSD pool and a Majorana UCCSD pool
         """
 
-        mol = SecondQuantizedMolecule(xyz_H4, 0, 0, "sto-3g", frozen_orbitals=[0])
+        mol = SecondQuantizedMolecule(xyz_H4, 0, 0, basis="sto-3g", frozen_orbitals=[0])
         opt_dict = {"molecule": mol, "max_cycles": 4, "verbose": False, "pool": get_majorana_uccgsd_pool,
                     "pool_args": {"n_sos": mol.n_active_sos}}
         adapt_solver = ADAPTSolver(opt_dict)
         adapt_solver.build()
         adapt_solver.simulate()
 
         self.assertAlmostEqual(adapt_solver.optimal_energy, -1.8945, places=3)
 
-        mol = SecondQuantizedMolecule(xyz_H4, 0, 0, "sto-3g", frozen_orbitals=[0])
+        mol = SecondQuantizedMolecule(xyz_H4, 0, 0, basis="sto-3g", frozen_orbitals=[0])
         opt_dict = {"molecule": mol, "max_cycles": 4, "verbose": False, "pool": get_majorana_uccsd_pool,
                     "pool_args": {"n_electrons": mol.n_active_electrons, "n_sos": mol.n_active_sos}}
         adapt_solver = ADAPTSolver(opt_dict)
         adapt_solver.build()
         adapt_solver.simulate()
 
         self.assertAlmostEqual(adapt_solver.optimal_energy, -1.8945, places=3)
@@ -91,15 +97,15 @@
         self.assertAlmostEqual(optimal_energy, -1.91062, places=3)
 
     def test_multiple_cycle_adapt_majorana_pool_with_deflation(self):
         """Solve H4 with one frozen orbtial with ADAPTSolver using 4 cycles and operators chosen
         from a Majorana UCCGSD pool followed by deflation for an orthogonal state triplet state.
         """
 
-        mol = SecondQuantizedMolecule(xyz_H4, 0, 0, "sto-3g", frozen_orbitals=[0])
+        mol = SecondQuantizedMolecule(xyz_H4, 0, 0, basis="sto-3g", frozen_orbitals=[0])
         opt_dict = {"molecule": mol, "max_cycles": 4, "verbose": False, "pool": get_majorana_uccgsd_pool,
                     "pool_args": {"n_sos": mol.n_active_sos}}
         adapt_solver = ADAPTSolver(opt_dict)
         adapt_solver.build()
         adapt_solver.simulate()
 
         self.assertAlmostEqual(adapt_solver.optimal_energy, -1.8945, places=3)
@@ -111,10 +117,42 @@
                     "deflation_circuits": deflation_circuits, "ref_state": ref_state, "deflation_coeff": 1}
         adapt_solver = ADAPTSolver(opt_dict)
         adapt_solver.build()
         optimal_energy = adapt_solver.simulate()
 
         self.assertAlmostEqual(optimal_energy, -1.91062, places=3)
 
+    def test_sym_projected(self):
+        """Solve Linear H3 with one frozen orbtial with ADAPTSolver using 4 cycles and operators chosen
+        from a Majorana UCCGSD pool, with a sz symmetry projection.
+        """
+
+        xyz_H3 = [("H", [0., 0., 0.]), ("H", [1., 0., 0.]), ("H", [2., 0., 0.])]
+        mol = SecondQuantizedMolecule(xyz_H3, 0, 1, basis="sto-3g")
+
+        # QPE based Sz projection.
+        def sz_check(n_state: int, molecule: SecondQuantizedMolecule, mapping: str, up_then_down):
+            n_qft = 3
+            spin_fe_op = spinz_operator(molecule.n_active_mos)
+            q_spin = fermion_to_qubit_mapping(spin_fe_op, mapping, molecule.n_active_sos, molecule.n_active_electrons, up_then_down, molecule.spin)
+
+            sym_var_circuit = Circuit([Gate("H", n_state + q) for q in range(n_qft)])
+            for j, i in enumerate(range(n_state, n_state+n_qft)):
+                sym_var_circuit += trotterize(2*q_spin+3, -2*np.pi/2**(j+1), control=i)
+            sym_var_circuit += get_qft_circuit(list(range(n_state+n_qft-1, n_state-1, -1)), inverse=True)
+            sym_var_circuit += Circuit([Gate("MEASURE", i) for i in range(n_state, n_state+n_qft)])
+            return sym_var_circuit
+
+        proj_circuit = sz_check(6, mol, "JW", False)
+
+        opt_dict = {"molecule": mol, "max_cycles": 4, "verbose": False, "pool": get_majorana_uccgsd_pool,
+                    "pool_args": {"n_sos": mol.n_active_sos}, "simulate_options": {"desired_meas_result": "100"},
+                    "projective_circuit": proj_circuit}
+        adapt_solver = ADAPTSolver(opt_dict)
+        adapt_solver.build()
+        adapt_solver.simulate()
+
+        self.assertAlmostEqual(adapt_solver.optimal_energy, -1.56835, places=5)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_iqcc_ilc_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_iqcc_ilc_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_iqcc_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_iqcc_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_sa_oo_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_sa_oo_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_sa_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_sa_vqe_solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
 import numpy as np
 
+from tangelo.linq import Circuit, Gate
 from tangelo.algorithms import BuiltInAnsatze, SA_VQESolver
 from tangelo.molecule_library import mol_H2_sto3g
 from tangelo.toolboxes.ansatz_generator import UCCSD
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.molecular_computation.rdms import matricize_2rdm
 
 
@@ -133,14 +134,39 @@
                        "deflation_coeff": 1.5, "ref_states": [[0, 0, 1, 1]]}
         vqe_solver_2 = SA_VQESolver(vqe_options)
         vqe_solver_2.build()
 
         energy = vqe_solver_2.simulate()
         self.assertAlmostEqual(exact_energies[2], energy, delta=1.e-3)
 
+    def test_projected_simulate_h2(self):
+        """Run SA-VQE on H2 molecule with a parity check projection, with UpCCGSD ansatz, JW qubit mapping,
+        ref_states and exact simulator.
+        """
+
+        sym_check = Circuit([Gate("CNOT", target=q, control=4) for q in {0, 2}] + [Gate("CNOT", target=q, control=5) for q in [1, 3]])
+        sym_check += Circuit([Gate("MEASURE", 4), Gate("MEASURE", 5)])
+
+        vqe_options = {"molecule": mol_H2_sto3g, "ansatz": BuiltInAnsatze.UpCCGSD, "qubit_mapping": "jw",
+                       "verbose": True, "ref_states": [[1, 1, 0, 0], [1, 0, 0, 1]], "weights": [1.2, 0.9],
+                       "projective_circuit": sym_check, "simulate_options": {"desired_meas_result": "00"}}
+        sa_vqe_solver = SA_VQESolver(vqe_options)
+        sa_vqe_solver.build()
+
+        # code to generate exact results.
+        # from pyscf import mcscf
+        # mc = mcscf.CASCI(mol_H2_sto3g.mean_field, 2, 2)
+        # mc.fcisolver.nroots = 3
+        # exact_energies = mc.casci()[0]
+        exact_energies = [-1.1372702, -0.5324790, -0.1699013]
+
+        # Use state averaging to get ground and first excited state.
+        _ = sa_vqe_solver.simulate()
+        np.testing.assert_array_almost_equal(exact_energies[:2], sa_vqe_solver.state_energies, decimal=3)
+
     def test_get_rdm_h2(self):
         """Compute RDMs with UCCSD ansatz, JW qubit mapping, optimized
         parameters, exact simulator (H2).
         """
 
         vqe_options = {"molecule": mol_H2_sto3g, "ansatz": BuiltInAnsatze.UCCSD, "qubit_mapping": "jw", "ref_states": [[1, 1, 0, 0]]}
         sa_vqe_solver = SA_VQESolver(vqe_options)
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_tetris_adapt_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_tetris_adapt_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tests/test_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_vqe_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 import numpy as np
 
-from tangelo.linq import get_backend
+from tangelo.linq import get_backend, Circuit, Gate
 from tangelo.helpers.utils import installed_backends
 from tangelo.linq.target import QiskitSimulator
 from tangelo.algorithms import BuiltInAnsatze, VQESolver
 from tangelo.molecule_library import mol_H2_sto3g, mol_H4_sto3g, mol_H4_cation_sto3g, mol_NaH_sto3g, mol_H4_sto3g_symm, mol_H4_sto3g_uhf_a1_frozen
 from tangelo.toolboxes.ansatz_generator.uccsd import UCCSD
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.molecular_computation.rdms import matricize_2rdm
 from tangelo.toolboxes.optimizers.rotosolve import rotosolve
+from tangelo.toolboxes.molecular_computation.molecule import SecondQuantizedMolecule
+from tangelo.toolboxes.ansatz_generator.fermionic_operators import spinz_operator
+from tangelo.toolboxes.ansatz_generator.ansatz_utils import trotterize, get_qft_circuit
 
 
 class VQESolverTest(unittest.TestCase):
 
     def test_instantiation_vqe(self):
         """Try instantiating VQESolver with basic input."""
 
@@ -261,25 +264,55 @@
         vqe_solver.build()
 
         energy = vqe_solver.simulate()
         self.assertAlmostEqual(energy, -1.789483, delta=1e-4)
 
     def test_simulate_qcc_h4(self):
         """Run VQE on H4 molecule, with QCC ansatz, JW qubit mapping, initial
-        parameters, exact simulator.
+        parameters, exact simulator. Followed by calculation with Sz symmetry projection
         """
 
         vqe_options = {"molecule": mol_H4_sto3g, "ansatz": BuiltInAnsatze.QCC, "qubit_mapping": "jw",
                         "verbose": False}
         vqe_solver = VQESolver(vqe_options)
         vqe_solver.build()
 
         energy = vqe_solver.simulate()
         self.assertAlmostEqual(energy, -1.963270, delta=1e-4)
 
+        # QPE based Sz projection.
+        def sz_check(n_state: int, molecule: SecondQuantizedMolecule, mapping: str, up_then_down):
+            n_qft = 3
+            spin_fe_op = spinz_operator(molecule.n_active_mos)
+            q_spin = fermion_to_qubit_mapping(spin_fe_op, mapping, molecule.n_active_sos, molecule.n_active_electrons, up_then_down, molecule.spin)
+
+            sym_var_circuit = Circuit([Gate("H", q) for q in range(n_state, n_state+n_qft)])
+            for j, i in enumerate(range(n_state, n_state+n_qft)):
+                sym_var_circuit += trotterize(2*q_spin+3, -2*np.pi/2**(j+1), control=i)
+            sym_var_circuit += get_qft_circuit(list(range(n_state+n_qft-1, n_state-1, -1)), inverse=True)
+            sym_var_circuit += Circuit([Gate("MEASURE", i) for i in range(n_state, n_state+n_qft)])
+            return sym_var_circuit
+
+        # Use a circuit with variational gates and mid-circuit measurements as the ansatz.
+        proj_circuit = sz_check(8, mol_H4_sto3g, "JW", vqe_solver.up_then_down)
+        var_circuit = vqe_solver.optimal_circuit + proj_circuit
+
+        vqe_solver_p = VQESolver({"ansatz": var_circuit, "qubit_hamiltonian": vqe_solver.qubit_hamiltonian, "simulate_options": {"desired_meas_result": "011"}})
+        vqe_solver_p.build()
+        energyp = vqe_solver_p.simulate()
+        self.assertAlmostEqual(energyp, -1.97622, delta=1e-4)
+
+        # Use a circuit with variational gates as the ansatz, add a projective circuit separately.
+        var_circuit = vqe_solver.optimal_circuit
+        vqe_solver_p = VQESolver({"ansatz": var_circuit, "qubit_hamiltonian": vqe_solver.qubit_hamiltonian,
+                                  "simulate_options": {"desired_meas_result": "011"}, "projective_circuit": proj_circuit})
+        vqe_solver_p.build()
+        energyp = vqe_solver_p.simulate()
+        self.assertAlmostEqual(energyp, -1.97622, delta=1e-4)
+
     def test_simulate_ilc_h4(self):
         """Run VQE on H4 molecule, with ILC ansatz, JW qubit mapping, initial
         parameters, exact simulator.
         """
 
         vqe_options = {"molecule": mol_H4_sto3g, "ansatz": BuiltInAnsatze.ILC, "qubit_mapping": "jw",
                         "verbose": False}
```

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/tetris_adapt_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tetris_adapt_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/algorithms/variational/vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/vqe_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 
 """Implements the variational quantum eigensolver (VQE) algorithm to solve
 electronic structure calculations.
 """
 
 import warnings
 import itertools
+from typing import Optional, Union, List
 
 from enum import Enum
 import numpy as np
-from openfermion.ops.operators.qubit_operator import QubitOperator
 
 from tangelo.helpers.utils import HiddenPrints
+from tangelo import SecondQuantizedMolecule
 from tangelo.linq import get_backend, Circuit
 from tangelo.linq.helpers.circuits.measurement_basis import measurement_basis_gates
-from tangelo.toolboxes.operators import count_qubits, FermionOperator
+from tangelo.toolboxes.operators import count_qubits, FermionOperator, QubitOperator
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.qubit_mappings.statevector_mapping import get_mapped_vector, vector_to_circuit
 from tangelo.toolboxes.post_processing.bootstrapping import get_resampled_frequencies
 from tangelo.toolboxes.optimizers import rotosolve
 import tangelo.toolboxes.ansatz_generator as agen
 
 
@@ -68,71 +69,73 @@
         qubit_mapping (str) : one of the supported qubit mapping identifiers.
         ansatz (Ansatze) : one of the supported ansatze.
         optimizer (function handle): a function defining the classical optimizer
             and its behavior.
         initial_var_params (str or array-like) : initial value for the classical
             optimizer.
         backend_options (dict): parameters to build the underlying compute backend (simulator, etc).
+        simulate_options (dict): Options for fine-control of the simulator backend, including desired measurement results, etc.
         penalty_terms (dict): parameters for penalty terms to append to target
             qubit Hamiltonian (see penalty_terms for more details).
         deflation_circuits (list[Circuit]): Deflation circuits to add an
             orthogonalization penalty with.
         deflation_coeff (float): The coefficient of the deflation.
         ansatz_options (dict): parameters for the given ansatz (see given ansatz
             file for details).
         up_then_down (bool): change basis ordering putting all spin up orbitals
             first, followed by all spin down. Default, False has alternating
                 spin up/down ordering.
         qubit_hamiltonian (QubitOperator-like): Self-explanatory.
         verbose (bool): Flag for VQE verbosity.
+        projective_circuit (Circuit): A terminal circuit that projects into the correct space, always added to
+            the end of the ansatz circuit.
         ref_state (array or Circuit): The reference configuration to use. Replaces HF state
             QMF, QCC, ILC require ref_state to be an array. UCC1, UCC3, VSQS can not use a
             different ref_state than HF by construction.
     """
 
     def __init__(self, opt_dict):
 
         default_backend_options = {"target": None, "n_shots": None, "noise_model": None}
-        default_options = {"molecule": None,
-                           "qubit_mapping": "jw", "ansatz": BuiltInAnsatze.UCCSD,
-                           "optimizer": self._default_optimizer,
-                           "initial_var_params": None,
-                           "backend_options": default_backend_options,
-                           "penalty_terms": None,
-                           "deflation_circuits": list(),
-                           "deflation_coeff": 1,
-                           "ansatz_options": dict(),
-                           "up_then_down": False,
-                           "qubit_hamiltonian": None,
-                           "verbose": False,
-                           "ref_state": None}
-
-        # Initialize with default values
-        self.__dict__ = default_options
-        # Overwrite default values with user-provided ones, if they correspond to a valid keyword
-        for k, v in opt_dict.items():
-            if k in default_options:
-                setattr(self, k, v)
-            else:
-                raise KeyError(f"Keyword :: {k}, not available in VQESolver")
+        copt_dict = opt_dict.copy()
+
+        self.molecule: Optional[SecondQuantizedMolecule] = copt_dict.pop("molecule", None)
+        self.qubit_mapping: str = copt_dict.pop("qubit_mapping", "jw")
+        self.ansatz: agen.Ansatz = copt_dict.pop("ansatz", BuiltInAnsatze.UCCSD)
+        self.optimizer = copt_dict.pop("optimizer", self._default_optimizer)
+        self.initial_var_params: Optional[Union[str, list]] = copt_dict.pop("initial_var_params", None)
+        self.backend_options: dict = copt_dict.pop("backend_options", default_backend_options)
+        self.penalty_terms: Optional[dict] = copt_dict.pop("penalty_terms", None)
+        self.simulate_options: dict = copt_dict.pop("simulate_options", dict())
+        self.deflation_circuits: Optional[List[Circuit]] = copt_dict.pop("deflation_circuits", list())
+        self.deflation_coeff: float = copt_dict.pop("deflation_coeff", 1)
+        self.ansatz_options: dict = copt_dict.pop("ansatz_options", dict())
+        self.up_then_down: bool = copt_dict.pop("up_then_down", False)
+        self.qubit_hamiltonian: QubitOperator = copt_dict.pop("qubit_hamiltonian", None)
+        self.verbose: bool = copt_dict.pop("verbose", False)
+        self.projective_circuit: Circuit = copt_dict.pop("projective_circuit", None)
+        self.ref_state: Optional[Union[list, Circuit]] = copt_dict.pop("ref_state", None)
+
+        if len(copt_dict) > 0:
+            raise KeyError(f"The following keywords are not supported in {self.__class__.__name__}: \n {copt_dict.keys()}")
 
         # Raise error/warnings if input is not as expected. Only a single input
         # must be provided to avoid conflicts.
         if not (bool(self.molecule) ^ bool(self.qubit_hamiltonian)):
             raise ValueError(f"A molecule OR qubit Hamiltonian object must be provided when instantiating {self.__class__.__name__}.")
 
         # The QCC & ILC ansatze require up_then_down=True when mapping="jw"
         if isinstance(self.ansatz, BuiltInAnsatze):
             if self.ansatz in (BuiltInAnsatze.QCC, BuiltInAnsatze.ILC) and self.qubit_mapping.lower() == "jw" and not self.up_then_down:
                 warnings.warn("Spin-orbital ordering shifted to all spin-up first then down to ensure efficient generator screening "
                               "for the Jordan-Wigner mapping with QCC-based ansatze.", RuntimeWarning)
                 self.up_then_down = True
             if self.ansatz == BuiltInAnsatze.pUCCD and self.qubit_mapping.lower() != "hcb":
                 warnings.warn("Forcing the hard-core boson mapping for the pUCCD ansatz.", RuntimeWarning)
-                self.mapping = "HCB"
+                self.qubit_mapping = "HCB"
             # QCC and QMF and ILC require a reference state that can be represented by a single layer of RZ-RX gates on each qubit.
             # This decomposition can not be determined from a general Circuit reference state.
             if isinstance(self.ref_state, Circuit):
                 if self.ansatz in [BuiltInAnsatze.QCC, BuiltInAnsatze.ILC, BuiltInAnsatze.QMF]:
                     raise ValueError("Circuit reference state is not supported for QCC or QMF")
             elif self.ref_state is not None:
                 self.ansatz_options["reference_state"] = "zero"
@@ -251,14 +254,16 @@
 
         optimal_energy, optimal_var_params = self.optimizer(self.energy_estimation, self.initial_var_params)
 
         self.optimal_var_params = optimal_var_params
         self.optimal_energy = optimal_energy
         self.ansatz.build_circuit(self.optimal_var_params)
         self.optimal_circuit = self.reference_circuit+self.ansatz.circuit if self.ref_state is not None else self.ansatz.circuit
+        if self.projective_circuit:
+            self.optimal_circuit += self.projective_circuit
         return self.optimal_energy
 
     def get_resources(self):
         """Estimate the resources required by VQE, with the current ansatz. This
         assumes "build" has been run, as it requires the ansatz circuit and the
         qubit Hamiltonian. Return information that pertains to the user, for the
         purpose of running an experiment on a classical simulator or a quantum
@@ -290,15 +295,17 @@
              float: energy computed by VQE using the ansatz and input
                 variational parameters.
         """
 
         # Update variational parameters, compute energy using the hardware backend
         self.ansatz.update_var_params(var_params)
         circuit = self.ansatz.circuit if self.ref_state is None else self.reference_circuit + self.ansatz.circuit
-        energy = self.backend.get_expectation_value(self.qubit_hamiltonian, circuit)
+        if self.projective_circuit:
+            circuit += self.projective_circuit
+        energy = self.backend.get_expectation_value(self.qubit_hamiltonian, circuit, **self.simulate_options)
 
         # Additional computation for deflation (optional)
         for circ in self.deflation_circuits:
             f_dict, _ = self.backend.simulate(circ + circuit.inverse())
             energy += self.deflation_coeff * f_dict.get("0"*self.ansatz.circuit.width, 0)
 
         if self.verbose:
@@ -376,15 +383,18 @@
                                                               mapping=self.qubit_mapping,
                                                               n_spinorbitals=n_active_sos,
                                                               n_electrons=n_active_electrons,
                                                               up_then_down=self.up_then_down,
                                                               spin=spin)
 
         self.ansatz.update_var_params(var_params)
-        expectation = self.backend.get_expectation_value(self.qubit_hamiltonian, ref_state+self.ansatz.circuit)
+        circuit = ref_state + self.ansatz.circuit
+        if self.projective_circuit:
+            circuit += self.projective_circuit
+        expectation = self.backend.get_expectation_value(self.qubit_hamiltonian, circuit, **self.simulate_options)
 
         # Restore the current target hamiltonian
         self.qubit_hamiltonian = tmp_hamiltonian
 
         return expectation
 
     def get_rdm(self, var_params, resample=False, sum_spin=True, ref_state=Circuit()):
```

### Comparing `tangelo-gc-0.3.4/tangelo/helpers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/helpers/math.py` & `tangelo-gc-0.4.0rc0/tangelo/helpers/math.py`

 * *Files 24% similar despite different names*

```diff
@@ -49,7 +49,33 @@
             # If there is only one 1 in the selected part, the pivot is
             # decremented.
             if len(indices) > 0:
                 bool_array[:, (indices[0], pivot)] = bool_array[:, (pivot, indices[0])]
                 pivot -= 1
 
     return bool_array
+
+
+def arrays_almost_equal_up_to_global_phase(array1, array2, atol=1e-6):
+    """
+    Checks if two arrays are almost equal up to a global phase.
+
+    Args:
+        array1 (array): Self-explanatory.
+        array2 (array): Self-explanatory.
+        atol (float) : Optional, absolute tolerance
+
+    Returns:
+        bool : True if arrays are almost equal up to a global phase, False otherwise.
+    """
+    if len(array1) != len(array2):
+        return False
+
+    array1 = np.asarray(array1)
+    array2 = np.asarray(array2)
+
+    if np.allclose(array1, array2, atol=atol):
+        return True
+
+    # Check for global phase difference
+    phase_diff = np.angle(array1[0] / array2[0])
+    return np.allclose(array1, array2 * np.exp(1j * phase_diff), atol=atol)
```

### Comparing `tangelo-gc-0.3.4/tangelo/helpers/utils.py` & `tangelo-gc-0.4.0rc0/tangelo/helpers/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,22 +69,27 @@
             )
             return func(*args, **kwargs)
         return new_func
     return deprecated_wrapper
 
 
 # List all built-in backends supported
-all_backends = {"qulacs", "qiskit", "cirq", "braket", "projectq", "qdk", "pennylane"}
+all_backends = {"qulacs", "qiskit", "cirq", "braket", "projectq", "qdk", "pennylane", "sympy", "stim"}
 all_backends_simulator = {"qulacs", "qiskit", "cirq", "qdk"}
 sv_backends_simulator = {"qulacs", "qiskit", "cirq"}
+symbolic_backends = {"sympy"}
+chem_backends = {"pyscf", "psi4"}
+clifford_backends_simulator = {"stim"}
 
 # Dictionary mapping package names to their identifier in this module
 packages = {p: p for p in all_backends}
 packages["qdk"] = "qsharp"
 
 # Figure out what is installed in user's environment
 installed_backends = {p_id for p_id, p_name in packages.items() if is_package_installed(p_name)}
 installed_simulator = installed_backends & all_backends_simulator
 installed_sv_simulator = installed_backends & sv_backends_simulator
+installed_chem_backends = {p_id for p_id in chem_backends if is_package_installed(p_id)}
+installed_clifford_simulators = {p_id for p_id in clifford_backends_simulator if is_package_installed(p_id)}
 
 # Check if qulacs installed (better performance for tests). If not, defaults to cirq (always installed with openfermion)
 default_simulator = "qulacs" if "qulacs" in installed_sv_simulator else "cirq"
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .gate import *
-from .circuit import Circuit, stack, remove_small_rotations, remove_redundant_gates
+from .circuit import Circuit, stack, remove_small_rotations, remove_redundant_gates, get_unitary_circuit_pieces
 from .translator import *
 from .simulator import get_backend
 from .target.backend import get_expectation_value_from_frequencies_oneterm
 from .target import backend_info, Backend
+from .noisy_simulation import NoiseModel
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/circuit.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """This abstract quantum circuit class allows to represent a quantum circuit,
 described by successive abstract quantum gate operations, without tying it to a
 particular backend. It also provides methods to compute some of its
 characteristics (width, size ...).
 """
 
 import copy
-from typing import List
+from typing import List, Tuple, Iterator
 
 import numpy as np
 from cirq.contrib.svg import SVGCircuit
 
 from tangelo.linq import Gate
 
 
@@ -51,14 +51,15 @@
         self.name = name
         self._gates = list()
         self._qubits_simulated = n_qubits
         self._qubit_indices = set() if not n_qubits else set(range(n_qubits))
         self._gate_counts = dict()
         self._n_qubit_gate_counts = dict()
         self._variational_gates = []
+        self._probabilities = dict()
 
         if gates:
             _ = [self.add_gate(g) for g in gates]
 
     def __str__(self):
         """Print info about the circuit and the gates it contains in a
         human-friendly format.
@@ -141,14 +142,29 @@
     @property
     def is_mixed_state(self):
         """Assume circuit leads to a mixed state due to mid-circuit measurement
         if any MEASURE gate was explicitly added by the user.
         """
         return "MEASURE" in self.counts
 
+    @property
+    def success_probabilities(self):
+        """Returns the dictionary of probabilities populated by simulating with different desired_meas_result.
+
+        The keys of the dictionary are bit strings, corresponding to the desired outcomes in the order
+        the measurement gates arise in the circuit.
+
+        Each bit string must be simulated using a backend with n_shots=None and desired_meas_result=bitstring
+        in order to populate the corresponding probability.
+        """
+        if not self.is_mixed_state:
+            return {"": 1}
+        else:
+            return self._probabilities
+
     def draw(self):
         """Method to output a prettier version of the circuit for use in jupyter notebooks that uses cirq SVGCircuit"""
         # circular import
         from tangelo.linq.translator.translate_cirq import translate_c_to_cirq
         cirq_circ = translate_c_to_cirq(self)
         # Remove identity gates that are added in translate_c_to_cirq (to ensure all qubits are initialized) before drawing.
         cirq_circ.__delitem__(0)
@@ -191,44 +207,49 @@
 
         # Keep track of gate counts separately for 1-qubit gates, 2-qubit gates, and so on
         n_qubit = len(g.target) if (g.control is None) else len(g.target) + len(g.control)
         self._n_qubit_gate_counts[n_qubit] = self._n_qubit_gate_counts.get(n_qubit, 0) + 1
 
     def depth(self):
         """ Return the depth of the quantum circuit, by computing the number of moments. Does not count
-        qubit initialization as a moment (unlike Cirq, for example).
+        qubit initialization as a moment (unlike Cirq, for example). Compute from scratch.
         """
+        # List of qubit indices involved in each moment. Look up dict for latest moment for each index.
         moments = list()
+        latest_moment = dict()
 
-        for g in self._gates:
+        # Traverse gates and compute moments
+        for g in self:
             qubits = set(g.target) if g.control is None else set(g.target + g.control)
 
             if not moments:
                 moments.append(qubits)
+                for i in qubits:
+                    latest_moment[i] = 0
             else:
-                # Find latest moment involving at least one of the qubits targeted by the current gate
-                # The current gate is part of the moment following that one
-                for i, m in reversed(list(enumerate(moments))):
-                    if m & qubits:
-                        if (i+1) < len(moments):
-                            moments[i+1] = moments[i+1] | qubits
-                        else:
-                            moments.append(qubits)
-                        break
-                    # Case where none of the target qubits have been used before
-                    elif i == 0:
-                        moments[0] = moments[0] | qubits
-
+                # Find latest moment involving one of the qubits targeted by the gate
+                # -1 means the qubit index was encountered for the very first time
+                b = max([latest_moment.get(i, -1) for i in qubits])
+                for i in qubits:
+                    latest_moment[i] = b + 1
+
+                # Case 1: Gate can be included in a previous moment
+                # Includes b = -1 case where all qubits are encountered for the 1st time
+                if (b + 1) < len(moments):
+                    moments[b + 1] = moments[b + 1] | qubits
+                # Case 2: Gate is part of a new moment
+                else:
+                    moments.append(qubits)
         return len(moments)
 
     def trim_qubits(self):
         """Trim unnecessary qubits and update indices with the lowest values possible.
         """
         qubits_in_use = set().union(*self.get_entangled_indices())
-        mapping = {ind: i for i, ind in enumerate(qubits_in_use)}
+        mapping = {ind: i for i, ind in enumerate(sorted(list(qubits_in_use)))}
         for g in self._gates:
             g.target = [mapping[ind] for ind in g.target]
             if g.control:
                 g.control = [mapping[ind] for ind in g.control]
 
         self._qubit_indices = set(range(len(qubits_in_use)))
         return self
@@ -433,7 +454,33 @@
             for qubit_i in qubits:
                 gate_qubits[qubit_i] += [(gi, gate)]
 
     # Remove gates that can be cancelled.
     gates = [gate for gate_i, gate in enumerate(circuit._gates) if gate_i not in indices_to_remove]
 
     return Circuit(gates)
+
+
+def get_unitary_circuit_pieces(circuit: Circuit) -> Tuple[List[Circuit], List[int]]:
+    """Split circuit into the unitary circuits between mid-circuit non-unitary MEASURE gates.
+
+    Args:
+        circuit (Circuit): the circuit to split
+
+    Returns:
+        List[Circuit]: The list of unitary circuits with a terminal non-unitary operation.
+        List[int]: The qubits that the "MEASURE" operation is applied to.
+    """
+
+    n_qubits = circuit.width
+    circuits, gates, measure_qubits = list(), list(), list()
+
+    for g in circuit:
+        if g.name != "MEASURE":
+            gates += [Gate(g.name, g.target, g.control, g.parameter, g.is_variational)]
+        else:
+            circuits += [Circuit(copy.deepcopy(gates), n_qubits=n_qubits)]
+            measure_qubits += [g.target[0]]
+            gates = list()
+    circuits += [Circuit(copy.deepcopy(gates), n_qubits=n_qubits)]
+
+    return circuits, measure_qubits
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/gate.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/gate.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Define an abstract quantum gate class holding information about a quantum
 gate operation, without tying it to a particular backend or an underlying
 mathematical operation.
 """
-from math import pi
+from math import pi, isclose
 from typing import Union
 
 from numpy import integer, ndarray, floating
+from sympy import Symbol
+
 
 ONE_QUBIT_GATES = {"H", "X", "Y", "Z", "S", "T", "RX", "RY", "RZ", "PHASE"}
 TWO_QUBIT_GATES = {"CNOT", "CX", "CY", "CZ", "CRX", "CRY", "CRZ", "CPHASE", "XX", "SWAP"}
 THREE_QUBIT_GATES = {"CSWAP"}
 
 ONE_TARGET_GATES = {"H", "X", "Y", "Z", "S", "T", "RX", "RY", "RZ", "PHASE",
                     "CNOT", "CX", "CY", "CZ", "CRX", "CRY", "CRZ", "CPHASE"}
 TWO_TARGET_GATES = {"XX", "SWAP", "CSWAP"}
 
 PARAMETERIZED_GATES = {"RX", "RY", "RZ", "PHASE", "CRX", "CRY", "CRZ", "CPHASE", "XX"}
 INVERTIBLE_GATES = {"H", "X", "Y", "Z", "S", "T", "RX", "RY", "RZ", "CH", "PHASE",
                     "CNOT", "CX", "CY", "CZ", "CRX", "CRY", "CRZ", "CPHASE", "XX", "SWAP",
                     "CSWAP"}
 
+CLIFFORD_GATES = {"H", "S", "X", "Z", "Y", "SDAG", "CNOT", "CX", "CY", "CZ", "SWAP", "CXSWAP"}
+
 
 class Gate(dict):
     """An abstract gate class that exposes all the gate information such as gate
     name, control and target qubit indices, parameter values. Assumes qubit
     indexation starts at index 0.
 
     Attributes:
@@ -161,22 +165,42 @@
         """Return the inverse (adjoint) of a gate.
 
         Return:
             Gate: the inverse of the gate.
         """
         if self.name not in INVERTIBLE_GATES:
             raise AttributeError(f"{self.name} is not an invertible gate")
+
+        if self.name in {"T", "S"}:
+            new_parameter = -pi / 2 if self.name == "S" else -pi / 4
+            return Gate("PHASE", self.target, self.control, new_parameter, self.is_variational)
+
         if self.parameter == "":
             new_parameter = ""
-        elif isinstance(self.parameter, (float, floating, int, integer)):
+        elif isinstance(self.parameter, (float, floating, int, integer, Symbol)):
             new_parameter = -self.parameter
-        elif self.name in {"T", "S"}:
-            new_parameter = -pi / 2 if self.name == "T" else -pi / 4
-            return Gate("PHASE", self.target, self.control, new_parameter, self.is_variational)
         else:
             raise AttributeError(f"{self.name} is not an invertible gate when parameter is {self.parameter}")
         return Gate(self.name, self.target, self.control, new_parameter, self.is_variational)
 
+    def is_clifford(self, abs_tol=1e-4):
+        """
+        Check if a quantum gate is a Clifford gate.
+
+        Args:
+            abs_tol (float) : Optional, Absolute tolerance for the difference between gate parameter clifford parameter values
+
+        Returns:
+            bool: True if the gate is in Clifford gate list or has a parameter corresponding to Clifford points,
+                  False otherwise.
+        """
+        if self.name in CLIFFORD_GATES:
+            return True
+        elif self.name in {"RX", "RY", "RZ", "PHASE"}:
+            return isclose(self.parameter % (pi / 2), 0, abs_tol=abs_tol)
+        else:
+            return False
+
     def serialize(self):
         return {"type": "Gate",
                 "params": {"name": self.name, "target": self.target,
                            "control": self.control, "parameter": self.parameter}}
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/helpers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/measurement_basis.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/measurement_basis.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/statevector.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/statevector.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/helpers/circuits/tests/test_statevector.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/test_statevector.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/helpers/operators/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .operators import *
+from .diagonal_coulomb import get_orbital_rotations
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/helpers/operators/operators.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/operators.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/noisy_simulation/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/noisy_simulation/noise_models.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/noise_models.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/qdk_template.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qdk_template.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/qpu_connection/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .qemist_cloud_connection import QEMISTCloudConnection
-from .ionq_connection import IonQConnection
-from .ibm_connection import IBMConnection
+from .dmet_problem_decomposition import Localization
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/qpu_connection/ibm_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/ibm_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/qpu_connection/ionq_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/ionq_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/qpu_connection/qemist_cloud_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/qemist_cloud_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/qpu_connection/qpu_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/qpu_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/simulator.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,13 +47,7 @@
             target = target_dict[target]
         except KeyError:
             raise ValueError(f"Error: backend {target} not supported. Available built-in options: {list(target_dict.keys())}")
     elif not issubclass(target, Backend):
         raise TypeError(f"Target must be a str or a subclass of Backend but received class {type(target).__name__}")
 
     return target(n_shots=n_shots, noise_model=noise_model, **kwargs)
-
-
-@deprecated("Please use get_backend.")
-def Simulator(target: Union[None, str, Type[Backend]] = default_simulator, n_shots: Union[None, int] = None,
-              noise_model=None, **kwargs):
-    return get_backend(target, n_shots, noise_model, **kwargs)
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/target/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # limitations under the License.
 
 from .backend import Backend
 from .target_cirq import CirqSimulator
 from .target_qiskit import QiskitSimulator
 from .target_qulacs import QulacsSimulator
 from .target_qdk import QDKSimulator
-from tangelo.helpers.utils import all_backends_simulator
+from .target_sympy import SympySimulator
+from .target_stim import StimSimulator
+from tangelo.helpers.utils import all_backends_simulator, clifford_backends_simulator
 
 
-target_dict = {"qiskit": QiskitSimulator, "cirq": CirqSimulator, "qdk": QDKSimulator, "qulacs": QulacsSimulator}
+target_dict = {"qiskit": QiskitSimulator, "cirq": CirqSimulator, "qdk": QDKSimulator, "qulacs": QulacsSimulator, "sympy": SympySimulator, "stim": StimSimulator}
 
 # Generate backend info dictionary
 backend_info = {sim_id: target_dict[sim_id].backend_info() for sim_id in all_backends_simulator}
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/target/backend.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,26 @@
 import abc
 import math
 from collections import Counter
 
 import numpy as np
 from scipy import stats
 from bitarray import bitarray
-from openfermion.ops import QubitOperator
 
 from tangelo.linq import Gate, Circuit
 from tangelo.linq.helpers.circuits.measurement_basis import measurement_basis_gates
+from tangelo.toolboxes.operators import QubitOperator
 
 
 def get_expectation_value_from_frequencies_oneterm(term, frequencies):
     """Return the expectation value of a single-term qubit-operator, given
     the result of a state-preparation.
 
     Args:
-        term (openfermion-style QubitOperator object): a qubit operator, with
-            only a single term.
+        term (QubitOperator): a single-term qubit operator.
         frequencies (dict): histogram of frequencies of measurements (assumed
             to be in lsq-first format).
 
     Returns:
         complex: The expectation value of this operator with regard to the
             state preparation.
     """
@@ -78,16 +77,15 @@
     return expectation_term
 
 
 def get_variance_from_frequencies_oneterm(term, frequencies):
     """Return the variance of the expectation value of a single-term qubit-operator, given
     the result of a state-preparation.
     Args:
-        term (openfermion-style QubitOperator object): a qubit operator, with
-            only a single term.
+        term (QubitOperator): a single-term qubit operator.
         frequencies (dict): histogram of frequencies of measurements (assumed
             to be in lsq-first format).
     Returns:
         complex: The variance of this operator with regard to the
             state preparation.
     """
 
@@ -108,14 +106,58 @@
         # Compute sample variance using state_binstr and term mask, update term variance
         sample = (-1) ** ((bitarray(mask) & bitarray(basis_state)).to01().count("1") % 2)
         variance_term += freq*(expectation_term - sample)**2
 
     return variance_term
 
 
+def collapse_statevector_to_desired_measurement(statevector, qubit, result, order="lsq_first"):
+    """Take 0 or 1 part of a statevector for a given qubit and return a normalized statevector and probability.
+
+    Args:
+        statevector (array): The statevector for which the collapse to the desired qubit value is performed.
+        qubit (int): Index of target qubit to collapse in the desired classical state.
+        result (int): 0 or 1.
+        order (string): The qubit ordering of the statevector, lsq_first or msq_first.
+
+    Returns:
+        array: The collapsed and renormalized statevector.
+        float: The probability for the desired measurement to occur.
+    """
+
+    n_qubits = round(math.log2(len(statevector)))
+
+    if 2**n_qubits != len(statevector):
+        raise ValueError(f"Statevector length of {len(statevector)} is not a power of 2.")
+
+    if qubit > n_qubits-1:
+        raise ValueError("qubit index to measure is larger than number of qubits in statevector")
+
+    if result not in {0, 1}:
+        raise ValueError(f"Result is not valid, must be an integer of 0 or 1 but received {result}")
+
+    if order.lower() not in {"lsq_first", "msq_first"}:
+        raise ValueError("Order must be lsq_first or msq_first")
+
+    before_index_length = 2**qubit if order == "lsq_first" else 2**(n_qubits-1-qubit)
+    after_index_length = 2**(n_qubits-1-qubit) if order == "lsq_first" else 2**qubit
+
+    sv_selected = np.reshape(statevector, (before_index_length, 2, after_index_length))
+    sv_selected[:, (result + 1) % 2, :] = 0
+    sv_selected = sv_selected.flatten()
+
+    sqrt_probability = np.linalg.norm(sv_selected)
+    if sqrt_probability < 1.e-14:
+        raise ValueError(f"Probability of desired measurement={0} for qubit={qubit} is zero.")
+
+    sv_selected = sv_selected/sqrt_probability  # casting issue if inplace for probability 1
+
+    return sv_selected, sqrt_probability**2
+
+
 class Backend(abc.ABC):
 
     def __init__(self, n_shots=None, noise_model=None):
         """Instantiate Backend object.
 
         Args:
             n_shots (int): Number of shots if using a shot-based simulator.
@@ -209,24 +251,24 @@
             numpy.array: The statevector, if available for the target backend
                 and requested by the user (if not, set to None).
         """
         n_meas = source_circuit.counts.get("MEASURE", 0)
 
         if desired_meas_result is not None:
             if not isinstance(desired_meas_result, str) or len(desired_meas_result) != n_meas:
-                raise ValueError("desired_meas result is not a string with the same length as the number of measurements"
+                raise ValueError("desired_meas result is not a string with the same length as the number of measurements "
                                  "in the circuit.")
             save_mid_circuit_meas = True
         elif save_mid_circuit_meas and return_statevector:
             if self.n_shots != 1:
-                raise ValueError("The combination of save_mid_circuit_meas and return_statevector without specifying desired_meas_result"
-                                 "is only valid for self.n_shots=1 as the result is a mixed state otherwise, "
+                raise ValueError("The combination of save_mid_circuit_meas and return_statevector without specifying desired_meas_result "
+                                 "is only valid for self.n_shots=1. The result is a mixed state otherwise, "
                                  f"but you requested n_shots={self.n_shots}.")
         elif source_circuit.is_mixed_state and not self.n_shots:
-            raise ValueError("Circuit contains MEASURE instruction, and is assumed to prepare a mixed state."
+            raise ValueError("Circuit contains MEASURE instruction, and is assumed to prepare a mixed state. "
                              "Please set the n_shots attribute to an appropriate value.")
 
         if source_circuit.width == 0:
             raise ValueError("Cannot simulate an empty circuit (e.g identity unitary) with unknown number of qubits.")
 
         # If the unitary is the identity (no gates) and no noise model, no need for simulation:
         # return all-zero state or sample from statevector
@@ -267,16 +309,15 @@
         statevector then it is used directly to compute expectation values, or
         draw samples if required. In the case of a noisy simulator, or if the
         statevector is not available on the target backend, individual shots
         must be run and the workflow is akin to what we would expect from an
         actual QPU.
 
         Args:
-            qubit_operator (openfermion-style QubitOperator class): a qubit
-                operator.
+            qubit_operator (QubitOperator): the qubit operator.
             state_prep_circuit (Circuit): an abstract circuit used for state preparation.
             initial_statevector (array): The initial statevector for the simulation
             desired_meas_result (str): The mid-circuit measurement results to select for.
 
         Returns:
             complex: The expectation value of this operator with regards to the
                 state preparation.
@@ -293,23 +334,24 @@
                 raise ValueError(f'Term {term} requires more qubits than the circuit contains ({state_prep_circuit.width})')
             if type(coef) in {complex, np.complex64, np.complex128}:
                 are_coefficients_real = False
 
         # If the underlying operator is hermitian, expectation value is real and can be computed right away
         if are_coefficients_real:
             if self._noise_model or not self.statevector_available \
-                    or state_prep_circuit.is_mixed_state or state_prep_circuit.size == 0:
+                    or (state_prep_circuit.is_mixed_state and self.n_shots is not None) or state_prep_circuit.size == 0:
                 return self._get_expectation_value_from_frequencies(qubit_operator,
                                                                     state_prep_circuit,
                                                                     initial_statevector=initial_statevector,
                                                                     desired_meas_result=desired_meas_result)
             elif self.statevector_available:
                 return self._get_expectation_value_from_statevector(qubit_operator,
                                                                     state_prep_circuit,
-                                                                    initial_statevector=initial_statevector)
+                                                                    initial_statevector=initial_statevector,
+                                                                    desired_meas_result=desired_meas_result)
 
         # Else, separate the operator into 2 hermitian operators, use linearity and call this function twice
         else:
             qb_op_real, qb_op_imag = QubitOperator(), QubitOperator()
             for term, coef in qubit_operator.terms.items():
                 qb_op_real.terms[term], qb_op_imag.terms[term] = coef.real, coef.imag
             qb_op_real.compress()
@@ -328,16 +370,15 @@
         statevector then it is used directly to compute variance (zero), or
         draw samples if required. In the case of a noisy simulator, or if the
         statevector is not available on the target backend, individual shots
         must be run and the workflow is akin to what we would expect from an
         actual QPU.
 
         Args:
-            qubit_operator (openfermion-style QubitOperator class): a qubit
-                operator.
+            qubit_operator (QubitOperator): the qubit operator.
             state_prep_circuit (Circuit): an abstract circuit used for state preparation.
             initial_statevector (list/array) : A valid statevector in the format
                 supported by the target backend.
             desired_meas_result (str): The mid-circuit measurement results to select for.
 
         Returns:
             complex: The variance of this operator with regard to the
@@ -383,47 +424,48 @@
         statevector then it is used directly to compute standard error (zero), or
         draw samples if required. In the case of a noisy simulator, or if the
         statevector is not available on the target backend, individual shots
         must be run and the workflow is akin to what we would expect from an
         actual QPU.
 
         Args:
-            qubit_operator (openfermion-style QubitOperator class): a qubit
-                operator.
+            qubit_operator (QubitOperator): the qubit operator.
             state_prep_circuit (Circuit): an abstract circuit used for state preparation.
             initial_statevector (list/array): A valid statevector in the format
                 supported by the target backend.
             desired_meas_result (str): The mid-circuit measurement results to select for.
 
         Returns:
             complex: The standard error of this operator with regard to the
                 state preparation.
         """
         variance = self.get_variance(qubit_operator, state_prep_circuit, initial_statevector, desired_meas_result=desired_meas_result)
         return np.sqrt(variance/self.n_shots) if self.n_shots else 0.
 
-    def _get_expectation_value_from_statevector(self, qubit_operator, state_prep_circuit, initial_statevector=None):
+    def _get_expectation_value_from_statevector(self, qubit_operator, state_prep_circuit, initial_statevector=None, desired_meas_result=None):
         r"""Take as input a qubit operator H and a state preparation returning a
         ket |\psi>. Return the expectation value <\psi | H | \psi>, computed
         without drawing samples (statevector only). Users should not be calling
         this function directly, please call "get_expectation_value" instead.
 
         Args:
-            qubit_operator (openfermion-style QubitOperator class): a qubit operator.
+            qubit_operator (QubitOperator): the qubit operator.
             state_prep_circuit (Circuit): an abstract circuit used for state preparation (only pure states).
             initial_statevector (array): The initial state of the system
 
         Returns:
             complex: The expectation value of this operator with regards to the
                 state preparation.
         """
+
         n_qubits = state_prep_circuit.width
 
         expectation_value = 0.
-        prepared_frequencies, prepared_state = self.simulate(state_prep_circuit, return_statevector=True, initial_statevector=initial_statevector)
+        prepared_frequencies, prepared_state = self.simulate(state_prep_circuit, return_statevector=True,
+                                                             initial_statevector=initial_statevector, desired_meas_result=desired_meas_result)
 
         if hasattr(self, "expectation_value_from_prepared_state"):
             return self.expectation_value_from_prepared_state(qubit_operator, n_qubits, prepared_state)
 
         # Otherwise, use generic statevector expectation value
         for term, coef in qubit_operator.terms.items():
 
@@ -455,15 +497,15 @@
 
     def _get_expectation_value_from_frequencies(self, qubit_operator, state_prep_circuit, initial_statevector=None, desired_meas_result=None):
         r"""Take as input a qubit operator H and a state preparation returning a
         ket |\psi>. Return the expectation value <\psi | H | \psi> computed
         using the frequencies of observable states.
 
         Args:
-            qubit_operator (openfermion-style QubitOperator class): a qubitoperator.
+            qubit_operator (QubitOperator): the qubit operator.
             state_prep_circuit (Circuit): an abstract circuit used for state preparation.
             initial_statevector (array): The initial state of the system
             desired_meas_result (str): The mid-circuit measurement results to select for.
 
         Returns:
             complex: The expectation value of this operator with regard to the
                 state preparation.
@@ -503,15 +545,15 @@
 
     def _get_variance_from_frequencies(self, qubit_operator, state_prep_circuit, initial_statevector=None, desired_meas_result=None):
         r"""Take as input a qubit operator H and a state preparation returning a
         ket |\psi>. Return the variance of <\psi | H | \psi> computed
         using the frequencies of observable states.
 
         Args:
-            qubit_operator (openfermion-style QubitOperator class): a qubit operator.
+            qubit_operator (QubitOperator): the qubit operator.
             state_prep_circuit (Circuit): an abstract circuit used for state preparation.
             initial_statevector (list/array) : A valid statevector in the format
                 supported by the target backend.
             desired_meas_result (str): The mid-circuit measurement results to select for.
 
         Returns:
             complex: The variance of this operator with regard to the
@@ -551,16 +593,15 @@
 
     @staticmethod
     def get_expectation_value_from_frequencies_oneterm(term, frequencies):
         """Return the expectation value of a single-term qubit-operator, given
         the result of a state-preparation.
 
         Args:
-            term (openfermion-style QubitOperator object): a qubit operator, with
-                only a single term.
+            term (QubitOperator): a single-term qubit operator
             frequencies (dict): histogram of frequencies of measurements (assumed
                 to be in lsq-first format).
 
         Returns:
             complex: The expectation value of this operator with regard to the
                 state preparation.
         """
@@ -569,16 +610,15 @@
 
     @staticmethod
     def get_variance_from_frequencies_oneterm(term, frequencies):
         """Return the variance of a single-term qubit-operator, given
         the result of a state-preparation.
 
         Args:
-            term (openfermion-style QubitOperator object): a qubit operator, with
-                only a single term.
+            term (QubitOperator): a single-term qubit operator.
             frequencies (dict): histogram of frequencies of measurements (assumed
                 to be in lsq-first format).
 
         Returns:
             complex: The variance of this operator with regard to the
                 state preparation.
         """
@@ -647,14 +687,29 @@
             string: The bit string of the integer in lsq-first order.
         """
         bs = bin(i).split('b')[-1]
         state_binstr = "0" * (n_qubits - len(bs)) + bs
 
         return state_binstr if use_ordering and (self.statevector_order == "lsq_first") else state_binstr[::-1]
 
+    def collapse_statevector_to_desired_measurement(self, statevector, qubit, result):
+        """Take 0 or 1 part of a statevector for a given qubit and return a normalized statevector and probability.
+
+        Args:
+            statevector (array): The statevector for which the collapse to the desired qubit value is performed.
+            qubit (int): The index of the qubit to collapse to the classical result.
+            result (string): "0" or "1".
+
+        Returns:
+            array: the collapsed and renormalized statevector
+            float: the probability this occured
+        """
+
+        return collapse_statevector_to_desired_measurement(statevector, qubit, result, self.backend_info()['statevector_order'])
+
     @staticmethod
     @abc.abstractmethod
     def backend_info() -> dict:
         """A dictionary that includes {'noisy_simulation': True or False,
                                        'statevector_available': True or False,
                                        'statevector_order': 'lsq_first' or 'msq_first'"""
         pass
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/target/target_cirq.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_cirq.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections import Counter
 
 import numpy as np
 
-from tangelo.linq import Circuit
+from tangelo.linq import Circuit, get_unitary_circuit_pieces
 from tangelo.linq.target.backend import Backend
 from tangelo.linq.translator import translate_circuit as translate_c
 from tangelo.linq.translator import translate_operator
 
 
 class CirqSimulator(Backend):
 
@@ -73,15 +73,15 @@
         # Only DensityMatrixSimulator handles noise well, can use Simulator, but it is slower
         if self._noise_model or (source_circuit.is_mixed_state and not save_mid_circuit_meas):
             cirq_simulator = self.cirq.DensityMatrixSimulator(dtype=np.complex128)
         else:
             cirq_simulator = self.cirq.Simulator(dtype=np.complex128)
 
         # If requested, set initial state
-        cirq_initial_statevector = initial_statevector if initial_statevector is not None else 0
+        cirq_initial_statevector = np.asarray(initial_statevector, dtype=complex) if initial_statevector is not None else 0
 
         # Calculate final density matrix and sample from that for noisy simulation or simulating mixed states
         if (self._noise_model or source_circuit.is_mixed_state) and not save_mid_circuit_meas:
             translated_circuit = translate_c(source_circuit, "cirq", output_options={"noise_model": self._noise_model,
                                                                                      "save_measurements": save_mid_circuit_meas})
             # cirq.dephase_measurements changes measurement gates to Krauss operators so simulators
             # can be called once and density matrix sampled repeatedly.
@@ -104,25 +104,57 @@
             samples = dict()
             for j in range(self.n_shots):
                 bitstr = "".join([str(job_sim.measurements[str(i)][j, 0]) for i in range(n_meas + source_circuit.width)])
                 samples[bitstr] = samples.get(bitstr, 0) + 1
             self.all_frequencies = {k: v / self.n_shots for k, v in samples.items()}
             frequencies = self.all_frequencies
 
-        # Run shot by shot and keep track of desired_meas_result only (generally slower)
+        # Run shot by shot and keep track of desired_meas_result only if n_shots is set
+        # Otherwised, Split circuit into chunks between mid-circuit measurements. Simulate a chunk, collapse the statevector according
+        # to the desired measurement and simulate the next chunk using this new statevector as input
         elif desired_meas_result or (save_mid_circuit_meas and return_statevector):
-            translated_circuit = translate_c(source_circuit, "cirq", output_options={"noise_model": self._noise_model,
-                                                                                     "save_measurements": True})
-            self._current_state = None
-            indices = list(range(source_circuit.width))
-            n_attempts = 0
+
+            # desired_meas_result without a noise model
+            if self.n_shots is None:
+                success_probability = 1
+                if initial_statevector is not None:
+                    sv = cirq_initial_statevector
+                else:
+                    sv = np.zeros(2**source_circuit.width)
+                    sv[0] = 1
+
+                unitary_circuits, qubits = get_unitary_circuit_pieces(source_circuit)
+
+                for i, circ in enumerate(unitary_circuits[:-1]):
+                    if circ.size > 0:
+                        translated_circuit = translate_c(circ, "cirq", output_options={"save_measurements": True})
+                        job_sim = cirq_simulator.simulate(translated_circuit, initial_state=sv)
+                        sv, cprob = self.collapse_statevector_to_desired_measurement(job_sim.final_state_vector, qubits[i], int(desired_meas_result[i]))
+                    else:
+                        sv, cprob = self.collapse_statevector_to_desired_measurement(sv, qubits[i], int(desired_meas_result[i]))
+                    success_probability *= cprob
+                source_circuit._probabilities[desired_meas_result] = success_probability
+
+                translated_circuit = translate_c(unitary_circuits[-1], "cirq", output_options={"save_measurements": True})
+                job_sim = cirq_simulator.simulate(translated_circuit, initial_state=sv)
+                self._current_state = job_sim.final_state_vector
+            # Either desired_meas_result with noise_model. Or 1 shot save_mid_circuit_meas
+            else:
+                translated_circuit = translate_c(source_circuit, "cirq", output_options={"noise_model": self._noise_model,
+                                                                                         "save_measurements": True})
+                self._current_state = None
+                indices = list(range(source_circuit.width))
 
             # Permit 0.1% probability events
+            n_attempts = 0
             max_attempts = 1000 if self.n_shots is None else 1000*self.n_shots
 
+            # Use density matrix simulator until success if noise_model.
+            # TODO: implement collapse operations for density matrix simulation.
+            # Loop also used for 1 shot if no desired_meas_result and save_mid_circuit_meas.
             while self._current_state is None and n_attempts < max_attempts:
                 job_sim = cirq_simulator.simulate(translated_circuit, initial_state=cirq_initial_statevector)
                 measure = "".join([str(job_sim.measurements[str(i)][0]) for i in range(n_meas)])
                 current_state = job_sim.final_density_matrix if self._noise_model else job_sim.final_state_vector
                 if measure == desired_meas_result or desired_meas_result is None:
                     self._current_state = current_state
                 n_attempts += 1
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/target/target_qdk.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qdk.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/target/target_qiskit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qiskit.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import math
 from collections import Counter
 
 import numpy as np
 
-from tangelo.linq import Circuit
+from tangelo.linq import Circuit, get_unitary_circuit_pieces
 from tangelo.linq.target.backend import Backend
 from tangelo.linq.translator import translate_circuit as translate_c
 from tangelo.linq.noisy_simulation.noise_models import get_qiskit_noise_model
 
 
 class QiskitSimulator(Backend):
     """Interface to the qiskit simulator."""
@@ -72,34 +72,44 @@
             translated_circuit = self.qiskit.transpile(translated_circuit, backend)
             translated_circuit.save_statevector()
             return backend, translated_circuit
 
         n_meas = source_circuit.counts.get("MEASURE", 0)
         qiskit_noise_model = get_qiskit_noise_model(self._noise_model) if self._noise_model else None
 
+        def load_statevector(translated_circuit, initial_statevector):
+            "Load statevector into translated_circuit"
+            n_qubits = int(math.log2(len(initial_statevector)))
+            n_meas = source_circuit.counts.get("MEASURE", 0)
+            n_registers = n_meas + source_circuit.width if save_mid_circuit_meas else source_circuit.width
+            initial_state_circuit = self.qiskit.QuantumCircuit(n_qubits, n_registers)
+            initial_state_circuit.initialize(initial_statevector, list(range(n_qubits)))
+            translated_circuit = initial_state_circuit.compose(translated_circuit)
+            return translated_circuit
+
         def run_and_measure_one_shot(backend, translated_circuit):
             "Return statevector and mid-circuit measurement for one shot"
             sim_results = backend.run(translated_circuit, noise_model=qiskit_noise_model, shots=1).result()
             current_state = sim_results.get_statevector(translated_circuit)
-            measure = next(iter(self.qiskit.result.marginal_counts(sim_results, indices=list(range(n_meas))).get_counts()))[::-1]
+            measure = next(iter(self.qiskit.result.marginal_counts(sim_results, indices=list(range(n_meas)), inplace=True).get_counts()))[::-1]
             return current_state, measure
 
-        translated_circuit = translate_c(source_circuit, "qiskit", output_options={"save_measurements": save_mid_circuit_meas})
-
-        # If requested, set initial state
-        if initial_statevector is not None:
-            if self._noise_model:
-                raise ValueError("Cannot load an initial state if using a noise model, with Qiskit")
-            else:
-                n_qubits = int(math.log2(len(initial_statevector)))
-                n_meas = source_circuit.counts.get("MEASURE", 0)
-                n_registers = n_meas + source_circuit.width if save_mid_circuit_meas else source_circuit.width
-                initial_state_circuit = self.qiskit.QuantumCircuit(n_qubits, n_registers)
-                initial_state_circuit.initialize(initial_statevector, list(range(n_qubits)))
-                translated_circuit = initial_state_circuit.compose(translated_circuit)
+        if desired_meas_result is not None and not self._noise_model:
+            # Split circuit into chunks between mid-circuit measurements. Simulate a chunk, collapse the statevector according
+            # to the desired measurement and simulate the next chunk using this new statevector as input
+            unitary_circuits, qubits = get_unitary_circuit_pieces(source_circuit)
+        else:
+            translated_circuit = translate_c(source_circuit, "qiskit", output_options={"save_measurements": save_mid_circuit_meas})
+
+            # If requested, set initial state
+            if initial_statevector is not None:
+                if self._noise_model:
+                    raise ValueError("Cannot load an initial state if using a noise model, with Qiskit")
+                else:
+                    translated_circuit = load_statevector(translated_circuit, initial_statevector)
 
         # Noiseless simulation using the statevector simulator
         if not self._noise_model and not source_circuit.is_mixed_state:
             backend, translated_circuit = aer_backend_with_statevector(translated_circuit)
 
             sim_results = backend.run(translated_circuit).result()
             current_state = sim_results.get_statevector(translated_circuit)
@@ -135,39 +145,55 @@
             if n_attempts == max_attempts:
                 raise ValueError(f"desired_meas_result was not measured after {n_attempts} attempts")
 
             self.all_frequencies = {k: v / self.n_shots for k, v in samples.items()}
             frequencies = self.all_frequencies
 
         # desired_meas_result without a noise model
+        # Split circuit into chunks between mid-circuit measurements. Simulate a chunk, collapse the statevector according
+        # to the desired measurement and simulate the next chunk using this new statevector as input
         elif desired_meas_result is not None:
-            backend, translated_circuit = aer_backend_with_statevector(translated_circuit)
 
-            samples = dict()
-            self._current_state = None
-            n_attempts = 0
+            success_probability = 1
 
-            # Permit 0.1% probability events
-            max_attempts = 1000
+            if initial_statevector is not None:
+                sv = np.asarray(initial_statevector, dtype=complex)
+            else:
+                sv = np.zeros(2**source_circuit.width)
+                sv[0] = 1.
 
-            while self._current_state is None and n_attempts < max_attempts:
-                current_state, measure = run_and_measure_one_shot(backend, translated_circuit)
+            for i, circ in enumerate(unitary_circuits[:-1]):
+                if circ.size != 0:
+                    translated_circuit = translate_c(circ, "qiskit", output_options={"save_measurements": False})
+                    translated_circuit = load_statevector(translated_circuit, sv)
+                    backend, translated_circuit = aer_backend_with_statevector(translated_circuit)
+                    sim_results = backend.run(translated_circuit).result()
+                    current_state = sim_results.get_statevector(translated_circuit)
+                    sv, cprob = self.collapse_statevector_to_desired_measurement(np.asarray(current_state), qubits[i],
+                                                                                 int(desired_meas_result[i]))
+                else:
+                    sv, cprob = self.collapse_statevector_to_desired_measurement(sv, qubits[i],
+                                                                                 int(desired_meas_result[i]))
 
-                if measure == desired_meas_result:
-                    self._current_state = current_state
-                    if self.n_shots is not None:
-                        self.all_frequencies = {measure + state[::-1]: count for state, count in current_state.sample_counts(self.n_shots).items()}
-                    else:
-                        freqs = self._statevector_to_frequencies(np.array(current_state))
-                        self.all_frequencies = {measure + meas: val for meas, val in freqs.items()}
+                success_probability *= cprob
 
-                n_attempts += 1
+            translated_circuit = translate_c(unitary_circuits[-1], "qiskit", output_options={"save_measurements": False})
+            translated_circuit = load_statevector(translated_circuit, sv)
+            backend, translated_circuit = aer_backend_with_statevector(translated_circuit)
+            sim_results = backend.run(translated_circuit).result()
+            current_state = sim_results.get_statevector(translated_circuit)
+            self._current_state = np.asarray(current_state)
 
-            if n_attempts == max_attempts:
-                raise ValueError(f"desired_meas_result was not measured after {n_attempts} attempts")
+            source_circuit._probabilities[desired_meas_result] = success_probability
+
+            if self.n_shots is not None:
+                self.all_frequencies = {desired_meas_result + state[::-1]: count for state, count in current_state.sample_counts(self.n_shots).items()}
+            else:
+                freqs = self._statevector_to_frequencies(np.array(current_state))
+                self.all_frequencies = {desired_meas_result + meas: val for meas, val in freqs.items()}
 
             frequencies = self.all_frequencies.copy()
 
         # mixed state with return statevector. Can be used to test the returned statevector given a measurement outcome.
         elif save_mid_circuit_meas and self.n_shots in [1]:
             backend, translated_circuit = aer_backend_with_statevector(translated_circuit)
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/target/target_qulacs.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qulacs.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 import os
 from collections import Counter
 
 import numpy as np
 
-from tangelo.linq import Circuit
+from tangelo.linq import Circuit, get_unitary_circuit_pieces
 from tangelo.linq.target.backend import Backend
 from tangelo.linq.translator import translate_circuit as translate_c
 from tangelo.linq.translator import translate_operator
 
 
 class QulacsSimulator(Backend):
 
@@ -60,16 +60,17 @@
 
         Returns:
             dict: A dictionary mapping multi-qubit states to their corresponding
                 frequency.
             numpy.array: The statevector, if available for the target backend
                 and requested by the user (if not, set to None).
         """
-        translated_circuit = translate_c(source_circuit, "qulacs", output_options={"noise_model": self._noise_model,
-                                                                                   "save_measurements": save_mid_circuit_meas})
+        if desired_meas_result is None:
+            translated_circuit = translate_c(source_circuit, "qulacs", output_options={"noise_model": self._noise_model,
+                                                                                       "save_measurements": save_mid_circuit_meas})
 
         n_meas = source_circuit.counts.get("MEASURE", 0)
 
         # Initialize state on GPU if available and desired. Default to CPU otherwise.
         if ('QuantumStateGpu' in dir(self.qulacs)) and (int(os.getenv("QULACS_USE_GPU", 0)) != 0):
             state = self.qulacs.QuantumStateGpu(source_circuit.width)
         else:
@@ -88,55 +89,78 @@
                 python_statevector = np.array(state.get_vector()) if return_statevector else None
                 samples = Counter(state.sampling(self.n_shots))  # this sampling still returns a list
             else:
                 python_statevector = np.array(state.get_vector())
                 frequencies = self._statevector_to_frequencies(python_statevector)
                 return (frequencies, python_statevector) if return_statevector else (frequencies, None)
 
-        # If a desired_meas_result, repeat until success if no noise model or repeat until n_shots desired_meas_results.
+        # If a desired_meas_result,
+        # If no noise model, Split circuit into chunks between mid-circuit measurements. Simulate a chunk, collapse the statevector according
+        # to the desired measurement and simulate the next chunk using this new statevector as input
+        # If noise_model, repeat until n_shots desired_meas_results.
         elif desired_meas_result is not None:
-            self._current_state = None
-            n_attempts = 0
-            n_success = 0
-            n_shots = self.n_shots if self.n_shots is not None else -1
-
-            # Permit 0.1% probability events
-            max_attempts = 1000*abs(n_shots)
-            samples = dict()
-            while self._current_state is None and n_attempts < max_attempts and n_success != n_shots:
-                translated_circuit.update_quantum_state(state)
-                measure = "".join([str(state.get_classical_value(i)) for i in range(n_meas)])
+            if not self._noise_model:
+                success_probability = 1
+                unitary_circuits, qubits = get_unitary_circuit_pieces(source_circuit)
+
+                for i, circ in enumerate(unitary_circuits[:-1]):
+                    if circ.size > 0:
+                        translated_circuit = translate_c(circ, "qulacs", output_options={"save_measurements": True})
+                        translated_circuit.update_quantum_state(state)
+                    sv, cprob = self.collapse_statevector_to_desired_measurement(state.get_vector(), qubits[i], int(desired_meas_result[i]))
+                    success_probability *= cprob
+                    state.load(sv)
 
-                if measure == desired_meas_result:
-                    python_statevector = state.get_vector()
-                    if self._noise_model:
-                        n_success += 1
-                        sample = state.sampling(1)[0]
-                        samples[sample] = samples.get(sample, 0) + 1
-                    else:
-                        self._current_state = python_statevector
-                        if self.n_shots is not None:
-                            samples = Counter(state.sampling(self.n_shots))
-                        else:
-                            frequencies = self._statevector_to_frequencies(python_statevector)
-                            self.all_frequencies = dict()
-                            for meas, val in frequencies.items():
-                                self.all_frequencies[measure + meas] = val
+                translated_circuit = translate_c(unitary_circuits[-1], "qulacs", output_options={"save_measurements": True})
+                translated_circuit.update_quantum_state(state)
+                python_statevector = state.get_vector()
+                self._current_state = python_statevector
+                source_circuit._probabilities[desired_meas_result] = success_probability
 
-                if initial_statevector is not None:
-                    state.load(initial_statevector)
+                if self.n_shots is not None:
+                    samples = Counter(state.sampling(self.n_shots))
                 else:
-                    state.set_zero_state()
-                n_attempts += 1
+                    frequencies = self._statevector_to_frequencies(python_statevector)
+                    self.all_frequencies = dict()
+                    for meas, val in frequencies.items():
+                        self.all_frequencies[desired_meas_result + meas] = val
+            else:
+                translated_circuit = translate_c(source_circuit, "qulacs", output_options={"noise_model": self._noise_model,
+                                                                                           "save_measurements": save_mid_circuit_meas})
+                self._current_state = None
+
+                n_success = 0
+
+                # Permit 0.1% probability events
+                n_attempts = 0
+                max_attempts = 1000*self.n_shots
+                samples = dict()
+
+                while self._current_state is None and n_attempts < max_attempts and n_success != self.n_shots:
+                    translated_circuit.update_quantum_state(state)
+                    measure = "".join([str(state.get_classical_value(i)) for i in range(n_meas)])
+
+                    if measure == desired_meas_result:
+                        python_statevector = state.get_vector()
+                        if self._noise_model:
+                            n_success += 1
+                            sample = state.sampling(1)[0]
+                            samples[sample] = samples.get(sample, 0) + 1
+
+                    if initial_statevector is not None:
+                        state.load(initial_statevector)
+                    else:
+                        state.set_zero_state()
+                    n_attempts += 1
 
-            if n_attempts == max_attempts:
-                raise ValueError(f"desired_meas_result was not measured after {n_attempts} attempts")
+                if n_attempts == max_attempts:
+                    raise ValueError(f"desired_meas_result was not measured after {n_attempts} attempts")
 
             if self.n_shots is not None:
-                self.all_frequencies = {measure + self._int_to_binstr(k, source_circuit.width): v / self.n_shots
+                self.all_frequencies = {desired_meas_result + self._int_to_binstr(k, source_circuit.width): v / self.n_shots
                                         for k, v in samples.items()}
 
             return (self.all_frequencies, python_statevector) if return_statevector else (self.all_frequencies, None)
 
         # No desired_meas_result, repeat simulation n_shot times and collect measurement data.
         # Same process for if noise model present or not.
         elif save_mid_circuit_meas:
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/test_circuits.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_circuits.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 
 import unittest
 import copy
 from math import pi
 from collections import Counter
 
-from tangelo.linq import Gate, Circuit, stack
+from tangelo.linq import Gate, Circuit, stack, get_unitary_circuit_pieces
 
 # Create several abstract circuits with different features
 mygates = [Gate("H", 2), Gate("CNOT", 1, control=0), Gate("CNOT", 2, control=1),
            Gate("Y", 0), Gate("RX", 1, parameter=2.)]
 
 circuit1 = Circuit()
 for gate in mygates:
@@ -297,10 +297,31 @@
     def test_iterate(self):
         """ Test if the iteration returns the expected list of gates. """
 
         self.assertEqual([g for g in circuit2], circuit2._gates)
         self.assertEqual([g for g in circuit3], circuit3._gates)
         self.assertEqual([g for g in circuit4], circuit4._gates)
 
+    def test_unitary_pieces(self):
+        """ Test the splitting of circuit into unitary pieces between measurements."""
+        test_circuit = Circuit([Gate("H", 0), Gate("H", 1), Gate("MEASURE", 0),
+                                Gate("X", 1), Gate("MEASURE", 1),
+                                Gate("H", 0), Gate("H", 1), Gate("CNOT", control=0, target=1), Gate("MEASURE", 0),
+                                Gate("MEASURE", 1),
+                                Gate("H", 0), Gate("MEASURE", 1)])
+        circuits = [Circuit([Gate("H", 0), Gate("H", 1)], n_qubits=2),
+                    Circuit([Gate("X", 1)], n_qubits=2),
+                    Circuit([Gate("H", 0), Gate("H", 1), Gate("CNOT", control=0, target=1)], n_qubits=2),
+                    Circuit(n_qubits=2),
+                    Circuit([Gate("H", 0)], n_qubits=2),
+                    Circuit(n_qubits=2)]
+        measure_qs = [0, 1, 0, 1, 1]
+        split_circuits, qubits_to_measure = get_unitary_circuit_pieces(test_circuit)
+
+        for i, circ in enumerate(circuits[:-1]):
+            self.assertEqual(circ, split_circuits[i])
+            self.assertEqual(measure_qs[i], qubits_to_measure[i])
+        self.assertEqual(circuits[-1], split_circuits[-1])
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/test_gates.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_gates.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,14 +81,36 @@
         self.assertEqual(RX_gate.inverse(), RX_gate_inverse)
 
         # Create a parameterized rotation on qubit 1 , with an undefined angle, that will be variational
         RZ_gate = Gate("RZ", 1, parameter="an expression", is_variational=True)
         with self.assertRaises(AttributeError):
             RZ_gate.inverse()
 
+    def test_is_clifford(self):
+        """ Test that some basic gates are correctly identified as Clifford or non Clifford"""
+
+        # test single qubit Clifford gates
+        for name in {"H", "S", "X", "Z", "Y", "SDAG"}:
+            self.assertEqual(True, Gate(name, 0).is_clifford())
+
+        # test two qubit Clifford gates
+        for name in {"CNOT", "CX", "CY", "CZ"}:
+            self.assertEqual(True, Gate(name, target=0, control=1).is_clifford())
+
+        # test parameterized single qubit gates at Clifford and non Clifford parameters
+        for name in {"RX", "RY", "RZ", "PHASE"}:
+            for clifford_point in [0, np.pi/2, np.pi, -np.pi/2, 4*np.pi]:
+                self.assertEqual(True, Gate(name, 0, parameter=clifford_point).is_clifford())
+            for non_clifford_point in [0.1, -np.pi/3, 5*np.pi/4, 1.5]:
+                self.assertEqual(False, Gate(name, 0, parameter=non_clifford_point).is_clifford())
+
+        # test two qubit non Clifford gates
+        for name in {"CRX", "CRY", "CRZ", "CPHASE"}:
+            self.assertEqual(False, Gate(name, target=0, control=1).is_clifford())
+
     def test_incorrect_gate(self):
         """ Test to catch a gate with inputs that do not make sense """
 
         self.assertRaises(ValueError, Gate, "H", -1)
         self.assertRaises(ValueError, Gate, "CNOT", 0, control=0.3)
         self.assertRaises(ValueError, Gate, 'X', target=0, control=1)
         self.assertRaises(ValueError, Gate, "CNOT", target=0, control=0)
@@ -122,10 +144,21 @@
 
         # Try to create a Hadamard gate acting on qubits 0 and 1.
         self.assertRaises(ValueError, Gate, "H", target=[0, 1])
 
         # Try to create a XX gate acting on qubits 0, 1 and 2.
         self.assertRaises(ValueError, Gate, "XX", target=[0, 1, 2])
 
+    def test_non_hermitian_gates_inverse(self):
+        """ Test that non-hermitian gates (S, T) can be inversed."""
+
+        S_gate = Gate("S", 0)
+        S_gate_inverse = Gate("PHASE", 0, parameter=-np.pi/2)
+        self.assertEqual(S_gate.inverse(), S_gate_inverse)
+
+        T_gate = Gate("T", 0)
+        T_gate_inverse = Gate("PHASE", 0, parameter=-np.pi/4)
+        self.assertEqual(T_gate.inverse(), T_gate_inverse)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/test_ibm_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_ibm_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import time
 
 import numpy as np
 
 from tangelo.helpers.utils import assert_freq_dict_almost_equal
 from tangelo.linq import Gate, Circuit, get_backend
-from tangelo.linq.qpu_connection import IBMConnection
+from tangelo.linq.qpu_connection.ibm_connection import IBMConnection
 from tangelo.toolboxes.operators import QubitOperator
 
 # Circuit and qubit operator for test
 circ = Circuit([Gate("H", 0), Gate("X", 1)])
 circ2 = Circuit([Gate("RX", 0, parameter=2.), Gate("RY", 1, parameter=-1.)])
 op = 1.0 * QubitOperator('Y0') - 2.0 * QubitOperator('Z0 X1')
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/test_ionq_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_ionq_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import unittest
 import os
 import pprint
 
 from tangelo.linq import Gate, Circuit
-from tangelo.linq.qpu_connection import IonQConnection
+from tangelo.linq.qpu_connection.ionq_connection import IonQConnection
 from tangelo.helpers.utils import assert_freq_dict_almost_equal
 
 circ1 = Circuit([Gate("H", 0), Gate("X", 1)])
 res_simulator_circ1 = {'01': 0.5, '11': 0.5}
 
 
 @unittest.skip("We do not want to store login information for automated testing")
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/test_simulator.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 """
 
 import unittest
 import os
 import time
 
 import numpy as np
-from openfermion.ops import QubitOperator
 from openfermion import load_operator, get_sparse_operator
 
+from tangelo.toolboxes.operators import QubitOperator
 from tangelo.linq import Gate, Circuit, get_backend
 from tangelo.linq.translator import translate_circuit as translate_c
 from tangelo.linq.gate import PARAMETERIZED_GATES
-from tangelo.helpers.utils import installed_simulator, installed_sv_simulator, installed_backends
 from tangelo.linq.target.backend import Backend, get_expectation_value_from_frequencies_oneterm
-from tangelo.helpers.utils import assert_freq_dict_almost_equal
+from tangelo.helpers.utils import installed_simulator, installed_sv_simulator, installed_backends, installed_clifford_simulators, assert_freq_dict_almost_equal
+
 
 path_data = os.path.dirname(os.path.abspath(__file__)) + '/data'
 
 # Simple circuit for superposition, also tells us qubit ordering as well immediately from the statevector
 # probabilities : |00> = 0.5  |01> = 0.5
 circuit1 = Circuit([Gate("H", 0)], n_qubits=2)
 
@@ -45,27 +45,37 @@
 
 # Circuit for the parametrized rotation gates Rx and Ry. Some convention about the sign of theta or a phase may appear
 circuit3 = Circuit([Gate("RX", 0, parameter=2.), Gate("RY", 1, parameter=-1.)])
 
 # Circuit for the parametrized rotation gate Rz. Some convention about the sign of theta or a phase may appear
 circuit4 = Circuit([Gate("RZ", 0, parameter=2.)], n_qubits=2)
 
-# Circuit that tests all gates that are supported on all simulators
+# Circuit that tests all gates that are supported on all general simulators
 init_gates = [Gate('H', 0), Gate('X', 1), Gate('H', 2)]
 one_qubit_gate_names = ["H", "X", "Y", "Z", "S", "T", "RX", "RY", "RZ", "PHASE"]
 one_qubit_gates = [Gate(name, target=0) if name not in PARAMETERIZED_GATES else Gate(name, target=0, parameter=0.5)
                    for name in one_qubit_gate_names]
 one_qubit_gates += [Gate(name, target=1) if name not in PARAMETERIZED_GATES else Gate(name, target=1, parameter=0.2)
                     for name in one_qubit_gate_names]
 two_qubit_gate_names = ["CNOT", "CH", "CX", "CY", "CZ", "CRX", "CRY", "CRZ", "CPHASE"]
 two_qubit_gates = [Gate(name, target=1, control=0) if name not in PARAMETERIZED_GATES
                    else Gate(name, target=1, control=0, parameter=0.5) for name in two_qubit_gate_names]
 swap_gates = [Gate('SWAP', target=[1, 0]), Gate('CSWAP', target=[1, 2], control=0)]
 circuit5 = Circuit(init_gates + one_qubit_gates + two_qubit_gates + swap_gates)
 
+# Circuit that tests all gates are supported on clifford simulator
+one_qubit_gate_names = ["H", "X", "Y", "Z", "S", "RX", "RY", "RZ"]
+one_qubit_gates = [Gate(name, target=0) if name not in PARAMETERIZED_GATES else Gate(name, target=0, parameter=-np.pi/2)
+                   for name in one_qubit_gate_names]
+one_qubit_gates += [Gate(name, target=1) if name not in PARAMETERIZED_GATES else Gate(name, target=1, parameter=np.pi)
+                    for name in one_qubit_gate_names]
+clifford_two_qubit_gate_names = ["CNOT", "CX", "CY", "CZ"]
+clifford_two_qubit_gates = [Gate(name, target=1, control=0) for name in clifford_two_qubit_gate_names]
+circuit_clifford = Circuit(init_gates + one_qubit_gates + clifford_two_qubit_gates + [Gate('SWAP', target=[1, 0])])
+
 # Circuit preparing a mixed-state (i.e. containing a MEASURE instruction in the middle of the circuit)
 circuit_mixed = Circuit([Gate("RX", 0, parameter=2.), Gate("RY", 1, parameter=-1.), Gate("MEASURE", 0), Gate("X", 0)])
 circuit_mixed_1 = Circuit([Gate("RX", 0, parameter=2.), Gate("RY", 0, parameter=-1.), Gate("MEASURE", 0), Gate("X", 0)])
 
 # Operators for testing the get_expectation_value functions
 op1 = 1.0 * QubitOperator('Z0')  # all Z
 op2 = 1.0 * QubitOperator('X1 Y0')  # X and Y
@@ -80,87 +90,89 @@
 ref_freqs.append({'00': 0.5, '10': 0.5})
 ref_freqs.append({'01': 0.5, '10': 0.5})
 ref_freqs.append({'00': 0.2248275934887, '10': 0.5453235594453, '01': 0.06709898823771, '11': 0.16274985882821})
 ref_freqs.append({'00': 1.0})
 ref_freqs.append({'000': 0.15972060437359714, '100': 0.2828171838599203, '010': 0.03984122195648572,
                   '110': 0.28281718385992016, '001': 0.15972060437359714, '101': 0.017620989809996816,
                   '011': 0.039841221956485706, '111': 0.01762098980999681})
+ref_freqs_clifford = {bs: 0.125 for bs in ['000', '100', '010', '110', '001', '101',  '011', '111']}
 reference_exp_values = np.array([[0., 0., 0.], [0., -1., 0.], [-0.41614684, 0.7651474, -1.6096484], [1., 0., 0.],
                                  [-0.20175269, -0.0600213, 1.2972912]])
+clifford_reference_exp_values = np.array([0, 0, 2])
 reference_mixed = {'01': 0.163, '11': 0.066, '10': 0.225, '00': 0.545}  # With Qiskit noiseless, 1M shots
 reference_all = {'101': 0.163, '011': 0.066, '010': 0.225, '100': 0.545}
 reference_mid = {'1': 0.7, '0': 0.3}
 
 
 class TestSimulateAllBackends(unittest.TestCase):
 
     def test_get_exp_value_operator_too_long(self):
         """ Ensure an error is returned if the qubit operator acts on more qubits than are present in the circuit """
-        for b in installed_simulator:
+        for b in (installed_simulator | installed_clifford_simulators):
             simulator = get_backend(target=b, n_shots=1)
             self.assertRaises(ValueError, simulator.get_expectation_value, op4, circuit1)
 
     def test_get_exp_value_empty_operator(self):
         """ If qubit operator is empty, the expectation value is 0 and no computation occurs """
-        for b in installed_simulator:
+        for b in (installed_simulator | installed_clifford_simulators):
             simulator = get_backend(target=b, n_shots=1)
             exp_value = simulator.get_expectation_value(QubitOperator(), circuit1)
             self.assertTrue(exp_value == 0.)
 
     def test_get_exp_value_constant_operator(self):
         """ The expectation of the identity term must be 1. """
-        for b in installed_simulator:
+        for b in (installed_simulator | installed_clifford_simulators):
             simulator = get_backend(target=b, n_shots=1)
             const_op = QubitOperator()
             const_op.terms = {(): 777.}
             exp_value = simulator._get_expectation_value_from_frequencies(const_op, circuit1)
             self.assertTrue(exp_value == 777.)
 
     def test_simulate_mixed_state(self):
         """ Test mid-circuit measurement (mixed-state simulation) for compatible/testable formats and backends."""
 
         results = dict()
         for b in installed_simulator:
-            sim = get_backend(target=b, n_shots=10 ** 5)
+            sim = get_backend(target=b, n_shots=10**5)
             results[b], _ = sim.simulate(circuit_mixed)
             assert_freq_dict_almost_equal(results[b], reference_mixed, 1e-2)
 
     def test_simulate_mixed_state_save_measures(self):
         """ Test mid-circuit measurement (mixed-state simulation) for all installed backends."""
         results = dict()
         for b in installed_simulator:
-            sim = get_backend(target=b, n_shots=10 ** 3)
+            sim = get_backend(target=b, n_shots=10**3)
             results[b], _ = sim.simulate(circuit_mixed, save_mid_circuit_meas=True)
             assert_freq_dict_almost_equal(results[b], reference_mixed, 8e-2)
             assert_freq_dict_almost_equal(sim.all_frequencies, reference_all, 8e-2)
             assert_freq_dict_almost_equal(sim.mid_circuit_meas_freqs, reference_mid, 8e-2)
 
     def test_simulate_mixed_state_desired_state(self):
         """ Test mid-circuit measurement (mixed-state simulation) for all installed backends."""
 
         results = dict()
         exact = {'11': 0.23046888414227926, '10': 0.7695311158577207}
         for b in installed_simulator:
-            sim = get_backend(target=b, n_shots=10 ** 3)
+            sim = get_backend(target=b, n_shots=10**3)
             results[b], _ = sim.simulate(circuit_mixed, desired_meas_result="0")
             assert_freq_dict_almost_equal(results[b], exact, 8.e-2)
 
     def test_desired_meas_len(self):
         """ Test if the desired_meas_result parameter is a string and of the right length."""
-        sim = get_backend(target="cirq", n_shots=10 ** 3)
+        sim = get_backend(target="cirq", n_shots=10**3)
         self.assertRaises(ValueError, sim.simulate, circuit_mixed, desired_meas_result=0)
         self.assertRaises(ValueError, sim.simulate, circuit_mixed, desired_meas_result="01")
 
     def test_get_exp_value_mixed_state(self):
         """ Test expectation value for mixed-state simulation. Computation done by drawing individual shots."""
 
         reference = 0.41614683  # Exact value
         results = dict()
         for b in installed_simulator:
-            sim = get_backend(target=b, n_shots=10 ** 5)
+            sim = get_backend(target=b, n_shots=10**5)
             results[b] = sim.get_expectation_value(op1, circuit_mixed)
             np.testing.assert_almost_equal(results[b], reference, decimal=2)
 
     def test_get_variance(self):
         """ Test variance for simple analytical circuit. """
 
         opx = 1.0 * QubitOperator("X0")
@@ -211,14 +223,19 @@
         """ Must return correct frequencies for simulation of different quantum circuits with statevector """
         for b in installed_sv_simulator:
             simulator = get_backend(target=b)
             for i, circuit in enumerate(circuits):
                 frequencies, _ = simulator.simulate(circuit)
                 assert_freq_dict_almost_equal(ref_freqs[i], frequencies, atol=1e-5)
 
+        for b in installed_clifford_simulators:
+            simulator = get_backend(target=b)
+            frequencies, _ = simulator.simulate(circuit_clifford)
+            assert_freq_dict_almost_equal(ref_freqs_clifford, frequencies, atol=1e-5)
+
     def test_simulate_mixed_state_desired_statevector(self):
         """ Test mid-circuit measurement (mixed-state simulation) for compatible/testable formats and backends when returning
         a statevector."""
 
         results = dict()
         results["qulacs"] = np.array([0. + 0.j, 0.87758256 + 0.j, 0. + 0.j, -0.47942554 + 0.j])
         results["qiskit"] = np.array([0. + 0.j, 0.87758256 + 0.j, 0. + 0.j, -0.47942554 + 0.j])
@@ -227,20 +244,23 @@
         freqs_exact = {'10': 0.7701511529340699, '11': 0.2298488470659301}
 
         for b in installed_sv_simulator:
             sim = get_backend(target=b, n_shots=None)
             f, sv = sim.simulate(circuit_mixed, desired_meas_result="0", return_statevector=True)
             np.testing.assert_array_almost_equal(sv, results[b])
             assert_freq_dict_almost_equal(f, freqs_exact, 1.e-7)
+            self.assertAlmostEqual(0.2919265817264289, circuit_mixed.success_probabilities["0"], places=7)
 
             # Test that initial_statevector is respected
-            f, sv = sim.simulate(Circuit([Gate("MEASURE", 0), Gate("MEASURE", 1)]), desired_meas_result="11",
+            meas_2_circuit = Circuit([Gate("MEASURE", 0), Gate("MEASURE", 1)])
+            f, sv = sim.simulate(meas_2_circuit, desired_meas_result="11",
                                  return_statevector=True, initial_statevector=initial_state)
             np.testing.assert_array_almost_equal(sv, initial_state)
             assert_freq_dict_almost_equal(f, {"11": 1}, 1.e-7)
+            self.assertAlmostEqual(1., meas_2_circuit.success_probabilities["11"], places=7)
 
             # Test that ValueError is raised for desired_meas_result="0" with probability 0. i.e. loop exits successfully
             self.assertRaises(ValueError, sim.simulate, Circuit([Gate("X", 0), Gate("MEASURE", 0)]), True, None, "0")
 
             sim = get_backend(target=b, n_shots=10**3)
             f, sv = sim.simulate(circuit_mixed, desired_meas_result="0", return_statevector=True)
             np.testing.assert_array_almost_equal(sv, results[b])
@@ -264,19 +284,24 @@
     def test_simulate_nshots_from_statevector(self):
         """
             Test the generation of samples following the distribution given by the exact frequencies obtained
             with a statevector simulator. For n_shots high enough, the resulting distribution must approximate
             the exact one.
         """
         for b in installed_sv_simulator:
-            simulator = get_backend(target=b, n_shots=10 ** 6)
+            simulator = get_backend(target=b, n_shots=10**6)
             for i, circuit in enumerate(circuits):
                 frequencies, _ = simulator.simulate(circuit)
                 assert_freq_dict_almost_equal(ref_freqs[i], frequencies, atol=1e-2)
 
+        for b in installed_clifford_simulators:
+            simulator = get_backend(target=b, n_shots=10**6)
+            frequencies, _ = simulator.simulate(circuit_clifford)
+            assert_freq_dict_almost_equal(ref_freqs_clifford, frequencies, atol=1e-2)
+
     def test_simulate_empty_circuit_from_statevector(self):
         """ Test the generation of frequencies using an initial_statevector and an empty_circuit """
         for b in installed_sv_simulator:
             simulator = get_backend(target=b)
             for i, circuit in enumerate(circuits):
                 _, statevector = simulator.simulate(circuit, return_statevector=True)
                 frequencies, _ = simulator.simulate(Circuit(n_qubits=circuit.width), initial_statevector=statevector)
@@ -288,14 +313,21 @@
             simulator = get_backend(target=b)
             exp_values = np.zeros((len(circuits), len(ops)), dtype=float)
             for i, circuit in enumerate(circuits):
                 for j, op in enumerate(ops):
                     exp_values[i][j] = simulator._get_expectation_value_from_statevector(op, circuit)
             np.testing.assert_almost_equal(exp_values, reference_exp_values, decimal=5)
 
+        for b in installed_clifford_simulators:
+            simulator = get_backend(target=b)
+            clifford_exp_values = np.zeros(len(ops))
+            for j, op in enumerate(ops):
+                clifford_exp_values[j] = simulator._get_expectation_value_from_statevector(op, circuit_clifford)
+            np.testing.assert_almost_equal(clifford_exp_values, clifford_reference_exp_values, decimal=5)
+
     def test_get_exp_value_from_frequencies_using_initial_statevector(self):
         """ Test the method computing the expectation value from frequencies, with a given simulator
             by generating the statevector first and sampling using an empty state_prep_circuit
         """
 
         for b in installed_sv_simulator:
             simulator = get_backend(target=b)
@@ -408,40 +440,40 @@
         """
         qubit_operator = load_operator("mol_H2_qubitham.data", data_directory=path_data, plain_text=True)
 
         with open(f"{path_data}/H2_UCCSD.qasm", "r") as circ_handle:
             openqasm_circ = circ_handle.read()
         abs_circ = translate_c(openqasm_circ, "tangelo", source="openqasm")
 
-        simulator = get_backend(target="qulacs", n_shots=10 ** 6)
+        simulator = get_backend(target="qulacs", n_shots=10**6)
         expected = -1.1372704
 
         energy = simulator.get_expectation_value(qubit_operator, abs_circ)
         self.assertAlmostEqual(energy, expected, delta=1e-3)
 
     def test_get_exp_value_mixed_state_desired_measurement_with_shots(self):
         """ Get expectation value of mixed state by post-selecting on desired measurement."""
         qubit_operator = QubitOperator("X0 X1") + QubitOperator("Y0 Y1") + QubitOperator("Z0 Z1") + QubitOperator("X0 Y1", 1j)
 
-        ham = get_sparse_operator(qubit_operator).toarray()
+        ham = get_sparse_operator(qubit_operator.to_openfermion()).toarray()
         exact_sv = np.array([0.+0.j, 0.+0.j, 0.87758256+0.j, -0.47942554+0.j])
         exact_exp = np.vdot(exact_sv, ham @ exact_sv)
 
         simulator = get_backend(n_shots=10**4)
         sim_exp = simulator.get_expectation_value(qubit_operator, circuit_mixed, desired_meas_result="0")
         self.assertAlmostEqual(exact_exp, sim_exp, delta=1.e-1)
 
     def test_get_exp_value_empty_circuit(self):
         """ If the circuit is empty and we have a non-zero number of qubits, frequencies just only show all-|0> state
         observed and compute the expectation value using these frequencies """
 
         empty_circuit = Circuit([], n_qubits=2)
         identity_circuit = Circuit([Gate('X', 0), Gate('X', 1)] * 2)
 
-        for b in installed_sv_simulator:
+        for b in (installed_sv_simulator | installed_clifford_simulators):
             simulator = get_backend(target=b)
             for op in [op1, op2]:
                 exp_value_empty = simulator.get_expectation_value(op, empty_circuit)
                 exp_value_identity = simulator.get_expectation_value(op, identity_circuit)
                 np.testing.assert_almost_equal(exp_value_empty, exp_value_identity, decimal=8)
 
     def test_get_exp_value_complex(self):
@@ -470,17 +502,23 @@
             simulator = get_backend(target=b)
             exp_values = np.zeros((len(circuits), len(ops)), dtype=float)
             for i, circuit in enumerate(circuits):
                 for j, op in enumerate(ops):
                     exp_values[i][j] = simulator._get_expectation_value_from_frequencies(op, circuit)
             np.testing.assert_almost_equal(exp_values, reference_exp_values, decimal=5)
 
+        for b in installed_clifford_simulators:
+            simulator = get_backend(target=b)
+            clifford_exp_values = np.zeros(len(ops))
+            for j, op in enumerate(ops):
+                clifford_exp_values[j] = simulator._get_expectation_value_from_frequencies(op, circuit_clifford)
+            np.testing.assert_almost_equal(clifford_exp_values, clifford_reference_exp_values, decimal=5)
+
 
 class TestSimulateMisc(unittest.TestCase):
-
     @unittest.skipIf("qdk" not in installed_backends, "Test Skipped: Backend not available \n")
     def test_n_shots_needed(self):
         """
             Raise an error if user chooses a target backend that does not provide access to a statevector and
             also does not provide a number of shots for the simulation.
         """
         self.assertRaises(ValueError, get_backend, target="qdk")
@@ -488,25 +526,25 @@
     @unittest.skipIf("qdk" not in installed_backends, "Test Skipped: Backend not available \n")
     def test_simulate_qdk(self):
         """
             Must return correct frequencies for simulation of different quantum circuits.
             The accuracy is correlated to the number of shots taken in the simulation.
             Backend: qdk.
         """
-        simulator = get_backend(target="qdk", n_shots=10 ** 4)
+        simulator = get_backend(target="qdk", n_shots=10**4)
         for i, circuit in enumerate(circuits):
             frequencies, _ = simulator.simulate(circuit)
             assert_freq_dict_almost_equal(ref_freqs[i], frequencies, atol=1e-1)
 
     @unittest.skipIf("qdk" not in installed_backends, "Test Skipped: Backend not available \n")
     def test_get_exp_value_from_frequencies_qdk(self):
         """ Test specific to QDK to ensure results are not impacted by code specific to frequency computation
             as well as the recompilation of the Q# file used in successive simulations """
 
-        simulator = get_backend(target="qdk", n_shots=10 ** 4)
+        simulator = get_backend(target="qdk", n_shots=10**4)
         exp_values = np.zeros((len(ops)), dtype=float)
         for j, op in enumerate(ops):
             exp_values[j] = simulator.get_expectation_value(op, circuit3)
         np.testing.assert_almost_equal(exp_values, reference_exp_values[2], decimal=1)
 
     def test_get_exp_value_from_frequencies_oneterm(self):
         """ Test static method computing the expectation value of one term, when the results of a simulation
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/test_simulator_noisy.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_simulator_noisy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 """
     A test class to check that the features related to noisy simulation are working as expected.
 """
 
 import unittest
 
 import numpy as np
-from openfermion.ops import QubitOperator
 
 from tangelo.linq import Gate, Circuit, get_backend, backend_info
 from tangelo.linq.noisy_simulation import NoiseModel, get_qiskit_noise_dict
 from tangelo.helpers.utils import default_simulator, installed_backends, assert_freq_dict_almost_equal
+from tangelo.toolboxes.operators import QubitOperator
 
 # Noisy simulation: circuits, noise models, references
 cn1 = Circuit([Gate('X', target=0)])
 cn2 = Circuit([Gate('CNOT', target=1, control=0)])
 circuit_mixed = Circuit([Gate("RX", 0, parameter=2.), Gate("RY", 1, parameter=-1.), Gate("MEASURE", 0), Gate("X", 0)])
 
 nmp, nmd, nmc, nmm = NoiseModel(), NoiseModel(), NoiseModel(), NoiseModel()
@@ -107,33 +107,33 @@
     def test_noisy_simulation_qulacs(self):
         """
             Test noisy simulation through qulacs.
             Currently tested: pauli noise, depolarization noise (1 and 2 qubit gates)
         """
 
         # Pauli noise for one- and two-qubit gates. Circuits are only a X gate, or just a CNOT gate.
-        s_nmp = get_backend(target='qulacs', n_shots=10 ** 6, noise_model=nmp)
+        s_nmp = get_backend(target='qulacs', n_shots=10**6, noise_model=nmp)
         res_pauli1, _ = s_nmp.simulate(cn1)
         assert_freq_dict_almost_equal(res_pauli1, ref_pauli1, 1e-2)
         res_pauli2, _ = s_nmp.simulate(cn2)
         assert_freq_dict_almost_equal(res_pauli2, ref_pauli2, 1e-2)
 
         # Depol noise for one- and two-qubit gates. Circuits are only a X gate or just a CNOT gate.
-        s_nmd = get_backend(target='qulacs', n_shots=10 ** 6, noise_model=nmd)
+        s_nmd = get_backend(target='qulacs', n_shots=10**6, noise_model=nmd)
         res_depol1, _ = s_nmd.simulate(cn1)
         assert_freq_dict_almost_equal(res_depol1, ref_depol1, 1e-2)
         res_depol2, _ = s_nmd.simulate(cn2)
         assert_freq_dict_almost_equal(res_depol2, ref_depol2, 1e-2)
 
         # Cumulate several noises on a given gate (here noise simplifies to identity)
-        s_nmc = get_backend(target='qulacs', n_shots=10 ** 6, noise_model=nmc)
+        s_nmc = get_backend(target='qulacs', n_shots=10**6, noise_model=nmc)
         res_cumul, _ = s_nmc.simulate(cn1)
         assert_freq_dict_almost_equal(res_cumul, ref_cumul, 1e-2)
 
-        s_nmm = get_backend(target="qulacs", n_shots=10 ** 4, noise_model=nmm)
+        s_nmm = get_backend(target="qulacs", n_shots=10**4, noise_model=nmm)
         res_mixed, _ = s_nmm.simulate(circuit_mixed)
         assert_freq_dict_almost_equal(res_mixed, ref_mixed, 7.e-2)
 
         s_nmm = get_backend(target="qulacs", n_shots=10**4, noise_model=nmm)
         res_mixed, _ = s_nmm.simulate(circuit_mixed, desired_meas_result="0")
         assert_freq_dict_almost_equal(ref_mixed_0, res_mixed, 7.e-2)
 
@@ -141,33 +141,33 @@
     def test_noisy_simulation_qiskit(self):
         """
             Test noisy simulation through qiskit.
             Currently tested: pauli noise, depolarization noise (1 and 2 qubit gates)
         """
 
         # Pauli noise for one- and two-qubit gates. Circuits are only a X gate, or just a CNOT gate.
-        s_nmp = get_backend(target='qiskit', n_shots=10 ** 6, noise_model=nmp)
+        s_nmp = get_backend(target='qiskit', n_shots=10**6, noise_model=nmp)
         res_pauli1, _ = s_nmp.simulate(cn1)
         assert_freq_dict_almost_equal(res_pauli1, ref_pauli1, 1e-2)
         res_pauli2, _ = s_nmp.simulate(cn2)
         assert_freq_dict_almost_equal(res_pauli2, ref_pauli2, 1e-2)
 
         # Depol noise for one- and two-qubit gates. Circuits are only a X gate or just a CNOT gate.
-        s_nmd = get_backend(target='qiskit', n_shots=10 ** 6, noise_model=nmd)
+        s_nmd = get_backend(target='qiskit', n_shots=10**6, noise_model=nmd)
         res_depol1, _ = s_nmd.simulate(cn1)
         assert_freq_dict_almost_equal(res_depol1, ref_depol1, 1e-2)
         res_depol2, _ = s_nmd.simulate(cn2)
         assert_freq_dict_almost_equal(res_depol2, ref_depol2, 1e-2)
 
         # Cumulate several noises on a given gate (here noise simplifies to identity)
-        s_nmp = get_backend(target='qiskit', n_shots=10 ** 6, noise_model=nmc)
+        s_nmp = get_backend(target='qiskit', n_shots=10**6, noise_model=nmc)
         res_cumul, _ = s_nmp.simulate(cn1)
         assert_freq_dict_almost_equal(res_cumul, ref_cumul, 1e-2)
 
-        s_nmm = get_backend(target="qiskit", n_shots=10 ** 4, noise_model=nmm)
+        s_nmm = get_backend(target="qiskit", n_shots=10**4, noise_model=nmm)
         res_mixed, _ = s_nmm.simulate(circuit_mixed)
         assert_freq_dict_almost_equal(ref_mixed, res_mixed, 7.e-2)
 
         # Test noise with desired measurement result
         s_nmm = get_backend(target="qiskit", n_shots=10**4, noise_model=nmm)
         res_mixed, _ = s_nmm.simulate(circuit_mixed, desired_meas_result="0")
         assert_freq_dict_almost_equal(ref_mixed_0, res_mixed, 7.e-2)
@@ -176,34 +176,34 @@
     def test_noisy_simulation_cirq(self):
         """
             Test noisy simulation through cirq.
             Currently tested: pauli noise, depolarization noise (1 and 2 qubit gates)
         """
 
         # Pauli noise for one- and two-qubit gates. Circuits are only a X gate, or just a CNOT gate.
-        s_nmp = get_backend(target='cirq', n_shots=10 ** 6, noise_model=nmp)
+        s_nmp = get_backend(target='cirq', n_shots=10**6, noise_model=nmp)
         res_pauli1, _ = s_nmp.simulate(cn1)
         assert_freq_dict_almost_equal(res_pauli1, ref_pauli1, 1e-2)
         res_pauli2, _ = s_nmp.simulate(cn2)
         assert_freq_dict_almost_equal(res_pauli2, ref_pauli2, 1e-2)
 
         # Depol noise for one- and two-qubit gates. Circuits are only a X gate or just a CNOT gate.
-        s_nmd = get_backend(target='cirq', n_shots=10 ** 6, noise_model=nmd)
+        s_nmd = get_backend(target='cirq', n_shots=10**6, noise_model=nmd)
         res_depol1, _ = s_nmd.simulate(cn1)
         assert_freq_dict_almost_equal(res_depol1, ref_depol1, 1e-2)
         res_depol2, _ = s_nmd.simulate(cn2)
         assert_freq_dict_almost_equal(res_depol2, ref_depol2, 1e-2)
 
         # Cumulate several noises on a given gate (here noise simplifies to identity)
-        s_nmc = get_backend(target='cirq', n_shots=10 ** 6, noise_model=nmc)
+        s_nmc = get_backend(target='cirq', n_shots=10**6, noise_model=nmc)
         res_cumul, _ = s_nmc.simulate(cn1)
         assert_freq_dict_almost_equal(res_cumul, ref_cumul, 1e-2)
 
         # Noisy mixed state without returning mid-circuit measurements
-        s_nmm = get_backend(target="cirq", n_shots=10 ** 4, noise_model=nmm)
+        s_nmm = get_backend(target="cirq", n_shots=10**4, noise_model=nmm)
         res_mixed, _ = s_nmm.simulate(circuit_mixed)
         assert_freq_dict_almost_equal(ref_mixed, res_mixed, 7.e-2)
 
         s_nmm = get_backend(target="cirq", n_shots=10**4, noise_model=nmm)
         res_mixed, _ = s_nmm.simulate(circuit_mixed, desired_meas_result="0")
         assert_freq_dict_almost_equal(ref_mixed_0, res_mixed, 7.e-2)
 
@@ -213,14 +213,28 @@
         assert_freq_dict_almost_equal(ref_mixed_0, res_mixed, 7.e-2)
         exact_sv = np.array([[ 0.15403023 + 0.j, -0.08414710 - 0.j,  0.00000000 + 0.j,  0.00000000 - 0.j],
                              [-0.08414710 - 0.j,  0.04596977 + 0.j,  0.00000000 - 0.j,  0.00000000 + 0.j],
                              [ 0.00000000 + 0.j,  0.00000000 - 0.j,  0.61612092 + 0.j, -0.33658839 - 0.j],
                              [ 0.00000000 - 0.j,  0.00000000 + 0.j, -0.33658839 - 0.j,  0.18387908 + 0.j]])
         np.testing.assert_array_almost_equal(sv, exact_sv)
 
+    @unittest.skipIf("stim" not in installed_backends, "Test Skipped: Backend not available \n")
+    def test_noisy_simulation_stim(self):
+        """
+            Test noisy simulation through stim.
+            Currently tested: pauli noise, depolarization noise (1 and 2 qubit gates)
+        """
+
+        # Pauli noise for one- and two-qubit gates. Circuits are only a X gate, or just a CNOT gate.
+        s_nmp = get_backend(target='stim', n_shots=10**6, noise_model=nmp)
+        res_pauli1, _ = s_nmp.simulate(cn1)
+        assert_freq_dict_almost_equal(res_pauli1, ref_pauli1, 1e-2)
+        res_pauli2, _ = s_nmp.simulate(cn2)
+        assert_freq_dict_almost_equal(res_pauli2, ref_pauli2, 1e-2)
+
     def test_get_expectation_value_noisy(self):
         """Test of the get_expectation_value function with a noisy simulator"""
         # Test Hamiltonian.
         H = QubitOperator()
         H.terms = {(): -14.41806525945003, ((0, 'Z'),): 0.0809953994342687,
                    ((1, 'Z'),): 0.0809953994342687, ((0, 'Z'), (1, 'Z')): 0.0077184273651725865,
                    ((0, 'X'), (1, 'X')): 0.0758664717894615}
@@ -237,21 +251,21 @@
         circuit.add_gate(Gate("RX", 1, parameter=10.995574287564))
         circuit.add_gate(Gate("H", 0))
 
         # No Noise model.
         nmp_no_noise = NoiseModel()
         noise = 0.00
         nmp_no_noise.add_quantum_error("CNOT", "pauli", [noise, noise, noise])
-        sim_no_noise = get_backend(target=default_simulator, n_shots=10 ** 6, noise_model=nmp_no_noise)
+        sim_no_noise = get_backend(target=default_simulator, n_shots=10**6, noise_model=nmp_no_noise)
 
         # Small Noise model
         nmp_small_noise = NoiseModel()
         noise = 0.01
         nmp_small_noise.add_quantum_error("CNOT", "pauli", [noise, noise, noise])
-        sim_small_noise = get_backend(target=default_simulator, n_shots=10 ** 6, noise_model=nmp_small_noise)
+        sim_small_noise = get_backend(target=default_simulator, n_shots=10**6, noise_model=nmp_small_noise)
 
         energy_no_noise = sim_no_noise.get_expectation_value(H, circuit)
         energy_small_noise = sim_small_noise.get_expectation_value(H, circuit)
 
         self.assertAlmostEqual(energy_no_noise, -14.58922316, delta=1e-2)
         self.assertAlmostEqual(energy_small_noise, -14.58922316, delta=1e-1)
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/test_translator_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_circuit.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,127 +15,134 @@
 """
     A test class to check that the translation process yields a circuit identical to the native one for the
     different backends supported
 """
 
 import unittest
 import os
+
 import numpy as np
-import time
 
 from tangelo.linq import Gate, Circuit
 from tangelo.linq.gate import PARAMETERIZED_GATES
 from tangelo.linq.translator import translate_circuit as translate_c
 from tangelo.helpers.utils import installed_backends
 
 path_data = os.path.dirname(os.path.realpath(__file__)) + '/data'
 
 gates = [Gate("H", 2), Gate("CNOT", 1, control=0), Gate("CNOT", 2, control=1), Gate("Y", 0), Gate("S", 0)]
 abs_circ = Circuit(gates) + Circuit([Gate("RX", 1, parameter=2.)])
+clifford_abs_circ = Circuit(gates) + Circuit([Gate("RX", 1, parameter=np.pi/2)])
 multi_controlled_gates = [Gate("X", 0), Gate("X", 1), Gate("CX", target=2, control=[0, 1])]
+multi_controlled_gates2 = [Gate("X", 0), Gate("X", 1), Gate("CNOT", target=2, control=[0, 1])]
 abs_multi_circ = Circuit(multi_controlled_gates)
+abs_multi_circ2 = Circuit(multi_controlled_gates2)
 init_gates = [Gate('H', 0), Gate('X', 1), Gate('H', 2)]
 one_qubit_gate_names = ["H", "X", "Y", "Z", "S", "T", "RX", "RY", "RZ", "PHASE"]
 one_qubit_gates = [Gate(name, target=0) if name not in PARAMETERIZED_GATES else Gate(name, target=0, parameter=0.5)
                    for name in one_qubit_gate_names]
 one_qubit_gates += [Gate(name, target=1) if name not in PARAMETERIZED_GATES else Gate(name, target=1, parameter=0.2)
                     for name in one_qubit_gate_names]
+clifford_one_qubit_gates = [Gate(name, target=0) if name not in PARAMETERIZED_GATES else Gate(name, target=0, parameter=np.pi)
+                   for name in one_qubit_gate_names.pop(5)[:-1]]
+clifford_one_qubit_gates += [Gate(name, target=1) if name not in PARAMETERIZED_GATES else Gate(name, target=1, parameter=-np.pi/2)
+                    for name in one_qubit_gate_names.pop(5)[:-1]]
 two_qubit_gate_names = ["CNOT", "CX", "CY", "CZ", "CPHASE", "CRZ"]
+clifford_two_qubit_gate_names = ["CNOT", "CX", "CY", "CZ"]
 two_qubit_gates = [Gate(name, target=1, control=0) if name not in PARAMETERIZED_GATES
                    else Gate(name, target=1, control=0, parameter=0.5) for name in two_qubit_gate_names]
+clifford_two_qubit_gates = [Gate(name, target=1, control=0) for name in clifford_two_qubit_gate_names]
 swap_gates = [Gate('SWAP', target=[1, 0]), Gate('CSWAP', target=[1, 2], control=0)]
 big_circuit = Circuit(init_gates + one_qubit_gates + two_qubit_gates + swap_gates + [Gate('XX', [0, 1], parameter=0.5)])
+clifford_big_circuit = Circuit(init_gates + clifford_one_qubit_gates + clifford_two_qubit_gates + [Gate('SWAP', target=[1, 0])])
 
 references = [0., 0.38205142 ** 2, 0., 0.59500984 ** 2, 0., 0.38205142 ** 2, 0., 0.59500984 ** 2]
 references_multi = [0., 0., 0., 0., 0., 0., 0., 1.]
 reference_big_lsq = [-0.29022980 + 0.20684454j, -0.34400320 + 0.12534970j,  0.21316957 + 0.23442923j,
                       0.15939614 + 0.15293439j, -0.36723378 + 0.29031223j, -0.04807413 + 0.0797184j,
                      -0.37427732 + 0.41885117j, -0.05511766 + 0.20825736j]
 reference_big_msq = [-0.29022979 + 0.20684454j, -0.36723376 + 0.29031221j,  0.21316958 + 0.23442923j,
                      -0.37427729 + 0.41885117j, -0.34400321 + 0.12534970j, -0.04807414 + 0.07971841j,
                       0.15939615 + 0.15293440j, -0.05511766 + 0.20825737j]
 
+clifford_ref = [0. + 0.j,  0.5+0.j,  0. - 0.5j, 0. + 0.j,  0. + 0.j,  0.5 + 0.j,  0. - 0.5j, 0. + 0.j]
+
 abs_circ_mixed = Circuit(gates) + Circuit([Gate("RX", 1, parameter=1.5), Gate("MEASURE", 0)])
 
 
 class TranslateCircuitTest(unittest.TestCase):
 
     @unittest.skipIf("qulacs" not in installed_backends, "Test Skipped: Backend not available \n")
     def test_qulacs(self):
         """
             Compares the results of a simulation with Qulacs using a qulacs circuit directly
             VS one obtained through translation from an abstract format
         """
         import qulacs
 
-        # Generates the qulacs circuit by translating from the abstract one
+        # Test 1: Simulation of trasnlated circuit VS native circuit
+        # Generates the qulacs circuit by translating from the abstract one, run the simulation afterwards
         translated_circuit = translate_c(abs_circ, "qulacs")
-
-        # Run the simulation
         state1 = qulacs.QuantumState(abs_circ.width)
         translated_circuit.update_quantum_state(state1)
 
         # Directly define the same circuit through qulacs
         # NB: this includes convention fixes for some parametrized rotation gates (-theta instead of theta)
         qulacs_circuit = qulacs.QuantumCircuit(3)
         qulacs_circuit.add_H_gate(2)
         qulacs_circuit.add_CNOT_gate(0, 1)
         qulacs_circuit.add_CNOT_gate(1, 2)
         qulacs_circuit.add_Y_gate(0)
         qulacs_circuit.add_S_gate(0)
         qulacs_circuit.add_RX_gate(1, -2.)  # Convention: sign of theta
 
-        # Run the simulation
+        # Run the simulation of the native qulacs circuit, assert state vectors are identical
         state2 = qulacs.QuantumState(abs_circ.width)
         qulacs_circuit.update_quantum_state(state2)
 
-        # Assert that both simulations returned the same state vector
         np.testing.assert_array_equal(state1.get_vector(), state2.get_vector())
 
-        # Generates the qulacs circuit by translating from the abstract one
+        # Test 2: Multi-controlled CNOT and multi-controlled X test
         translated_circuit = translate_c(abs_multi_circ, "qulacs")
-
-        # Run the simulation
         state1 = qulacs.QuantumState(abs_multi_circ.width)
         translated_circuit.update_quantum_state(state1)
+        translated_circuit = translate_c(abs_multi_circ2, "qulacs")
+        state1b = qulacs.QuantumState(abs_multi_circ2.width)
+        translated_circuit.update_quantum_state(state1b)
 
-        # Directly define the same circuit through qulacs
-        # NB: this includes convention fixes for some parametrized rotation gates (-theta instead of theta)
+        # Test against native circuit
         qulacs_circuit = qulacs.QuantumCircuit(3)
         qulacs_circuit.add_X_gate(0)
         qulacs_circuit.add_X_gate(1)
         mat_gate = qulacs.gate.to_matrix_gate(qulacs.gate.X(2))
         mat_gate.add_control_qubit(0, 1)
         mat_gate.add_control_qubit(1, 1)
         qulacs_circuit.add_gate(mat_gate)
 
-        # Run the simulation
+        # Run, assert state vectors are equal.
         state2 = qulacs.QuantumState(abs_multi_circ.width)
         qulacs_circuit.update_quantum_state(state2)
-
-        # Assert that both simulations returned the same state vector
         np.testing.assert_array_equal(state1.get_vector(), state2.get_vector())
+        np.testing.assert_array_equal(state1b.get_vector(), state2.get_vector())
 
-        # Test that the translated circuit reports the same result for all cross-supported gates
+        # Test 3: translated circuit reports the same result for all cross-supported gates
         translated_circuit = translate_c(big_circuit, "qulacs")
-
-        # Run the simulation
         state1 = qulacs.QuantumState(big_circuit.width)
         translated_circuit.update_quantum_state(state1)
         np.testing.assert_array_almost_equal(state1.get_vector(), reference_big_msq, decimal=6)
 
     @unittest.skipIf("qiskit" not in installed_backends, "Test Skipped: Backend not available \n")
     def test_qiskit(self):
         """
             Compares the results of a simulation with Qiskit using a qiskit circuit directly
             VS one obtained through translation from an abstract format
         """
 
         import qiskit
-        from qiskit.providers.aer import AerSimulator
+        from qiskit_aer import AerSimulator
 
         # Generate the qiskit circuit by translating from the abstract one and print it
         translated_circuit = translate_c(abs_circ, "qiskit")
 
         # Generate the qiskit circuit directly and print it
         circ = qiskit.QuantumCircuit(3, 3)
         circ.h(2)
@@ -162,28 +169,14 @@
 
         # Return error when attempting to use qiskit with multiple controls
         self.assertRaises(ValueError, translate_c, abs_multi_circ, "qiskit")
 
         # Generate the qiskit circuit by translating from the abstract one and print it
         translated_circuit = translate_c(big_circuit, "qiskit")
 
-        # Big translate/translate back test (32000 gates)
-        very_big_circuit = big_circuit*10**3
-        tstart1 = time.time()
-        qc_very_big_circuit = translate_c(very_big_circuit, "qiskit")
-        tstop1 = time.time()
-        print(f"Circuit -> QuantumCircuit took {tstop1-tstart1:.2f} s")
-
-        tstart2 = time.time()
-        c_very_big_circuit = translate_c(qc_very_big_circuit, "tangelo", source="qiskit")
-        tstop2 = time.time()
-        print(f"QuantumCircuit -> Circuit took {tstop2-tstart2:.2f} s")
-
-        self.assertEqual(c_very_big_circuit, very_big_circuit)
-
         # Simulate both circuits, assert state vectors are equal
         qiskit_simulator = AerSimulator(method="statevector")
         translated_circuit = qiskit.transpile(translated_circuit, qiskit_simulator)
         translated_circuit.save_statevector()
         sim_results = qiskit_simulator.run(translated_circuit).result()
         np.testing.assert_array_almost_equal(sim_results.get_statevector(translated_circuit), reference_big_msq, decimal=6)
 
@@ -192,55 +185,58 @@
         """
             Compares the results of a simulation with cirq using a cirq circuit directly
             VS one obtained through translation from an abstract format
         """
 
         import cirq
 
-        # Generate the qiskit circuit by translating from the abstract one and print it
+        # Translated circuit
         translated_circuit = translate_c(abs_circ, "cirq")
 
-        # Generate the cirq circuit directly and print it
+        # Native circuit
         qubit_labels = cirq.LineQubit.range(3)
         circ = cirq.Circuit()
         circ.append(cirq.H(qubit_labels[2]))
         circ.append(cirq.CNOT(qubit_labels[0], qubit_labels[1]))
         circ.append(cirq.CNOT(qubit_labels[1], qubit_labels[2]))
         circ.append(cirq.Y(qubit_labels[0]))
         circ.append(cirq.S(qubit_labels[0]))
         gate_rx = cirq.rx(2.)
         circ.append(gate_rx(qubit_labels[1]))
 
         # Simulate both circuits, assert state vectors are equal
         cirq_simulator = cirq.Simulator()
-
         job_sim = cirq_simulator.simulate(circ)
         v1 = job_sim.final_state_vector
-
         job_sim = cirq_simulator.simulate(translated_circuit)
         v2 = job_sim.final_state_vector
-
         np.testing.assert_array_equal(v1, v2)
 
+        # Test 2: multi-controlled gates
         translated_circuit = translate_c(abs_multi_circ, "cirq")
         circ = cirq.Circuit()
         circ.append(cirq.X(qubit_labels[0]))
         circ.append(cirq.X(qubit_labels[1]))
         next_gate = cirq.X.controlled(num_controls=2)
         circ.append(next_gate(qubit_labels[0], qubit_labels[1], qubit_labels[2]))
 
         job_sim = cirq_simulator.simulate(circ)
         v1 = job_sim.final_state_vector
-
         job_sim = cirq_simulator.simulate(translated_circuit)
         v2 = job_sim.final_state_vector
+        np.testing.assert_array_equal(v1, v2)
 
+        # Test 3: multi-controlled CNOT turn into multi-controlled X
+        # The same statevector is expected.
+        translated_circuit2 = translate_c(abs_multi_circ2, "cirq")
+        job_sim = cirq_simulator.simulate(translated_circuit2)
+        v2 = job_sim.final_state_vector
         np.testing.assert_array_equal(v1, v2)
 
-        # Test that translated circuit is correct for all cross-supported gates
+        # Test 4: translated circuit must be correct for all cross-supported gates
         translated_circuit = translate_c(big_circuit, "cirq")
         job_sim = cirq_simulator.simulate(translated_circuit)
         np.testing.assert_array_almost_equal(job_sim.final_state_vector, reference_big_lsq, decimal=6)
 
     @unittest.skipIf("qdk" not in installed_backends, "Test Skipped: Backend not available \n")
     def test_qdk(self):
         """ Compares the frequencies computed by the QDK/Q# shot-based simulator to the theoretical ones """
@@ -266,14 +262,18 @@
         # Compares with theoretical probabilities obtained through a statevector simulator
         np.testing.assert_almost_equal(np.array(probabilities), np.array(references), 2)
 
         # Generate the qdk circuit by translating from the abstract one and print it
         translated_circuit = translate_c(abs_multi_circ, "qdk")
         print(translated_circuit)
 
+        # Check that multi-controlled CNOT is changed correctly to multi-controlled "CX"
+        translated_circuit2 = translate_c(abs_multi_circ2, "qdk")
+        self.assertEqual(translated_circuit, translated_circuit2)
+
         # Write to file
         with open('tmp_circuit.qs', 'w+') as f_out:
             f_out.write(translated_circuit)
 
         # Compile all qsharp files found in directory and import the qsharp operation
         import qsharp
         qsharp.reload()
@@ -497,10 +497,57 @@
             return qml.state()
 
         v1 = circuit(translated_circuit)
 
         # Compare statevectors
         np.testing.assert_array_almost_equal(v1, reference_big_lsq, decimal=6)
 
+    @unittest.skipIf("sympy" not in installed_backends, "Test Skipped: Sympy backend not available \n")
+    def test_to_sympy(self):
+        """Translate abtract format to sympy format."""
+
+        from sympy.physics.quantum.gate import HadamardGate, XGate, YGate, ZGate, CNotGate
+
+        # Equivalent native sympy circuit.
+        ref_circ = ZGate(3) * YGate(1) * XGate(0) * CNotGate(0, 1) * HadamardGate(2)
+
+        gates = [Gate("H", 2), Gate("CNOT", 1, control=0), Gate("X", 0), Gate("Y", 1), Gate("Z", 3)]
+        abs_circ = Circuit(gates)
+
+        # Generate the sympy circuit by translating from the abstract one.
+        translated_circuit = translate_c(abs_circ, "sympy")
+
+        self.assertEqual(translated_circuit, ref_circ)
+
+    @unittest.skipIf("stim" not in installed_backends, "Test Skipped: Backend not available \n")
+    def test_stim_translate(self):
+        """ Compares stim translated circuit with one made directly with stim"""
+
+        import stim
+        # Create stim circuit from Tangelo circuit
+        translated_circuit = translate_c(clifford_abs_circ, "stim")
+        # Assert against native equivalent stim circuit
+        circ = stim.Circuit()
+        for qubit in range(clifford_abs_circ.width):
+            circ.append("I", [qubit])
+        circ.append("H", [2])
+        circ.append("CNOT", [0, 1])
+        circ.append("CNOT", [1, 2])
+        circ.append("Y", [0])
+        circ.append("S", [0])
+        circ.append("S_DAG", [1])
+        circ.append("H", [1])
+        circ.append("S_DAG", [1])
+        assert(circ == translated_circuit)
+
+    @unittest.skipIf("stim" not in installed_backends, "Test Skipped: Backend not available \n")
+    def test_stim_tableau(self):
+        """ Compares stim statevector produced by tableau with reference state"""
+
+        from tangelo.linq.translator.translate_stim import translate_tableau
+        # Get statevector from tableau
+        v1 = translate_tableau(clifford_big_circuit).state_vector()
+        np.testing.assert_array_almost_equal(v1, clifford_ref, decimal=6)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/tests/test_translator_qubitop.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_qubitop.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,26 +45,26 @@
         with self.assertRaises(NotImplementedError):
             translate_operator(tangelo_op, source="tangelo", target="targetnotsupported")
 
     @unittest.skipIf("qiskit" not in installed_backends, "Test Skipped: Qiskit not available \n")
     def test_qiskit_to_tangelo(self):
         """Test translation from a qiskit to a tangelo operator."""
 
-        from qiskit.opflow.primitive_ops import PauliSumOp
-        qiskit_op = PauliSumOp.from_list([("ZYX", 2.), ("III", 3.)])
+        from qiskit.quantum_info.operators import SparsePauliOp
+        qiskit_op = SparsePauliOp.from_list([("ZYX", 2.), ("III", 3.)])
 
         test_op = translate_operator(qiskit_op, source="qiskit", target="tangelo")
         self.assertEqual(test_op, tangelo_op)
 
     @unittest.skipIf("qiskit" not in installed_backends, "Test Skipped: Qiskit not available \n")
     def test_tangelo_to_qiskit(self):
         """Test translation from a tangelo to a qiskit operator."""
 
-        from qiskit.opflow.primitive_ops import PauliSumOp
-        qiskit_op = PauliSumOp.from_list([("ZYX", 2.), ("III", 3.)])
+        from qiskit.quantum_info.operators import SparsePauliOp
+        qiskit_op = SparsePauliOp.from_list([("ZYX", 2.), ("III", 3.)])
 
         test_op = translate_operator(tangelo_op, source="tangelo", target="qiskit")
         self.assertEqual(qiskit_op, test_op)
 
     @unittest.skipIf("cirq" not in installed_backends, "Test Skipped: Cirq not available \n")
     def test_cirq_to_tangelo(self):
         """Test translation from a cirq to a tangelo operator."""
@@ -181,48 +181,19 @@
 
         self.assertEqual(projectq_op, test_op)
 
     @unittest.skipIf("qiskit" not in installed_backends, "Test Skipped: Qiskit not available \n")
     def test_tangelo_to_qiskit_H2_eigenvalues(self):
         """Test eigenvalues resulting from a tangelo to qiskit translation."""
 
-        from qiskit.algorithms import NumPyEigensolver
-
         qu_op = load_operator("H2_JW_occfirst.data", data_directory=pwd_this_test+"/data", plain_text=True)
         test_op = translate_operator(qu_op, source="tangelo", target="qiskit")
 
         eigenvalues_tangelo = eigenspectrum(qu_op)
 
-        qiskit_solver = NumPyEigensolver(2**4)
-        eigenvalues_qiskit = qiskit_solver.compute_eigenvalues(test_op)
-
-        np.testing.assert_array_almost_equal(eigenvalues_tangelo, eigenvalues_qiskit.eigenvalues)
-
-    @unittest.skipIf("qiskit" not in installed_backends, "Test Skipped: Qiskit not available \n")
-    def test_tangelo_to_qiskit_big(self):
-        """Test translation from a tangelo to a qiskit operator, for a large input"""
-
-        n_qubits = 10
-        n_terms = 3**n_qubits
-
-        # Build large operator made of all possible "full" Pauli words (no 'I') of length n_qubits
-        terms = {tuple(zip(range(n_qubits), pw)): 1.0 for pw in product(['X', 'Y', 'Z'], repeat=n_qubits)}
-        q_op = QubitOperator()
-        q_op.terms = terms
-
-        s, t = "tangelo", "qiskit"
-        tstart1 = time.time()
-        tmp_op = translate_operator(q_op, source=s, target=t)
-        tstop1 = time.time()
-        print(f"Qubit operator conversion {s} to {t}: {tstop1 - tstart1:.1f} (terms = {n_terms})")
-
-        t, s = s, t
-        tstart2 = time.time()
-        q_op2 = translate_operator(tmp_op, source=s, target=t)
-        tstop2 = time.time()
-        print(f"Qubit operator conversion {s} to {t}: {tstop2 - tstart2:.1f} (terms = {n_terms})")
+        eigenvalues_qiskit = np.linalg.eigh(test_op.to_matrix(sparse=False))[0]
 
-        assert(q_op == q_op2)
+        np.testing.assert_array_almost_equal(eigenvalues_tangelo, eigenvalues_qiskit)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from tangelo.helpers.utils import installed_backends
 
-from .translate_braket import translate_braket, get_braket_gates
-from .translate_qiskit import translate_qiskit, get_qiskit_gates
-from .translate_qulacs import translate_qulacs, get_qulacs_gates
-from .translate_cirq import translate_cirq, get_cirq_gates
-from .translate_json_ionq import translate_json_ionq, get_ionq_gates
-from .translate_qdk import translate_qsharp, get_qdk_gates
-from .translate_projectq import translate_projectq, _translate_projectq2abs, get_projectq_gates
-from .translate_openqasm import translate_openqasm, _translate_openqasm2abs, get_openqasm_gates
+from .translate_braket import get_braket_gates
+from .translate_qiskit import get_qiskit_gates
+from .translate_qulacs import get_qulacs_gates
+from .translate_cirq import get_cirq_gates
+from .translate_json_ionq import get_ionq_gates
+from .translate_qdk import get_qdk_gates
+from .translate_projectq import get_projectq_gates
+from .translate_openqasm import get_openqasm_gates
+from .translate_pennylane import get_pennylane_gates
+from .translate_sympy import get_sympy_gates
 from .translate_qubitop import translate_operator
 from .translate_circuit import translate_circuit
-from .translate_pennylane import get_pennylane_gates
 
 
 def get_supported_gates():
     """List all supported gates for all backends found"""
 
     supported_gates = dict()
     supported_gates["projectq"] = sorted(get_projectq_gates().keys())
@@ -36,9 +37,10 @@
     supported_gates["qdk"] = sorted(get_qdk_gates().keys())
     supported_gates["openqasm"] = sorted(get_openqasm_gates().keys())
     supported_gates["qulacs"] = sorted(get_qulacs_gates().keys())
     supported_gates["qiskit"] = sorted(get_qiskit_gates().keys())
     supported_gates["cirq"] = sorted(get_cirq_gates().keys())
     supported_gates["braket"] = sorted(get_braket_gates().keys())
     supported_gates["pennylane"] = sorted(get_pennylane_gates().keys())
+    supported_gates["sympy"] = sorted(get_sympy_gates().keys())
 
     return supported_gates
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/qdk_template.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/qdk_template.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_braket.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_braket.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 to account for:
 - how the gate names differ between the source backend to the target backend.
 - how the order and conventions for some of the inputs to the gate operations
     may also differ.
 """
 
 from tangelo.linq import Circuit, Gate
-from tangelo.helpers import deprecated
 
 
 def get_braket_gates():
     """Map gate name of the abstract format to the equivalent methods of the
     braket.circuits.Circuit class API and supported gates:
     https://amazon-braket-sdk-python.readthedocs.io/en/latest/_apidoc/braket.circuits.circuit.html
     """
@@ -55,28 +54,14 @@
     GATE_BRAKET["SWAP"] = BraketCircuit.swap
     GATE_BRAKET["CSWAP"] = BraketCircuit.cswap
     # GATE_BRAKET["MEASURE"] = ? (mid-circuit measurement currently unsupported?)
 
     return GATE_BRAKET
 
 
-@deprecated("Please use the translate_circuit function.")
-def translate_braket(source_circuit):
-    """Take in an abstract circuit, return a quantum circuit object as defined
-    in the Python Braket SDK.
-
-    Args:
-        source_circuit: quantum circuit in the abstract format.
-
-    Returns:
-        braket.circuits.Circuit: quantum circuit in Python Braket SDK format.
-    """
-    return translate_c_to_braket(source_circuit)
-
-
 def translate_c_to_braket(source_circuit):
     """Take in an abstract circuit, return a quantum circuit object as defined
     in the Python Braket SDK.
 
     Args:
         source_circuit: quantum circuit in the abstract format.
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_circuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,29 @@
 from tangelo.linq.translator.translate_json_ionq import translate_c_to_json_ionq, translate_c_from_json_ionq
 from tangelo.linq.translator.translate_openqasm import translate_c_to_openqasm, translate_c_from_openqasm
 from tangelo.linq.translator.translate_projectq import translate_c_to_projectq, translate_c_from_projectq
 from tangelo.linq.translator.translate_qdk import translate_c_to_qsharp
 from tangelo.linq.translator.translate_qiskit import translate_c_to_qiskit, translate_c_from_qiskit
 from tangelo.linq.translator.translate_qulacs import translate_c_to_qulacs
 from tangelo.linq.translator.translate_pennylane import translate_c_to_pennylane
-
+from tangelo.linq.translator.translate_sympy import translate_c_to_sympy
+from tangelo.linq.translator.translate_stim import translate_c_to_stim
 
 FROM_TANGELO = {
     "braket": translate_c_to_braket,
     "cirq": translate_c_to_cirq,
     "ionq": translate_c_to_json_ionq,
     "openqasm": translate_c_to_openqasm,
     "projectq": translate_c_to_projectq,
     "qdk": translate_c_to_qsharp,
     "qiskit": translate_c_to_qiskit,
     "qulacs": translate_c_to_qulacs,
-    "pennylane": translate_c_to_pennylane
+    "pennylane": translate_c_to_pennylane,
+    "stim": translate_c_to_stim,
+    "sympy": translate_c_to_sympy
 }
 
 TO_TANGELO = {
     "braket": translate_c_from_braket,
     "ionq": translate_c_from_json_ionq,
     "openqasm": translate_c_from_openqasm,
     "projectq": translate_c_from_projectq,
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_cirq.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_cirq.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 - how the order and conventions for some of the inputs to the gate operations
     may also differ.
 """
 
 from math import pi
 
 from tangelo.toolboxes.operators import QubitOperator
-from tangelo.helpers import deprecated
 
 
 def get_cirq_gates():
     """Map gate name of the abstract format to the equivalent methods of the
     cirq class API and supported gates: https://quantumai.google/cirq/gates.
     """
     import cirq
@@ -39,14 +38,15 @@
     GATE_CIRQ["X"] = cirq.X
     GATE_CIRQ["Y"] = cirq.Y
     GATE_CIRQ["Z"] = cirq.Z
     GATE_CIRQ["CX"] = cirq.X
     GATE_CIRQ["CY"] = cirq.Y
     GATE_CIRQ["CZ"] = cirq.Z
     GATE_CIRQ["S"] = cirq.S
+    GATE_CIRQ["SDAG"] = cirq.ZPowGate(exponent=-0.5)
     GATE_CIRQ["T"] = cirq.T
     GATE_CIRQ["CH"] = cirq.H
     GATE_CIRQ["RX"] = cirq.rx
     GATE_CIRQ["RY"] = cirq.ry
     GATE_CIRQ["RZ"] = cirq.rz
     GATE_CIRQ["CNOT"] = cirq.CNOT
     GATE_CIRQ["CRZ"] = cirq.rz
@@ -57,30 +57,14 @@
     GATE_CIRQ["XX"] = cirq.XXPowGate
     GATE_CIRQ["SWAP"] = cirq.SWAP
     GATE_CIRQ["CSWAP"] = cirq.SWAP
     GATE_CIRQ["MEASURE"] = cirq.measure
     return GATE_CIRQ
 
 
-@deprecated("Please use the translate_circuit function.")
-def translate_cirq(source_circuit):
-    """Take in an abstract circuit, return an equivalent cirq QuantumCircuit
-    instance.
-
-    Args:
-        source_circuit: quantum circuit in the abstract format.
-
-    Returns:
-        cirq.Circuit: a corresponding cirq Circuit. Right now, the structure is
-            of LineQubit. It is possible in the future that we may support
-            NamedQubit or GridQubit.
-    """
-    return translate_c_to_cirq(source_circuit)
-
-
 def translate_c_to_cirq(source_circuit, noise_model=None, save_measurements=False):
     """Take in an abstract circuit, return an equivalent cirq QuantumCircuit
     object.
 
     Args:
         source_circuit (Circuit): quantum circuit in the abstract format.
         noise_model (NoiseModel): The noise model to use
@@ -104,18 +88,20 @@
     # cirq will otherwise only initialize qubits that have gates
     target_circuit.append(cirq.I.on_each(qubit_list))
 
     measure_count = 0
 
     # Maps the gate information properly. Different for each backend (order, values)
     for gate in source_circuit._gates:
-        if (gate.control is not None) and gate.name != 'CNOT':
+        if gate.control is not None:
             num_controls = len(gate.control)
             control_list = [qubit_list[c] for c in gate.control]
-        if gate.name in {"H", "X", "Y", "Z", "S", "T"}:
+            if gate.name == 'CNOT' and num_controls > 1:
+                gate.name = 'CX'
+        if gate.name in {"H", "X", "Y", "Z", "S", "SDAG", "T"}:
             target_circuit.append(GATE_CIRQ[gate.name](qubit_list[gate.target[0]]))
         elif gate.name in {"CH", "CX", "CY", "CZ"}:
             next_gate = GATE_CIRQ[gate.name].controlled(num_controls)
             target_circuit.append(next_gate(*control_list, qubit_list[gate.target[0]]))
         elif gate.name in {"RX", "RY", "RZ"}:
             next_gate = GATE_CIRQ[gate.name](gate.parameter)
             target_circuit.append(next_gate(qubit_list[gate.target[0]]))
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_json_ionq.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_json_ionq.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 necessary to account for:
 - how the gate names differ between the source backend to the target backend.
 - how the order and conventions for some of the inputs to the gate operations
     may also differ.
 """
 
 from tangelo.linq import Circuit, Gate
-from tangelo.helpers import deprecated
 
 
 def get_ionq_gates():
     """Map gate name of the abstract format to the equivalent gate name used in
     the json IonQ format. For more information:
     - https://dewdrop.ionq.co/
     - https://docs.ionq.co
@@ -42,30 +41,14 @@
         GATE_JSON_IONQ[name] = name[1:].lower()
     GATE_JSON_IONQ["CNOT"] = "x"
     GATE_JSON_IONQ["PHASE"] = "z"
     GATE_JSON_IONQ["CPHASE"] = "z"
     return GATE_JSON_IONQ
 
 
-@deprecated("Please use the translate_circuit function.")
-def translate_json_ionq(source_circuit):
-    """Take in an abstract circuit, return a dictionary following the IonQ JSON
-    format as described below.
-    https://dewdrop.ionq.co/#json-specification
-
-    Args:
-        source_circuit: quantum circuit in the abstract format.
-
-    Returns:
-        dict: representation of the quantum circuit following the IonQ JSON
-            format.
-    """
-    return translate_c_to_json_ionq(source_circuit)
-
-
 def translate_c_to_json_ionq(source_circuit):
     """Take in an abstract circuit, return a dictionary following the IonQ JSON
     format as described below.
     https://dewdrop.ionq.co/#json-specification
 
     Args:
         source_circuit: quantum circuit in the abstract format.
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_openqasm.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_openqasm.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,20 +23,19 @@
     may also differ.
 """
 
 import re
 from math import pi
 
 from tangelo.linq import Gate, Circuit
-from tangelo.helpers import deprecated
 
 
 def get_openqasm_gates():
     """Map gate name of the abstract format to the equivalent gate name used in
-    openqasm OpenQASM is a general format that allows users to express a quantum
+    OpenQASM. OpenQASM is a general format that allows users to express a quantum
     program, define conditional operations manipulating quantum and qubit
     registers, as well as defining new quantum unitaries. We however make the
     choice here to support well-known gate operations.
     """
 
     GATE_OPENQASM = dict()
     for name in {"H", "X", "Y", "Z", "S", "T", "RX", "RY", "RZ", "MEASURE",
@@ -45,50 +44,14 @@
     GATE_OPENQASM["CNOT"] = "cx"
     GATE_OPENQASM["PHASE"] = "p"
     GATE_OPENQASM["CPHASE"] = "cp"
 
     return GATE_OPENQASM
 
 
-@deprecated("Please use the translate_circuit function.")
-def translate_openqasm(source_circuit):
-    """Take in an abstract circuit, return a OpenQASM 2.0 string using IBM
-    Qiskit (they are the reference for OpenQASM).
-
-    Args:
-        source_circuit: quantum circuit in the abstract format.
-
-    Returns:
-        str: the corresponding OpenQASM program, as per IBM Qiskit.
-    """
-    return translate_c_to_openqasm(source_circuit)
-
-
-@deprecated("Please use the translate_circuit function.")
-def _translate_openqasm2abs(source_circuit):
-    """Take an OpenQASM 2.0 string as input (as defined by IBM Qiskit), return
-    the equivalent abstract circuit. Only a subset of OpenQASM supported, mostly
-    to be able to go back and forth QASM and abstract representations to
-    leverage tools and innovation implemented to work in the QASM format. Not
-    designed to support elaborate QASM programs defining their own operations.
-    Compatible with qiskit.QuantumCircuit.from_qasm method.
-
-    Assumes single-qubit measurement instructions only. Final qubit register
-    measurement is implicit.
-
-    Args:
-        openqasm_string(str): an OpenQASM program, as a string, as defined by
-            IBM Qiskit.
-
-    Returns:
-        Circuit: corresponding quantum circuit in the abstract format.
-    """
-    return translate_c_from_openqasm(source_circuit)
-
-
 def translate_c_to_openqasm(source_circuit):
     """Take in an abstract circuit, return a OpenQASM 2.0 string using IBM
     Qiskit (they are the reference for OpenQASM).
 
     Args:
         source_circuit: quantum circuit in the abstract format.
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_pennylane.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_pennylane.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_projectq.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_projectq.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     may also differ.
 """
 
 import re
 
 from tangelo.linq import Gate, Circuit
 from tangelo.toolboxes.operators import QubitOperator
-from tangelo.helpers import deprecated
 
 
 def get_projectq_gates():
     """Map gate name of the abstract format to the equivalent gate name used in
     projectq API and supported gates:
     https://projectq.readthedocs.io/en/latest/projectq.ops.html
     """
@@ -42,47 +41,14 @@
         GATE_PROJECTQ[name] = name[0] + name[1:].lower()
     GATE_PROJECTQ["CNOT"] = "CX"
     GATE_PROJECTQ["PHASE"] = "R"
 
     return GATE_PROJECTQ
 
 
-@deprecated("Please use the translate_circuit function.")
-def translate_projectq(source_circuit):
-    """Take in an abstract circuit, return a string containing equivalent
-    projectq instructions.
-
-    Args:
-        source_circuit: quantum circuit in the abstract format.
-
-    Returns:
-        str: the corresponding projectq instructions (allocation , gates,
-            deallocation).
-    """
-    return translate_c_to_projectq(source_circuit)
-
-
-@deprecated("Please use the translate_circuit function.")
-def _translate_projectq2abs(projectq_str):
-    """Convenience function to help people move away from their ProjectQ
-    workflow. Take ProjectQ instructions, expressed as a string, similar to one
-    from the ProjectQ `CommandPrinter` engine. Will bundle all qubit allocation
-    (resp. deallocation) at the beginning (resp. end) of the circuit. Example
-    available in the `examples` folder.
-
-    Args:
-        projectq_str(str): ProjectQ program, as a string (Allocate, Deallocate,
-            gate operations...).
-
-    Returns:
-        Circuit: corresponding quantum circuit in the abstract format.
-    """
-    return translate_c_from_projectq(projectq_str)
-
-
 def translate_c_to_projectq(source_circuit):
     """Take in an abstract circuit, return a string containing equivalent
     projectq instructions.
 
     Args:
         source_circuit: quantum circuit in the abstract format.
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_qdk.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 In order to produce an equivalent circuit for the target backend, it is
 necessary to account for:
 - how the gate names differ between the source backend to the target backend.
 - how the order and conventions for some of the inputs to the gate operations
     may also differ.
 """
 
-from tangelo.helpers import deprecated
-
 
 def get_qdk_gates():
     """Map gate name of the abstract format to the equivalent gate name used in
     Q# operations API and supported gates:
     https://docs.microsoft.com/en-us/qsharp/api/qsharp/microsoft.quantum.intrinsic
     """
 
@@ -44,30 +42,14 @@
         GATE_QDK[name] = name[1:]
     GATE_QDK["SWAP"] = "SWAP"
     GATE_QDK["MEASURE"] = "M"
 
     return GATE_QDK
 
 
-@deprecated("Please use the translate_circuit function.")
-def translate_qsharp(source_circuit):
-    """Take in an abstract circuit, generate the corresponding Q# operation
-    (state prep + measurement) string, in the appropriate Q# template. The Q#
-    output can be written to file and will be compiled at runtime.
-
-    Args:
-        source_circuit: quantum circuit in the abstract format.
-
-    Returns:
-        str: The Q# code (operation + template). This needs to be written into a
-            .qs file, and compiled at runtime.
-    """
-    return translate_c_to_qsharp(source_circuit)
-
-
 def translate_c_to_qsharp(source_circuit, operation="MyQsharpOperation", save_measurements=False):
     """Take in an abstract circuit, generate the corresponding Q# operation
     (state prep + measurement) string, in the appropriate Q# template. The Q#
     output can be written to file and will be compiled at runtime.
 
     Args:
         source_circuit: quantum circuit in the abstract format.
@@ -93,19 +75,21 @@
 #    qsharp_string += "body (...) {\n\n"
     qsharp_string += f"\tmutable c = new Result[{n_c}];\n"
     qsharp_string += f"\tusing (qreg = Qubit[{source_circuit.width}]) {{\n"
 
     # Generate Q# strings with the right syntax, order and values for the gate inputs
     body_str = ""
     for gate in source_circuit._gates:
-        if gate.control is not None and gate.name != "CNOT":
+        if gate.control is not None:
             control_string = '['
             num_controls = len(gate.control)
             for i, c in enumerate(gate.control):
                 control_string += f'qreg[{c}]]' if i == num_controls - 1 else f'qreg[{c}], '
+            if num_controls > 1 and gate.name == 'CNOT':
+                gate.name = 'CX'
 
         if gate.name in {"H", "X", "Y", "Z", "S", "T"}:
             body_str += f"\t\t{GATE_QDK[gate.name]}(qreg[{gate.target[0]}]);\n"
         elif gate.name in {"RX", "RY", "RZ", "PHASE"}:
             body_str += f"\t\t{GATE_QDK[gate.name]}({gate.parameter}, qreg[{gate.target[0]}]);\n"
         elif gate.name in {"CNOT"}:
             body_str += f"\t\t{GATE_QDK[gate.name]}(qreg[{gate.control[0]}], qreg[{gate.target[0]}]);\n"
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_qiskit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qiskit.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 The module also enables bidirectional conversion between qiskit and Tangelo
 qubit operators (linear combination of Pauli operators)
 """
 
 from tangelo.linq import Circuit, Gate
 from tangelo.toolboxes.operators import QubitOperator
 from tangelo.linq.helpers import pauli_of_to_string, pauli_string_to_of
-from tangelo.helpers import deprecated
 
 
 def get_qiskit_gates():
     """Map gate name of the Tangelo format to the equivalent add_gate method of
     Qiskit's QuantumCircuit class API and supported gates:
     https://qiskit.org/documentation/stubs/qiskit.circuit.QuantumCircuit.html
     """
@@ -62,27 +61,14 @@
     GATE_QISKIT["CSWAP"] = qiskit.QuantumCircuit.cswap
     GATE_QISKIT["PHASE"] = qiskit.QuantumCircuit.p
     GATE_QISKIT["CPHASE"] = qiskit.QuantumCircuit.cp
     GATE_QISKIT["MEASURE"] = qiskit.QuantumCircuit.measure
     return GATE_QISKIT
 
 
-@deprecated("Please use the translate_circuit function.")
-def translate_qiskit(source_circuit):
-    """Take in a Circuit, return an equivalent qiskit.QuantumCircuit
-
-    Args:
-        source_circuit (Circuit): quantum circuit in the Tangelo format.
-
-    Returns:
-        qiskit.QuantumCircuit: the corresponding quantum circuit in Qiskit format.
-    """
-    return translate_c_to_qiskit(source_circuit)
-
-
 def translate_c_to_qiskit(source_circuit: Circuit, save_measurements=False):
     """Take in a Circuit, return an equivalent qiskit.QuantumCircuit
 
     Args:
         source_circuit (Circuit): quantum circuit in the abstract format.
         save_measurements (bool): Return mid-circuit measurements in the order
             they appear in the circuit in the classical registers
@@ -168,55 +154,55 @@
     target_circuit = Circuit(gates)
 
     return target_circuit
 
 
 def translate_op_to_qiskit(qubit_operator, n_qubits):
     """Helper function to translate a Tangelo QubitOperator to a qiskit
-    PauliSumOp. Qiskit must be installed for the function to work.
+    SparsePauliOp. Qiskit must be installed for the function to work.
 
     Args:
         qubit_operator (tangelo.toolboxes.operators.QubitOperator): Self-explanatory.
         n_qubits (int): Number of qubits relevant to the operator.
 
     Returns:
-        (qiskit.opflow.primitive_ops.PauliSumOp): Qiskit qubit operator.
+        (qiskit.quantum_info.operators.SparsePauliOp): Qiskit qubit operator.
     """
 
     # Import qiskit qubit operator.
-    from qiskit.opflow.primitive_ops import PauliSumOp
+    from qiskit.quantum_info.operators import SparsePauliOp
 
     # Convert each term sequencially.
     term_list = list()
     for term_tuple, coeff in qubit_operator.terms.items():
         term_string = pauli_of_to_string(term_tuple, n_qubits)
 
         # Reverse the string because of qiskit convention.
         term_list += [(term_string[::-1], coeff)]
 
-    return PauliSumOp.from_list(term_list)
+    return SparsePauliOp.from_list(term_list)
 
 
 def translate_op_from_qiskit(qubit_operator):
-    """Helper function to translate a qiskit PauliSumOp to a Tangelo
+    """Helper function to translate a qiskit SparsePauliOp to a Tangelo
     QubitOperator.
 
     Args:
-        qubit_operator (qiskit.opflow.primitive_ops.PauliSumOp): Self-explanatory.
+        qubit_operator (qiskit.quantum_info.operators.SparsePauliOp): Self-explanatory.
 
     Returns:
         (tangelo.toolboxes.operators.QubitOperator): Tangelo qubit operator.
     """
 
     # Create a dictionary to append all terms at once.
     terms_dict = dict()
-    for pauli_word in qubit_operator:
+    terms = qubit_operator.to_list()
+    for term_string, coeff in terms:
         # Inversion of the string because of qiskit ordering.
-        term_string = pauli_word.to_pauli_op().primitive.to_label()[::-1]
-        term_tuple = pauli_string_to_of(term_string)
-        terms_dict[tuple(term_tuple)] = complex(pauli_word.coeffs)
+        term_tuple = pauli_string_to_of(term_string[::-1])
+        terms_dict[tuple(term_tuple)] = coeff
 
     # Create and copy the information into a new QubitOperator.
     tangelo_op = QubitOperator()
     tangelo_op.terms = terms_dict
 
     return tangelo_op
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_qubitop.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qubitop.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 
 from tangelo.toolboxes.operators import count_qubits, QubitOperator
 from tangelo.linq.translator.translate_qiskit import translate_op_from_qiskit, translate_op_to_qiskit
 from tangelo.linq.translator.translate_cirq import translate_op_from_cirq, translate_op_to_cirq
 from tangelo.linq.translator.translate_qulacs import translate_op_from_qulacs, translate_op_to_qulacs
 from tangelo.linq.translator.translate_pennylane import translate_op_from_pennylane, translate_op_to_pennylane
 from tangelo.linq.translator.translate_projectq import translate_op_from_projectq, translate_op_to_projectq
+from tangelo.linq.translator.translate_sympy import translate_op_to_sympy
 
 
 FROM_TANGELO = {
     "qiskit": translate_op_to_qiskit,
     "cirq": translate_op_to_cirq,
     "qulacs": translate_op_to_qulacs,
     "pennylane": translate_op_to_pennylane,
-    "projectq": translate_op_to_projectq
+    "projectq": translate_op_to_projectq,
+    "sympy": translate_op_to_sympy
 }
 
 TO_TANGELO = {
     "qiskit": translate_op_from_qiskit,
     "cirq": translate_op_from_cirq,
     "qulacs": translate_op_from_qulacs,
     "pennylane": translate_op_from_pennylane,
@@ -67,18 +69,18 @@
         qubit_operator = TO_TANGELO[source](qubit_operator)
 
     if target != "tangelo":
         if target not in FROM_TANGELO:
             raise NotImplementedError(f"Qubit operator conversion from {source} to {target} is not supported.")
 
         # For translation functions that need an explicit number of qubits.
-        if target in {"qiskit"}:
+        if target in {"qiskit", "sympy"}:
             # The count_qubits function has no way to detect the number of
             # qubits when an operator is only a tensor product of I.
-            if qubit_operator == QubitOperator((), qubit_operator.constant):
+            if qubit_operator == QubitOperator((), qubit_operator.constant) and n_qubits is None:
                 raise ValueError("The number of qubits (n_qubits) must be provided.")
             n_qubits = count_qubits(qubit_operator) if n_qubits is None else n_qubits
             qubit_operator = FROM_TANGELO[target](qubit_operator, n_qubits)
         else:
             qubit_operator = FROM_TANGELO[target](qubit_operator)
 
     return qubit_operator
```

### Comparing `tangelo-gc-0.3.4/tangelo/linq/translator/translate_qulacs.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qulacs.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 - how the order and conventions for some of the inputs to the gate operations
     may also differ.
 """
 
 from numpy import exp, cos, sin
 
 from tangelo.toolboxes.operators import QubitOperator
-from tangelo.helpers import deprecated
 
 
 def get_qulacs_gates():
     """Map gate name of the abstract format to the equivalent add_gate method of
     Qulacs's QuantumCircuit class API and supported gates:
     http://qulacs.org/class_quantum_circuit.html
     """
@@ -58,32 +57,14 @@
     GATE_QULACS["XX"] = qulacs.gate.DenseMatrix
     GATE_QULACS["SWAP"] = qulacs.QuantumCircuit.add_SWAP_gate
     GATE_QULACS["CSWAP"] = qulacs.gate.SWAP
     GATE_QULACS["MEASURE"] = qulacs.gate.Measurement
     return GATE_QULACS
 
 
-@deprecated("Please use the translate_circuit function.")
-def translate_qulacs(source_circuit, noise_model=None):
-    """Take in an abstract circuit, return an equivalent qulacs QuantumCircuit
-    instance. If provided with a noise model, will add noisy gates at
-    translation. Not very useful to look at, as qulacs does not provide much
-    information about the noisy gates added when printing the "noisy circuit".
-
-    Args:
-        source_circuit: quantum circuit in the abstract format.
-        noise_model: A NoiseModel object from this package, located in the
-            noisy_simulation subpackage.
-
-    Returns:
-        qulacs.QuantumCircuit: the corresponding qulacs quantum circuit.
-    """
-    return translate_c_to_qulacs(source_circuit, noise_model)
-
-
 def translate_c_to_qulacs(source_circuit, noise_model=None, save_measurements=False):
     """Take in an abstract circuit, return an equivalent qulacs QuantumCircuit
     instance. If provided with a noise model, will add noisy gates at
     translation. Not very useful to look at, as qulacs does not provide much
     information about the noisy gates added when printing the "noisy circuit".
 
     Args:
@@ -104,14 +85,16 @@
     GATE_QULACS = get_qulacs_gates()
     target_circuit = qulacs.QuantumCircuit(source_circuit.width)
 
     measure_count = 0
 
     # Maps the gate information properly. Different for each backend (order, values)
     for gate in source_circuit._gates:
+        if gate.name == 'CNOT' and len(gate.control) > 1:
+            gate.name = 'CX'
         if gate.name in {"H", "X", "Y", "Z", "S", "T"}:
             (GATE_QULACS[gate.name])(target_circuit, gate.target[0])
         elif gate.name in {"CH", "CX", "CY", "CZ"}:
             mat_gate = qulacs.gate.to_matrix_gate(GATE_QULACS[gate.name](gate.target[0]))
             for c in gate.control:
                 mat_gate.add_control_qubit(c, 1)
             target_circuit.add_gate(mat_gate)
```

### Comparing `tangelo-gc-0.3.4/tangelo/molecule_library.py` & `tangelo-gc-0.4.0rc0/tangelo/molecule_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Module to create some molecules used in the package unittest."""
 
 
 from tangelo import Molecule, SecondQuantizedMolecule
+from tangelo.helpers.utils import is_package_installed
 
+has_pyscf = is_package_installed("pyscf")
 
 # Dihydrogen.
 xyz_H2 = [
     ("H", (0., 0., 0.)),
     ("H", (0., 0., 0.7414))
 ]
 mol_H2_sto3g = SecondQuantizedMolecule(xyz_H2, q=0, spin=0, basis="sto-3g")
@@ -38,17 +40,17 @@
     ("H", [0.7071067811865476, 0.0, 0.0]),
     ("H", [0.0, 0.7071067811865476, 0.0]),
     ("H", [-1.0071067811865476, 0.0, 0.0]),
     ("H", [0.0, -1.0071067811865476, 0.0])
 ]
 mol_H4_sto3g = SecondQuantizedMolecule(xyz_H4, q=0, spin=0, basis="sto-3g")
 mol_H4_sto3g_symm = SecondQuantizedMolecule(xyz_H4, q=0, spin=0, basis="sto-3g", symmetry=True)
-mol_H4_minao = SecondQuantizedMolecule(xyz_H4, q=0, spin=0, basis="minao")
+mol_H4_minao = SecondQuantizedMolecule(xyz_H4, q=0, spin=0, basis="minao") if has_pyscf else None
 mol_H4_cation_sto3g = SecondQuantizedMolecule(xyz_H4, q=1, spin=1, basis="sto-3g")
-mol_H4_doublecation_minao = SecondQuantizedMolecule(xyz_H4, q=2, spin=0, basis="minao")
+mol_H4_doublecation_minao = SecondQuantizedMolecule(xyz_H4, q=2, spin=0, basis="minao") if has_pyscf else None
 mol_H4_doublecation_321g = SecondQuantizedMolecule(xyz_H4, q=2, spin=0, basis="3-21g")
 mol_H4_sto3g_uhf_a1_frozen = SecondQuantizedMolecule(xyz_H4, q=0, spin=0, basis="sto-3g", uhf=True, frozen_orbitals=[[1], []])
 
 # Decahydrogen.
 xyz_H10 = [
     ("H", ( 0.970820393250,  0.000000000000, 0.)),
     ("H", ( 0.785410196625,  0.570633909777, 0.)),
@@ -57,15 +59,15 @@
     ("H", (-0.785410196625,  0.570633909777, 0.)),
     ("H", (-0.970820393250,  0.000000000000, 0.)),
     ("H", (-0.785410196625, -0.570633909777, 0.)),
     ("H", (-0.300000000000, -0.923305061153, 0.)),
     ("H", ( 0.300000000000, -0.923305061153, 0.)),
     ("H", ( 0.785410196625, -0.570633909777, 0.))
 ]
-mol_H10_minao = SecondQuantizedMolecule(xyz_H10, q=0, spin=0, basis="minao")
+mol_H10_minao = SecondQuantizedMolecule(xyz_H10, q=0, spin=0, basis="minao") if has_pyscf else None
 mol_H10_321g = SecondQuantizedMolecule(xyz_H10, q=0, spin=0, basis="3-21g")
 
 
 # Water.
 xyz_H2O = [
     ("O", (0., 0., 0.11779)),
     ("H", (0., 0.75545, -0.47116)),
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .dmet_problem_decomposition import Localization
+from ._helpers.helper_classes import Fragment, Link
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,39 +17,48 @@
 The construction of the bath orbitals (the orbitals which include the
 environment effect from the surrounding part) is done here.
 """
 
 import numpy as np
 
 
-def dmet_fragment_bath(mol, t_list, temp_list, onerdm_low):
+def dmet_fragment_bath(mol, t_list, temp_list, onerdm_low, virtual_orbital_threshold=1e-13, verbose=False):
     """ Construct the bath orbitals for DMET fragment calculation.
 
     Args:
         mol (pyscf.gto.Mole): The molecule to simulate (The full molecular
             system).
         t_list (list): Number of [0] fragment & [1] bath orbitals (int).
         temp_list (list): [0] Minimum and [1] maximum number for the active
             orbitals (int).
         onerdm_low (numpy.array): One-particle RDM from the low-level
             calculation (float64).
+        virtual_orbital_threshold (float): Occupation threshold for the density
+            matrix, used to discard virtual orbitals.
+        verbose (bool): Print the orbital occupancy eigenvalues for prototyping
+            purposes (setting virtual_orbital_threshold).
 
     Returns:
         numpy.array: The bath orbitals (float64).
         numpy.array: Orbital energies (float64).
     """
 
     # Extract the one-particle RDM for the active space
     onerdm_embedded = dmet_onerdm_embed(mol, temp_list, onerdm_low)
 
     # Diagonalize it
     e, c = np.linalg.eigh(onerdm_embedded)
 
-    # Sort the eigenvectors with the eigenvalues
-    e_sorted, c_sorted = dmet_bath_orb_sort(t_list, e, c)
+    # Sort the eigenvectors with the eigenvalues (should be positive unless
+    # there is numerical noise, therefore we take the absolute values).
+    e = np.abs(e)
+    if verbose:
+        print(f"\t{e}\n")
+
+    e_sorted, c_sorted = dmet_bath_orb_sort(t_list, e, c, virtual_orbital_threshold)
 
     # Add the core contribution
     bath_orb, e_core = dmet_add_to_bath_orb(mol, t_list, temp_list, e_sorted, c_sorted)
 
     return bath_orb, e_core
 
 
@@ -86,36 +95,39 @@
         onerdm_temp = onerdm_temp3[:temp_list[0], :]
         onerdm_temp2 = onerdm_temp3[temp_list[1]:, :]
         onerdm_temp3 = np.vstack((onerdm_temp, onerdm_temp2))
 
     return onerdm_temp3
 
 
-def dmet_bath_orb_sort(t_list, e_before, c_before):
+def dmet_bath_orb_sort(t_list, e_before, c_before, virtual_orbital_threshold):
     """ Sort the bath orbitals with the eigenvalues (orbital energies).
 
     Args:
         t_list (list): Number of [0] fragment & [1] bath orbitals (int).
         e_before (numpy.array): Orbitals energies before sorting (float64).
         c_before (numpy.array): Coefficients of the orbitals before sorting
             (float64).
+        virtual_orbital_threshold (float): Occupation threshold for the density
+            matrix, used to discard virtual orbitals.
 
     Returns:
         numpy.array: Sorted orbital energies (float64).
         numpy.array: Coefficients of the sorted orbitals (float64).
     """
 
     # Sort the orbital energies (Occupation of 1.0 should come first...)
     new_index = np.maximum(-e_before, e_before - 2.0).argsort()
 
     # Throw away some orbitals above threshold
-    thresh_orb = np.sum(-np.maximum(-e_before, e_before - 2.0)[new_index] > 1e-13)
+    thresh_orb = np.sum(-np.maximum(-e_before, e_before - 2.0)[new_index] > virtual_orbital_threshold)
 
     # Determine the number of bath orbitals
     norb = min(np.sum(thresh_orb), t_list[0])
+
     t_list.append(norb)
 
     # Sort the bath orbitals with its energies
     e_new = e_before[new_index]
     c_new = c_before[:, new_index]
 
     return e_new, c_new
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_fragment.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_fragment.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_onerdm.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_onerdm.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_orbitals.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_orbitals.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 full system mean-field calculation is done here.
 
 Localization schemes based on Intrisic atomic orbitals (IAO) (dmet_iao.py),
 Lowdin, meta-Lowdin, and Boys can be selected. The latter three rely on external
 PySCF program. However, using Boys localization is not recommended.
 """
 
-from pyscf import scf, ao2mo
 import numpy as np
 
 
 class dmet_orbitals:
     """ Localize the SCF orbitals and calculate the integrals
 
     This class handles the information from the calculation of the entire
@@ -64,14 +63,17 @@
             mf (pyscf.scf.RHF): The mean field of the molecule (The full
                 molecule).
             active_space (list): The active space in DMET calculation. All
                 orbitals in the initial SCF calculation (int).
             localization_function (string): Localization scheme.
             uhf (bool): Flag for an unrestricted mean-field.
         """
+        from pyscf import scf, ao2mo
+        self.pyscfscf = scf
+        self.pyscfao2mo = ao2mo
 
         # General quantities.
         self.mol_full = mol
         self.mf_full = mf
         self.low_scf_energy = mf.e_tot
 
         # Define the active space if possible.
@@ -92,22 +94,25 @@
 
         self.number_active_electrons = int(np.rint(self.mf_full.mol.nelectron - np.sum(self.mf_full.mo_occ[self.dmet_active_orbitals == 0])))
 
         # RHF
         if self.mol_full.spin == 0:
             # Obtain the elements from the low-level SCF calculations.
             low_scf_dm = self.mf_full.mo_coeff @ np.diag(self.mf_full.mo_occ) @ self.mf_full.mo_coeff.T
-            low_scf_twoint = scf.hf.get_veff(self.mf_full.mol, low_scf_dm, 0, 0, 1)
+            low_scf_twoint = self.pyscfscf.hf.get_veff(self.mf_full.mol, low_scf_dm, 0, 0, 1)
             self.low_scf_fock = self.mf_full.mol.intor("cint1e_kin_sph") + self.mf_full.mol.intor("cint1e_nuc_sph") + low_scf_twoint
+            # Add effective core potential to Fock matrix if applicable.
+            if len(self.mol_full._ecpbas) > 0:
+                self.low_scf_fock += self.mf_full.mol.intor_symmetric('ECPscalar')
 
             # Define the core space if possible (Initial calculations treat the entire molecule ...).
             core_mo_dm = np.array(self.mf_full.mo_occ, copy=True)
             core_mo_dm[self.dmet_active_orbitals == 1] = 0
             core_ao_dm = self.mf_full.mo_coeff @ np.diag(core_mo_dm) @ self.mf_full.mo_coeff.T
-            core_twoint = scf.hf.get_veff(self.mf_full.mol, core_ao_dm, 0, 0, 1)
+            core_twoint = self.pyscfscf.hf.get_veff(self.mf_full.mol, core_ao_dm, 0, 0, 1)
             core_oneint = self.low_scf_fock - low_scf_twoint + core_twoint
 
             # Define the energies and matrix elements based on the localized orbitals.
             self.core_constant_energy = self.mf_full.mol.energy_nuc() + np.einsum("ij,ij->", core_oneint - 0.5*core_twoint, core_ao_dm)
             self.active_oneint = self.localized_mo.T @ core_oneint @ self.localized_mo
             self.active_fock = self.localized_mo.T @ self.low_scf_fock @ self.localized_mo
         # ROHF
@@ -133,19 +138,19 @@
             self.active_fock_beta = self.localized_mo.T @ low_scf_fock_beta @ self.localized_mo
 
             rdm_a = self.localized_mo.T @ low_scf_rdm[0] @ self.localized_mo
             rdm_b = self.localized_mo.T @ low_scf_rdm[1] @ self.localized_mo
             rdm_total = np.array((rdm_a, rdm_b))
 
             overlap = np.eye(self.number_active_orbitals)
-            two_int = scf.hf.get_veff(self.mol_full, rdm_total, 0, 0, 1)
+            two_int = self.pyscfscf.hf.get_veff(self.mol_full, rdm_total, 0, 0, 1)
             new_fock_alpha = self.active_oneint + (self.localized_mo.T @ two_int[0] @ self.localized_mo)
             new_fock_beta = self.active_oneint + (self.localized_mo.T @ two_int[1] @ self.localized_mo)
             fock_total = np.array((new_fock_alpha, new_fock_beta))
-            self.active_fock = scf.rohf.get_roothaan_fock(fock_total, rdm_total, overlap)
+            self.active_fock = self.pyscfscf.rohf.get_roothaan_fock(fock_total, rdm_total, overlap)
 
     def _unrestricted_init(self):
         """Initialize the attributes for an unrestricted mean-field."""
 
         low_scf_fock_alpha, low_scf_fock_beta = self.mf_full.get_fock()
         core_oneint = self.mf_full.get_hcore()
 
@@ -181,17 +186,17 @@
         """
 
         # Calculate one-electron integrals.
         frag_oneint = bath_orb[:, : norb_high].T @ self.active_oneint @ bath_orb[:, : norb_high]
 
         # Calculate the fock matrix.
         density_matrix = self.localized_mo @ onerdm_core @ self.localized_mo.T
-        two_int = scf.hf.get_veff(self.mol_full, density_matrix, 0, 0, 1)
+        two_int = self.pyscfscf.hf.get_veff(self.mol_full, density_matrix, 0, 0, 1)
         new_fock = self.active_oneint + (self.localized_mo.T @ two_int @ self.localized_mo)
         frag_fock = bath_orb[:, : norb_high].T @ new_fock @ bath_orb[:, : norb_high]
 
         # Calculate the two-electron integrals.
         coefficients = np.dot(self.localized_mo, bath_orb[:, : norb_high])
-        frag_twoint = ao2mo.outcore.full_iofree(self.mol_full, coefficients, compact=False).reshape(
+        frag_twoint = self.pyscfao2mo.outcore.full_iofree(self.mol_full, coefficients, compact=False).reshape(
                                                 norb_high,  norb_high,  norb_high,  norb_high)
 
         return frag_oneint, frag_fock, frag_twoint
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_scf.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 """Perform fragment SCF calculation.
 
 The fragment SCF calculation for DMET calculation is done here.
 """
 
-from pyscf import gto, scf, ao2mo
 import numpy as np
 
 
 def dmet_fragment_scf_rhf(t_list, two_ele, fock, n_electrons, n_orbitals, guess_orbitals, chemical_potential):
     """Perform SCF calculation.
 
     Args:
@@ -37,15 +36,15 @@
 
     Returns:
         pyscf.scf.RHF: The mean field of the molecule (Fragment calculation).
         numpy.array: The fock matrix with chemical potential subtracted
             (float64).
         pyscf.gto.Mole: The molecule to simulate (Fragment calculation).
     """
-
+    from pyscf import gto, scf, ao2mo
     # Deep copy the fock matrix
     fock_frag_copy = fock.copy()
 
     # Subtract the chemical potential to make the number of electrons consistent
     for orb in range(t_list[0]):
         fock_frag_copy[orb, orb] -= chemical_potential
 
@@ -89,14 +88,15 @@
     Returns:
         pyscf.scf.ROHF or pyscf.scf.UHF: The mean field of the molecule
             (Fragment calculation).
         numpy.array: The fock matrix with chemical potential subtracted
             (float64).
         pyscf.gto.Mole: The molecule to simulate (Fragment calculation).
     """
+    from pyscf import gto, scf, ao2mo
 
     # Deep copy the fock matrix
     fock_frag_copy = fock.copy()
 
     for orb in range(nele_ab[0]):
         fock_frag_copy[orb, orb] -= chemical_potential
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/_helpers/dmet_scf_guess.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf_guess.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Employ DMET as a problem decomposition technique."""
 
 from enum import Enum
+from typing import Union, List, Callable, Dict
+
 import numpy as np
-from pyscf import gto, scf
 import scipy
 import warnings
 
+from tangelo.helpers.utils import is_package_installed
+from tangelo import SecondQuantizedMolecule
 from tangelo.problem_decomposition.dmet import _helpers as helpers
 from tangelo.problem_decomposition.problem_decomposition import ProblemDecomposition
 from tangelo.problem_decomposition.electron_localization import iao_localization, meta_lowdin_localization, nao_localization
-from tangelo.problem_decomposition.dmet.fragment import SecondQuantizedDMETFragment
 from tangelo.algorithms import FCISolver, CCSDSolver, VQESolver
 from tangelo.toolboxes.post_processing.mc_weeny_rdm_purification import mcweeny_purify_2rdm
-from tangelo.toolboxes.molecular_computation.rdms import pad_rdms_with_frozen_orbitals
+from tangelo.toolboxes.molecular_computation.rdms import pad_rdms_with_frozen_orbitals_restricted, \
+    pad_rdms_with_frozen_orbitals_unrestricted
+from tangelo.toolboxes.molecular_computation.integral_solver_pyscf import mol_to_pyscf
 
 
 class Localization(Enum):
     """Enumeration of the electron localization supported by DMET."""
     meta_lowdin = 0
     iao = 1
     nao = 2
@@ -64,57 +68,61 @@
             and its behavior.
         initial_chemical_potential (float) : Initial value for the chemical
             potential.
         solvers_options (list or dict): List of dictionaries for the solver
             options. If only a single dictionary is passed, the same options are
             applied for every solver. This will raise an error if different
             solvers are parsed.
+        virtual_orbital_threshold (float): Occupation threshold for the virtual
+            orbital space. Setting it to 0. is the equivalent of turning off
+            the virtual orbital space truncation.
+            Default=1e-13.
         verbose (bool) : Flag for DMET verbosity.
     """
 
     def __init__(self, opt_dict):
-
+        if not is_package_installed("pyscf"):
+            raise ModuleNotFoundError(f"Using {self.__class__.__name__} requires the installation of the pyscf package.")
+        from pyscf import gto, scf
+        from tangelo.problem_decomposition.dmet.fragment import SecondQuantizedDMETFragment
         default_ccsd_options = dict()
         default_fci_options = dict()
         default_vqe_options = {"qubit_mapping": "jw",
                                "initial_var_params": "ones",
                                "verbose": False}
 
-        default_options = {"molecule": None,
-                           "electron_localization": Localization.meta_lowdin,
-                           "fragment_atoms": list(),
-                           "fragment_solvers": "ccsd",
-                           "fragment_frozen_orbitals": list(),
-                           "optimizer": self._default_optimizer,
-                           "initial_chemical_potential": 0.0,
-                           "solvers_options": list(),
-                           "verbose": False}
+        copt_dict = opt_dict.copy()
+        self.molecule: SecondQuantizedMolecule = copt_dict.pop("molecule", None)
+        self.electron_localization: Localization = copt_dict.pop("electron_localization", Localization.meta_lowdin)
+        self.fragment_atoms: List[int] = copt_dict.pop("fragment_atoms", list())
+        self.fragment_solvers: Union[str, List[str]] = copt_dict.pop("fragment_solvers", "ccsd")
+        self.fragment_frozen_orbitals: List[List[Union[int, str]]] = copt_dict.pop("fragment_frozen_orbitals", list())
+        self.optimizer: Callable[..., float] = copt_dict.pop("optimizer", self._default_optimizer)
+        self.initial_chemical_potential: float = copt_dict.pop("initial_chemical_potential", 0.0)
+        self.solvers_options: List[dict] = copt_dict.pop("solvers_options", list())
+        self.virtual_orbital_threshold: float = copt_dict.pop("virtual_orbital_threshold", 1e-13)
+        self.verbose: bool = copt_dict.pop("verbose", False)
 
         self.builtin_localization = set(Localization)
 
-        # Initialize with default values
-        self.__dict__ = default_options
-        # Overwrite default values with user-provided ones, if they correspond to a valid keyword
-        for k, v in opt_dict.items():
-            if k in default_options:
-                setattr(self, k, v)
-            else:
-                raise KeyError(f"Keyword :: {k}, not available in DMETProblemDecomposition.")
+        self.fragment_builder = SecondQuantizedDMETFragment
+
+        if len(copt_dict) > 0:
+            raise KeyError(f"The following keywords are not supported in {self.__class__.__name__}: \n {copt_dict.keys()}")
 
         # Raise error/warnings if input is not as expected
         if not self.molecule:
             raise ValueError(f"A SecondQuantizedMolecule object must be provided when instantiating DMETProblemDecomposition.")
 
-        if self.molecule.uhf or self.molecule.spin != 0:
-            raise NotImplementedError("ROHF-DMET and UHF-DMET have been disabled temporarily for code validation purposes.")
+        self.uhf = self.molecule.uhf
 
         # Converting our interface to pyscf.mol.gto and pyscf.scf (used by this
         # code).
         self.mean_field = self.molecule.mean_field
-        self.molecule = self.molecule.to_pyscf(self.molecule.basis)
+        self.molecule = mol_to_pyscf(self.molecule, self.molecule.basis, ecp=self.molecule.ecp)
 
         # If fragment_atoms is detected as a nested list of int, atoms are reordered to be
         # consistent with a list of numbers representing the number of atoms in each fragment.
         if isinstance(self.fragment_atoms, list) and all(isinstance(list_atoms, list) for list_atoms in self.fragment_atoms):
             fragment_atoms_flatten = [atom_id for frag in self.fragment_atoms for atom_id in frag]
 
             if max(fragment_atoms_flatten) >= self.molecule.natm:
@@ -139,15 +147,15 @@
 
             # Attribution of the expected fragment_atoms and a reordered molecule.
             self.molecule = new_molecule
             self.fragment_atoms = new_fragment_atoms
 
             # Force recomputing the mean field if the atom ordering has been changed.
             warnings.warn("The mean field will be recomputed even if one has been provided by the user.", RuntimeWarning)
-            self.mean_field = scf.RHF(self.molecule)
+            self.mean_field = scf.UHF(self.molecule) if self.uhf else scf.RHF(self.molecule)
             self.mean_field.verbose = 0
             self.mean_field.scf()
 
         # Check if the number of fragment sites is equal to the number of atoms in the molecule
         if self.molecule.natm != sum(self.fragment_atoms):
             raise RuntimeError("The number of fragment sites is not equal to the number of atoms in the molecule")
 
@@ -190,15 +198,15 @@
         # Define during the building phase (self.build()).
         self.orbitals = None
         self.orb_list = None
         self.orb_list2 = None
         self.onerdm_low = None
 
         # If save_results in _oneshot_loop is True, the dict is populated.
-        self.solver_fragment_dict = dict()
+        self.solver_fragment_dict: Dict[int, VQESolver] = dict()
 
         # To keep track the number of iteration (was done with an energy list
         # before).
         self.n_iter = 0
 
     @property
     def quantum_fragments_data(self):
@@ -234,21 +242,27 @@
                 self.electron_localization = nao_localization
             else:
                 raise ValueError(f"Unsupported ansatz. Built-in localization methods:\n\t{self.builtin_localization}")
         elif not callable(self.electron_localization):
             raise TypeError(f"Invalid electron localization function. Expecting a function.")
 
         # Construct orbital object.
-        self.orbitals = helpers._orbitals(self.molecule, self.mean_field, range(self.molecule.nao_nr()), self.electron_localization, False)
+        self.orbitals = helpers._orbitals(self.molecule, self.mean_field, range(self.molecule.nao_nr()), self.electron_localization, self.uhf)
 
         # TODO: remove last argument, combining fragments not supported.
         self.orb_list, self.orb_list2, _ = helpers._fragment_constructor(self.molecule, self.fragment_atoms, 0)
 
         # Calculate the 1-RDM for the entire molecule.
-        self.onerdm_low = helpers._low_rdm_rhf(self.orbitals.active_fock, self.orbitals.number_active_electrons)
+        if self.molecule.spin == 0 and not self.uhf:
+            self.onerdm_low = helpers._low_rdm_rhf(self.orbitals.active_fock, self.orbitals.number_active_electrons)
+        else:
+            self.onerdm_low = helpers._low_rdm_rohf_uhf(self.orbitals.active_fock_alpha,
+                                                        self.orbitals.active_fock_beta,
+                                                        self.orbitals.number_active_electrons_alpha,
+                                                        self.orbitals.number_active_electrons_beta)
 
     def simulate(self):
         """Perform DMET loop to optimize the chemical potential. It converges
         when the electron summation across all fragments is the same as the
         number of electron in the molecule.
 
         Returns:
@@ -333,31 +347,46 @@
         scf_fragments = list()
 
         for i, norb in enumerate(self.orb_list):
             t_list = list()
             t_list.append(norb)
             temp_list = self.orb_list2[i]
 
+            if self.verbose:
+                print(f"\tSCF Occupancy Eigenvalues for Fragment Number : # {i}")
+
             # Construct bath orbitals.
-            bath_orb, e_occupied = helpers._fragment_bath(self.orbitals.mol_full, t_list, temp_list, self.onerdm_low)
+            bath_orb, e_occupied = helpers._fragment_bath(self.orbitals.mol_full, t_list, temp_list,
+                                                          self.onerdm_low, self.virtual_orbital_threshold, self.verbose)
 
             # Obtain one particle rdm for a fragment.
             norb_high, nelec_high, onerdm_high = helpers._fragment_rdm(t_list, bath_orb, e_occupied,
                                                                        self.orbitals.number_active_electrons)
 
             # Obtain one particle rdm for a fragment.
             one_ele, fock, two_ele = self.orbitals.dmet_fragment_hamiltonian(bath_orb, norb_high, onerdm_high)
 
             # Construct guess orbitals for fragment SCF calculations.
             # Carry out SCF calculation for a fragment.
-            guess_orbitals = helpers._fragment_guess_rhf(t_list, bath_orb, chemical_potential, norb_high, nelec_high,
-                                                            self.orbitals.active_fock)
-            mf_fragment, fock_frag_copy, mol_frag = helpers._fragment_scf_rhf(
-                t_list, two_ele, fock, nelec_high, norb_high, guess_orbitals,
-                chemical_potential)
+            if self.uhf or self.molecule.spin != 0:
+                guess_orbitals, nelec_high_ab = helpers._fragment_guess_rohf_uhf(
+                    t_list, bath_orb, chemical_potential, norb_high, nelec_high,
+                    self.orbitals.active_fock_alpha, self.orbitals.active_fock_beta,
+                    self.orbitals.number_active_electrons_alpha,
+                    self.orbitals.number_active_electrons_beta)
+
+                mf_fragment, fock_frag_copy, mol_frag = helpers._fragment_scf_rohf_uhf(
+                    nelec_high_ab, two_ele, fock, nelec_high, norb_high,
+                    guess_orbitals, chemical_potential, self.uhf)
+            else:
+                guess_orbitals = helpers._fragment_guess_rhf(t_list, bath_orb, chemical_potential, norb_high, nelec_high,
+                                                             self.orbitals.active_fock)
+                mf_fragment, fock_frag_copy, mol_frag = helpers._fragment_scf_rhf(
+                    t_list, two_ele, fock, nelec_high, norb_high, guess_orbitals,
+                    chemical_potential)
 
             scf_fragments.append([mf_fragment, fock_frag_copy, mol_frag, t_list, one_ele, two_ele, fock])
 
         return scf_fragments
 
     def _oneshot_loop(self, chemical_potential, save_results=False, resample=False, n_shots=None, purify=False, rdm_measurements=None):
         """Perform the DMET loop. This is the cost function which is optimized
@@ -425,16 +454,16 @@
             # Unpacking the information for the selected fragment.
             mf_fragment, fock_frag_copy, mol_frag, t_list, one_ele, two_ele, fock = info_fragment
 
             # Interface with our data strcuture.
             # We create a dummy SecondQuantizedMolecule with a DMETFragment class.
             # It has the same important attributes and methods to be used with
             # functions of this package.
-            dummy_mol = SecondQuantizedDMETFragment(mol_frag, mf_fragment, fock,
-                fock_frag_copy, t_list, one_ele, two_ele, False,
+            dummy_mol = self.fragment_builder(mol_frag, mf_fragment, fock,
+                fock_frag_copy, t_list, one_ele, two_ele, self.uhf,
                 self.fragment_frozen_orbitals[i])
 
             if self.verbose:
                 print("\t\tFragment Number : # ", i + 1)
                 print("\t\t------------------------")
 
             # TODO: Changing this into something more simple is preferable. There
@@ -465,27 +494,34 @@
                         raise ValueError("n_shots must be specified in original calculation or in error calculation")
                 else:
                     system = {"molecule": dummy_mol}
                     solver_fragment = VQESolver({**system, **solver_options})
                     solver_fragment.build()
                     solver_fragment.simulate()
 
-                if purify and solver_fragment.molecule.n_active_electrons == 2:
+                if purify and solver_fragment.molecule.n_active_electrons == 2 and not self.uhf:
                     onerdm, twordm = solver_fragment.get_rdm(solver_fragment.optimal_var_params, resample=resample, sum_spin=False)
                     onerdm, twordm = mcweeny_purify_2rdm(twordm)
+                elif self.uhf:
+                    onerdm, twordm = solver_fragment.get_rdm_uhf(solver_fragment.optimal_var_params, resample=resample)
                 else:
                     onerdm, twordm = solver_fragment.get_rdm(solver_fragment.optimal_var_params, resample=resample)
                 if save_results:
                     self.solver_fragment_dict[i] = solver_fragment
                     self.rdm_measurements[i] = self.solver_fragment_dict[i].rdm_freq_dict
 
             # Compute the fragment energy and sum up the number of electrons
-            onerdm_padded, twordm_padded = pad_rdms_with_frozen_orbitals(dummy_mol, onerdm, twordm)
-            fragment_energy, onerdm = self._compute_energy_restricted(dummy_mol, onerdm_padded, twordm_padded)
-            n_electron_frag = np.trace(onerdm[: t_list[0], : t_list[0]])
+            if self.uhf:
+                onerdm_padded, twordm_padded = pad_rdms_with_frozen_orbitals_unrestricted(dummy_mol, onerdm, twordm)
+                fragment_energy, onerdm_a, onerdm_b = self._compute_energy_unrestricted(dummy_mol, onerdm_padded, twordm_padded)
+                n_electron_frag = np.trace(onerdm_a[ : t_list[0], : t_list[0]]) + np.trace(onerdm_b[ : t_list[0], : t_list[0]])
+            else:
+                onerdm_padded, twordm_padded = pad_rdms_with_frozen_orbitals_restricted(dummy_mol, onerdm, twordm)
+                fragment_energy, onerdm = self._compute_energy_restricted(dummy_mol, onerdm_padded, twordm_padded)
+                n_electron_frag = np.trace(onerdm[: t_list[0], : t_list[0]])
 
             number_of_electron += n_electron_frag
 
             # Sum up the energy.
             energy_temp += fragment_energy
 
             if self.verbose:
@@ -514,16 +550,16 @@
         # Iterate across all fragment and compute their energies.
         # The total energy is stored in energy_temp.
         for i, info_fragment in enumerate(scf_fragments):
 
             # Unpacking the information for the selected fragment.
             mf_fragment, fock_frag_copy, mol_frag, t_list, one_ele, two_ele, fock = info_fragment
 
-            dummy_mol = SecondQuantizedDMETFragment(mol_frag, mf_fragment, fock,
-                fock_frag_copy, t_list, one_ele, two_ele, False,
+            dummy_mol = self.fragment_builder(mol_frag, mf_fragment, fock,
+                fock_frag_copy, t_list, one_ele, two_ele, self.uhf,
                 self.fragment_frozen_orbitals[i])
 
             # Buiding SCF fragments and quantum circuit. Resources are then
             # estimated. For classical sovlers, this functionality is not
             # implemented yet.
             solver_fragment = self.fragment_solvers[i]
             solver_options = self.solvers_options[i]
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/dmet/fragment.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/fragment.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         self.q = self.molecule.charge
         self.spin = self.molecule.spin
         self.active_spin = self.spin
 
         self.basis = self.molecule.basis
 
-        self.n_mos = len(self.mean_field.mo_energy)
+        self.n_mos = len(self.mean_field.mo_energy[0]) if self.uhf else len(self.mean_field.mo_energy)
         self.mo_occ = self.mean_field.mo_occ
 
         list_of_active_frozen = convert_frozen_orbitals(self, self.frozen_orbitals)
         self.active_occupied = list_of_active_frozen[0]
         self.frozen_occupied = list_of_active_frozen[1]
         self.active_virtual = list_of_active_frozen[2]
         self.frozen_virtual = list_of_active_frozen[3]
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/iao_localization.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/iao_localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 Note that minimal basis cannot be used for IAO because the idea of IAO is to map
 on minao minimal basis set.
 
 For details, refer to:
     - G. Knizia, JCTC 9, 4834-4843 (2013).
 """
 
-from pyscf import gto
-from pyscf.lo import iao
 from functools import reduce
-from pyscf.lo import orth
 import numpy as np
 import scipy
 
 
 def iao_localization(mol, mf):
     """Localize the orbitals using IAO localization.
 
@@ -64,14 +61,17 @@
     Args:
         mol (pyscf.gto.Mole): The molecule to simulate.
         mf (pyscf.scf.RHF): The mean field of the molecule.
 
     Returns:
         numpy.array: The localized orbitals for the occupied space (float64).
     """
+    from pyscf import gto
+    from pyscf.lo import iao
+    from pyscf.lo import orth
 
     #   Get MO coefficient of occupied MOs
     occupied_orbitals = mf.mo_coeff[:, mf.mo_occ > 0.5]
 
     #   Get mol data in minao basis
     min_mol = iao.reference_mol(mol)
 
@@ -114,14 +114,16 @@
     Args:
         mol (pyscf.gto.Mole): The molecule to simulate.
         iao_ref (numpy.array): IAO in occupied space (float64).
 
     Returns:
         numpy.array: IAO in complementary space (float64).
     """
+    from pyscf.lo import iao
+    from pyscf.lo import orth
 
     #   Get the total number of AOs
     norbital_total = mol.nao_nr()
 
     #   Calculate the Overlaps for total basis
     s1 = mol.intor_symmetric("int1e_ovlp")
 
@@ -220,14 +222,15 @@
         mf (pyscf.scf.RHF): The mean field of the molecule.
         iao1 (numpy.array): IAO for occupied space (float64).
         iao2 (numpy.array): IAO for complementary space (float64).
 
     Returns:
         numpy.array: The rearranged IAO (float64).
     """
+    from pyscf.lo import orth
 
     # Calclate the integrals for assignment
     number_orbitals = mol.nao_nr()
     r_int1e = mol.intor("cint1e_r_sph", 3)
     iao_combine = np.hstack((iao1, iao2))
 
     # Calculate atom center for each orbital
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/meta_lowdin_localization.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/meta_lowdin_localization.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,20 @@
 The orbital localization of the canonical orbitals  using Meta-Löwdin
 localization is done here. `pyscf.lo` is used.
 
 For details, refer to:
     - Q. Sun et al., JCTC 10, 3784-3790 (2014).
 """
 
-from pyscf.lo import orth
-
 
 def meta_lowdin_localization(mol, mf):
     """Localize the orbitals using Meta-Löwdin localization.
 
     Args:
         mol (pyscf.gto.Mole): The molecule to simulate.
         mf (pyscf.scf.RHF): The mean field of the molecule.
 
     Returns:
         numpy.array: The localized orbitals (float64).
     """
+    from pyscf.lo import orth
     return orth.orth_ao(mol, "meta_lowdin")
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/electron_localization/nao_localization.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/nao_localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 localization is done here. `pyscf.lo` is used.
 
 For details, refer to:
     - Alan E. Reed, Robert B. Weinstock, and Frank Weinhold.
       Natural population analysis. J. Chem. Phys., 83(2):735-746, 1985.
 """
 
-from pyscf.lo import orth
-
 
 def nao_localization(mol, mf):
     """Localize the orbitals using NAO localization.
 
     Args:
         mol (pyscf.gto.Mole): The molecule to simulate.
         mf (pyscf.scf): The mean field of the molecule.
 
     Returns:
         numpy.array: The localized orbitals (float64).
     """
+    from pyscf.lo import orth
     return orth.orth_ao(mf, "NAO")
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/incremental/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/incremental/mifno_helper.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/mifno_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 
     def __repr__(self):
         """Format the object to print the energies and the fragment information
         as a pandas.DataFrame.
         """
 
         data_fragments = self.to_dataframe
+        data_fragments.drop(["problem_handle"], axis=1, inplace=True)
         data_fragments.drop(["frozen_orbitals_truncated"], axis=1, inplace=True)
         data_fragments.drop(["complete_orbital_space"], axis=1, inplace=True)
         str_rep = f"(All the energy values are in hartree)\n" \
                   f"Total MI-FNO energy = {self.e_tot}\n" \
                   f"Correlation energy = {self.e_corr}\n" \
                   f"Mean-field energy = {self.e_mf}\n" \
                   f"{data_fragments}"
@@ -185,15 +186,15 @@
         """The user can select the fragment information (python dictionary) with
         the [] operator.
         """
         return self.frag_info_flattened[frag_id]
 
     @property
     def to_dataframe(self):
-        """Outputs the fragment informations as a pandas.DataFrame."""
+        """Outputs fragment information as a pandas.DataFrame."""
         df = pd.DataFrame.from_dict(self.frag_info_flattened, orient="index")
 
         # Replace frozen_orbitals_truncated=None with an empty list.
         df["frozen_orbitals_truncated"] = df["frozen_orbitals_truncated"].apply(lambda d: d if isinstance(d, list) else [])
         df["complete_orbital_space"] = df["complete_orbital_space"].apply(lambda d: d if isinstance(d, list) else [])
 
         return df.drop(["mo_coefficients"], axis=1)
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from ._helpers.helper_classes import Fragment, Link
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/_helpers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/_helpers/capping_groups.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/capping_groups.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/_helpers/helper_classes.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/helper_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,94 @@
 
 """Fragment class, used in construction of ONIOM layers -- contains details of
 both the constituent geometry (i.e. which atoms from system are in fragment,
 which bonds are broken and how to fix them) as well as the solver(s) to use.
 """
 
 import warnings
+from typing import Union, List
 
 import numpy as np
 from scipy.spatial.transform import Rotation as R
 
 from tangelo import SecondQuantizedMolecule
 from tangelo.algorithms import CCSDSolver, FCISolver, VQESolver, MINDO3Solver, ADAPTSolver, QITESolver
 from tangelo.problem_decomposition.oniom._helpers.capping_groups import elements, chemical_groups
 
 
+class Link:
+
+    def __init__(self, staying, leaving, factor=1.0, species="H"):
+        """Bonds broken during the layer-construction process in ONIOM must be
+        mended. This class represents a broken-bond link, and has associated
+        methods to generate a new bond, appending the intended species.
+
+        Args:
+            staying (int): Atom id retained.
+            leaving (int): Atom id lost.
+            factor (float) optional: Rescale length of bond, from that in the
+                original molecule.
+            species (str) optional: Atomic species or a chemical group
+                identifier for new link. Can be a list (first element = "X" to
+                detect the orientation) for a custom chemical group.
+        """
+
+        self.staying = staying
+        self.leaving = leaving
+        self.factor = factor
+
+        if isinstance(species, str) and species in elements:
+            self.species = [(species, (0., 0., 0.))]
+        elif isinstance(species, str) and species in chemical_groups:
+            self.species = chemical_groups[species]
+        elif isinstance(species, (list, tuple)) and species[0][0].upper() == "X":
+            self.species = species
+        else:
+            raise ValueError(f"{species} is not supported. It must be a string identifier or a list of atoms (with a ghost atom ('X') as the first element).")
+
+    def relink(self, geometry):
+        """Create atom at location of mended-bond link.
+
+        Args:
+            geometry (list of positions): Atomic positions in format
+                [[str,tuple(float,float,float)],...].
+
+        Returns:
+            list: List of atomic species and position (x, y, z) of replacement
+                atom / chemical group.
+        """
+
+        elements = [a[0] for a in self.species if a[0].upper() != "X"]
+        chem_group_xyz = np.array([[a[1][0], a[1][1], a[1][2]] for a in self.species if a[0].upper() != "X"])
+
+        staying = np.array(geometry[self.staying][1])
+        leaving = np.array(geometry[self.leaving][1])
+
+        # Rotation (if not a single atom).
+        if len(elements) > 1:
+            axis_old = leaving - staying
+            axis_new = chem_group_xyz[0] - np.array(self.species[0][1])
+
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", UserWarning)
+                rot, _ = R.align_vectors([axis_old], [axis_new])
+            chem_group_xyz = rot.apply(chem_group_xyz)
+
+        # Move the atom / group to the right position in space.
+        replacement = self.factor*(leaving-staying) + staying
+        translation = replacement - chem_group_xyz[0]
+        chem_group_xyz += translation
+
+        return [(element, (xyz[0], xyz[1], xyz[2])) for element, xyz in zip(elements, chem_group_xyz)]
+
+
 class Fragment:
 
-    def __init__(self, solver_low, options_low=None, solver_high=None, options_high=None, selected_atoms=None, charge=0, spin=0, broken_links=None):
+    def __init__(self, solver_low: str, options_low: dict = None, solver_high: str = None, options_high: dict = None,
+                 selected_atoms: Union[int, List[int]] = None, charge: int = 0, spin: int = 0, broken_links: List[Link] = None):
         """Fragment class for the ONIOM solver. Each fragment can have broken
         links. In this case, they are capped with a chosen atom. Each fragment
         can also have up to two solvers (low and high accuracy).
 
         Args:
             solver_low (str): Specification of low accuracy solver for fragment.
             options_low (dict): Specification of low accuracy solver options.
@@ -142,15 +210,15 @@
     def get_mol(self, basis, frozen=None):
         """Get the molecule object for this fragment (with a specified basis).
 
         Returns:
             SecondQuantizedMolecule: Molecule object.
         """
 
-        return SecondQuantizedMolecule(self.geometry, self.charge, self.spin, basis, frozen_orbitals=frozen)
+        return SecondQuantizedMolecule(self.geometry, self.charge, self.spin, basis=basis, frozen_orbitals=frozen)
 
     @staticmethod
     def get_energy(molecule, solver):
         """Get the energy for a specific solver.
 
         Args:
             molecule (SecondQuantizedMolecule): Molecule for this fragment (with
@@ -208,73 +276,7 @@
         if isinstance(self.solver_low, quantum_solvers):
             resources = self.solver_low.get_resources()
 
         if isinstance(self.solver_high, quantum_solvers):
             resources = self.solver_high.get_resources()
 
         return resources
-
-
-class Link:
-
-    def __init__(self, staying, leaving, factor=1.0, species="H"):
-        """Bonds broken during the layer-construction process in ONIOM must be
-        mended. This class represents a broken-bond link, and has associated
-        methods to generate a new bond, appending the intended species.
-
-        Args:
-            staying (int): Atom id retained.
-            leaving (int): Atom id lost.
-            factor (float) optional: Rescale length of bond, from that in the
-                original molecule.
-            species (str) optional: Atomic species or a chemical group
-                identifier for new link. Can be a list (first element = "X" to
-                detect the orientation) for a custom chemical group.
-        """
-
-        self.staying = staying
-        self.leaving = leaving
-        self.factor = factor
-
-        if isinstance(species, str) and species in elements:
-            self.species = [(species, (0., 0., 0.))]
-        elif isinstance(species, str) and species in chemical_groups:
-            self.species = chemical_groups[species]
-        elif isinstance(species, (list, tuple)) and species[0][0].upper() == "X":
-            self.species = species
-        else:
-            raise ValueError(f"{species} is not supported. It must be a string identifier or a list of atoms (with a ghost atom ('X') as the first element).")
-
-    def relink(self, geometry):
-        """Create atom at location of mended-bond link.
-
-        Args:
-            geometry (list of positions): Atomic positions in format
-                [[str,tuple(float,float,float)],...].
-
-        Returns:
-            list: List of atomic species and position (x, y, z) of replacement
-                atom / chemical group.
-        """
-
-        elements = [a[0] for a in self.species if a[0].upper() != "X"]
-        chem_group_xyz = np.array([[a[1][0], a[1][1], a[1][2]] for a in self.species if a[0].upper() != "X"])
-
-        staying = np.array(geometry[self.staying][1])
-        leaving = np.array(geometry[self.leaving][1])
-
-        # Rotation (if not a single atom).
-        if len(elements) > 1:
-            axis_old = leaving - staying
-            axis_new = chem_group_xyz[0] - np.array(self.species[0][1])
-
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore", UserWarning)
-                rot, _ = R.align_vectors([axis_old], [axis_new])
-            chem_group_xyz = rot.apply(chem_group_xyz)
-
-        # Move the atom / group to the right position in space.
-        replacement = self.factor*(leaving-staying) + staying
-        translation = replacement - chem_group_xyz[0]
-        chem_group_xyz += translation
-
-        return [(element, (xyz[0], xyz[1], xyz[2])) for element, xyz in zip(elements, chem_group_xyz)]
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/oniom/oniom_problem_decomposition.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/oniom_problem_decomposition.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,45 +25,42 @@
 Reference:
     - The ONIOM Method and Its Applications. Lung Wa Chung, W. M. C. Sameera,
     Romain Ramozzi, Alister J. Page, Miho Hatanaka, Galina P. Petrova,
     Travis V. Harris, Xin Li, Zhuofeng Ke, Fengyi Liu, Hai-Bei Li, Lina Ding
     and Keiji Morokuma
     Chemical Reviews 2015 115 (12), 5678-5796. DOI: 10.1021/cr5004419.
 """
+from typing import List, Union, Tuple
 
 from tangelo.problem_decomposition.problem_decomposition import ProblemDecomposition
+from tangelo.problem_decomposition.oniom._helpers.helper_classes import Fragment
 from tangelo.toolboxes.molecular_computation.molecule import atom_string_to_list
 
 
 class ONIOMProblemDecomposition(ProblemDecomposition):
 
     def __init__(self, opt_dict):
         """Main class for the ONIOM hybrid solver. It defines layers with
         different electronic solvers.
 
         Attributes:
-            geometry (strin or list): XYZ atomic coords (in "str float float..."
+            geometry (string or list): XYZ atomic coords (in "str float float..."
                 or [[str, (float, float, float)], ...] format).
             fragments (list of Fragment): Specification of different
                 system-subgroups and their solvers.
             verbose (bolean): Verbose flag.
         """
 
-        default_options = {"geometry": None,
-                           "fragments": list(),
-                           "verbose": False}
-
-        # Initialize with default values
-        self.__dict__ = default_options
-        # Overwrite default values with user-provided ones, if they correspond to a valid keyword
-        for k, v in opt_dict.items():
-            if k in default_options:
-                setattr(self, k, v)
-            else:
-                raise KeyError(f"Keyword :: {k}, not available in {self.__class__.__name__}.")
+        copt_dict = opt_dict.copy()
+        self.geometry: Union[str, List[Tuple[str, Tuple[float]]]] = copt_dict.pop("geometry", None)
+        self.fragments: List[Fragment] = copt_dict.pop("fragments", list())
+        self.verbose: bool = copt_dict.pop("verbose", False)
+
+        if len(copt_dict.keys()) > 0:
+            raise KeyError(f"Keywords :: {copt_dict.keys()}, not available in {self.__class__.__name__}.")
 
         # Raise error/warnings if input is not as expected
         if not self.geometry or not self.fragments:
             raise ValueError(f"A geometry and models must be provided when instantiating ONIOMProblemDecomposition.")
 
         self.geometry = atom_string_to_list(self.geometry) if isinstance(self.geometry, str) else self.geometry
         self.distribute_atoms()
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/problem_decomposition.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/problem_decomposition.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 import numpy as np
+import scipy
 
+from tangelo import SecondQuantizedMolecule
 from tangelo.molecule_library import mol_H4_doublecation_minao, mol_H4_doublecation_321g, mol_H10_321g, mol_H10_minao
 from tangelo.problem_decomposition import DMETProblemDecomposition
 from tangelo.problem_decomposition.dmet import Localization
 from tangelo.algorithms.variational import VQESolver
 from tangelo.toolboxes.molecular_computation.rdms import matricize_2rdm
 
 
@@ -257,14 +259,33 @@
                     }
 
         solver = DMETProblemDecomposition(opt_dmet)
         solver.build()
         energy = solver.simulate()
         self.assertAlmostEqual(energy, -4.41503, places=4)
 
+    def test_dmet_ecp(self):
+        """Tests the DMET energy for Zn with ECP with custom optimizer."""
+        def optimizer(func, var_params):
+            """Custom optimizer used as convergence sometimes fails with default."""
+            def func2(params):
+                val = func(params)
+                return val.real*val.real
+            result = scipy.optimize.minimize(func2, var_params, tol=1.e-1)
+            return result.x[0]
+
+        mol_zn = SecondQuantizedMolecule("Zn", q=2, spin=0, basis="lanl2dz", ecp="lanl2dz")
+
+        options_zn_dmet = {"molecule": mol_zn, "fragment_atoms": [1], "fragment_solvers": "ccsd", "optimizer": optimizer}
+
+        solver = DMETProblemDecomposition(options_zn_dmet)
+        solver.build()
+        energy = solver.simulate()
+        self.assertAlmostEqual(energy, -62.77176, places=4)
+
     def test_dmet_wrong_number_frozen_orbitals(self):
         """Tests if the program raises the error when the number of frozen
         orbital elements is not equal to the number of fragment.
         """
 
         opt_dmet = {"molecule": mol_H10_321g,
                     "fragment_atoms": [1]*10,
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet_fragment.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_fragment.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet_oneshot_loop.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_oneshot_loop.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet_orbitals.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_orbitals.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_dmet_vqe.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_vqe.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/dmet/test_osdmet.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_osdmet.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     O               0.000000    0.676045   -0.258863
     O               0.000000   -0.676045   -0.258863
 """
 
 
 class OSDMETProblemDecompositionTest(unittest.TestCase):
 
-    @unittest.skip("Open-shell DMET has been disabled.")
     def test_lio2_sto6g_rohf(self):
         """Tests the result from OS-DMET (ROHF) against a value from a reference
         implementation with nao localization and CCSD solution to fragments.
         """
 
         mol_lio2 = SecondQuantizedMolecule(LiO2, q=0, spin=1, basis="STO-6G", frozen_orbitals=None, uhf=False)
 
@@ -44,15 +43,14 @@
 
         dmet_solver = DMETProblemDecomposition(opt_dmet)
         dmet_solver.build()
         energy = dmet_solver.simulate()
 
         self.assertAlmostEqual(energy, -156.6317605935, places=4)
 
-    @unittest.skip("Open-shell DMET has been disabled.")
     def test_lio2_sto6g_uhf(self):
         """Tests the result from OS-DMET (UHF) against a value from a reference
         implementation with nao localization and CCSD solution to fragments.
         """
 
         mol_lio2 = SecondQuantizedMolecule(LiO2, q=0, spin=1, basis="STO-6G", frozen_orbitals=None, uhf=True)
```

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/test_capping.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_capping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/test_oniom.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_oniom.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/problem_decomposition/tests/oniom/test_oniom_quantum.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_oniom_quantum.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_general_unitary_cc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_general_unitary_cc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_hea_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_hea_circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_qubit_cc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_cc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_qubit_ilc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_ilc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_qubit_mf.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_mf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_unitary_cc_openshell.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_cc_openshell.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_unitary_cc_paired.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_cc_paired.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/_unitary_majorana_cc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_majorana_cc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/adapt_ansatz.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/adapt_ansatz.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/ansatz.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ansatz.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/ansatz_utils.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ansatz_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,19 @@
 """
 
 from copy import deepcopy
 from itertools import combinations
 
 import numpy as np
 from openfermion.ops import FermionOperator as ofFermionOperator
-from openfermion.ops import InteractionOperator as ofInteractionOperator
 from openfermion.ops import QubitOperator as ofQubitOperator
 
 from tangelo.linq import Circuit, Gate
 from tangelo.toolboxes.operators import FermionOperator, QubitOperator
-from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping, get_fermion_operator
+from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 
 
 def pauli_op_to_gate(index, op, inverse=False):
     """Return the change-of-basis gates required to map pauli words to quantum
     circuit as per Whitfield 2010 (https://arxiv.org/pdf/1001.3855.pdf).
     """
     if op == "X":
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/fermionic_operators.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/fermionic_operators.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/hea.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/hea.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/ilc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ilc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/penalty_terms.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/penalty_terms.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/puccd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/puccd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/qcc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/qcc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/qmf.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/qmf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/rucc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/rucc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_adapt_ansatz.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_adapt_ansatz.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_ansatz_util.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_ansatz_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
             qubit_hamiltonian = fermion_to_qubit_mapping(fermion_operator=fermion_operator,
                                                          mapping=mapping,
                                                          n_spinorbitals=mol_H4_sto3g.n_active_sos,
                                                          n_electrons=mol_H4_sto3g.n_active_electrons,
                                                          up_then_down=True)
 
-            ham_mat = get_sparse_operator(qubit_hamiltonian).toarray()
+            ham_mat = get_sparse_operator(qubit_hamiltonian.to_openfermion()).toarray()
             evolve_exact = expm(-1j * time * ham_mat) @ refwave
 
             options = {"up_then_down": True,
                        "qubit_mapping": mapping,
                        "n_spinorbitals": mol_H4_sto3g.n_active_sos,
                        "n_electrons": mol_H4_sto3g.n_active_electrons}
             tcircuit, phase = trotterize(fermion_operator, trotter_order=1, n_trotter_steps=1, time=time,
@@ -71,15 +71,15 @@
 
             qubit_hamiltonian = fermion_to_qubit_mapping(fermion_operator=fermion_operator,
                                                          mapping=mapping,
                                                          n_spinorbitals=mol_H4_sto3g.n_active_sos,
                                                          n_electrons=mol_H4_sto3g.n_active_electrons,
                                                          up_then_down=True)
 
-            ham_mat = get_sparse_operator(qubit_hamiltonian).toarray()
+            ham_mat = get_sparse_operator(qubit_hamiltonian.to_openfermion()).toarray()
             evolve_exact = expm(-1j * time * ham_mat) @ refwave
 
             tcircuit, phase = trotterize(qubit_hamiltonian, trotter_order=1, n_trotter_steps=1, time=time,
                                          return_phase=True)
             _, wavefunc = sim.simulate(tcircuit, return_statevector=True, initial_statevector=refwave)
             wavefunc *= phase
             overlap = np.dot(np.conj(evolve_exact), wavefunc)
@@ -99,15 +99,15 @@
 
         qubit_hamiltonian = fermion_to_qubit_mapping(fermion_operator=fermion_operator,
                                                      mapping=mapping,
                                                      n_spinorbitals=mol_H4_sto3g.n_active_sos,
                                                      n_electrons=mol_H4_sto3g.n_active_electrons,
                                                      up_then_down=True)
 
-        ham_mat = get_sparse_operator(qubit_hamiltonian).toarray()
+        ham_mat = get_sparse_operator(qubit_hamiltonian.to_openfermion()).toarray()
         evolve_exact = expm(-1j * time * ham_mat) @ refwave
 
         for trotter_order, n_trotter_steps in [(1, 1), (2, 1), (1, 2), (4, 1), (6, 1)]:
 
             tcircuit, phase = trotterize(qubit_hamiltonian, time, n_trotter_steps, trotter_order, return_phase=True)
             _, wavefunc = sim.simulate(tcircuit, return_statevector=True, initial_statevector=refwave)
             wavefunc *= phase
@@ -140,15 +140,15 @@
         evolve_exact = refwave
         total_fermion_operator = FermionOperator()
         # evolve each term separately and apply to resulting wavefunction
         for i in range(3):
             total_fermion_operator += fermion_operators[i]
             qubit_hamiltonian = fermion_to_qubit_mapping(fermion_operator=fermion_operators[i],
                                                          mapping=mapping)
-            ham_mat = get_sparse_operator(qubit_hamiltonian, n_qubits=4).toarray()
+            ham_mat = get_sparse_operator(qubit_hamiltonian.to_openfermion(), n_qubits=4).toarray()
             evolve_exact = expm(-1j * time[next(iter(fermion_operators[i].terms))] * ham_mat) @ evolve_exact
 
         # Apply trotter-suzuki steps using different times for each term
         tcircuit, phase = trotterize(total_fermion_operator, trotter_order=1, n_trotter_steps=1, time=time, return_phase=True)
         _, wavefunc = sim.simulate(tcircuit, return_statevector=True, initial_statevector=refwave)
         wavefunc *= phase
 
@@ -167,15 +167,15 @@
         # Generate initial wavefunction
         reference_circuit = Circuit([Gate("X", 0), Gate("X", 3)])
         _, refwave = sim.simulate(reference_circuit, return_statevector=True)
 
         # Exactly evolve for each time step
         evolve_exact = refwave
         for i in range(3):
-            ham_mat = get_sparse_operator(qubit_operator_list[i], n_qubits=4).toarray()
+            ham_mat = get_sparse_operator(qubit_operator_list[i].to_openfermion(), n_qubits=4).toarray()
             evolve_exact = expm(-1j * time[next(iter(qubit_operator_list[i].terms))] * ham_mat) @ evolve_exact
 
         # Apply trotter-suzuki with different times for each qubit operator term
         total_qubit_operator = QubitOperator()
         for qu_op in reversed(qubit_operator_list):
             total_qubit_operator += qu_op
         tcircuit, phase = trotterize(total_qubit_operator, trotter_order=2, n_trotter_steps=2, time=time, return_phase=True)
@@ -215,15 +215,15 @@
             for each term
         """
 
         # Generate qubit operator with state 9 having eigenvalue 0.25
         qu_op = (QubitOperator("X0 X1", 0.125) + QubitOperator("Y1 Y2", 0.125) + QubitOperator("Z2 Z3", 0.125)
                  + QubitOperator("", 0.125))
 
-        ham_mat = get_sparse_operator(qu_op).toarray()
+        ham_mat = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, wavefunction = eigh(ham_mat)
 
         # Append four qubits in the zero state to eigenvector 9
         wave_9 = wavefunction[:, 9]
         for i in range(4):
             wave_9 = np.kron(wave_9, np.array([1, 0]))
 
@@ -271,17 +271,17 @@
         """ Verify that tr(rho^3 pa) for a pauliword pa is correct.
         Uses the exponential error suppression circuit
         """
 
         qu_op = QubitOperator("X0 Y1", 0.125) + QubitOperator("Y1 Y2", 0.125) + QubitOperator("Z2 Z3", 0.125)
         pa = QubitOperator("X0 X1 X2 X3", 1)
 
-        ham_mat = get_sparse_operator(qu_op).toarray()
+        ham_mat = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, wavefunction = eigh(ham_mat)
-        pamat = get_sparse_operator(pa).toarray()
+        pamat = get_sparse_operator(pa.to_openfermion()).toarray()
 
         mixed_wave = np.sqrt(3)/2*wavefunction[:, -1] + 1/2*wavefunction[:, 0]
         mixed_wave_3 = np.kron(np.kron(mixed_wave, mixed_wave), mixed_wave)
         full_start_vec = np.kron(mixed_wave_3, np.array([1, 0]))
         rho = np.outer(mixed_wave, mixed_wave)
         rho3 = rho @ rho @ rho
         exact = np.trace(rho3 @ pamat)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_fermionic_operators.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_fermionic_operators.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_general_unitary_cc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_general_unitary_cc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_hea.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_hea.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_ilc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_ilc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_penalty_terms.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_penalty_terms.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_puccd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_puccd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_qcc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_qcc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_qmf.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_qmf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_rucc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_rucc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_uccgd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_uccgd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_uccsd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_uccsd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_upccgsd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_upccgsd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_variational_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_variational_circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/tests/test_vsqs.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_vsqs.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 import unittest
 import os
 
 import numpy as np
 from openfermion import load_operator
 
+from tangelo.linq import get_backend
 from tangelo.molecule_library import mol_H2_sto3g
 from tangelo.toolboxes.operators import QubitOperator
 from tangelo.toolboxes.qubit_mappings import jordan_wigner, symmetry_conserving_bravyi_kitaev
 from tangelo.toolboxes.ansatz_generator import VSQS
-from tangelo.linq import get_backend
 from tangelo.toolboxes.qubit_mappings.statevector_mapping import get_reference_circuit
 
 # For openfermion.load_operator function.
 pwd_this_test = os.path.dirname(os.path.abspath(__file__))
 
 
 class VSQSTest(unittest.TestCase):
@@ -67,25 +67,29 @@
         # Assert energy returned is as expected for given parameters
         sim = get_backend()
         vsqs_ansatz.update_var_params([0.66666667, 0.9698286, 0.21132472, 0.6465473])
         energy = sim.get_expectation_value(qubit_hamiltonian, vsqs_ansatz.circuit)
         self.assertAlmostEqual(energy, -1.1372701255155757, delta=1e-6)
 
     def test_vsqs_H4_doublecation(self):
-        """Verify closed-shell VSQS functionalities for H4 2+ by using saved qubit hamiltonian and initial hamiltonian"""
+        """ Verify closed-shell VSQS functionalities for H4 2+ by using saved qubit and initial hamiltonians """
 
         var_params = [-2.53957674, 0.72683888, 1.08799500, 0.49836183,
                       -0.23020698, 0.93278630, 0.50591026, 0.50486903]
 
-        # Build qubit hamiltonian for energy evaluation
-        qubit_hamiltonian = load_operator("mol_H4_doublecation_minao_qubitham_jw_b.data", data_directory=pwd_this_test+"/data", plain_text=True)
-        initial_hamiltonian = load_operator("mol_H4_doublecation_minao_init_qubitham_jw_b.data", data_directory=pwd_this_test+"/data", plain_text=True)
-        reference_state = get_reference_circuit(8, 2, "jw", up_then_down=True, spin=0)
+        # Build qubit hamiltonian for energy evaluation, loading them with Openfermion.
+        qubit_ofhamiltonian = load_operator("mol_H4_doublecation_minao_qubitham_jw_b.data", data_directory=pwd_this_test+"/data", plain_text=True)
+        initial_ofhamiltonian = load_operator("mol_H4_doublecation_minao_init_qubitham_jw_b.data", data_directory=pwd_this_test+"/data", plain_text=True)
+
+        # Load into Tangelo operators
+        qubit_hamiltonian = QubitOperator.from_openfermion(qubit_ofhamiltonian)
+        initial_hamiltonian = QubitOperator.from_openfermion(initial_ofhamiltonian)
 
         # Build circuit
+        reference_state = get_reference_circuit(8, 2, "jw", up_then_down=True, spin=0)
         vsqs_ansatz = VSQS(qubit_hamiltonian=qubit_hamiltonian, h_init=initial_hamiltonian, reference_state=reference_state,
                            intervals=5, time=5, trotter_order=2)
         vsqs_ansatz.build_circuit()
 
         # Assert energy returned is as expected for given parameters
         sim = get_backend()
         vsqs_ansatz.update_var_params(var_params)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/uccgd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/uccgd.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 Refs:
 
 """
 
 import numpy as np
 from openfermion import hermitian_conjugated
-from openfermion import FermionOperator as ofFermionOperator
 from itertools import combinations_with_replacement, product
 
 from tangelo.linq import Circuit
+from tangelo.toolboxes.operators import FermionOperator
 from tangelo.toolboxes.ansatz_generator.ansatz import Ansatz
 from tangelo.toolboxes.ansatz_generator.ansatz_utils import get_exponentiated_qubit_operator_circuit
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.qubit_mappings.statevector_mapping import get_reference_circuit
 
 
 class UCCGD(Ansatz):
@@ -176,30 +176,33 @@
     def _get_qubit_operator(self):
         """Construct UCCGD FermionOperator for variational
         parameters, and translate to QubitOperator via relevant qubit mapping.
 
         Returns:
             QubitOperator: qubit-encoded elements of the UCCGD
         """
-        fermion_op = ofFermionOperator()
+        fermion_op = FermionOperator()
         n_mos = self.n_spinorbitals // 2
         p = -1
         for indices in combinations_with_replacement(range(n_mos), 4):
             if len(set(indices)) >= 2:  # are they not all equal
                 u, w, v, t = indices
                 p = p + 1
                 for sig, tau in product(range(2), repeat=2):
-                    c_op = ofFermionOperator(((2*t+sig, 1), (2*v+tau, 1), (2*w+tau, 0), (2*u+sig, 0)), self.var_params[p])
-                    c_op += ofFermionOperator(((2*v+sig, 1), (2*t+tau, 1), (2*u+tau, 0), (2*w+sig, 0)), self.var_params[p])
+                    c_op = FermionOperator(((2*t+sig, 1), (2*v+tau, 1), (2*w+tau, 0), (2*u+sig, 0)), self.var_params[p])
+                    c_op += FermionOperator(((2*v+sig, 1), (2*t+tau, 1), (2*u+tau, 0), (2*w+sig, 0)), self.var_params[p])
                     fermion_op += c_op - hermitian_conjugated(c_op)
 
         qubit_op = fermion_to_qubit_mapping(fermion_operator=fermion_op,
                                             mapping=self.qubit_mapping,
                                             n_spinorbitals=self.n_spinorbitals,
                                             n_electrons=self.n_electrons,
                                             up_then_down=self.up_then_down)
 
+        print(type(fermion_op))
+        print(type(qubit_op))
+
         # Cast all coefs to floats (rotations angles are real)
         for key in qubit_op.terms:
             qubit_op.terms[key] = float(qubit_op.terms[key].imag)
         qubit_op.compress()
         return qubit_op
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/uccsd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/uccsd.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,26 +24,26 @@
         I. Tavernelli. Phys. Rev. A 98, 022322 (2018).
     - I.O. Sokolov, P.Kl. Barkoutsos, P.J. Ollitrault, D. Greenberg, J. Rice,
         M. Pistoia, and I. Tavernelli. J. Chem. Phys. 152, 124107 (2020).
     - Y. Shen, X. Zhang, S. Zhang, J.N. Zhang, M.H. Yung, and K. Kim.
         Physical Review A 95, 020501 (2017).
 """
 
-import itertools
 import numpy as np
-from pyscf import mp
 from openfermion.circuits import uccsd_singlet_generator
 
+from tangelo import SecondQuantizedMolecule
 from tangelo.linq import Circuit
-
-from .ansatz import Ansatz
-from .ansatz_utils import exp_pauliword_to_gates
-from ._unitary_cc_openshell import uccsd_openshell_paramsize, uccsd_openshell_generator, uccsd_openshell_get_packed_amplitudes
+from tangelo.helpers.utils import is_package_installed
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.qubit_mappings.statevector_mapping import get_reference_circuit
+from tangelo.toolboxes.molecular_computation import IntegralSolverPySCF
+from .ansatz import Ansatz
+from .ansatz_utils import exp_pauliword_to_gates
+from ._unitary_cc_openshell import uccsd_openshell_paramsize, uccsd_openshell_generator
 
 
 class UCCSD(Ansatz):
     """This class implements the UCCSD ansatz. Currently, closed-shell and
     restricted open-shell UCCSD are supported. This implies that the mean-field
     is computed with the RHF or ROHF reference integrals.
 
@@ -92,19 +92,18 @@
         # set total number of parameters
         self.n_var_params = self.n_singles + self.n_doubles
 
         # Supported reference state initialization
         # TODO: support for others
         self.supported_reference_state = {"HF", "zero"}
         # Supported var param initialization
-        self.supported_initial_var_params = {"ones", "random", "mp2"} if (self.spin == 0 and not self.molecule.uhf) else {"ones", "random"}
+        self.supported_initial_var_params = {"ones", "random", "mp2"}
 
         # Default initial parameters for initialization
-        # TODO: support for openshell MP2 initialization
-        self.var_params_default = "mp2" if (self.spin == 0 and not self.molecule.uhf) else "ones"
+        self.var_params_default = "mp2"
         self.reference_state = reference_state
 
         self.var_params = None
         self.circuit = None
 
     def set_var_params(self, var_params=None):
         """Set values for variational parameters, such as zeros, random numbers,
@@ -248,36 +247,39 @@
         # Cast all coefs to floats (rotations angles are real)
         for key in qubit_op.terms:
             qubit_op.terms[key] = float(qubit_op.terms[key].imag)
         qubit_op.compress()
         return qubit_op
 
     def _compute_mp2_params(self):
-        """Computes the MP2 initial variational parameters. Compute the initial
-        variational parameters with PySCF MP2 calculation, and then reorders the
-        elements into the appropriate convention. MP2 only has doubles (T2)
-        amplitudes, thus the single (T1) amplitudes are set to a small non-zero
-        value and added. The ordering is single, double (diagonal), double
-        (non-diagonal).
+        """Compute the MP2 initial variational parameters. Only double
+        excitation amplitudes are retrieved from an MP2 calculation (singles
+        set to a small number close to 0).
 
         Returns:
             list of float: The initial variational parameters.
         """
-        if self.molecule.uhf:
-            raise NotImplementedError(f"MP2 initialization is not currently implemented for UHF reference in {self.__class__}")
-
-        mp2_fragment = mp.MP2(self.molecule.mean_field, frozen=self.molecule.frozen_mos)
-        mp2_fragment.verbose = 0
-        _, mp2_t2 = mp2_fragment.kernel()
 
-        # Get singles amplitude. Just get "up" amplitude, since "down" should be the same
-        singles = [2.e-5] * (self.n_virtual * self.n_occupied)
-
-        # Get singles and doubles amplitudes associated with one spatial occupied-virtual pair
-        doubles_1 = [-mp2_t2[q, q, p, p]/2. if (abs(-mp2_t2[q, q, p, p]/2.) > 1e-15) else 0.
-                     for p, q in itertools.product(range(self.n_virtual), range(self.n_occupied))]
+        if not is_package_installed("pyscf"):
+            supported_initial_var_params = self.supported_initial_var_params.copy()
+            supported_initial_var_params.remove("mp2")
+            raise ValueError(f"PySCF is required for MP2 initial parameters in {self.__class__.__name__}.\n"
+                             f"Other supported keywords for initializing variational parameters are {supported_initial_var_params}. "
+                             f"An array of floats of length {self.n_var_params} can also be provided.\n"
+                             f"The above keywords or array can also be provided to variational algorithms through the 'initial_var_params' keyword.")
+
+        # Import here to solve an AttributeError: partially initialized module
+        # tangelo.toolboxes.ansatz_generator' has no attribute 'UCCSD'
+        # (most likely due to a circular import).
+        from tangelo.algorithms.classical.mp2_solver import MP2Solver
+
+        if not isinstance(self.molecule.solver, IntegralSolverPySCF):
+            pymol = SecondQuantizedMolecule(self.molecule.xyz, self.molecule.q, self.molecule.spin, basis=self.molecule.basis,
+                                            ecp=self.molecule.ecp, symmetry=self.molecule.symmetry, uhf=self.molecule.uhf,
+                                            frozen_orbitals=self.molecule.frozen_orbitals)
+        else:
+            pymol = self.molecule
 
-        # Get doubles amplitudes associated with two spatial occupied-virtual pairs
-        doubles_2 = [-mp2_t2[q, s, p, r] for (p, q), (r, s)
-                     in itertools.combinations(itertools.product(range(self.n_virtual), range(self.n_occupied)), 2)]
+        mp2 = MP2Solver(pymol)
+        mp2.simulate()
 
-        return singles + doubles_1 + doubles_2
+        return mp2.get_mp2_amplitudes()
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/upccgsd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/upccgsd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/variational_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/variational_circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/ansatz_generator/vsqs.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/vsqs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module defines the Variationally Scheduled Quantum Simulation class. It provides an
 Adiabatic State Preparation (ASP) inspired ansatz as described in https://arxiv.org/abs/2003.09913."""
 
 import numpy as np
-from openfermion import QubitOperator as ofQubitOperator
 
 from .ansatz import Ansatz
 from .ansatz_utils import get_exponentiated_qubit_operator_circuit
-from tangelo.toolboxes.operators import FermionOperator
 from tangelo.linq import Circuit
+from tangelo.toolboxes.operators import FermionOperator, QubitOperator
 from tangelo.toolboxes.qubit_mappings.mapping_transform import get_qubit_number, fermion_to_qubit_mapping
 from tangelo.toolboxes.qubit_mappings.statevector_mapping import get_reference_circuit
 
 
 class VSQS(Ansatz):
     """This class implements the Variationally Scheduled Quantum Simulator (VSQS) for state preparation as described in
     https://arxiv.org/abs/2003.09913
@@ -64,15 +63,15 @@
         if trotter_order in [1, 2]:
             self.trotter_order = trotter_order
         else:
             raise ValueError("Only trotter_order = 1, 2 is supported")
 
         if molecule is None:
             self.qubit_hamiltonian = qubit_hamiltonian
-            if not isinstance(h_init, ofQubitOperator):
+            if not isinstance(h_init, QubitOperator):
                 raise ValueError("When providing a qubit hamiltonian, an initial qubit Hamiltonian must also be provided")
             self.h_init = h_init
             if not isinstance(reference_state, Circuit):
                 raise ValueError("Reference state Circuit must be provided when simulating a qubit hamiltonian directly")
             self.reference_state = reference_state
         else:
             if molecule.uhf:
@@ -98,15 +97,15 @@
         self.n_h_final = len(self.h_final_list)
         self.h_init_list = qu_op_to_list(self.h_init)
         self.n_h_init = len(self.h_init_list)
         if self.h_nav is None:
             self.stride = 2
             self.n_h_nav = 0
         else:
-            if isinstance(self.h_nav, ofQubitOperator):
+            if isinstance(self.h_nav, QubitOperator):
                 self.stride = 3
                 self.h_nav_list = qu_op_to_list(self.h_nav)
                 self.n_h_nav = len(self.h_nav_list)
             else:
                 raise ValueError("Navigator Hamiltonian must be a QubitOperator")
 
         self.n_var_params = (intervals - 1) * self.stride
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,8 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .diagonal_coulomb import get_orbital_rotations
+from .operators import FermionOperator, QubitOperator, QubitHamiltonian, BosonOperator
+from .operators import count_qubits, normal_ordered, squared_normal_ordered, list_to_fermionoperator, qubitop_to_qubitham
+from .multiformoperator import MultiformOperator
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/diagonal_coulomb.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/diagonal_coulomb.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/discrete_clock.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/discrete_clock.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/grid_circuits.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/grid_circuits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/lcu.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/lcu.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/multiproduct.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/multiproduct.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/qsp.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/qsp.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_diagonal_coulomb.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_diagonal_coulomb.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
-from openfermion import get_sparse_operator, linalg
+from openfermion import linalg, get_sparse_operator
 
 from tangelo.linq import get_backend, Circuit
 from tangelo.molecule_library import mol_H4_sto3g
 from tangelo.toolboxes.circuits import get_orbital_rotations
 
 # Initiate simulator using cirq as it has the same ordering as openfermion and we are using an exact eigenvector to test
 sim = get_backend(target="cirq")
 
 
-class diagonal_coulomb_Test(unittest.TestCase):
+class DiagonalCoulombTest(unittest.TestCase):
 
     def test_orbital_rotations(self):
         """Test calculating energy expectation value of H4 hamiltonian by decomposing into diagional terms"""
 
         # Generate ground state wavefunction from JW transformed fermionic_hamiltonian
         ham = get_sparse_operator(mol_H4_sto3g.fermionic_hamiltonian)
         eig, state_vec = linalg.get_ground_state(ham)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_discrete_clock.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_discrete_clock.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 import math
 
-from openfermion import get_sparse_operator
 import numpy as np
 from scipy.linalg import expm
+from openfermion import get_sparse_operator
 
-from tangelo.linq import get_backend, Circuit
+from tangelo.molecule_library import mol_H2_sto3g
 from tangelo.helpers.utils import installed_backends
+from tangelo.linq import get_backend, Circuit
 from tangelo.linq.helpers.circuits.statevector import StateVector
-from tangelo.toolboxes.operators.operators import QubitOperator
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
-from tangelo.toolboxes.ansatz_generator.ansatz_utils import get_qft_circuit, trotterize
-from tangelo.molecule_library import mol_H2_sto3g
+from tangelo.toolboxes.ansatz_generator.ansatz_utils import trotterize
 from tangelo.toolboxes.circuits.discrete_clock import get_discrete_clock_circuit
 from tangelo.toolboxes.circuits.grid_circuits import get_psquared_circuit, get_xsquared_circuit
 
 # Test for both "cirq" and if available "qulacs". These have different orderings.
 # qiskit is not currently supported because does not have multi controlled general gates.
 backends = ["cirq", "qulacs"] if "qulacs" in installed_backends else ["cirq"]
 # Initiate Simulator using cirq for phase estimation tests as it has the same ordering as openfermion
@@ -41,15 +40,15 @@
 
     def test_time_independant_hamiltonian(self):
         """Test time-evolution of discrete clock for a time-independant Hamiltonian"""
 
         qu_op = fermion_to_qubit_mapping(mol_H2_sto3g.fermionic_hamiltonian, "scbk", mol_H2_sto3g.n_active_sos, mol_H2_sto3g.n_active_electrons,
                                          True, 0)
 
-        ham = get_sparse_operator(qu_op).toarray()
+        ham = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, vecs = np.linalg.eigh(ham)
         vec = (vecs[:, 0] + vecs[:, 1])/np.sqrt(2)
 
         time = 10.
         exact = expm(-1j*ham*time)@vec
 
         def trotter_func(t0, time, n_trotter_steps, control):
@@ -58,16 +57,16 @@
         for backend in backends:
             sim = get_backend(backend)
             statevector_order = sim.backend_info()["statevector_order"]
             sv = StateVector(vec, order=statevector_order)
             sv_circuit = sv.initializing_circuit()
 
             for k in [2, 3]:
-                taylor_circuit = get_discrete_clock_circuit(trotter_func=trotter_func, trotter_kwargs={}, time=time, mp_order=k, n_state_qus=2,
-                                                            n_time_steps=4)
+                taylor_circuit = get_discrete_clock_circuit(trotter_func=trotter_func, trotter_kwargs={},
+                                                            time=time, mp_order=k, n_state_qus=2, n_time_steps=4)
                 _, v = sim.simulate(sv_circuit + taylor_circuit, return_statevector=True)
                 n_ancilla = 2 + math.ceil(np.log2(k+2))
                 len_ancilla = 2**n_ancilla
                 v = v.reshape([4, len_ancilla])[:, 0] if statevector_order == "lsq_first" else v.reshape([len_ancilla, 4])[0, :]
                 self.assertAlmostEqual(1, np.abs(v.conj().dot(exact)), delta=1.e-1**k)
 
     def test_time_dependant_hamiltonian(self):
@@ -104,17 +103,17 @@
             statevector_order = sim.backend_info()["statevector_order"]
             vec = psiexact(gridpts, 0)
             sv = StateVector(vec, order=statevector_order)
             sv_circuit, phase = sv.initializing_circuit(return_phase=True)
 
             for k in [2, 3]:
                 qubit_list = list(reversed(range(n_qubits))) if statevector_order == "lsq_first" else list((range(n_qubits)))
-                taylor_circuit = get_discrete_clock_circuit(trotter_func=trotter_func, trotter_kwargs={"dx": dx, "qubit_list": qubit_list}, time=time,
-                                                            mp_order=k, n_state_qus=6,
-                                                            n_time_steps=2)
+                taylor_circuit = get_discrete_clock_circuit(trotter_func=trotter_func,
+                                                            trotter_kwargs={"dx": dx, "qubit_list": qubit_list}, time=time,
+                                                            mp_order=k, n_state_qus=6, n_time_steps=2)
                 _, v = sim.simulate(sv_circuit + taylor_circuit, return_statevector=True)
                 n_ancilla = 1 + math.ceil(np.log2(k+2))
                 len_ancilla = 2**n_ancilla
                 v = v.reshape([n_pts, len_ancilla])[:, 0] if statevector_order == "lsq_first" else v.reshape([len_ancilla, n_pts])[0, :]
                 self.assertAlmostEqual(1, (v.conj().dot(exact)*np.exp(-1j*phase)).real, delta=1.e-1**k)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_grid.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_grid.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
-import math
 
-from openfermion import get_sparse_operator
 import numpy as np
-from scipy.linalg import expm
 
 from tangelo.linq import get_backend
 from tangelo.linq.helpers.circuits.statevector import StateVector
 from tangelo.helpers.utils import installed_backends
 from tangelo.toolboxes.ansatz_generator.ansatz_utils import get_qft_circuit
 from tangelo.toolboxes.post_processing.histogram import Histogram
 from tangelo.toolboxes.circuits.grid_circuits import get_psquared_circuit, get_xsquared_circuit
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_lcu.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_lcu.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 import math
 
-from openfermion import get_sparse_operator
 import numpy as np
 from scipy.linalg import expm
+from openfermion import get_sparse_operator
 
 from tangelo.linq import get_backend
 from tangelo.helpers.utils import installed_backends
 from tangelo.linq.helpers.circuits.statevector import StateVector
 from tangelo.toolboxes.operators.operators import QubitOperator
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.ansatz_generator.ansatz_utils import get_qft_circuit
@@ -32,23 +32,23 @@
 # qiskit is not currently supported because does not have multi controlled general gates.
 backends = ["cirq", "qulacs"] if "qulacs" in installed_backends else ["cirq"]
 # Initiate Simulator using cirq for phase estimation tests as it has the same ordering as openfermion
 # and we are using an exact eigenvector for testing.
 sim_cirq = get_backend("cirq")
 
 
-class lcu_Test(unittest.TestCase):
+class LCUTest(unittest.TestCase):
 
     def test_get_truncated_taylor_series(self):
         """Test time-evolution of truncated Taylor series for different orders and times"""
 
         qu_op = fermion_to_qubit_mapping(mol_H2_sto3g.fermionic_hamiltonian, "scbk", mol_H2_sto3g.n_active_sos, mol_H2_sto3g.n_active_electrons,
                                          True, 0)
         n_qubits_qu_op = math.ceil(math.log2(len(qu_op.terms)))
-        ham = get_sparse_operator(qu_op).toarray()
+        ham = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, vecs = np.linalg.eigh(ham)
         vec = (vecs[:, 0] + vecs[:, 1])/np.sqrt(2)
 
         time = 1.9
         exact = expm(-1j*ham*time)@vec
 
         for backend in backends:
@@ -61,29 +61,31 @@
             for k in [1, 2, 3, 4]:
                 taylor_circuit = get_truncated_taylor_series(qu_op, k, time)
                 _, v = sim.simulate(sv_circuit + taylor_circuit, return_statevector=True)
                 len_ancilla = 2**(k+k*n_qubits_qu_op+1)
                 v = v.reshape([4, len_ancilla])[:, 0] if statevector_order == "lsq_first" else v.reshape([len_ancilla, 4])[0, :]
                 self.assertAlmostEqual(1, np.abs(v.conj().dot(exact)), delta=3.e-1**k)
 
-        # Raise ValueError if Taylor series order is less than 1 or greater than 4 or imaginary coefficients in qubit operator
+        # Raise ValueError if Taylor series order is less than 1 or greater than 4
+        # or imaginary coefficients in qubit operator
         self.assertRaises(ValueError, get_truncated_taylor_series, qu_op, 0, time)
         self.assertRaises(ValueError, get_truncated_taylor_series, qu_op * 1j, 2, time)
 
     def test_get_oaa_lcu_circuit(self):
-        """Test time-evolution of truncated Taylor series for order k = 3 passing explicitly calculated qubit operator exponential"""
+        """Test time-evolution of truncated Taylor series for order k = 3 passing explicitly calculated
+        qubit operator exponential"""
 
-        qu_op = fermion_to_qubit_mapping(mol_H2_sto3g.fermionic_hamiltonian, "scbk", mol_H2_sto3g.n_active_sos, mol_H2_sto3g.n_active_electrons,
-                                         True, 0)
+        qu_op = fermion_to_qubit_mapping(mol_H2_sto3g.fermionic_hamiltonian, "scbk",
+                                         mol_H2_sto3g.n_active_sos, mol_H2_sto3g.n_active_electrons, True, 0)
         time = 0.5
         # Generate explicit qubit operator exponential
         exp_qu_op = 1 + -1j*qu_op*time + (-1j*qu_op*time)**2/2 + (-1j*qu_op*time)**3/6
         exp_qu_op.compress()
         n_qubits_qu_op = math.ceil(math.log2(len(exp_qu_op.terms)))
-        ham = get_sparse_operator(qu_op).toarray()
+        ham = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, vecs = np.linalg.eigh(ham)
         vec = (vecs[:, 0] + vecs[:, 1])/np.sqrt(2)
 
         exact = expm(-1j*ham*time)@vec
         len_ancilla = 2**(n_qubits_qu_op)
 
         for backend in backends:
@@ -105,15 +107,15 @@
         phase estimation.
         """
 
         # Generate qubit operator with state 9 having eigenvalue 0.25
         qu_op = (QubitOperator("X0 X1", 0.125) + QubitOperator("Y1 Y2", 0.125) + QubitOperator("Z2 Z3", 0.125)
                  + QubitOperator("", 0.125))
 
-        ham_mat = get_sparse_operator(qu_op).toarray()
+        ham_mat = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, wavefunction = np.linalg.eigh(ham_mat)
 
         # Kronecker product 13 qubits in the zero state to eigenvector 9 to account for ancilla qubits
         wave_9 = wavefunction[:, 9]
         for i in range(13):
             wave_9 = np.kron(wave_9, np.array([1, 0]))
 
@@ -139,15 +141,15 @@
         phase estimation.
         """
 
         # Generate qubit operator with state 9 having eigenvalue 0.25
         qu_op = (QubitOperator("X0 X1", 0.125) + QubitOperator("Y1 Y2", 0.125) + QubitOperator("Z2 Z3", 0.125)
                  + QubitOperator("", 0.125))
 
-        ham_mat = get_sparse_operator(qu_op).toarray()
+        ham_mat = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, wavefunction = np.linalg.eigh(ham_mat)
 
         # break time into 6 parts so 1-norm is less than 2. i.e. can use Oblivious Amplitude Amplification
         time = -2 * np.pi / 6
 
         # Generate explicit qubit operator exponential
         exp_qu_op = 1 + -1j*qu_op*time + (-1j*qu_op*time)**2/2 + (-1j*qu_op*time)**3/6
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_mp.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
-import math
 
-from openfermion import get_sparse_operator
 import numpy as np
 from scipy.linalg import expm
+from openfermion import get_sparse_operator
 
 from tangelo.linq import get_backend
 from tangelo.helpers.utils import installed_backends
 from tangelo.linq.helpers.circuits.statevector import StateVector
 from tangelo.toolboxes.operators.operators import QubitOperator
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.ansatz_generator.ansatz_utils import get_qft_circuit
@@ -37,18 +36,19 @@
 
 
 class MultiProductTest(unittest.TestCase):
 
     def test_time_evolution(self):
         """Test time-evolution of multi-product circuit for different orders"""
 
-        qu_op = fermion_to_qubit_mapping(mol_H2_sto3g.fermionic_hamiltonian, "scbk", mol_H2_sto3g.n_active_sos, mol_H2_sto3g.n_active_electrons,
+        qu_op = fermion_to_qubit_mapping(mol_H2_sto3g.fermionic_hamiltonian, "scbk",
+                                         mol_H2_sto3g.n_active_sos, mol_H2_sto3g.n_active_electrons,
                                          True, 0)
 
-        ham = get_sparse_operator(qu_op).toarray()
+        ham = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, vecs = np.linalg.eigh(ham)
         vec = (vecs[:, 0] + vecs[:, 1])/np.sqrt(2)
 
         time = 1.9
         exact = expm(-1j*ham*time)@vec
 
         for backend in backends:
@@ -77,27 +77,28 @@
         phase estimation.
         """
 
         # Generate qubit operator with state 9 having eigenvalue 0.25
         qu_op = (QubitOperator("X0 X1", 0.125) + QubitOperator("Y1 Y2", 0.125) + QubitOperator("Z2 Z3", 0.125)
                  + QubitOperator("", 0.125))
 
-        ham_mat = get_sparse_operator(qu_op).toarray()
+        ham_mat = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, wavefunction = np.linalg.eigh(ham_mat)
 
         # Kronecker product 13 qubits in the zero state to eigenvector 9 to account for ancilla qubits
         wave_9 = wavefunction[:, 9]
         for i in range(6):
             wave_9 = np.kron(wave_9, np.array([1, 0]))
 
         qubit_list = [9, 8, 7]
 
         pe_circuit = get_qft_circuit(qubit_list)
         for i, qubit in enumerate(qubit_list):
-            pe_circuit += get_multi_product_circuit(operator=qu_op, n_state_qus=4, order=5, time=-(2*np.pi)*2**i, control=qubit)
+            pe_circuit += get_multi_product_circuit(operator=qu_op, n_state_qus=4, order=5,
+                                                    time=-(2*np.pi)*2**i, control=qubit)
         pe_circuit += get_qft_circuit(qubit_list, inverse=True)
 
         freqs, _ = sim_cirq.simulate(pe_circuit, initial_statevector=wave_9)
         # Trace out all but final 3 indices
         trace_freq = dict()
         for key, value in freqs.items():
             trace_freq[key[-3:]] = trace_freq.get(key[-3:], 0) + value
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/circuits/tests/test_qsp.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_qsp.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,46 +10,46 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
-from openfermion import get_sparse_operator
 import numpy as np
 from scipy.linalg import expm
+from openfermion import get_sparse_operator
 
 from tangelo.linq import get_backend, backend_info
 from tangelo.helpers.utils import installed_backends
 from tangelo.linq.helpers.circuits.statevector import StateVector
-from tangelo.toolboxes.operators.operators import QubitOperator
+from tangelo.toolboxes.operators import QubitOperator
 from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping
 from tangelo.toolboxes.ansatz_generator.ansatz_utils import get_qft_circuit
 from tangelo.molecule_library import mol_H2_sto3g
 from tangelo.toolboxes.circuits.lcu import get_lcu_qubit_op_info
 from tangelo.toolboxes.circuits.qsp import get_qsp_hamiltonian_simulation_circuit, get_qsp_hamiltonian_simulation_qubit_list
 
 # Test for both "cirq" and if available "qulacs". These have different orderings.
 # qiskit is not currently supported because does not have multi controlled general gates.
 backends = ["cirq", "qulacs"] if "qulacs" in installed_backends else ["cirq"]
 # Initiate Simulator using cirq for phase estimation tests as it has the same ordering as openfermion
 # and we are using an exact eigenvector for testing.
 sim_cirq = get_backend("cirq")
 
 
-class lcu_Test(unittest.TestCase):
+class QSPTest(unittest.TestCase):
 
     def test_get_qsp_circuit(self):
         """Test QSP time-evolution"""
 
-        qu_op = fermion_to_qubit_mapping(mol_H2_sto3g.fermionic_hamiltonian, "scbk", mol_H2_sto3g.n_active_sos, mol_H2_sto3g.n_active_electrons,
-                                         True, 0)
+        qu_op = fermion_to_qubit_mapping(mol_H2_sto3g.fermionic_hamiltonian, "scbk",
+                                         mol_H2_sto3g.n_active_sos, mol_H2_sto3g.n_active_electrons, True, 0)
         # need to ensure eigenvalues are between -1 and 1
         qu_op /= 1.2
-        ham = get_sparse_operator(qu_op).toarray()
+        ham = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, vecs = np.linalg.eigh(ham)
         vec = (vecs[:, 0] + vecs[:, 2])/np.sqrt(2)
 
         time = 1.9
         exact = expm(-1j*ham*time)@vec
 
         for backend in backends:
@@ -72,15 +72,15 @@
         phase estimation.
         """
 
         # Generate qubit operator with state 9 having eigenvalue 0.25
         qu_op = (QubitOperator("X0 X1", 0.125) + QubitOperator("Y1 Y2", 0.125) + QubitOperator("Z2 Z3", 0.125)
                  + QubitOperator("", 0.125))
 
-        ham_mat = get_sparse_operator(qu_op).toarray()
+        ham_mat = get_sparse_operator(qu_op.to_openfermion()).toarray()
         _, wavefunction = np.linalg.eigh(ham_mat)
 
         # Kronecker product 13 qubits in the zero state to eigenvector 9 to account for ancilla qubits
         wave_9 = wavefunction[:, 9]
         for i in range(8):
             wave_9 = np.kron(wave_9, np.array([1, 0]))
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/adaptive.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/adaptive.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/classical_shadows.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/classical_shadows.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/derandomized.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/derandomized.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/classical_shadows/randomized.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/randomized.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/estimate_measurements.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/estimate_measurements.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/qubit_terms_grouping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/qubit_terms_grouping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_adaptive_classical_shadows.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_adaptive_classical_shadows.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_measurements.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_measurements.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import unittest
 import os
 from openfermion import load_operator
 
 from tangelo.helpers.utils import default_simulator
-from tangelo.linq import translator, get_backend, Circuit
+from tangelo.linq import translate_circuit, get_backend, Circuit
 from tangelo.linq.helpers import measurement_basis_gates
 from tangelo.toolboxes.operators import QubitOperator
 from tangelo.toolboxes.measurements import get_measurement_estimate
 
 path_data = os.path.dirname(os.path.abspath(__file__)) + '/data'
 
 op1 = 1. * QubitOperator('X1 Y0')
@@ -73,15 +73,15 @@
     def test_measurement_uniform_H2(self):
         """ Test on UCCSD H2 usecase that uniform measurement estimation method guarantees on average the level
         of accuracy expected by the user """
 
         # Load state preparation circuit
         with open(f"{path_data}/H2_UCCSD.qasm", "r") as f:
             openqasm_circ = f.read()
-        abs_circ = translator._translate_openqasm2abs(openqasm_circ)
+        abs_circ = translate_circuit(openqasm_circ, source="openqasm", target="tangelo")
 
         # Load qubit Hamiltonian
         qb_ham = load_operator("mol_H2_qubitham.data", data_directory=path_data, plain_text=True)
 
         # Get exact expectation value using a simulator
         sim_exact = get_backend()
         freqs_exact, _ = sim_exact.simulate(abs_circ)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 import os
 
 from openfermion import load_operator
-from openfermion.ops import QubitOperator
 
-from tangelo.linq import translator, get_backend, Circuit
+from tangelo.linq import translate_circuit, get_backend, Circuit
 from tangelo.helpers import measurement_basis_gates
+from tangelo.toolboxes.operators import QubitOperator
 from tangelo.toolboxes.measurements import group_qwc, exp_value_from_measurement_bases, \
     check_bases_commute_qwc, map_measurements_qwc
 
 path_data = os.path.dirname(os.path.abspath(__file__)) + '/data'
 
 
 class TermsGroupingTest(unittest.TestCase):
@@ -93,15 +93,15 @@
 
         # Group Hamiltonian terms using qubitwise commutativity
         grouped_ops = group_qwc(qb_ham, seed=0)
 
         # Load an optimized quantum circuit (UCCSD) to compute something meaningful in this test
         with open(f"{path_data}/H2_UCCSD.qasm", "r") as f:
             openqasm_circ = f.read()
-        abs_circ = translator._translate_openqasm2abs(openqasm_circ)
+        abs_circ = translate_circuit(openqasm_circ, source="openqasm", target="tangelo")
 
         # Only simulate and measure the wavefunction in the required bases (simulator or QPU), store in dict.
         histograms = dict()
         sim = get_backend()
         for basis, sub_op in grouped_ops.items():
             full_circuit = abs_circ + Circuit(measurement_basis_gates(basis))
             histograms[basis], _ = sim.simulate(full_circuit)
@@ -121,15 +121,15 @@
 
         # Group Hamiltonian terms using qubitwise commutativity
         grouped_ops = group_qwc(qb_ham, seed=0)
 
         # Load an optimized quantum circuit (UCCSD) to compute something meaningful in this test
         with open(f"{path_data}/H4_UCCSD.qasm", "r") as f:
             openqasm_circ = f.read()
-        abs_circ = translator._translate_openqasm2abs(openqasm_circ)
+        abs_circ = translate_circuit(openqasm_circ, source="openqasm", target="tangelo")
 
         # Only simulate and measure the wavefunction in the required bases (simulator or QPU), store in dict.
         histograms = dict()
         sim = get_backend()
         for basis, sub_op in grouped_ops.items():
             full_circuit = abs_circ + Circuit(measurement_basis_gates(basis))
             histograms[basis], _ = sim.simulate(full_circuit)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/coefficients.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/coefficients.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/frozen_orbitals.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/frozen_orbitals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 """This module defines functions to get suggestions for freezing orbitals. Those
 functions take a molecule and return an integer or a list of orbital indices for
 freezing orbitals. Depending on the function, a Molecule or a
 SecondQuantizedMolecule object can be used.
 """
 
+from collections import Counter
+
 import numpy as np
 
 
 def get_frozen_core(molecule):
     """Function to compute the number of frozen orbitals. This function is only
     for the core (occupied orbitals).
 
@@ -39,15 +41,15 @@
     core_orbitals = {
         "H": 0, "He": 0,
         "Li": 1, "Be": 1, "B": 1, "C": 1, "N": 1, "O": 1, "F": 1, "Ne": 1,
         "Na": 5, "Mg": 5, "Al": 5, "Si": 5, "P": 5, "S": 5, "Cl": 5, "Ar": 5
     }
 
     # Counting how many of each element is in the molecule.
-    elements = {i: molecule.elements.count(i) for i in molecule.elements}
+    elements = Counter([e[0] for e in molecule.xyz])
     frozen_core = sum([v * core_orbitals.get(k, 0) for k, v in elements.items()])
 
     return frozen_core
 
 
 def get_orbitals_excluding_homo_lumo(molecule, homo_minus_n=0, lumo_plus_n=0):
     """Function that returns a list of orbitals to freeze if the user wants to
@@ -93,15 +95,15 @@
 
     Returns:
         tuple of list: Active occupied, frozen occupied, active virtual and
             frozen virtual orbital indices.
     """
 
     if frozen_orbitals == "frozen_core":
-        frozen_orbitals = get_frozen_core(sec_mol.to_pyscf(sec_mol.basis)) if not sec_mol.ecp else 0
+        frozen_orbitals = get_frozen_core(sec_mol) if not sec_mol.ecp else 0
     elif frozen_orbitals is None:
         frozen_orbitals = 0
 
     # First case: frozen_orbitals is an int.
     # The first n MOs are frozen.
     if isinstance(frozen_orbitals, (int, np.integer)):
         frozen_orbitals = list(range(frozen_orbitals))
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/molecule.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/molecule.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 """
 
 import copy
 from dataclasses import dataclass, field
 from itertools import product
 
 import numpy as np
-from pyscf import gto, scf, ao2mo, symm, lib
 import openfermion
 import openfermion.ops.representations as reps
 from openfermion.utils import down_index, up_index
 from openfermion.chem.molecular_data import spinorb_from_spatial
 from openfermion.ops.representations.interaction_operator import get_active_space_integrals as of_get_active_space_integrals
 
+from tangelo.helpers.utils import is_package_installed
+from tangelo.toolboxes.molecular_computation import IntegralSolver, IntegralSolverPsi4, IntegralSolverEmpty
+from tangelo.toolboxes.molecular_computation.integral_solver_pyscf import mol_to_pyscf, IntegralSolverPySCF
 from tangelo.toolboxes.molecular_computation.frozen_orbitals import convert_frozen_orbitals
 from tangelo.toolboxes.qubit_mappings.mapping_transform import get_fermion_operator
 
 
 def atom_string_to_list(atom_string):
     """Convert atom coordinate string (typically stored in text files) into a
     list/tuple representation suitable for openfermion.MolecularData.
@@ -74,78 +76,74 @@
 
     Attributes:
         xyz (array-like or string): Nested array-like structure with elements
             and coordinates (ex:[ ["H", (0., 0., 0.)], ...]). Can also be a
             multi-line string.
         q (float): Total charge.
         spin (int): Absolute difference between alpha and beta electron number.
+        solver (IntegralSolver): The class that performs the mean field and integral computation.
         n_atom (int): Self-explanatory.
         n_electrons (int): Self-explanatory.
         n_min_orbitals (int): Number of orbitals with a minimal basis set.
 
     Properties:
         elements (list): List of all elements in the molecule.
         coords (array of float): N x 3 coordinates matrix.
     """
     xyz: list or str
     q: int = 0
     spin: int = 0
+    if is_package_installed("pyscf"):
+        default_solver = IntegralSolverPySCF
+    elif is_package_installed("psi4"):
+        default_solver = IntegralSolverPsi4
+    else:
+        default_solver = IntegralSolverEmpty
+
+    solver: IntegralSolver = field(default_factory=default_solver)
 
     # Defined in __post_init__.
     n_atoms: int = field(init=False)
     n_electrons: int = field(init=False)
 
     def __post_init__(self):
-        mol = self.to_pyscf()
-        self.n_atoms = mol.natm
-        self.n_electrons = mol.nelectron
+        if isinstance(self.solver, IntegralSolverEmpty):
+            raise ValueError("PySCF or Psi4 must be installed or a custom solver (IntegralSolver) instance must be provided.")
+        self.solver.set_physical_data(self)
 
     @property
     def elements(self):
+        """(list): List of all elements in the molecule."""
         return [self.xyz[i][0] for i in range(self.n_atoms)]
 
     @property
     def coords(self):
+        """(array of float): N x 3 coordinates matrix."""
         return np.array([self.xyz[i][1] for i in range(self.n_atoms)])
 
-    def to_pyscf(self, basis="CRENBL", symmetry=False, ecp=None):
-        """Method to return a pyscf.gto.Mole object.
-
-        Args:
-            basis (string): Basis set.
-            symmetry (bool): Flag to turn symmetry on
-            ecp (dict): Dictionary with ecp definition for each atom e.g. {"Cu": "crenbl"}
-
-        Returns:
-            pyscf.gto.Mole: PySCF compatible object.
-        """
-
-        mol = gto.Mole(atom=self.xyz)
-        mol.basis = basis
-        mol.charge = self.q
-        mol.spin = self.spin
-        mol.symmetry = symmetry
-        mol.ecp = ecp if ecp else dict()
-        mol.build()
-
-        self.xyz = list()
-        for sym, xyz in mol._atom:
-            self.xyz += [tuple([sym, tuple([x*lib.parameters.BOHR for x in xyz])])]
-
-        return mol
-
     def to_file(self, filename, format=None):
         """Write molecule geometry to filename in specified format
 
         Args:
             filename (str): The name of the file to output the geometry.
             format (str): The output type of "raw", "xyz", or "zmat". If None, will be inferred by the filename
+                Unless using IntegralSolverPySCF, only "xyz" is supported.
         """
-        mol = self.to_pyscf()
-        mol.tofile(filename, format)
+        if isinstance(self.solver, IntegralSolverPySCF):
+            mol = mol_to_pyscf(self)
+            mol.tofile(filename, format)
+        elif filename[-3:] == 'xyz' or format == 'xyz':
+            f = open(filename, "w") if format is None else open(filename+".xyz", "w")
+            f.write(f"{self.n_atoms}\n")
+            f.write("XYZ from Tangelo\n")
+            for name, positions in self.xyz:
+                f.write(f"{name} {positions[0]} {positions[1]} {positions[2]}\n")
+            f.close
+        else:
+            raise ValueError("Tangelo only supports xyz format unless using IntegralSolverPySCF")
 
     def to_openfermion(self, basis="sto-3g"):
         """Method to return a openfermion.MolecularData object.
 
         Args:
             basis (string): Basis set.
 
@@ -207,27 +205,25 @@
     frozen_orbitals: list or int = field(default="frozen_core", repr=False)
 
     # Defined in __post_init__.
     mf_energy: float = field(init=False)
     mo_energies: list = field(init=False)
     mo_occ: list = field(init=False)
 
-    mean_field: scf = field(init=False)
-
     n_mos: int = field(init=False)
     n_sos: int = field(init=False)
 
     active_occupied: list = field(init=False)
     frozen_occupied: list = field(init=False)
     active_virtual: list = field(init=False)
     frozen_virtual: list = field(init=False)
 
     def __post_init__(self):
         super().__post_init__()
-        self._compute_mean_field()
+        self.solver.compute_mean_field(self)
         self.freeze_mos(self.frozen_orbitals)
 
     @property
     def n_active_electrons(self):
         return sum(self.n_active_ab_electrons)
 
     @property
@@ -295,73 +291,23 @@
     @property
     def mo_coeff(self):
         """This property returns the molecular orbital coefficients.
 
         Returns:
             np.array: MO coefficient as a numpy array.
         """
-        return self.mean_field.mo_coeff
+        return self.solver.mo_coeff
 
     @mo_coeff.setter
     def mo_coeff(self, new_mo_coeff):
         # Asserting the new molecular coefficient matrix have the same dimensions.
-        if self.uhf:
-            assert len(new_mo_coeff) == 2, "Must provide [alpha mo_coeff, beta_mo_coeff]"
-            assert ((self.mean_field.mo_coeff[0].shape == new_mo_coeff[0].shape) and
-                    (self.mean_field.mo_coeff[1].shape == new_mo_coeff[1].shape)), \
-                   f"The new molecular coefficients has shape {[new_mo_coeff[0].shape, new_mo_coeff[1].shape]}"\
-                   f" shape: expected shape is {[self.mean_field.mo_coeff[0].shape, self.mean_field.mo_coeff[1].shape]}."
-        else:
-            assert self.mean_field.mo_coeff.shape == new_mo_coeff.shape, \
-                   f"The new molecular coefficients matrix has a {new_mo_coeff.shape}"\
-                   f" shape: expected shape is {self.mean_field.mo_coeff.shape}."
-        self.mean_field.mo_coeff = np.array(new_mo_coeff)
-
-    def _compute_mean_field(self):
-        """Computes the mean-field for the molecule. Depending on the molecule
-        spin, it does a restricted or a restriction open-shell Hartree-Fock
-        calculation.
-
-        It is also used for defining attributes related to the mean-field
-        (mf_energy, mo_energies, mo_occ, n_mos and n_sos).
-        """
-
-        molecule = self.to_pyscf(self.basis, self.symmetry, self.ecp)
-
-        self.mean_field = scf.RHF(molecule) if not self.uhf else scf.UHF(molecule)
-        self.mean_field.verbose = 0
-        # Force broken symmetry for uhf calculation when spin is 0 as shown in
-        # https://github.com/sunqm/pyscf/blob/master/examples/scf/32-break_spin_symm.py
-        if self.uhf and self.spin == 0:
-            dm_alpha, dm_beta = self.mean_field.get_init_guess()
-            dm_beta[:1, :] = 0
-            dm = (dm_alpha, dm_beta)
-            self.mean_field.kernel(dm)
-        else:
-            self.mean_field.kernel()
-
-        self.mean_field.analyze()
-        if not self.mean_field.converged:
-            raise ValueError("Hartree-Fock calculation did not converge")
-
-        if self.symmetry:
-            self.mo_symm_ids = list(symm.label_orb_symm(self.mean_field.mol, self.mean_field.mol.irrep_id,
-                                                        self.mean_field.mol.symm_orb, self.mean_field.mo_coeff))
-            irrep_map = {i: s for s, i in zip(molecule.irrep_name, molecule.irrep_id)}
-            self.mo_symm_labels = [irrep_map[i] for i in self.mo_symm_ids]
-        else:
-            self.mo_symm_ids = None
-            self.mo_symm_labels = None
-
-        self.mf_energy = self.mean_field.e_tot
-        self.mo_energies = self.mean_field.mo_energy
-        self.mo_occ = self.mean_field.mo_occ
-
-        self.n_mos = molecule.nao_nr()
-        self.n_sos = 2*self.n_mos
+        assert self.solver.mo_coeff.shape == (new_mo_coeff := np.array(new_mo_coeff)).shape, \
+            f"The new molecular coefficients matrix has a {new_mo_coeff.shape}"\
+            f" shape: expected shape is {self.solver.mo_coeff.shape}."
+        self.solver.mo_coeff = new_mo_coeff
 
     def _get_fermionic_hamiltonian(self, mo_coeff=None):
         """This method returns the fermionic hamiltonian. It written to take
         into account calls for this function is without argument, and attributes
         are parsed into it.
 
         Args:
@@ -446,160 +392,81 @@
             two_electron_integrals = two_electron_integrals.transpose(0, 3, 1, 2)
 
             # Computing the total energy from integrals and provided RDMs.
             e = core_constant + np.sum(one_electron_integrals * one_rdm) + 0.5*np.sum(two_electron_integrals * two_rdm)
 
         return e.real
 
-    def get_active_space_integrals(self, mo_coeff=None):
+    def get_integrals(self, mo_coeff=None, fold_frozen=True):
         """Computes core constant, one_body, and two-body coefficients with frozen orbitals folded into one-body coefficients
-        and core constant
+        and core constant for mo_coeff if fold_frozen is True
+
         For UHF
         one_body coefficients are [alpha one_body, beta one_body]
         two_body coefficients are [alpha-alpha two_body, alpha-beta two_body, beta-beta two_body]
 
         Args:
             mo_coeff (array): The molecular orbital coefficients to use to generate the integrals
+            fold_frozen (bool): If False, the full integral matrices and core constant are returned.
+                If True, the core constant, one_body, and two-body coefficients are calculated with frozen orbitals
+                folded into one-body coefficients and core constant. Default True
 
         Returns:
             (float, array or List[array], array or List[array]): (core_constant, one_body coefficients, two_body coefficients)
         """
+        if not self.uhf:
+            core_constant, one_body_integrals, two_body_integrals = self.solver.get_integrals(self, mo_coeff)
+            if fold_frozen:
+                core_offset, one_body_integrals, two_body_integrals = of_get_active_space_integrals(one_body_integrals,
+                                                                                                    two_body_integrals,
+                                                                                                    self.frozen_occupied,
+                                                                                                    self.active_mos)
 
-        return self.get_integrals(mo_coeff, True)
+                # Adding frozen electron contribution to core constant.
+                core_constant += core_offset
+        else:
+            core_constant, one_body_integrals, two_body_integrals = self.solver.get_integrals(self, mo_coeff)
+            if fold_frozen:
+                core_constant, one_body_integrals, two_body_integrals = self._get_active_space_integrals_uhf(core_constant,
+                                                                                                             one_body_integrals,
+                                                                                                             two_body_integrals)
+        return core_constant, one_body_integrals, two_body_integrals
 
-    def get_full_space_integrals(self, mo_coeff=None):
-        """Computes core constant, one_body, and two-body integrals for all orbitals
+    def get_active_space_integrals(self, mo_coeff=None):
+        """Computes core constant, one_body, and two-body coefficients with frozen orbitals folded into one-body coefficients
+        and core constant
         For UHF
         one_body coefficients are [alpha one_body, beta one_body]
         two_body coefficients are [alpha-alpha two_body, alpha-beta two_body, beta-beta two_body]
 
         Args:
-            mo_coeff (array): The molecular orbital coefficients to use to generate the integrals.
+            mo_coeff (array): The molecular orbital coefficients to use to generate the integrals
 
         Returns:
             (float, array or List[array], array or List[array]): (core_constant, one_body coefficients, two_body coefficients)
         """
 
-        return self.get_integrals(mo_coeff, False)
+        return self.get_integrals(mo_coeff, True)
 
-    def get_integrals(self, mo_coeff=None, consider_frozen=True):
-        """Computes core constant, one_body, and two-body coefficients for a given active space and mo_coeff
+    def get_full_space_integrals(self, mo_coeff=None):
+        """Computes core constant, one_body, and two-body integrals for all orbitals
         For UHF
         one_body coefficients are [alpha one_body, beta one_body]
         two_body coefficients are [alpha-alpha two_body, alpha-beta two_body, beta-beta two_body]
 
         Args:
             mo_coeff (array): The molecular orbital coefficients to use to generate the integrals.
-            consider_frozen (bool): If True, the frozen orbitals are folded into the one_body and core constant terms.
 
         Returns:
             (float, array or List[array], array or List[array]): (core_constant, one_body coefficients, two_body coefficients)
         """
 
-        # Pyscf molecule to get integrals.
-        pyscf_mol = self.to_pyscf(self.basis, self.symmetry, self.ecp)
-        if mo_coeff is None:
-            mo_coeff = self.mean_field.mo_coeff
-
-        if self.uhf:
-            if consider_frozen:
-                return self._get_active_space_integrals_uhf(mo_coeff=mo_coeff)
-            else:
-                one_body, two_body = self._compute_uhf_integrals(mo_coeff)
-                return float(pyscf_mol.energy_nuc()), one_body, two_body
-
-        # Corresponding to nuclear repulsion energy and static coulomb energy.
-        core_constant = float(pyscf_mol.energy_nuc())
-
-        # get_hcore is equivalent to int1e_kin + int1e_nuc.
-        one_electron_integrals = mo_coeff.T @ self.mean_field.get_hcore() @ mo_coeff
-
-        # Getting 2-body integrals in atomic and converting to molecular basis.
-        two_electron_integrals = ao2mo.kernel(pyscf_mol.intor("int2e"), mo_coeff)
-        two_electron_integrals = ao2mo.restore(1, two_electron_integrals, len(mo_coeff))
-
-        # PQRS convention in openfermion:
-        # h[p,q]=\int \phi_p(x)* (T + V_{ext}) \phi_q(x) dx
-        # h[p,q,r,s]=\int \phi_p(x)* \phi_q(y)* V_{elec-elec} \phi_r(y) \phi_s(x) dxdy
-        # The convention is not the same with PySCF integrals. So, a change is
-        # made before performing the truncation for frozen orbitals.
-        two_electron_integrals = two_electron_integrals.transpose(0, 2, 3, 1)
-        if consider_frozen:
-            core_offset, one_electron_integrals, two_electron_integrals = of_get_active_space_integrals(one_electron_integrals,
-                                                                                                        two_electron_integrals,
-                                                                                                        self.frozen_occupied,
-                                                                                                        self.active_mos)
-
-            # Adding frozen electron contribution to core constant.
-            core_constant += core_offset
-
-        return core_constant, one_electron_integrals, two_electron_integrals
-
-    def _compute_uhf_integrals(self, mo_coeff):
-        """Compute 1-electron and 2-electron integrals
-        The return is formatted as
-        [numpy.ndarray]*2 numpy array h_{pq} for alpha and beta blocks
-        [numpy.ndarray]*3 numpy array storing h_{pqrs} for alpha-alpha, alpha-beta, beta-beta blocks
-
-        Args:
-            List[array]: The molecular orbital coefficients for both spins [alpha, beta]
-
-        Returns:
-            List[array], List[array]: One and two body integrals
-        """
-        # step 1 : find nao, nmo (atomic orbitals & molecular orbitals)
-
-        # molecular orbitals (alpha and beta will be the same)
-        # Lets take alpha blocks to find the shape and things
-
-        # molecular orbitals
-        nmo = self.nmo = mo_coeff[0].shape[1]
-        # atomic orbitals
-        nao = self.nao = mo_coeff[0].shape[0]
-
-        # step 2 : obtain Hcore Hamiltonian in atomic orbitals basis
-        hcore = self.mean_field.get_hcore()
-
-        # step 3 : obatin two-electron integral in atomic basis
-        eri = ao2mo.restore(8, self.mean_field._eri, nao)
-
-        # step 4 : create the placeholder for the matrices
-        # one-electron matrix (alpha, beta)
-        hpq = []
-
-        # step 5 : do the mo transformation
-        # step the mo coeff alpha and beta
-        mo_a = mo_coeff[0]
-        mo_b = mo_coeff[1]
-
-        # mo transform the hcore
-        hpq.append(mo_a.T.dot(hcore).dot(mo_a))
-        hpq.append(mo_b.T.dot(hcore).dot(mo_b))
-
-        # mo transform the two-electron integrals
-        eri_a = ao2mo.incore.full(eri, mo_a)
-        eri_b = ao2mo.incore.full(eri, mo_b)
-        eri_ba = ao2mo.incore.general(eri, (mo_a, mo_a, mo_b, mo_b), compact=False)
-
-        # Change the format of integrals (full)
-        eri_a = ao2mo.restore(1, eri_a, nmo)
-        eri_b = ao2mo.restore(1, eri_b, nmo)
-        eri_ba = eri_ba.reshape(nmo, nmo, nmo, nmo)
-
-        # # convert this into the order OpenFemion like to receive
-        two_body_integrals_a = np.asarray(eri_a.transpose(0, 2, 3, 1), order='C')
-        two_body_integrals_b = np.asarray(eri_b.transpose(0, 2, 3, 1), order='C')
-        two_body_integrals_ab = np.asarray(eri_ba.transpose(0, 2, 3, 1), order='C')
-
-        # Gpqrs has alpha, alphaBeta, Beta blocks
-        Gpqrs = (two_body_integrals_a, two_body_integrals_ab, two_body_integrals_b)
-
-        return hpq, Gpqrs
+        return self.get_integrals(mo_coeff, False)
 
-    def _get_active_space_integrals_uhf(self, occupied_indices=None, active_indices=None, mo_coeff=None):
+    def _get_active_space_integrals_uhf(self, core_constant, one_body_integrals, two_body_integrals, occupied_indices=None, active_indices=None):
         """Get active space integrals with uhf reference
         The return is
         (core_constant,
         [alpha one_body, beta one_body],
         [alpha-alpha two_body, alpha-beta two_body, beta-beta two_body])
 
         Args:
@@ -607,27 +474,19 @@
             active_indices (array-like): The active orbital indices
             mo_coeff (List[array]): The molecular orbital coefficients to use to generate the integrals.
 
         Returns:
             (float, List[array], List[array]): Core constant, one body integrals, two body integrals
         """
 
-        if mo_coeff is None:
-            mo_coeff = self.mean_field.mo_coeff
-
-        # Get integrals.
-        one_body_integrals, two_body_integrals = self._compute_uhf_integrals(mo_coeff)
-
         occupied_indices = self.frozen_occupied if occupied_indices is None else occupied_indices
         active_indices = self.active_mos if active_indices is None else active_indices
         if (len(active_indices) < 1):
             raise ValueError('Some active indices required for reduction.')
 
-        # Determine core constant
-        core_constant = self.mean_field.mol.energy_nuc()
         # alpha part
         for i in occupied_indices[0]:
             core_constant += one_body_integrals[0][i, i]
             # alpha part of j
             for j in occupied_indices[0]:
                 core_constant += 0.5*(two_body_integrals[0][i, j, j, i]-two_body_integrals[0][i, j, i, j])
             # beta part of j
@@ -640,15 +499,15 @@
             # alpha part of j
             for j in occupied_indices[0]:
                 core_constant += 0.5*(two_body_integrals[1][j, i, i, j])   # i, j are swaped to make BetaAlpha same as AlphaBeta
             # beta part of j
             for j in occupied_indices[1]:
                 core_constant += 0.5*(two_body_integrals[2][i, j, j, i]-two_body_integrals[2][i, j, i, j])
 
-        # Modified one electon integrals
+        # Modified one electron integrals
         one_body_integrals_new_aa = np.copy(one_body_integrals[0])
         one_body_integrals_new_bb = np.copy(one_body_integrals[1])
 
         # alpha alpha block
         for u, v in product(active_indices[0], repeat=2):         # u is u_a, v i v_a
             for i in occupied_indices[0]:  # i belongs to alpha block
                 one_body_integrals_new_aa[u, v] += (two_body_integrals[0][i, u, v, i] - two_body_integrals[0][i, u, i, v])
@@ -676,33 +535,26 @@
         TwInt_ab = two_body_integrals[1][np.ix_(active_indices[0], active_indices[1],
                                                 active_indices[1], active_indices[0])]
 
         two_body_integrals_new = [TwInt_aa, TwInt_ab, TwInt_bb]
 
         return core_constant, one_body_integrals_new, two_body_integrals_new
 
-    def _get_molecular_hamiltonian_uhf(self, occupied_indices=None,
-                                       active_indices=None):
+    def _get_molecular_hamiltonian_uhf(self):
         """Output arrays of the second quantized Hamiltonian coefficients.
         Note:
             The indexing convention used is that even indices correspond to
             spin-up (alpha) modes and odd indices correspond to spin-down
             (beta) modes.
 
-        Args:
-            occupied_indices(list): A list of spatial orbital indices
-                indicating which orbitals should be considered doubly occupied.
-            active_indices(list): A list of spatial orbital indices indicating
-                which orbitals should be considered active.
-
         Returns:
             InteractionOperator: The molecular hamiltonian
         """
 
-        constant, one_body_integrals, two_body_integrals = self._get_active_space_integrals_uhf(occupied_indices, active_indices)
+        constant, one_body_integrals, two_body_integrals = self.get_active_space_integrals()
 
         # Lets find the dimensions
         n_orb_a = one_body_integrals[0].shape[0]
         n_orb_b = one_body_integrals[1].shape[0]
 
         # TODO: Implement more compact ordering. May be possible by defining own up_index and down_index functions
         # Instead of
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/rdms.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver_pyscf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,294 +1,282 @@
-# Copyright 2023 1QB Information Technologies Inc.
+# Copyright 2023 Good Chemistry Company.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Module containing functions to manipulate 1- and 2-RDMs."""
-
-import itertools as it
+import os
 
 import numpy as np
-from pyscf.lib import takebak_2d
 
-from tangelo.toolboxes.molecular_computation.coefficients import spatial_from_spinorb
-from tangelo.linq.helpers import pauli_string_to_of, pauli_of_to_string, get_compatible_bases
-from tangelo.toolboxes.operators import FermionOperator
-from tangelo.toolboxes.measurements import ClassicalShadow
-from tangelo.toolboxes.post_processing import Histogram, aggregate_histograms
-from tangelo.toolboxes.qubit_mappings.mapping_transform import fermion_to_qubit_mapping, get_qubit_number
-
-
-def matricize_2rdm(two_rdm, n_orbitals):
-    """Turns the two_rdm tensor into a matrix for test purposes."""
-
-    l = 0
-    sq = n_orbitals * n_orbitals
-    jpqrs = np.zeros((n_orbitals, n_orbitals), dtype=int)
-    for i in range(n_orbitals):
-        for j in range(n_orbitals):
-            jpqrs[i, j] = l
-            l += 1
-
-    rho = np.zeros((sq, sq), dtype=complex)
-    for i in range(n_orbitals):
-        for j in range(n_orbitals):
-            ij = jpqrs[i, j]
-            for k in range(n_orbitals):
-                for l in range(n_orbitals):
-                    kl = jpqrs[k, l]
-                    rho[ij, kl] += two_rdm[i, k, j, l]
-    return rho
+from tangelo.toolboxes.molecular_computation.integral_solver import IntegralSolver
 
 
-def compute_rdms(ferm_ham, mapping, up_then_down, exp_vals=None, exp_data=None, shadow=None, return_spinsum=True, **eval_args):
-    """
-    Compute the 1- and 2-RDM and their spin-summed versions
-    using a FermionOperator and experimental frequency data in the form of a
-    classical shadow or a dictionary of frequency histograms.
-    Exactly one of the following must be provided by the user:
-    exp_vals, exp_data or shadow
+def mol_to_pyscf(mol, basis="CRENBL", symmetry=False, ecp=None):
+    """Method to return a pyscf.gto.Mole object.
 
     Args:
-        ferm_ham (FermionicOperator): Fermionic operator with n_spinorbitals, n_electrons, and spin defined
-        mapping (str): Qubit mapping
-        up_then_down (bool): Spin ordering for the mapping
-        exp_vals (dict): Optional, dictionary of Pauli word expectation values
-        exp_data (dict): Optional, dictionary of {basis: histogram} where basis is the measurement basis
-            and histogram is a {bitstring: frequency} dictionary
-        shadow (ClassicalShadow): Optional, a classical shadow object
-        return_spinsum (bool): Optional, if True, return also the spin-summed RDMs
-        eval_args: Optional arguments to pass to the ClassicalShadow object
+        sqmol (SecondQuantizedMolecule or Molecule): The molecule to export to a pyscf molecule.
+        basis (string): Basis set.
+        symmetry (bool): Flag to turn symmetry on
+        ecp (dict): Dictionary with ecp definition for each atom e.g. {"Cu": "crenbl"}
 
     Returns:
-        complex array: 1-RDM
-        complex array: 2-RDM
-        complex array: spin-summed 1-RDM
-        complex array: spin-summed 2-RDM
+        pyscf.gto.Mole: PySCF compatible object.
     """
-    onerdm = np.zeros((ferm_ham.n_spinorbitals,) * 2, dtype=complex)
-    twordm = np.zeros((ferm_ham.n_spinorbitals,) * 4, dtype=complex)
+    from pyscf import gto
 
-    # Optional arguments are mutually exclusive, return error if several of them have been passed
-    if [exp_vals, exp_data, shadow].count(None) != 2:
-        raise RuntimeError("Arguments exp_vals, exp_data and shadow are mutually exclusive. Provide exactly one of them.")
+    pymol = gto.Mole(atom=mol.xyz)
+    pymol.basis = basis
+    pymol.charge = mol.q
+    pymol.spin = mol.spin
+    pymol.symmetry = symmetry
+    pymol.ecp = ecp if ecp else dict()
+    pymol.build()
+
+    return pymol
+
+
+class IntegralSolverPySCF(IntegralSolver):
+    """Electronic Structure integration for pyscf"""
+
+    def __init__(self, chkfile=None):
+        """Initialize the integral solver class for pyscf. A chkfile path can be
+        provided.
+
+        Regarding the chkfile, three scenarios are possible:
+        - A chkfile path is provided, but the file doesn't exist: it creates
+            a chkfile at the end of the SCF calculation.
+        - A chkfile path is provided and a file already exists: the initial
+            guess is taken from the chkfile and this file is updated at the end
+            of the calculation.
+        - No chkfile path is provided: The SCF initial guess stays the default
+            one (minao). No chkfile is created.
+
+        Args:
+            chkfile (string): Path of the chkfile.
+        """
+
+        from pyscf import gto, lib, scf, symm, ao2mo
+        self.gto = gto
+        self.lib = lib
+        self.scf = scf
+        self.symm = symm
+        self.ao2mo = ao2mo
+        self.chkfile = chkfile
+
+    def set_physical_data(self, mol):
+        """Set molecular data that is independant of basis set in mol
+
+        Modify mol variable:
+            mol.xyz to (list): Nested array-like structure with elements and coordinates
+                                            (ex:[ ["H", (0., 0., 0.)], ...]) in angstrom
+        Add to mol:
+            mol.n_electrons (int): Self-explanatory.
+            mol.n_atoms (int): Self-explanatory.
+
+        Args:
+            mol (Molecule or SecondQuantizedMolecule): Class to add the other variables given populated.
+                mol.xyz (in appropriate format for solver): Definition of molecular geometry.
+                mol.q (float): Total charge.
+                mol.spin (int): Absolute difference between alpha and beta electron number.
+        """
+        pymol = mol_to_pyscf(mol)
+        mol.xyz = list()
+        for sym, xyz in pymol._atom:
+            mol.xyz += [tuple([sym, tuple([x*self.lib.parameters.BOHR for x in xyz])])]
+
+        mol.n_atoms = pymol.natm
+        mol.n_electrons = pymol.nelectron
+
+    def compute_mean_field(self, sqmol):
+        """Run a unrestricted/restricted (openshell-)Hartree-Fock calculation and modify/add the following
+        variables to sqmol
+
+        Modify sqmol variables.
+            sqmol.mf_energy (float): Mean-field energy (RHF or ROHF energy depending on the spin).
+            sqmol.mo_energies (list of float): Molecular orbital energies.
+            sqmol.mo_occ (list of float): Molecular orbital occupancies (between 0. and 2.).
+            sqmol.n_mos (int): Number of molecular orbitals with a given basis set.
+            sqmol.n_sos (int): Number of spin-orbitals with a given basis set.
+
+        Add to sqmol:
+            self.mo_coeff (ndarray or List[ndarray]): array of molecular orbital coefficients (MO coeffs) if RHF ROHF
+                                                        list of arrays [alpha MO coeffs, beta MO coeffs] if UHF
+
+        Args:
+            sqmol (SecondQuantizedMolecule): Populated variables of Molecule plus
+                sqmol.basis (string): Basis set.
+                sqmol.ecp (dict): The effective core potential (ecp) for any atoms in the molecule.
+                    e.g. {"C": "crenbl"} use CRENBL ecp for Carbon atoms.
+                sqmol.symmetry (bool or str): Whether to use symmetry in RHF or ROHF calculation.
+                    Can also specify point group using string. e.g. "Dooh", "D2h", "C2v", ...
+                sqmol.uhf (bool): If True, Use UHF instead of RHF or ROHF reference. Default False
+
+
+        """
+
+        molecule = mol_to_pyscf(sqmol, sqmol.basis, sqmol.symmetry, sqmol.ecp)
+
+        sqmol.mean_field = self.scf.RHF(molecule) if not sqmol.uhf else self.scf.UHF(molecule)
+        sqmol.mean_field.verbose = 0
+
+        chkfile_found = False
+        if self.chkfile:
+            chkfile_found = os.path.exists(self.chkfile)
+            sqmol.mean_field.chkfile = self.chkfile
+
+        # Force broken symmetry for uhf calculation when spin is 0 as shown in
+        # https://github.com/sunqm/pyscf/blob/master/examples/scf/32-break_spin_symm.py
+        if sqmol.uhf and sqmol.spin == 0 and not chkfile_found:
+            dm_alpha, dm_beta = sqmol.mean_field.get_init_guess()
+            dm_beta[:1, :] = 0
+            dm = (dm_alpha, dm_beta)
+            sqmol.mean_field.kernel(dm)
+        else:
+            sqmol.mean_field.init_guess = "chkfile" if chkfile_found else "minao"
+            sqmol.mean_field.kernel()
 
-    # Initialize exp_vals
-    if isinstance(exp_vals, dict) and set(map(type, exp_vals)) == {str}:
-        exp_vals = {pauli_string_to_of(term): exp_val for term, exp_val in exp_vals.items()}
+        sqmol.mean_field.analyze()
+        if not sqmol.mean_field.converged:
+            raise ValueError("Hartree-Fock calculation did not converge")
+
+        if sqmol.symmetry:
+            sqmol.mo_symm_ids = list(self.symm.label_orb_symm(sqmol.mean_field.mol, sqmol.mean_field.mol.irrep_id,
+                                                              sqmol.mean_field.mol.symm_orb, sqmol.mean_field.mo_coeff))
+            irrep_map = {i: s for s, i in zip(molecule.irrep_name, molecule.irrep_id)}
+            sqmol.mo_symm_labels = [irrep_map[i] for i in sqmol.mo_symm_ids]
+        else:
+            sqmol.mo_symm_ids = None
+            sqmol.mo_symm_labels = None
 
-    if isinstance(exp_data, dict) and set(map(type, exp_data)) == {str}:
-        exp_data = {pauli_string_to_of(term): data for term, data in exp_data.items()}
+        sqmol.mf_energy = sqmol.mean_field.e_tot
+        sqmol.mo_energies = sqmol.mean_field.mo_energy
+        sqmol.mo_occ = sqmol.mean_field.mo_occ
 
-    if exp_vals is None:
-        exp_vals = dict()
+        sqmol.n_mos = molecule.nao_nr()
+        sqmol.n_sos = 2*sqmol.n_mos
 
-    n_qubits = get_qubit_number(mapping, ferm_ham.n_spinorbitals)
+        self.mo_coeff = sqmol.mean_field.mo_coeff
 
-    # Go over all terms in fermionic Hamiltonian
-    for term in ferm_ham.terms:
-        length = len(term)
+    def get_integrals(self, sqmol, mo_coeff=None):
+        r"""Computes core constant, one_body, and two-body integrals for all orbitals
 
-        if not term:
-            continue
+        one-body integrals should be in the form
+        h[p,q]= \int \phi_p(x)* (T + V_{ext}) \phi_q(x) dx
 
-        # Fermionic term with a prefactor of 1.0.
-        fermionic_term = FermionOperator(term, 1.0)
+        two-body integrals should be in the form
+        h[p,q,r,s] = \int \phi_p(x) * \phi_q(y) * V_{elec-elec} \phi_r(y) \phi_s(x) dxdy
 
-        qubit_term = fermion_to_qubit_mapping(fermion_operator=fermionic_term,
-                                              n_spinorbitals=ferm_ham.n_spinorbitals,
-                                              n_electrons=ferm_ham.n_electrons,
-                                              mapping=mapping,
-                                              up_then_down=up_then_down,
-                                              spin=ferm_ham.spin)
-        qubit_term.compress()
+        Using molecular orbitals \phi_j(x) = \sum_{ij} A_i(x) mo_coeff_{i,j} where A_i(x) are the atomic orbitals.
 
-        # Loop to go through all qubit terms.
-        eigenvalue = 0.
+        For UHF (if sqmol.uhf is True)
+        one_body coefficients are [alpha one_body, beta one_body]
+        two_body coefficients are [alpha-alpha two_body, alpha-beta two_body, beta-beta two_body]
 
-        if isinstance(shadow, ClassicalShadow):
-            eigenvalue = shadow.get_observable(qubit_term, **eval_args)
-        else:
-            for qterm, coeff in qubit_term.terms.items():
-                if coeff.real != 0:
+        where one_body and two_body are appropriately sized arrays for each spin sector.
 
-                    # qterm = (), i.e. tensor product of I.
-                    if not qterm:
-                        exp_val = 1.
-                    # Already computed expectation value of qterm.
-                    elif qterm in exp_vals:
-                        exp_val = exp_vals[qterm]
-                    # Case where there is at least one missing entry in exp_vals
-                    # (in this case, exp_data is None and we cannot compute the
-                    # eigenvalue).
-                    elif exp_data is None:
-                        raise RuntimeError(f"Missing {qterm} entry in exp_vals.")
-                    # Expectation value that can be computed from exp_data.
-                    else:
-                        ps = pauli_of_to_string(qterm, n_qubits)
-                        bases = get_compatible_bases(ps, [pauli_of_to_string(term, n_qubits) for term in exp_data.keys()])
-
-                        if not bases:
-                            raise RuntimeError(f"No experimental data for basis {qterm}.")
-
-                        hist = aggregate_histograms(*[Histogram(exp_data[pauli_string_to_of(basis)]) for basis in bases])
-                        exp_val = hist.get_expectation_value(qterm, 1.)
-                        exp_vals[qterm] = exp_val
-
-                    eigenvalue += coeff * exp_val
-
-        # Put the values in np arrays (differentiate 1- and 2-RDM)
-        if length == 2:
-            iele, jele = (int(ele[0]) for ele in tuple(term[0:2]))
-            onerdm[iele, jele] += eigenvalue
-        elif length == 4:
-            iele, jele, kele, lele = (int(ele[0]) for ele in tuple(term[0:4]))
-            twordm[iele, lele, jele, kele] += eigenvalue
-
-    if return_spinsum:
-        onerdm_spinsum = np.zeros((ferm_ham.n_spinorbitals//2,) * 2, dtype=complex)
-        twordm_spinsum = np.zeros((ferm_ham.n_spinorbitals//2,) * 4, dtype=complex)
-
-        # Construct spin-summed 1-RDM.
-        for i, j in it.product(range(onerdm.shape[0]), repeat=2):
-            onerdm_spinsum[i//2, j//2] += onerdm[i, j]
-
-        # Construct spin-summed 2-RDM.
-        for i, j, k, l in it.product(range(twordm.shape[0]), repeat=4):
-            twordm_spinsum[i//2, j//2, k//2, l//2] += twordm[i, j, k, l]
-
-        return onerdm, twordm, onerdm_spinsum, twordm_spinsum
-    else:
-        return onerdm, twordm
-
-
-def energy_from_rdms(ferm_op, one_rdm, two_rdm):
-    """Computes the molecular energy from one- and two-particle reduced
-    density matrices (RDMs). Coefficients (integrals) are computed from the
-    fermionic Hamiltonian provided.
+        Args:
+            sqmol (SecondQuantizedMolecule) : SecondQuantizedMolecule populated with all variables defined above
+            mo_coeff : Molecular orbital coefficients to use for calculating the integrals, instead of self.mo_coeff
 
-    Args:
-        ferm_op (FermionOperator): Self-explanatory.
-        one_rdm (numpy.array): One-particle density matrix in MO basis.
-        two_rdm (numpy.array): Two-particle density matrix in MO basis.
+        Returns:
+            (float, array or List[array], array or List[array]): (core_constant, one_body coefficients, two_body coefficients)
+        """
 
-    Returns:
-        float: Molecular energy.
-    """
+        # Pyscf molecule to get integrals.
+        pyscf_mol = mol_to_pyscf(sqmol, sqmol.basis, sqmol.symmetry, sqmol.ecp)
+        if mo_coeff is None:
+            mo_coeff = self.mo_coeff
 
-    core_constant, one_electron_coeffs, two_electron_coeffs = ferm_op.get_coeffs()
-    one_electron_integrals, two_electron_integrals = spatial_from_spinorb(one_electron_coeffs, two_electron_coeffs)
+        if sqmol.uhf:
+            one_body, two_body = self.compute_uhf_integrals(sqmol, mo_coeff)
+            return float(pyscf_mol.energy_nuc()), one_body, two_body
 
-    # PQRS convention in openfermion:
-    # h[p,q]=\int \phi_p(x)* (T + V_{ext}) \phi_q(x) dx
-    # h[p,q,r,s]=\int \phi_p(x)* \phi_q(y)* V_{elec-elec} \phi_r(y) \phi_s(x) dxdy
-    # The convention is not the same with PySCF integrals. So, a change is
-    # reverse back after performing the truncation for frozen orbitals
-    two_electron_integrals = two_electron_integrals.transpose(0, 3, 1, 2)
+        # Corresponding to nuclear repulsion energy and static coulomb energy.
+        core_constant = float(pyscf_mol.energy_nuc())
 
-    # Computing the total energy from integrals and provided RDMs.
-    e = core_constant + np.sum(one_electron_integrals * one_rdm) + np.sum(two_electron_integrals * two_rdm)
+        # get_hcore is equivalent to int1e_kin + int1e_nuc.
+        one_electron_integrals = mo_coeff.T @ sqmol.mean_field.get_hcore() @ mo_coeff
 
-    return e.real
+        # Getting 2-body integrals in atomic and converting to molecular basis.
+        two_electron_integrals = self.ao2mo.kernel(pyscf_mol.intor("int2e"), mo_coeff)
+        two_electron_integrals = self.ao2mo.restore(1, two_electron_integrals, len(mo_coeff))
 
+        # PQRS convention in openfermion:
+        # h[p,q]=\int \phi_p(x)* (T + V_{ext}) \phi_q(x) dx
+        # h[p,q,r,s]=\int \phi_p(x)* \phi_q(y)* V_{elec-elec} \phi_r(y) \phi_s(x) dxdy
+        # The convention is not the same with PySCF integrals. So, a change is
+        # made before performing the truncation for frozen orbitals.
+        two_electron_integrals = two_electron_integrals.transpose(0, 2, 3, 1)
 
-def pad_rdms_with_frozen_orbitals(sec_mol, onerdm, twordm):
-    """Function to pad the RDMs with the frozen orbitals data. It is based on
-    the pyscf.cccsd_rdm code, where we can set with_frozen=True.
+        return core_constant, one_electron_integrals, two_electron_integrals
 
-    Source:
-        https://github.com/pyscf/pyscf/blob/master/pyscf/cc/ccsd_rdm.py
+    def compute_uhf_integrals(self, sqmol, mo_coeff):
+        """Compute 1-electron and 2-electron integrals
+        The return is formatted as
+        [numpy.ndarray]*2 numpy array h_{pq} for alpha and beta blocks
+        [numpy.ndarray]*3 numpy array storing h_{pqrs} for alpha-alpha, alpha-beta, beta-beta blocks
 
-    Args:
-        sec_mol (SecondQuantizedMolecule): Self-explanatory.
-        onerdm (numpy.array): One-particle reduced density matrix (shape of
-            (N_active_mos,)*2).
-        twordm (numpy.array): Two-particle reduced density matrix (shape of
-            (N_active_mos,)*4).
+        Args:
+            sqmol (SecondQuantizedMolecule): The SecondQuantizedMolecule object to calculated UHF integrals for.
+            mo_coeff (List[array]): The molecular orbital coefficients for both spins [alpha, beta]
 
-    Returns:
-        numpy.array: One-particle reduced density matrix (shape of
-            (N_total_mos,)*2).
-        numpy.array: Two-particle reduced density matrix (shape of
-            (N_total_mos,)*4).
-    """
+        Returns:
+            List[array], List[array]: One and two body integrals
+        """
+        # step 1 : find nao, nmo (atomic orbitals & molecular orbitals)
+
+        # molecular orbitals (alpha and beta will be the same)
+        # Lets take alpha blocks to find the shape and things
+
+        # molecular orbitals
+        nmo = mo_coeff[0].shape[1]
+        # atomic orbitals
+        nao = mo_coeff[0].shape[0]
+
+        # step 2 : obtain Hcore Hamiltonian in atomic orbitals basis
+        hcore = sqmol.mean_field.get_hcore()
+
+        # step 3 : obatin two-electron integral in atomic basis
+        eri = self.ao2mo.restore(8, sqmol.mean_field._eri, nao)
+
+        # step 4 : create the placeholder for the matrices
+        # one-electron matrix (alpha, beta)
+        hpq = []
+
+        # step 5 : do the mo transformation
+        # step the mo coeff alpha and beta
+        mo_a = mo_coeff[0]
+        mo_b = mo_coeff[1]
+
+        # mo transform the hcore
+        hpq.append(mo_a.T.dot(hcore).dot(mo_a))
+        hpq.append(mo_b.T.dot(hcore).dot(mo_b))
+
+        # mo transform the two-electron integrals
+        eri_a = self.ao2mo.incore.full(eri, mo_a)
+        eri_b = self.ao2mo.incore.full(eri, mo_b)
+        eri_ba = self.ao2mo.incore.general(eri, (mo_a, mo_a, mo_b, mo_b), compact=False)
 
-    if sec_mol.uhf:
-        raise NotImplementedError("The RDMs padding with an UHF mean-field is not implemented.")
+        # Change the format of integrals (full)
+        eri_a = self.ao2mo.restore(1, eri_a, nmo)
+        eri_b = self.ao2mo.restore(1, eri_b, nmo)
+        eri_ba = eri_ba.reshape(nmo, nmo, nmo, nmo)
 
-    # Defining the number of MOs and occupation numbers with and without the
-    # frozen orbitals.
-    n_mos = sec_mol.n_mos
-    n_mos0 = sec_mol.n_active_mos
-    n_occ = np.count_nonzero(sec_mol.mo_occ > 0)
-    n_occ0 = n_occ - len(sec_mol.frozen_occupied)
-    moidx = np.array(sec_mol.active_mos)
-
-    # Creating a dummy one rdm with all diagonal elements set to 2. After that,
-    # the true one rdm is embedded in this bigger matrix.
-    onerdm_padded = np.zeros((n_mos,)*2, dtype=onerdm.dtype)
-    onerdm_padded[np.diag_indices(n_occ)] = 2.
-    onerdm_padded[moidx[:, None], moidx] = onerdm
-
-    # Deleting the one rdm contribution in the two rdm. This must be done to
-    # redo the operation later with the one rdm with the frozen orbital.
-    twordm = twordm.transpose(1, 0, 3, 2)
-
-    onerdm_without_diag = np.copy(onerdm)
-    onerdm_without_diag[np.diag_indices(n_occ0)] -= 2
-
-    onerdm_without_diag_times_2 = onerdm_without_diag * 2
-    onerdm_without_diag_T = onerdm_without_diag.T
-
-    for i in range(n_occ0):
-        twordm[i, i, :, :] -= onerdm_without_diag_times_2
-        twordm[:, :, i, i] -= onerdm_without_diag_times_2
-        twordm[:, i, i, :] += onerdm_without_diag
-        twordm[i, :, :, i] += onerdm_without_diag_T
-
-    for i, j in it.product(range(n_occ0), repeat=2):
-        twordm[i, i, j, j] -= 4
-        twordm[i, j, j, i] += 2
-
-    # Creating a dummy two rdm.
-    dm2 = np.zeros((n_mos,)*4, dtype=twordm.dtype)
-
-    idx = (moidx.reshape(-1, 1) * n_mos + moidx).ravel()
-
-    # This part is meant to replicate
-    # https://github.com/pyscf/pyscf/blob/8b3fef8cf18f10d430261d4a8bea21fadf19bb1f/pyscf/cc/ccsd_rdm.py#L343-L351.
-    # The output is not catched, maybe for memory efficiency purposes (elements
-    # of dm2 changed inplace?).
-    takebak_2d(dm2.reshape(n_mos**2, n_mos**2),
-               twordm.reshape(n_mos0**2, n_mos0**2), idx, idx)
-    twordm_padded = dm2
-
-    # The next few lines will reembed the on rdm, but with the frozen orbital
-    # elements of the one rdm matrix.
-    onerdm_padded_without_diag = np.copy(onerdm_padded)
-    onerdm_padded_without_diag[np.diag_indices(n_occ)] -= 2
-
-    onerdm_padded_without_diag_times_2 = onerdm_padded_without_diag * 2
-    onerdm_padded_without_diag_T = onerdm_padded_without_diag.T
-
-    for i in range(n_occ):
-        twordm_padded[i, i, :, :] += onerdm_padded_without_diag_times_2
-        twordm_padded[:, :, i, i] += onerdm_padded_without_diag_times_2
-        twordm_padded[:, i, i, :] -= onerdm_padded_without_diag
-        twordm_padded[i, :, :, i] -= onerdm_padded_without_diag_T
-
-    for i, j in it.product(range(n_occ), repeat=2):
-        twordm_padded[i, i, j, j] += 4
-        twordm_padded[i, j, j, i] -= 2
+        # convert this into the physicist ordering for OpenFermion
+        two_body_integrals_a = np.asarray(eri_a.transpose(0, 2, 3, 1), order='C')
+        two_body_integrals_b = np.asarray(eri_b.transpose(0, 2, 3, 1), order='C')
+        two_body_integrals_ab = np.asarray(eri_ba.transpose(0, 2, 3, 1), order='C')
 
-    twordm_padded = twordm_padded.transpose(1, 0, 3, 2)
+        # Gpqrs has alpha, alphaBeta, Beta blocks
+        Gpqrs = (two_body_integrals_a, two_body_integrals_ab, two_body_integrals_b)
 
-    return onerdm_padded, twordm_padded
+        return hpq, Gpqrs
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/test_coefficients.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_coefficients.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/molecular_computation/tests/test_molecule.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_molecule.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import numpy as np
 from openfermion.utils import load_operator
 
 from tangelo import SecondQuantizedMolecule
 from tangelo.molecule_library import mol_H2_sto3g, xyz_H2O
 from tangelo.toolboxes.molecular_computation.molecule import atom_string_to_list
+from tangelo.toolboxes.molecular_computation.integral_solver import IntegralSolver
 
 # For openfermion.load_operator function.
 pwd_this_test = os.path.dirname(os.path.abspath(__file__))
 
 H2_list = [("H", (0., 0., 0.)), ("H", (0., 0., 0.7414))]
 H2_string = """
 H       0.0        0.0        0.0
@@ -57,23 +58,23 @@
 class SecondQuantizedMoleculeTest(unittest.TestCase):
 
     def test_instantiate_H2(self):
         """Verify basic properties of molecule object through instantiation of
         MolecularData class.
         """
 
-        molecule = SecondQuantizedMolecule(H2_list, 0, 0, "sto-3g")
+        molecule = SecondQuantizedMolecule(H2_list, 0, 0, basis="sto-3g")
 
         assert(molecule.elements == ["H"]*2)
         assert(molecule.basis == "sto-3g")
         assert(molecule.spin == 0)
         assert(molecule.q == 0)
         assert(molecule.n_electrons == 2)
 
-        molecule = SecondQuantizedMolecule(H2_file_xyz, 0, 0, "sto-3g")
+        molecule = SecondQuantizedMolecule(H2_file_xyz, 0, 0, basis="sto-3g")
         assert(molecule.elements == ["H"]*2)
         assert(molecule.basis == "sto-3g")
         assert(molecule.spin == 0)
         assert(molecule.q == 0)
         assert(molecule.n_electrons == 2)
         atom_list_close(molecule.xyz, H2_list, 1.e-14)
 
@@ -137,32 +138,81 @@
         # "Cu" has 29 electrons but the ecp reduces this to 19. The active electrons are 19 - 8 * 2 = 3
         assert(molecule.n_active_electrons == 3)
         assert(molecule.n_active_mos == 35)
 
     def test_mo_coeff_setter(self):
         """Verify the dimension check in the mo_coeff setter."""
 
-        molecule = SecondQuantizedMolecule(H2_list, 0, 0, "sto-3g")
+        molecule = SecondQuantizedMolecule(H2_list, 0, 0, basis="sto-3g")
 
         # Should work.
         dummy_mo_coeff = np.ones((2, 2))
         molecule.mo_coeff = dummy_mo_coeff
 
         # Should raise an AssertionError.
         bad_dummy_mo_coeff = np.ones((3, 3))
         with self.assertRaises(AssertionError):
             molecule.mo_coeff = bad_dummy_mo_coeff
 
-        molecule = SecondQuantizedMolecule(H2_list, 0, 0, "sto-3g", uhf=True)
+        molecule = SecondQuantizedMolecule(H2_list, 0, 0, basis="sto-3g", uhf=True)
 
         # Should work.
         dummy_mo_coeff = [np.ones((2, 2))]*2
         molecule.mo_coeff = dummy_mo_coeff
 
         # Should raise an AssertionError.
         bad_dummy_mo_coeff = [np.ones((3, 3))]*2
         with self.assertRaises(AssertionError):
             molecule.mo_coeff = bad_dummy_mo_coeff
 
+    def test_custom_solver_H2(self):
+        """Verify that using a custom ESSolver that only stores molecular data functions correctly returns
+        energy_from_rdms and fermion_hamiltonian
+        """
+
+        molecule = SecondQuantizedMolecule(H2_list, 0, 0, basis="sto-3g")
+
+        core_constant, one_body_integrals, two_body_integrals = molecule.get_full_space_integrals()
+
+        class IntegralSolverDummy(IntegralSolver):
+            def set_physical_data(self, mol):
+                mol.xyz = H2_list
+                mol.n_electrons = 2
+                mol.n_atoms = 2
+
+            def compute_mean_field(self, sqmol):
+                sqmol.mf_energy = molecule.mf_energy
+                sqmol.mo_energies = molecule.mo_energies
+                sqmol.mo_occ = molecule.mo_occ
+                sqmol.n_mos = molecule.n_mos
+                sqmol.n_sos = molecule.n_sos
+                self.mo_coeff = molecule.mo_coeff.copy()
+
+            def get_integrals(self, sqmol, mo_coeff=None):
+                return core_constant, one_body_integrals, two_body_integrals
+
+        molecule_dummy = SecondQuantizedMolecule(H2_list, 0, 0, IntegralSolverDummy(), basis="sto-3g", frozen_orbitals=[])
+
+        rdm1 = [[ 1.97453997e+00, -7.05987336e-17],
+                [-7.05987336e-17,  2.54600303e-02]]
+
+        rdm2 = [
+            [[[ 1.97453997e+00, -7.96423130e-17],
+              [-7.96423130e-17,  3.21234218e-33]],
+             [[-7.96423130e-17, -2.24213843e-01],
+              [ 0.00000000e+00,  9.04357944e-18]]],
+            [[[-7.96423130e-17,  0.00000000e+00],
+              [-2.24213843e-01,  9.04357944e-18]],
+             [[ 3.21234218e-33,  9.04357944e-18],
+              [ 9.04357944e-18,  2.54600303e-02]]]
+            ]
+
+        e_rdms = molecule_dummy.energy_from_rdms(rdm1, rdm2)
+        self.assertAlmostEqual(e_rdms, -1.1372701, delta=1e-5)
+
+        ferm_op = molecule_dummy.fermionic_hamiltonian
+        ref_ferm_op = load_operator("H2_ferm_op.data", data_directory=pwd_this_test+"/data", plain_text=True)
+        self.assertEqual(ferm_op, ref_ferm_op)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/multiformoperator.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/multiformoperator.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/operators.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 import numpy as np
 from scipy.special import comb
 import openfermion as of
 
 from tangelo.toolboxes.molecular_computation.coefficients import spatial_from_spinorb
 
+COEFFICIENT_TYPES = (int, float, complex, np.integer, np.floating)
+
 
 class FermionOperator(of.FermionOperator):
     """Custom FermionOperator class. Based on openfermion's, with additional functionalities.
     """
 
     def __init__(self, term=None, coefficient=1., n_spinorbitals=None, n_electrons=None, spin=None):
         super(FermionOperator, self).__init__(term, coefficient)
@@ -71,14 +73,18 @@
             if (self.n_spinorbitals, self.n_electrons, self.spin) != (None, None, None):
                 raise RuntimeError("openfermion FermionOperator did not define a necessary attribute")
             else:
                 f_op = FermionOperator()
                 f_op.terms = other.terms.copy()
                 return super(FermionOperator, self).__iadd__(f_op)
 
+        elif isinstance(other, COEFFICIENT_TYPES):
+            self.constant += other
+            return self
+
         else:
             raise RuntimeError(f"You cannot add FermionOperator and {other.__class__}.")
 
     def __add__(self, other):
         return self.__iadd__(other)
 
     def __radd__(self, other):
@@ -164,14 +170,28 @@
 
 
 class QubitOperator(of.QubitOperator):
     """Currently, this class is coming from openfermion. Can be later on be
     replaced by our own implementation.
     """
 
+    @classmethod
+    def from_openfermion(cls, of_qop):
+        """ Enable instantiation of a QubitOperator from an openfermion QubitOperator object.
+
+        Args:
+            of_qop (openfermion QubitOperator): an existing qubit operator defined with Openfermion
+
+        Returns:
+            corresponding QubitOperator object.
+        """
+        qop = cls()
+        qop.terms = of_qop.terms.copy()
+        return qop
+
     def frobenius_norm_compression(self, epsilon, n_qubits):
         """Reduces the number of operator terms based on its Frobenius norm
         and a user-defined threshold, epsilon. The eigenspectrum of the
         compressed operator will not deviate more than epsilon. For more
         details, see J. Chem. Theory Comput. 2020, 16, 2, 1055-1063.
 
         Args:
@@ -226,29 +246,34 @@
         for term in self.terms:
             if term:
                 indices = list(zip(*term))[0]
                 qubit_indices.update(indices)
 
         return qubit_indices
 
+    def to_openfermion(self):
+        """Converts Tangelo QubitOperator to openfermion"""
+        qu_op = of.QubitOperator()
+        qu_op.terms = self.terms.copy()
+        return qu_op
+
 
 class QubitHamiltonian(QubitOperator):
     """QubitHamiltonian objects are essentially openfermion.QubitOperator
     objects, with extra attributes. The mapping procedure (mapping) and the
     qubit ordering (up_then_down) are incorporated into the class. In addition
     to QubitOperator, several checks are done when performing arithmetic
     operations on QubitHamiltonians.
 
     Attributes:
         term (openfermion-like): Same as openfermion term formats.
         coefficient (complex): Coefficient for this term.
         mapping (string): Mapping procedure for fermionic to qubit encoding
             (ex: "JW", "BK", etc.).
-        up_then_down (bool): Whether or not spin ordering is all up then
-            all down.
+        up_then_down (bool): Whether spin ordering is all up then all down.
 
     Properties:
         n_terms (int): Number of terms in this qubit Hamiltonian.
     """
 
     def __init__(self, term=None, coefficient=1., mapping=None, up_then_down=None):
         super(QubitOperator, self).__init__(term, coefficient)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/taper_qubits.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/taper_qubits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/test_multiformoperator.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_multiformoperator.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/test_operators.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,17 +103,20 @@
         self.assertEqual(fop_1, fop_2)
 
         # Test in-place addition
         fop = FermionOperator("0^ 0", 2.)
         fop += FermionOperator("0^ 1", 3.)
         self.assertEqual(fop, fop_1)
 
+        # Test addition with coefficient
+        self.assertEqual(2. + fop_1, fop_2 + 2.)
+
         # Test addition with non-compatible type
         with self.assertRaises(RuntimeError):
-            fop + 1
+            fop + "a"
 
     def test_mul(self):
         # Test in-place multiplication
         fop_1 = FermionOperator("0^ 0", 2.)
         fop_1 *= of.FermionOperator("0^ 1", 3.)
         # Test multiplication
         fop_2 = FermionOperator("0^ 0", 2.) * of.FermionOperator("0^ 1", 3.)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/test_taper_qubits.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_taper_qubits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/tests/test_z2_tapering.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_z2_tapering.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/operators/z2_tapering.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/z2_tapering.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/optimizers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/optimizers/rotosolve.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/rotosolve.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/bootstrapping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/bootstrapping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/extrapolation.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/extrapolation.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/histogram.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/histogram.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/mc_weeny_rdm_purification.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/mc_weeny_rdm_purification.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/post_selection.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/post_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,17 @@
         circuit (Circuit): A quantum circuit to be equipped with symmetry verification
         sym_op (string): The symmetry operator to be verified.
             Can be a Pauli string, OpenFermion style list or a QubitOperator
 
     Returns:
         Circuit: The input circuit appended with the proper basis rotation
             and entanglement with an ancilla qubit, which is added as the last qubit.
-            This appends an additional qubit to the circuit."""
+            This appends an additional qubit to the circuit.
+    """
+
     if isinstance(sym_op, QubitOperator):
         op_len = count_qubits(sym_op)
     else:
         op_len = len(sym_op)
 
     n_qubits = circuit.width
 
@@ -77,29 +79,32 @@
             filter results based on the first qubit with the |1> state and
             the second qubit with the |0> state measured.
 
     Returns:
         dict: A dictionary of post-selected, renormalized frequencies
             and bitstrings with removed ancilla qubits
     """
+
     hist = Histogram(freqs, n_shots=0)
     hist.post_select(expected_outcomes)
     return hist.frequencies
 
 
 def strip_post_selection(freqs, *qubits):
     """Convenience function to remove the symmetry ancilla qubit
     and aggregate data to recreate results without post-selection.
 
     Args:
         freqs (dict): A dictionary of {bitstring: frequency} as returned from a quantum device
         qubits (variable number of int): The ancilla qubit indices to be removed from the bitstrings
 
     Returns:
-        dict: A frequency dictionary with the qubits stripped and data aggregated"""
+        dict: A frequency dictionary with the qubits stripped and data aggregated
+    """
+
     hist = Histogram(freqs, n_shots=0)
     hist.remove_qubit_indices(*qubits)
     return hist.frequencies
 
 
 def split_frequency_dict(frequencies, indices, desired_measurement=None):
     """Marginalize the frequencies dictionary over the indices.
@@ -111,15 +116,17 @@
     Args:
         frequencies (dict): The input frequency dictionary
         indices (list): The list of indices in the frequency dictionary to marginalize over
         desired_measurement (str): The bit string that is to be selected
 
     Returns:
         dict: The marginal frequencies for provided indices
-        dict: The marginal frequencies for remaining indices"""
+        dict: The marginal frequencies for remaining indices
+    """
+
     key_length = len(next(iter(frequencies)))
     other_indices = [i for i in range(key_length) if i not in indices]
 
     midcirc_dict = strip_post_selection(frequencies, *other_indices)
 
     if desired_measurement is None:
         marginal_dict = strip_post_selection(frequencies, *indices)
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/test_extrapolation.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_extrapolation.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/test_histogram.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/post_processing/tests/test_post_selection.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_post_selection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .jordan_wigner import jordan_wigner
 from .bravyi_kitaev import bravyi_kitaev
 from .symmetry_conserving_bravyi_kitaev import symmetry_conserving_bravyi_kitaev
 from .jkmn import jkmn
+from .combinatorial import combinatorial
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/hcb.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/hcb.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/jkmn.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/jkmn.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/jordan_wigner.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/jordan_wigner.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/mapping_transform.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/mapping_transform.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/statevector_mapping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/statevector_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 translate into a Circuit.
 """
 
 
 import warnings
 
 import numpy as np
-from openfermion import QubitOperator
+from openfermion.ops.operators import QubitOperator
 from openfermion.transforms import bravyi_kitaev_code
 from openfermion.transforms.opconversions.bravyi_kitaev_tree import _transform_ladder_operator, FenwickTree
 
 from tangelo.linq import Gate, Circuit
 from tangelo.toolboxes.qubit_mappings.jkmn import jkmn_prep_vector
 
 available_mappings = {"JW", "BK", "SCBK", "JKMN"}
```

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.3.4/tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.assertEqual(circuit.size, sum(vector))
         self.assertEqual(circuit.width, vector.size)
 
     def test_all_same_energy_mol_H4_sto3g_and_mol_H2O_sto3g(self):
         """Check that all mappings return statevectors that have the same energy expectation
         for an even number of electrons and various spins. Molecules tested are H4, and H2O
         with frozen_orbitals=[0, 7] which failed previously for scbk"""
-        mols = [mol_H4_sto3g, SecondQuantizedMolecule(xyz_H2O, 0, 0, "sto-3g", frozen_orbitals=[0, 7])]
+        mols = [mol_H4_sto3g, SecondQuantizedMolecule(xyz_H2O, 0, 0, basis="sto-3g", frozen_orbitals=[0, 7])]
         circuits = dict()
         qu_ops = dict()
         for mol in mols:
             ferm_op = mol.fermionic_hamiltonian
             qu_ops = dict()
             for transform in spin_ind_transforms:
                 qu_ops[transform] = fermion_to_qubit_mapping(ferm_op,
```

### Comparing `tangelo-gc-0.3.4/tangelo_gc.egg-info/SOURCES.txt` & `tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 tangelo/_version.py
 tangelo/molecule_library.py
 tangelo/algorithms/__init__.py
 tangelo/algorithms/electronic_structure_solver.py
 tangelo/algorithms/classical/__init__.py
 tangelo/algorithms/classical/ccsd_solver.py
 tangelo/algorithms/classical/fci_solver.py
+tangelo/algorithms/classical/mp2_solver.py
 tangelo/algorithms/classical/semi_empirical_solver.py
 tangelo/algorithms/classical/tests/__init__.py
 tangelo/algorithms/classical/tests/test_ccsd_solver.py
 tangelo/algorithms/classical/tests/test_fci_solver.py
+tangelo/algorithms/classical/tests/test_mp2_solver.py
 tangelo/algorithms/classical/tests/test_semi_empirical_solver.py
 tangelo/algorithms/projective/__init__.py
 tangelo/algorithms/projective/quantum_imaginary_time.py
 tangelo/algorithms/projective/tests/__init__.py
 tangelo/algorithms/projective/tests/test_qite.py
 tangelo/algorithms/variational/__init__.py
 tangelo/algorithms/variational/adapt_vqe_solver.py
@@ -40,55 +42,65 @@
 tangelo/linq/__init__.py
 tangelo/linq/circuit.py
 tangelo/linq/gate.py
 tangelo/linq/qdk_template.py
 tangelo/linq/simulator.py
 tangelo/linq/helpers/__init__.py
 tangelo/linq/helpers/circuits/__init__.py
+tangelo/linq/helpers/circuits/clifford_circuits.py
 tangelo/linq/helpers/circuits/measurement_basis.py
 tangelo/linq/helpers/circuits/statevector.py
 tangelo/linq/helpers/circuits/tests/__init__.py
+tangelo/linq/helpers/circuits/tests/test_clifford_circuits.py
 tangelo/linq/helpers/circuits/tests/test_statevector.py
 tangelo/linq/helpers/operators/__init__.py
 tangelo/linq/helpers/operators/operators.py
 tangelo/linq/noisy_simulation/__init__.py
 tangelo/linq/noisy_simulation/noise_models.py
 tangelo/linq/qpu_connection/__init__.py
+tangelo/linq/qpu_connection/braket_connection.py
 tangelo/linq/qpu_connection/ibm_connection.py
 tangelo/linq/qpu_connection/ionq_connection.py
 tangelo/linq/qpu_connection/qemist_cloud_connection.py
 tangelo/linq/qpu_connection/qpu_connection.py
 tangelo/linq/target/__init__.py
 tangelo/linq/target/backend.py
 tangelo/linq/target/target_cirq.py
 tangelo/linq/target/target_qdk.py
 tangelo/linq/target/target_qiskit.py
 tangelo/linq/target/target_qulacs.py
+tangelo/linq/target/target_stim.py
+tangelo/linq/target/target_sympy.py
 tangelo/linq/tests/__init__.py
+tangelo/linq/tests/test_braket_connection.py
 tangelo/linq/tests/test_circuits.py
 tangelo/linq/tests/test_gates.py
 tangelo/linq/tests/test_ibm_connection.py
 tangelo/linq/tests/test_ionq_connection.py
 tangelo/linq/tests/test_simulator.py
 tangelo/linq/tests/test_simulator_noisy.py
+tangelo/linq/tests/test_symbolic_simulator.py
 tangelo/linq/tests/test_translator_circuit.py
+tangelo/linq/tests/test_translator_perf.py
 tangelo/linq/tests/test_translator_qubitop.py
 tangelo/linq/translator/__init__.py
 tangelo/linq/translator/qdk_template.py
 tangelo/linq/translator/translate_braket.py
 tangelo/linq/translator/translate_circuit.py
 tangelo/linq/translator/translate_cirq.py
 tangelo/linq/translator/translate_json_ionq.py
 tangelo/linq/translator/translate_openqasm.py
 tangelo/linq/translator/translate_pennylane.py
 tangelo/linq/translator/translate_projectq.py
 tangelo/linq/translator/translate_qdk.py
 tangelo/linq/translator/translate_qiskit.py
 tangelo/linq/translator/translate_qubitop.py
 tangelo/linq/translator/translate_qulacs.py
+tangelo/linq/translator/translate_stim.py
+tangelo/linq/translator/translate_sympy.py
 tangelo/problem_decomposition/__init__.py
 tangelo/problem_decomposition/problem_decomposition.py
 tangelo/problem_decomposition/dmet/__init__.py
 tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py
 tangelo/problem_decomposition/dmet/fragment.py
 tangelo/problem_decomposition/dmet/_helpers/__init__.py
 tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py
@@ -190,30 +202,37 @@
 tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py
 tangelo/toolboxes/measurements/tests/test_measurements.py
 tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py
 tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py
 tangelo/toolboxes/molecular_computation/__init__.py
 tangelo/toolboxes/molecular_computation/coefficients.py
 tangelo/toolboxes/molecular_computation/frozen_orbitals.py
+tangelo/toolboxes/molecular_computation/integral_solver.py
+tangelo/toolboxes/molecular_computation/integral_solver_psi4.py
+tangelo/toolboxes/molecular_computation/integral_solver_pyscf.py
 tangelo/toolboxes/molecular_computation/molecule.py
 tangelo/toolboxes/molecular_computation/rdms.py
 tangelo/toolboxes/molecular_computation/tests/__init__.py
 tangelo/toolboxes/molecular_computation/tests/test_coefficients.py
 tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py
 tangelo/toolboxes/molecular_computation/tests/test_molecule.py
+tangelo/toolboxes/molecular_computation/tests/test_nopyscf.py
+tangelo/toolboxes/molecular_computation/tests/test_psi4.py
 tangelo/toolboxes/molecular_computation/tests/test_rdms.py
 tangelo/toolboxes/operators/__init__.py
 tangelo/toolboxes/operators/multiformoperator.py
 tangelo/toolboxes/operators/operators.py
 tangelo/toolboxes/operators/taper_qubits.py
+tangelo/toolboxes/operators/trim_trivial_qubits.py
 tangelo/toolboxes/operators/z2_tapering.py
 tangelo/toolboxes/operators/tests/__init__.py
 tangelo/toolboxes/operators/tests/test_multiformoperator.py
 tangelo/toolboxes/operators/tests/test_operators.py
 tangelo/toolboxes/operators/tests/test_taper_qubits.py
+tangelo/toolboxes/operators/tests/test_trim_trivial_qubits.py
 tangelo/toolboxes/operators/tests/test_z2_tapering.py
 tangelo/toolboxes/optimizers/__init__.py
 tangelo/toolboxes/optimizers/rotosolve.py
 tangelo/toolboxes/post_processing/__init__.py
 tangelo/toolboxes/post_processing/bootstrapping.py
 tangelo/toolboxes/post_processing/extrapolation.py
 tangelo/toolboxes/post_processing/histogram.py
@@ -222,22 +241,24 @@
 tangelo/toolboxes/post_processing/tests/__init__.py
 tangelo/toolboxes/post_processing/tests/test_extrapolation.py
 tangelo/toolboxes/post_processing/tests/test_histogram.py
 tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py
 tangelo/toolboxes/post_processing/tests/test_post_selection.py
 tangelo/toolboxes/qubit_mappings/__init__.py
 tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py
+tangelo/toolboxes/qubit_mappings/combinatorial.py
 tangelo/toolboxes/qubit_mappings/hcb.py
 tangelo/toolboxes/qubit_mappings/jkmn.py
 tangelo/toolboxes/qubit_mappings/jordan_wigner.py
 tangelo/toolboxes/qubit_mappings/mapping_transform.py
 tangelo/toolboxes/qubit_mappings/statevector_mapping.py
 tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py
 tangelo/toolboxes/qubit_mappings/tests/__init__.py
 tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py
+tangelo/toolboxes/qubit_mappings/tests/test_combinatorial.py
 tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py
 tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py
 tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py
 tangelo_gc.egg-info/PKG-INFO
 tangelo_gc.egg-info/SOURCES.txt
 tangelo_gc.egg-info/dependency_links.txt
 tangelo_gc.egg-info/requires.txt
```

