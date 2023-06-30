# Comparing `tmp/keylime-7.2.5.tar.gz` & `tmp/keylime-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keylime-7.2.5.tar", last modified: Fri Jun  2 17:22:59 2023, max compression
+gzip compressed data, was "keylime-7.3.0.tar", last modified: Fri Jun 30 17:17:29 2023, max compression
```

## Comparing `keylime-7.2.5.tar` & `keylime-7.3.0.tar`

### file list

```diff
@@ -1,186 +1,187 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.465957 keylime-7.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 17:22:46.000000 keylime-7.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-02 17:22:46.000000 keylime-7.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-02 17:22:59.465957 keylime-7.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-02 17:22:46.000000 keylime-7.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-02 17:22:46.000000 keylime-7.2.5/_pypi-notice.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.445955 keylime-7.2.5/keylime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/agentstates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/backport_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ca_impl_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ca_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cert_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.449956 keylime-7.2.5/keylime/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cli/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cloud_verifier_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    65426 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cloud_verifier_tornado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.449956 keylime-7.2.5/keylime/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20465 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/convert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/convert_runtime_policy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22220 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/create_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/sign_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/user_data_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.449956 keylime-7.2.5/keylime/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/da/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/attest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/da/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/rekor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/sqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/tsa_rfc3161.py
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/db/keylime_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/db/registrar_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/db/verifier_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/dsse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/dsse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/dsse/dsse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/dsse/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/dsse/x509.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/fs_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/ima/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/dm_grammar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18388 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/file_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    24265 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/ima.py
--rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/ima_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/ima_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/keylime_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/mba/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.457956 keylime-7.2.5/keylime/mba/elchecking/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/mbpolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/mba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.457956 keylime-7.2.5/keylime/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.461957 keylime-7.2.5/keylime/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/039322ea079b_add_generator_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/registrar_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/registrar_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/requests_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/revocation_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/signing.py
--rw-r--r--   0 runner    (1001) docker     (123)    74523 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tornado_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.461957 keylime-7.2.5/keylime/tpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/ec_crypto_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm2_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm2_objects_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    31669 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm_bootlog_enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm_ek_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/web_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.449956 keylime-7.2.5/keylime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-02 17:22:46.000000 keylime-7.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-02 17:22:59.469957 keylime-7.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-02 17:22:46.000000 keylime-7.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.441955 keylime-7.2.5/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.461957 keylime-7.2.5/templates/2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/agent.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/ca.j2
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/logging.j2
--rw-r--r--   0 runner    (1001) docker     (123)    26831 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/registrar.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/tenant.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/verifier.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.465957 keylime-7.2.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ca_impl_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ca_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_convert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_fs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ima_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ima_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ima_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_policy_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_registrar_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_retry_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_signing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_tpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_verifier_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_web_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.163187 keylime-7.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 17:17:19.000000 keylime-7.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-30 17:17:19.000000 keylime-7.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-30 17:17:29.163187 keylime-7.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-30 17:17:19.000000 keylime-7.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 17:17:19.000000 keylime-7.3.0/_pypi-notice.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.135187 keylime-7.3.0/keylime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/agentstates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/backport_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ca_impl_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ca_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cert_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.135187 keylime-7.3.0/keylime/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cli/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cloud_verifier_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65012 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cloud_verifier_tornado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.139186 keylime-7.3.0/keylime/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20465 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/convert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/convert_runtime_policy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22220 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/create_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/sign_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/user_data_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.139186 keylime-7.3.0/keylime/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.139186 keylime-7.3.0/keylime/da/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/attest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.143187 keylime-7.3.0/keylime/da/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/rekor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/sqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/tsa_rfc3161.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.143187 keylime-7.3.0/keylime/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/db/keylime_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/db/registrar_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/db/verifier_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.143187 keylime-7.3.0/keylime/dsse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/dsse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/dsse/dsse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/dsse/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/dsse/x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/fs_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/ima/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/dm_grammar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18388 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/file_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/ima.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/ima_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/keylime_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/mba/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/mba/elchecking/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/mbpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/mba/elparsing/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elparsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elparsing/tpm2_tools_elparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elparsing/tpm_bootlog_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/mba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.155187 keylime-7.3.0/keylime/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/039322ea079b_add_generator_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/registrar_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/registrar_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/requests_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/revocation_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77727 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tornado_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.159187 keylime-7.3.0/keylime/tpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/ec_crypto_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm2_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm2_objects_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm_ek_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/web_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.135187 keylime-7.3.0/keylime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:17:28.000000 keylime-7.3.0/keylime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-30 17:17:19.000000 keylime-7.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-30 17:17:29.163187 keylime-7.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-30 17:17:19.000000 keylime-7.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.127186 keylime-7.3.0/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.159187 keylime-7.3.0/templates/2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/agent.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/ca.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/logging.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    26824 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/registrar.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/tenant.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/verifier.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.163187 keylime-7.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ca_impl_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ca_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_convert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_fs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ima_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ima_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ima_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_mba_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_policy_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_registrar_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_retry_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_verifier_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_web_util.py
```

### Comparing `keylime-7.2.5/LICENSE` & `keylime-7.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/PKG-INFO` & `keylime-7.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keylime
-Version: 7.2.5
+Version: 7.3.0
 Summary: TPM-based key bootstrapping and system integrity measurement system for cloud
 Home-page: https://keylime.dev
 Author: Keylime Community
 Author-email: keylime@groups.io
 License: Apache-2.0
 Project-URL: Source, https://github.com/keylime/keylime
 Project-URL: Documentation, https://keylime.readthedocs.io/en/latest/
```

### Comparing `keylime-7.2.5/README.md` & `keylime-7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/agentstates.py` & `keylime-7.3.0/keylime/agentstates.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/api_version.py` & `keylime-7.3.0/keylime/api_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/backport_dataclasses.py` & `keylime-7.3.0/keylime/backport_dataclasses.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/ca_impl_openssl.py` & `keylime-7.3.0/keylime/ca_impl_openssl.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/ca_util.py` & `keylime-7.3.0/keylime/ca_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cert_utils.py` & `keylime-7.3.0/keylime/cert_utils.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cli/options.py` & `keylime-7.3.0/keylime/cli/options.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cli/policies.py` & `keylime-7.3.0/keylime/cli/policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from typing import Any, Dict, List, Optional, Tuple
 
 from keylime import config, keylime_logging
 from keylime.cmd import convert_runtime_policy
 from keylime.ima import file_signatures, ima
 from keylime.mba import mba
-from keylime.tpm.tpm_abstract import TPM_Utilities
+from keylime.tpm import tpm_util
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
@@ -59,15 +59,15 @@
     runtime_policy = ""
     runtime_policy_key = ""
 
     # Set up PCR values
     if "tpm_policy" in args and args["tpm_policy"] is not None:
         tpm_policy_str = args["tpm_policy"]
 
-    tpm_policy = TPM_Utilities.readPolicy(tpm_policy_str)
+    tpm_policy = tpm_util.readPolicy(tpm_policy_str)
     logger.info("TPM PCR Mask from policy is %s", tpm_policy["mask"])
 
     if len(args["ima_sign_verification_keys"]) > 0:
         # Auto-enable IMA (or-bit mask)
         tpm_policy["mask"] = hex(int(tpm_policy["mask"], 0) | (1 << config.IMA_PCR))
 
         logger.warning(
@@ -165,15 +165,15 @@
             if args["mb_refstate"] == "default":
                 args["mb_refstate"] = config.get("tenant", "mb_refstate")
             mb_refstate_data = mba.load_policy_file(args["mb_refstate"])
         else:
             raise UserError("Invalid measured boot reference state (intended state) provided")
 
     # Set up measured boot (TPM event log) reference state
-    if TPM_Utilities.check_mask(tpm_policy["mask"], config.MEASUREDBOOT_PCRS[2]):
+    if tpm_util.check_mask(tpm_policy["mask"], config.MEASUREDBOOT_PCRS[2]):
         # Process measured boot reference state
         mb_refstate = mb_refstate_data
 
     return (
         tpm_policy,
         mb_refstate,
         runtime_policy_name,
```

### Comparing `keylime-7.2.5/keylime/cloud_verifier_common.py` & `keylime-7.3.0/keylime/cloud_verifier_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from keylime import config, crypto, json, keylime_logging
 from keylime.agentstates import AgentAttestState, AgentAttestStates, TPMClockInfo
 from keylime.common import algorithms
 from keylime.db.verifier_db import VerfierMain
 from keylime.failure import Component, Event, Failure
 from keylime.ima import file_signatures
 from keylime.ima.types import RuntimePolicyType
-from keylime.tpm.tpm_abstract import TPM_Utilities
+from keylime.tpm import tpm_util
 from keylime.tpm.tpm_main import Tpm
 
 # setup logging
 logger = keylime_logging.init_logging("cloudverifier_common")
 
 GLOBAL_TPM_INSTANCE: Optional[Tpm] = None
 DEFAULT_VERIFIER_ID: str = "default"
@@ -241,15 +241,15 @@
 
 def prepare_get_quote(agent: Dict[str, Any]) -> Dict[str, Union[str, int]]:
     """This method encapsulates the action required to invoke a quote request on the Cloud Agent.
 
     This method is part of the polling loop of the thread launched on Tenant POST.
     """
     agentAttestState = get_AgentAttestStates().get_by_agent_id(agent["agent_id"])
-    agent["nonce"] = TPM_Utilities.random_password(20)
+    agent["nonce"] = tpm_util.random_password(20)
 
     tpm_policy = ast.literal_eval(agent["tpm_policy"])
     params = {
         "nonce": agent["nonce"],
         "mask": tpm_policy["mask"],
         "ima_ml_entry": agentAttestState.get_next_ima_ml_entry(),
     }
```

### Comparing `keylime-7.2.5/keylime/cloud_verifier_tornado.py` & `keylime-7.3.0/keylime/cloud_verifier_tornado.py`

 * *Files 1% similar despite different names*

```diff
@@ -998,16 +998,15 @@
         raise NotImplementedError()
 
 
 async def invoke_get_quote(
     agent: Dict[str, Any], runtime_policy: str, need_pubkey: bool, timeout: float = 60.0
 ) -> None:
     failure = Failure(Component.INTERNAL, ["verifier"])
-    if agent is None:
-        raise Exception("agent deleted while being processed")
+
     params = cloud_verifier_common.prepare_get_quote(agent)
 
     partial_req = "1"
     if need_pubkey:
         partial_req = "0"
 
     # TODO: remove special handling after initial upgrade
@@ -1071,18 +1070,17 @@
             logger.exception(e)
             failure.add_event(
                 "exception", {"context": "Agent caused the verifier to throw an exception", "data": str(e)}, False
             )
             asyncio.ensure_future(process_agent(agent, states.FAILED, failure))
 
 
-async def invoke_provide_v(agent: Optional[Dict[str, Any]], timeout: float = 60.0) -> None:
+async def invoke_provide_v(agent: Dict[str, Any], timeout: float = 60.0) -> None:
     failure = Failure(Component.INTERNAL, ["verifier"])
-    if agent is None:
-        raise Exception("Agent deleted while being processed")
+
     if agent.get("pending_event") is not None:
         agent["pending_event"] = None
 
     v_json_message = cloud_verifier_common.prepare_v(agent)
 
     # TODO: remove special handling after initial upgrade
     kwargs = {}
@@ -1111,18 +1109,15 @@
             )
             failure.add_event("no_v", {"message": "Unexpected provide V response", "data": response.status_code}, False)
             asyncio.ensure_future(process_agent(agent, states.FAILED, failure))
     else:
         asyncio.ensure_future(process_agent(agent, states.GET_QUOTE))
 
 
-async def invoke_notify_error(agent: Optional[Dict[str, Any]], tosend: Dict[str, Any], timeout: float = 60.0) -> None:
-    if agent is None:
-        logger.warning("Agent deleted while being processed")
-        return
+async def invoke_notify_error(agent: Dict[str, Any], tosend: Dict[str, Any], timeout: float = 60.0) -> None:
     kwargs = {
         "data": tosend,
     }
     if agent["ssl_context"]:
         kwargs["context"] = agent["ssl_context"]
 
     res = tornado_requests.request(
@@ -1182,18 +1177,14 @@
             except asyncio.TimeoutError as e:
                 logger.error("Timeout during notifying error to agents: %s", e)
 
 
 async def process_agent(
     agent: Dict[str, Any], new_operational_state: int, failure: Failure = Failure(Component.INTERNAL, ["verifier"])
 ) -> None:
-    # Convert to dict if the agent arg is a db object
-    if not isinstance(agent, dict):
-        agent = _from_db_obj(agent)
-
     session = get_session()
     try:  # pylint: disable=R1702
         main_agent_operational_state = agent["operational_state"]
         stored_agent = None
         try:
             stored_agent = (
                 session.query(VerfierMain)
```

### Comparing `keylime-7.2.5/keylime/cmd/convert_config.py` & `keylime-7.3.0/keylime/cmd/convert_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cmd/convert_runtime_policy.py` & `keylime-7.3.0/keylime/cmd/convert_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cmd/create_policy.py` & `keylime-7.3.0/keylime/cmd/create_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cmd/registrar.py` & `keylime-7.3.0/keylime/cmd/registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cmd/sign_runtime_policy.py` & `keylime-7.3.0/keylime/cmd/sign_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cmd/user_data_encrypt.py` & `keylime-7.3.0/keylime/cmd/user_data_encrypt.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/cmd/verifier.py` & `keylime-7.3.0/keylime/cmd/verifier.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     # if we are configured to auto-migrate the DB, check if there are any migrations to perform
     if config.has_option("verifier", "auto_migrate_db") and config.getboolean("verifier", "auto_migrate_db"):
         apply("cloud_verifier")
 
     # Load explicitly the policy modules into Keylime for the verifier,
     # so that they are not loaded accidentally from other components
     mba.load_policy_engine()
+    mba.load_parser_engine()
     cloud_verifier_tornado.main()
 
 
 if __name__ == "__main__":
     try:
         main()
     except Exception as e:
```

### Comparing `keylime-7.2.5/keylime/cmd_exec.py` & `keylime-7.3.0/keylime/cmd_exec.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/common/algorithms.py` & `keylime-7.3.0/keylime/common/algorithms.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/common/migrations.py` & `keylime-7.3.0/keylime/common/migrations.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/common/states.py` & `keylime-7.3.0/keylime/common/states.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/common/validators.py` & `keylime-7.3.0/keylime/common/validators.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/common/version.py` & `keylime-7.3.0/keylime/common/version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/config.py` & `keylime-7.3.0/keylime/config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/crypto.py` & `keylime-7.3.0/keylime/crypto.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/da/attest.py` & `keylime-7.3.0/keylime/da/attest.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         default="last",
         help='end date for attestation window in IS0 8601 format (e.g., "2008-09-03T21:56:35"), or keyworkd "last"',
     )
 
     args = parser.parse_args()
 
     mba.load_policy_engine()
+    mba.load_parser_engine()
 
     rmcb = config.get("registrar", "durable_attestation_import", fallback="")
     rmc = record.get_record_mgt_class(rmcb)
     if not rmc:
         return
 
     rmc = rmc("registrar")
```

### Comparing `keylime-7.2.5/keylime/da/examples/file.py` & `keylime-7.3.0/keylime/da/examples/file.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/da/examples/redis.py` & `keylime-7.3.0/keylime/da/examples/redis.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/da/examples/rekor.py` & `keylime-7.3.0/keylime/da/examples/rekor.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/da/examples/sqldb.py` & `keylime-7.3.0/keylime/da/examples/sqldb.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/da/examples/tsa_rfc3161.py` & `keylime-7.3.0/keylime/da/examples/tsa_rfc3161.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/da/record.py` & `keylime-7.3.0/keylime/da/record.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/db/keylime_db.py` & `keylime-7.3.0/keylime/db/keylime_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/db/registrar_db.py` & `keylime-7.3.0/keylime/db/registrar_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/db/verifier_db.py` & `keylime-7.3.0/keylime/db/verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/dsse/dsse.py` & `keylime-7.3.0/keylime/dsse/dsse.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/dsse/ecdsa.py` & `keylime-7.3.0/keylime/dsse/ecdsa.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/dsse/x509.py` & `keylime-7.3.0/keylime/dsse/x509.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/failure.py` & `keylime-7.3.0/keylime/failure.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/ima/ast.py` & `keylime-7.3.0/keylime/ima/ast.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/ima/dm_grammar.py` & `keylime-7.3.0/keylime/ima/dm_grammar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/ima/file_signatures.py` & `keylime-7.3.0/keylime/ima/file_signatures.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/ima/ima.py` & `keylime-7.3.0/keylime/ima/ima.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import enum
 import functools
 import hashlib
 import json
-from typing import Any, Dict, List, Optional, Pattern, Set, TextIO, Tuple, Type
+from typing import Any, Dict, List, Optional, Pattern, Tuple, Type
 
 import jsonschema
 
 from keylime import config, keylime_logging, signing
 from keylime.agentstates import AgentAttestState
 from keylime.common import algorithms, validators
 from keylime.common.algorithms import Hash
@@ -100,102 +100,14 @@
                 }
             },
         }
     },
 }
 
 
-class IMAMeasurementList:
-    """IMAMeasurementList models the IMA measurement lists's last known
-    two numbers of entries and filesizes
-    """
-
-    instance = None
-    entries: Set[Tuple[int, int]]
-
-    @staticmethod
-    def get_instance() -> "IMAMeasurementList":
-        """Return a singleton"""
-        if not IMAMeasurementList.instance:
-            IMAMeasurementList.instance = IMAMeasurementList()
-        return IMAMeasurementList.instance
-
-    def __init__(self) -> None:
-        """Constructor"""
-        self.entries = set()
-        self.reset()
-
-    def reset(self) -> None:
-        """Reset the variables"""
-        self.entries = set()
-
-    def update(self, num_entries: int, filesize: int) -> None:
-        """Update the number of entries and current filesize of the log."""
-        if len(self.entries) > 256:
-            for entry in self.entries:
-                self.entries.discard(entry)
-                break
-        self.entries.add((num_entries, filesize))
-
-    def find(self, nth_entry: int) -> Tuple[int, int]:
-        """Find the closest entry to the n-th entry and return its number
-        and filesize to seek to, return 0, 0 if nothing was found.
-        """
-        best = (0, 0)
-        for entry in self.entries:
-            if entry[0] > best[0] and entry[0] <= nth_entry:
-                best = entry
-        return best
-
-
-def read_measurement_list(ima_log_file: TextIO, nth_entry: int) -> Tuple[Optional[str], int, int]:
-    """Read the IMA measurement list starting from a given entry.
-    The entry may be of any value 0 <= entry <= entries_in_log where
-    entries_in_log + 1 indicates that the client wants to read the next entry
-    once available. If the entry is outside this range, the function will
-    automatically read from the 0-th entry.
-    This function returns the measurement list and the entry from where it
-    was read and the current number of entries in the file.
-    """
-    IMAML = IMAMeasurementList.get_instance()
-    ml = None
-
-    # Try to find the closest entry to the nth_entry
-    num_entries, filesize = IMAML.find(nth_entry)
-
-    if not ima_log_file:
-        IMAML.reset()
-        nth_entry = 0
-        logger.warning("IMA measurement list not available: %s", config.IMA_ML)
-    else:
-        ima_log_file.seek(filesize)
-        filedata = ima_log_file.read()
-        # filedata now corresponds to starting list at entry number 'IMAML.num_entries'
-        # find n-th entry and determine number of total entries in file now
-        offset = 0
-        while True:
-            try:
-                if nth_entry == num_entries:
-                    ml = filedata[offset:]
-                o = filedata.index("\n", offset)
-                offset = o + 1
-                num_entries += 1
-            except ValueError:
-                break
-        # IMAML.filesize corresponds to position for entry number 'IMAML.num_entries'
-        IMAML.update(num_entries, filesize + offset)
-
-        # Nothing found? User request beyond next-expected entry.
-        # Start over with entry 0. This cannot recurse again.
-        if ml is None:
-            return read_measurement_list(ima_log_file, 0)
-
-    return ml, nth_entry, num_entries
-
-
 def _validate_ima_ng(
     exclude_regex: Optional[Pattern[str]],
     runtime_policy: Optional[RuntimePolicyType],
     digest: ast.Digest,
     path: ast.Name,
     hash_types: str = "digests",
 ) -> Failure:
@@ -213,15 +125,15 @@
 
         hex_hash = digest.hash.hex()
         if hex_hash not in accept_list:
             logger.warning(
                 "Hashes for file %s don't match %s not in %s",
                 path.name,
                 hex_hash,
-                runtime_policy,
+                str(accept_list),
             )
             failure.add_event(
                 "runtime_policy_hash",
                 {
                     "message": "Hash not found in runtime policy",
                     "got": hex_hash,
                     "expected": accept_list,
```

### Comparing `keylime-7.2.5/keylime/ima/ima_dm.py` & `keylime-7.3.0/keylime/ima/ima_dm.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/ima/types.py` & `keylime-7.3.0/keylime/ima/types.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/json.py` & `keylime-7.3.0/keylime/json.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/keylime_logging.py` & `keylime-7.3.0/keylime/keylime_logging.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/mba/elchecking/example.py` & `keylime-7.3.0/keylime/mba/elchecking/example.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/mba/elchecking/mbpolicy.py` & `keylime-7.3.0/keylime/mba/elchecking/mbpolicy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from keylime import config, keylime_logging
 from keylime.failure import Component, Failure
 from keylime.mba.elchecking import tests
 
 logger = keylime_logging.init_logging("measured_boot")
 
 
-def evaluate_policy(
+def evaluate_bootlog(
     mb_refstate_str: Optional[str],
     mb_measurement_data: tests.Data,
     pcrs_inquote: Set[int],
     agent_id: str,
 ) -> Failure:
     failure = Failure(Component.MEASURED_BOOT)
```

### Comparing `keylime-7.2.5/keylime/mba/elchecking/policies.py` & `keylime-7.3.0/keylime/mba/elchecking/policies.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/mba/elchecking/tests.py` & `keylime-7.3.0/keylime/mba/elchecking/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 from keylime.common.algorithms import Hash
 
 # This module defines the abstraction of a Test (of JSON data)
 # and several specific test classes.
 # A Test can be used multiple times, even concurrently.
 
 # Data is the type of Python data that corresponds to JSON values.
-Data = typing.Union[
-    int, float, str, bool, typing.Tuple["Data", ...], typing.Mapping[str, "Data"], typing.List["Data"], None
-]
+# Data = typing.Union[
+#    int, float, str, bool, typing.Tuple["Data", ...], typing.Mapping[str, "Data"], typing.List["Data"], None
+# ]
+# GA: removing recursive definition because mypy cannot handle it.
+
+Data = object
 
 # Globals is a dict of variables for communication among tests.
 # There is a distinct dict for each top-level use of a test.
 Globals = typing.Dict[str, Data]
 
 # PCR_Contents maps digest name to map from PCR index to PCR value.
 # Here digest name is something like 'sha256'.
```

### Comparing `keylime-7.2.5/keylime/migrations/alembic.ini` & `keylime-7.3.0/keylime/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/env.py` & `keylime-7.3.0/keylime/migrations/env.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/039322ea079b_add_generator_column.py` & `keylime-7.3.0/keylime/migrations/versions/039322ea079b_add_generator_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py` & `keylime-7.3.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py` & `keylime-7.3.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py` & `keylime-7.3.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py` & `keylime-7.3.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py` & `keylime-7.3.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def upgrade_cloud_verifier():
     # get existing table metadata
     conn = op.get_bind()
     meta = sa.MetaData()
     meta.reflect(bind=conn, only=("verifiermain",))
     verifiermain = meta.tables["verifiermain"]
 
-    res = conn.execute("SELECT id, name FROM allowlists")
+    res = conn.execute(sa.text("SELECT id, name FROM allowlists"))
     results = res.fetchall()
 
     # Update new foreign key column with associated items in the "allowlists" table
     for allowlist_id, name in results:
         conn.execute(
             verifiermain.update().where(verifiermain.c.agent_id == name).values(**{"ima_policy_id": allowlist_id})
         )
```

### Comparing `keylime-7.2.5/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py` & `keylime-7.3.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py` & `keylime-7.3.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py` & `keylime-7.3.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py` & `keylime-7.3.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 def upgrade_cloud_verifier():
     # get existing table metadata
     conn = op.get_bind()
     meta = sa.MetaData()
     meta.reflect(bind=conn, only=("allowlists",))
     allowlists = meta.tables["allowlists"]
-    results = conn.execute("SELECT id, ima_policy FROM allowlists").fetchall()
+    results = conn.execute(sa.text("SELECT id, ima_policy FROM allowlists")).fetchall()
 
     # Update allowlist entries with converted IMA policies
     for old_ima_policy_id, old_ima_policy in results:
         try:
             old_ima_policy = json.loads(old_ima_policy)
         except Exception as e:
             message = "Error loading JSON-formatted Keylime policy: %s", repr(e)
@@ -88,15 +88,15 @@
 
 def downgrade_cloud_verifier():
     # get existing table metadata
     conn = op.get_bind()
     meta = sa.MetaData()
     meta.reflect(bind=conn, only=("allowlists",))
     allowlists = meta.tables["allowlists"]
-    results = conn.execute("SELECT id, ima_policy FROM allowlists").fetchall()
+    results = conn.execute(sa.text("SELECT id, ima_policy FROM allowlists")).fetchall()
 
     # Update allowlist entries with converted IMA policies
     for ima_policy_id, ima_policy in results:
         try:
             ima_policy = json.loads(ima_policy)
         except Exception as e:
             message = "Error loading JSON-formatted Keylime policy: %s", repr(e)
```

### Comparing `keylime-7.2.5/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py` & `keylime-7.3.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py` & `keylime-7.3.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py` & `keylime-7.3.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py` & `keylime-7.3.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     pass
 
 
 def upgrade_cloud_verifier():
     # Migrate existing agent info to the allowlists table.
     conn = op.get_bind()
 
-    res = conn.execute("SELECT agent_id, tpm_policy, allowlist FROM verifiermain")
+    res = conn.execute(sa.text("SELECT agent_id, tpm_policy, allowlist FROM verifiermain"))
     results = res.fetchall()
     old_policy = [{"name": r[0], "tpm_policy": r[1], "ima_policy": r[2]} for r in results]
 
     # get existing table metadata
     meta = sa.MetaData()
     meta.reflect(bind=conn, only=("allowlists",))
     allowlists = meta.tables["allowlists"]
@@ -57,15 +57,15 @@
     # Migrate existing agent info to the allowlist column in verifiermain.
     conn = op.get_bind()
     meta = sa.MetaData()
     meta.reflect(bind=conn, only=("verifiermain", "allowlists"))
     verifiermain = meta.tables["verifiermain"]
     allowlists = meta.tables["allowlists"]
 
-    res = conn.execute("SELECT name, ima_policy FROM allowlists")
+    res = conn.execute(sa.text("SELECT name, ima_policy FROM allowlists"))
     results = res.fetchall()
 
     # Put allowlists back into the "allowlist" column, and delete from the "allowlists" database
     for name, ima_policy in results:
         conn.execute(verifiermain.update().where(verifiermain.c.agent_id == name).values(**{"allowlist": ima_policy}))
         conn.execute(allowlists.delete().where(allowlists.c.name == name))
```

### Comparing `keylime-7.2.5/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py` & `keylime-7.3.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py` & `keylime-7.3.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py` & `keylime-7.3.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py` & `keylime-7.3.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py` & `keylime-7.3.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py` & `keylime-7.3.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py` & `keylime-7.3.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py` & `keylime-7.3.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py` & `keylime-7.3.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py` & `keylime-7.3.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py` & `keylime-7.3.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py` & `keylime-7.3.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py` & `keylime-7.3.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/registrar_client.py` & `keylime-7.3.0/keylime/registrar_client.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/registrar_common.py` & `keylime-7.3.0/keylime/registrar_common.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/requests_client.py` & `keylime-7.3.0/keylime/requests_client.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/revocation_notifier.py` & `keylime-7.3.0/keylime/revocation_notifier.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/signing.py` & `keylime-7.3.0/keylime/signing.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/tenant.py` & `keylime-7.3.0/keylime/tenant.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 from keylime import ca_util, cert_utils, config, crypto, keylime_logging, registrar_client, signing, web_util
 from keylime.agentstates import AgentAttestState
 from keylime.cli import options, policies
 from keylime.cmd import user_data_encrypt
 from keylime.common import algorithms, retry, states, validators
 from keylime.ip_util import bracketize_ipv6
 from keylime.requests_client import RequestsClient
-from keylime.tpm import tpm2_objects
-from keylime.tpm.tpm_abstract import TPM_Utilities
+from keylime.tpm import tpm2_objects, tpm_util
 from keylime.tpm.tpm_main import Tpm
 
 # setup logging
 logger = keylime_logging.init_logging("tenant")
 
 
 # special exception that suppresses stack traces when it happens
@@ -83,14 +82,18 @@
     trusted_server_ca: List[str] = []
     enable_agent_mtls: bool = False
     verify_server_cert: bool = False
     verify_custom: Optional[str] = None
 
     request_timeout: Optional[int] = None
 
+    agent_fid_str: Optional[str] = None
+    verifier_fid_str: Optional[str] = None
+    registrar_fid_str: Optional[str] = None
+
     # Context with the trusted CA certificates from the configuration
     tls_context: Optional[ssl.SSLContext] = None
 
     # Context with the agent's mTLS certificate
     agent_tls_context: Optional[ssl.SSLContext] = None
 
     payload: Optional[bytes] = None
@@ -153,14 +156,27 @@
         else:
             logger.warning("TLS is disabled.")
 
     @property
     def verifier_base_url(self) -> str:
         return f"{bracketize_ipv6(self.verifier_ip)}:{self.verifier_port}"
 
+    def set_full_id_str(self) -> None:
+        self.agent_fid_str = f"Agent {self.agent_uuid}"
+        if self.agent_ip:
+            self.agent_fid_str = f"{self.agent_fid_str} ({self.agent_ip}:{self.agent_port})"
+        self.verifier_fid_str = "Verifier"
+        if self.verifier_id:
+            self.verifier_fid_str = f"{self.verifier_fid_str} {self.verifier_id}"
+        if self.verifier_ip:
+            self.verifier_fid_str = f"{self.verifier_fid_str} ({self.verifier_ip}:{self.verifier_port})"
+        self.registrar_fid_str = "Registrar"
+        if self.registrar_ip:
+            self.registrar_fid_str = f"{self.registrar_fid_str} ({self.registrar_ip}:{self.registrar_port})"
+
     def init_add(self, args: Dict[str, Any]) -> None:
         """Set up required values. Command line options can overwrite these config values
 
         Arguments:
             args {[string]} -- agent_ip|agent_port|cv_agent_ip
         """
         if "agent_ip" in args:
@@ -192,28 +208,31 @@
         # Check if a contact ip and port for the agent was found
         if self.agent_ip is None:
             raise UserError("The contact ip address for the agent was not specified.")
 
         if self.agent_port is None:
             raise UserError("The contact port for the agent was not specified.")
 
+        self.set_full_id_str()
+
         # Auto-detection for API version
         self.supported_version = args["supported_version"]
         if self.supported_version is None:
             # Default to 1.0 if the agent did not send a mTLS certificate
             if self.registrar_data.get("mtls_cert", None) is None:
                 self.supported_version = "1.0"
             else:
                 # Try to connect to the agent to get supported version
                 if self.registrar_data["mtls_cert"] == "disabled":
                     self.enable_agent_mtls = False
                     logger.warning(
-                        "Warning: mTLS for agents is disabled: the identity of each node will be based on the properties of the TPM only. "
+                        "Warning: mTLS for %s is disabled: the identity of each node will be based on the properties of the TPM only. "
                         "Unless you have strict control of your network, it is strongly advised that remote code execution should be disabled, "
-                        'by setting "payload_script=" and "extract_payload_zip=False" under "[agent]" in agent configuration file.'
+                        'by setting "payload_script=" and "extract_payload_zip=False" under "[agent]" in agent configuration file.',
+                        self.agent_fid_str,
                     )
                     tls_context = None
                 else:
                     # Store the agent self-signed certificate as a string
                     self.verify_custom = self.registrar_data["mtls_cert"]
 
                     if not self.agent_tls_context:
@@ -439,20 +458,22 @@
             ekcert {str} -- The endorsement key, either None, "emulator", or base64 encoded der cert
 
         Returns:
             [type] -- [description]
         """
         if config.getboolean("tenant", "require_ek_cert"):
             if ekcert == "emulator" and config.DISABLE_EK_CERT_CHECK_EMULATOR:
-                logger.info("Not checking ekcert of TPM emulator")
+                logger.info("Not checking ekcert of TPM emulator for %s", self.agent_fid_str)
             elif ekcert is None:
-                logger.warning("No EK cert provided, require_ek_cert option in config set to True")
+                logger.warning(
+                    "No EK cert provided, require_ek_cert option in config set to True for %s", self.agent_fid_str
+                )
                 return False
             elif not self.tpm_instance.verify_ek(base64.b64decode(ekcert), config.get("tenant", "tpm_cert_store")):
-                logger.warning("Invalid EK certificate")
+                logger.warning("Invalid EK certificate for %s", self.agent_fid_str)
                 return False
 
         return True
 
     def validate_tpm_quote(self, public_key: str, quote: str, hash_alg: algorithms.Hash) -> bool:
         """Validate TPM Quote received from the Agent
 
@@ -464,46 +485,44 @@
         Raises:
             UserError: [description]
 
         Returns:
             [type] -- [description]
         """
         if self.registrar_data is None:
-            logger.warning("AIK not found in registrar, quote not validated")
+            logger.warning(
+                "AIK not found in %s, quote not validated for %s", self.registrar_fid_str, self.agent_fid_str
+            )
             return False
 
         if not self.nonce:
-            logger.warning("Nonce has not been set!")
+            logger.warning("Nonce has not been set for %s!", self.agent_fid_str)
             return False
 
         failure = self.tpm_instance.check_quote(
             AgentAttestState(self.agent_uuid),
             self.nonce,
             public_key,
             quote,
             self.registrar_data["aik_tpm"],
             hash_alg=hash_alg,
             compressed=(self.supported_version == "1.0"),
         )
         if failure:
             if self.registrar_data["regcount"] > 1:
                 logger.error(
-                    "WARNING: This UUID had more than one ek-ekcert registered to it! This might indicate that your system is misconfigured or a malicious host is present. Run 'regdelete' for this agent and restart"
+                    "WARNING: %s had more than one ek-ekcert registered to it! This might indicate that your system is misconfigured or a malicious host is present. Run 'regdelete' for this agent and restart",
+                    self.agent_fid_str,
                 )
-                sys.exit()
             return False
 
-        if self.registrar_data["regcount"] > 1:
-            logger.warning(
-                "WARNING: This UUID had more than one ek-ekcert registered to it! This might indicate that your system is misconfigured. Run 'regdelete' for this agent and restart"
-            )
-
         if not config.getboolean("tenant", "require_ek_cert") and config.get("tenant", "ek_check_script") == "":
             logger.warning(
-                "DANGER: EK cert checking is disabled and no additional checks on EKs have been specified with ek_check_script option. Keylime is not secure!!"
+                "DANGER: EK cert checking is disabled and no additional checks on EKs have been specified with ek_check_script option for %s. Keylime is not secure!!",
+                self.agent_fid_str,
             )
             return True
 
         # check EK cert and make sure it matches EK
         if not self.check_ek(self.registrar_data["ekcert"]):
             return False
         # if agent is virtual, check phyisical EK cert and make sure it matches phyiscal EK
@@ -515,15 +534,15 @@
         script = config.get("tenant", "ek_check_script")
         if not script:
             return True
 
         if script[0] != "/":
             script = os.path.join(config.WORK_DIR, script)
 
-        logger.info("Checking EK with script %s", script)
+        logger.info("Checking EK for %s with script %s", self.agent_fid_str, script)
         # now we need to exec the script with the ek and ek cert in vars
         env = os.environ.copy()
         env["AGENT_UUID"] = self.agent_uuid
         env["EK"] = (
             tpm2_objects.pubkey_from_tpm2b_public(
                 base64.b64decode(self.registrar_data["ek_tpm"]),
             )
@@ -576,173 +595,190 @@
         do_cv = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
         response = do_cv.post(
             (f"/v{self.api_version}/agents/{self.agent_uuid}"), data=json_message, timeout=self.request_timeout
         )
 
         if response.status_code == 503:
             logger.error(
-                "Cannot connect to Verifier at %s with Port %s. Connection refused.",
-                self.verifier_ip,
-                self.verifier_port,
+                "Cannot connect to %s while adding %s. Connection refused.",
+                self.verifier_fid_str,
+                self.agent_fid_str,
             )
             sys.exit()
         elif response.status_code == 504:
-            logger.error("Verifier at %s with Port %s timed out.", self.verifier_ip, self.verifier_port)
+            logger.error("%s timed out while adding %s.", self.verifier_fid_str, self.agent_fid_str)
             sys.exit()
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response.status_code == 409:
             # this is a conflict, need to update or delete it
             print(response_json)
             sys.exit()
         elif response.status_code != 200:
             keylime_logging.log_http_response(logger, logging.ERROR, response_json)
             logger.error(
-                "POST command response: %s Unexpected response from Cloud Verifier: %s",
+                "POST command response: %s Unexpected response from %s: %s",
                 response.status_code,
+                self.verifier_fid_str,
                 response.text,
             )
             sys.exit()
         else:
             numtries = 0
             added = False
 
             while not added:
                 reponse_json = self.do_cvstatus()
                 if reponse_json["code"] != 200:
                     numtries += 1
                     if numtries >= self.maxr:
                         logger.error(
-                            "Agent ID %s still not added to the Verifier after %d tries",
-                            self.agent_uuid,
+                            "%s still not added to %s after %d tries",
+                            self.agent_fid_str,
+                            self.verifier_fid_str,
                             numtries,
                         )
                         sys.exit()
                     next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                     logger.info(
-                        "Agent ID %s still not added to the Verifier at try %d of %d , trying again in %s seconds...",
-                        self.agent_uuid,
+                        "%s still not added to %s at try %d/%d, trying again in %d seconds...",
+                        self.agent_fid_str,
+                        self.verifier_fid_str,
                         numtries,
                         self.maxr,
                         next_retry,
                     )
                     time.sleep(next_retry)
                 else:
                     added = True
 
             if added:
                 logger.info(
-                    "Agent ID %s added to the Verifier after %d tries",
-                    self.agent_uuid,
+                    "%s added to %s after %d tries",
+                    self.agent_fid_str,
+                    self.verifier_fid_str,
                     numtries,
                 )
 
     def do_cvstatus(self) -> Dict[str, Any]:
         """Perform operational state look up for agent on the verifier"""
 
+        self.set_full_id_str()
+
         do_cvstatus = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
 
         response = do_cvstatus.get((f"/v{self.api_version}/agents/{self.agent_uuid}"), timeout=self.request_timeout)
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response.status_code == 503:
             logger.error(
-                "Cannot connect to Verifier at %s with Port %s. Connection refused.",
-                self.verifier_ip,
-                self.verifier_port,
+                "Cannot connect to %s. Connection refused.",
+                self.verifier_fid_str,
             )
             return response_json
         if response.status_code == 504:
-            logger.error("Verifier at %s with Port %s timed out.", self.verifier_ip, self.verifier_port)
+            logger.error("%s timed out.", self.verifier_fid_str)
             return response_json
         if response.status_code == 404:
+            # Marked for deletion (need to modify the code on CI tests)
             logger.info(
                 "Verifier at %s with Port %s does not have agent %s.",
                 self.verifier_ip,
                 self.verifier_port,
                 self.agent_uuid,
             )
+            logger.info(
+                "%s does not exist on %s.",
+                self.agent_fid_str,
+                self.verifier_fid_str,
+            )
             return response_json
 
         if response.status_code == 200:
             res = response_json.pop("results")
             response_json["results"] = {self.agent_uuid: res}
 
             operational_state = states.state_to_str(response_json["results"][self.agent_uuid]["operational_state"])
             response_json["results"][self.agent_uuid]["operational_state"] = operational_state
 
-            logger.info("Agent Info:\n%s", json.dumps(response_json["results"]))
+            logger.info("Agent Info from %s:\n%s", self.verifier_fid_str, json.dumps(response_json["results"]))
 
             return response_json
 
         logger.info(
-            "Status command response: %s. Unexpected response from Cloud Verifier %s on port %s. %s",
+            "Status command response: %s. Unexpected response from %s. %s",
             response.status_code,
-            self.verifier_ip,
-            self.verifier_port,
+            self.verifier_fid_str,
             str(response),
         )
         return response_json
 
     def do_cvlist(self) -> Union[requests.Response, Dict[str, Any]]:
         """List all agent statuses in cloudverifier"""
 
         do_cvstatus = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
 
         verifier_id = ""
         if self.verifier_id is not None:
             verifier_id = self.verifier_id
 
+        self.set_full_id_str()
+
         response = do_cvstatus.get(f"/v{self.api_version}/agents/?verifier={verifier_id}", timeout=self.request_timeout)
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response.status_code == 503:
             logger.error(
-                "Cannot connect to Verifier at %s with Port %s. Connection refused.",
-                self.verifier_ip,
-                self.verifier_port,
+                "Cannot connect to %s. Connection refused.",
+                self.verifier_fid_str,
             )
             return response_json
         if response.status_code == 504:
-            logger.error("Verifier at %s with Port %s timed out.", self.verifier_ip, self.verifier_port)
+            logger.error("%s timed out.", self.verifier_fid_str)
             return response_json
         if response.status_code == 404:
             logger.info(
-                "Verifier at %s with Port %s does not have agent %s.",
-                self.verifier_ip,
-                self.verifier_port,
-                self.agent_uuid,
+                "%s does not have any agents",
+                self.verifier_fid_str,
             )
             return response_json
         if response.status_code == 200:
-            logger.info('From verifier %s port %s retrieved: "%s"', self.verifier_ip, self.verifier_port, response_json)
+            # Marked for deletion (need to modify the code on CI tests)
+            logger.info(
+                'From verifier %s port %s retrieved: "%s"\n', self.verifier_ip, self.verifier_port, response_json
+            )
+
+            logger.info(
+                "Agent list from %s retrieved: \n%s", self.verifier_fid_str, json.dumps(response_json["results"])
+            )
 
             return response
 
         logger.info(
-            "Status command response: %s. Unexpected response from Cloud Verifier %s on port %s. %s",
+            "Status command response: %s. Unexpected response from %s. %s",
             response.status_code,
-            self.verifier_ip,
-            self.verifier_port,
+            self.verifier_fid_str,
             str(response),
         )
         return response
 
     def do_cvbulkinfo(self) -> Dict[str, Any]:
-        """Perform operational state look up for agent"""
+        """Perform operational state look up for all agents"""
 
         do_cvstatus = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
 
         verifier_id = ""
         if self.verifier_id is not None:
             verifier_id = self.verifier_id
 
+        self.set_full_id_str()
+
         response = do_cvstatus.get(
             f"/v{self.api_version}/agents/?bulk={True}&verifier={verifier_id}", timeout=self.request_timeout
         )
 
         response_json = Tenant._jsonify_response(response, print_response=False)
 
         if response.status_code == 200:
@@ -751,138 +787,167 @@
                     response_json["results"][agent]["operational_state"]
                 )
             logger.info("Bulk Agent Info:\n%s", json.dumps(response_json["results"]))
 
             return response_json
 
         raise UserError(
-            f"Bulk Status: Unexpected response from Verifier {self.verifier_ip} on port {self.verifier_port}. Response status code is {response.status_code}"
+            f"Bulk Status: Unexpected response from {self.verifier_fid_str}. Response status code is {response.status_code}"
         )
 
     def do_cvdelete(self, verifier_check: bool = True) -> None:
         """Delete agent from Verifier."""
+
+        self.set_full_id_str()
+
         if verifier_check:
             cvresponse = self.do_cvstatus()
 
             if not isinstance(cvresponse, dict):
                 keylime_logging.log_http_response(logger, logging.ERROR, cvresponse)
                 sys.exit()
 
             if cvresponse["code"] == 404:
                 logger.info(
-                    "Agent ID %s deleted from Verifier",
-                    self.agent_uuid,
+                    "The %s is deleted from %s",
+                    self.agent_fid_str,
+                    self.verifier_fid_str,
                 )
                 return
 
             if self.agent_uuid in cvresponse["results"]:
                 self.verifier_ip = cvresponse["results"][self.agent_uuid]["verifier_ip"]
                 self.verifier_port = cvresponse["results"][self.agent_uuid]["verifier_port"]
+                self.verifier_id = cvresponse["results"][self.agent_uuid]["verifier_id"]
+                self.agent_ip = cvresponse["results"][self.agent_uuid]["ip"]
+                self.agent_port = cvresponse["results"][self.agent_uuid]["port"]
+                self.set_full_id_str()
 
         do_cvdelete = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
         response = do_cvdelete.delete(f"/v{self.api_version}/agents/{self.agent_uuid}", timeout=self.request_timeout)
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response_json["code"] == 503:
             logger.error(
-                "Cannot connect to Verifier at %s with Port %s. Connection refused.",
-                self.verifier_ip,
-                self.verifier_port,
+                "Cannot connect to %s to delete %s. Connection refused.",
+                self.verifier_fid_str,
+                self.agent_fid_str,
             )
             keylime_logging.log_http_response(logger, logging.ERROR, response_json)
             sys.exit()
 
         if response_json["code"] == 504:
-            logger.error("Verifier at %s with Port %s timed out.", self.verifier_ip, self.verifier_port)
+            logger.error("%s timed out while deleting %s.", self.verifier_fid_str, self.agent_fid_str)
             keylime_logging.log_http_response(logger, logging.ERROR, response_json)
             sys.exit()
 
         if response_json["code"] == 202:
             numtries = 0
             deleted = False
 
             while not deleted:
                 reponse_json = self.do_cvstatus()
                 if reponse_json["code"] != 404:
                     numtries += 1
                     if numtries >= self.maxr:
                         logger.error(
-                            "Agent ID %s still not deleted from the Verifier after %d tries",
-                            self.agent_uuid,
+                            "%s was not deleted from %s after %d tries",
+                            self.agent_fid_str,
+                            self.verifier_fid_str,
                             numtries,
                         )
                         sys.exit()
                     next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                     logger.info(
-                        "Agent ID %s still not deleted from the Verifier at try %d of %d , trying again in %s seconds...",
-                        self.agent_uuid,
+                        "%s still not deleted from %s at try %d/%d, trying again in %s seconds...",
+                        self.agent_fid_str,
+                        self.verifier_fid_str,
                         numtries,
                         self.maxr,
                         next_retry,
                     )
                     time.sleep(next_retry)
                 else:
                     deleted = True
 
             if deleted:
                 logger.info(
-                    "Agent ID %s deleted from the Verifier after %d tries",
-                    self.agent_uuid,
+                    "%s was deleted from %s after %d tries",
+                    self.agent_fid_str,
+                    self.verifier_fid_str,
                     numtries,
                 )
-
+                # Marked for deletion (need to modify the code on CI tests)
                 logger.info("Agent %s deleted from the CV", self.agent_uuid)
 
     def do_regstatus(self) -> Dict[str, Any]:
         if not self.registrar_ip or not self.registrar_port:
             raise UserError("registrar_ip and registrar_port have both to be set in the configuration")
 
+        self.set_full_id_str()
+
         agent_info = registrar_client.getData(self.registrar_ip, self.registrar_port, self.agent_uuid, self.tls_context)
 
         if not agent_info:
             logger.info(
+                # Marked for deletion (the message should be replaced by the 3 following commented out lines)
                 "Agent %s does not exist on the registrar. Please register the agent with the registrar.",
                 self.agent_uuid,
+                # "%s does not exist on %s. Check the agent logs to for error messages while attempting to get registered.",
+                # self.agent_fid_str,
+                # self.registrar_fid_str,
             )
             response = {
                 "code": 404,
+                # Marked for deletion. The "status" field should be replaced by "status": f"{self.agent_fid_str} does not exist on {self.registrar_fid_str}.",
                 "status": f"Agent {self.agent_uuid} does not exist on "
                 f"registrar {self.registrar_ip} port {self.registrar_port}.",
                 "results": {},
             }
             logger.info(json.dumps(response))
             return response
 
+        # Marked for deletion (the "status" line need to be changed to f"registrar {self.registrar_ip} port {self.registrar_port}.")
         response = {
             "code": 200,
             "status": f"Agent {self.agent_uuid} exists on "
             f"registrar {self.registrar_ip} port {self.registrar_port}.",
             "results": {},
         }
+
         assert isinstance(response["results"], dict)
         response["results"][self.agent_uuid] = agent_info
         response["results"][self.agent_uuid]["operational_state"] = states.state_to_str(states.REGISTERED)
 
+        logger.info("Status from %s: %s", self.registrar_fid_str, response["status"])
         logger.info(json.dumps(response))
+        logger.info("Agent Info from %s:\n%s", self.registrar_fid_str, json.dumps(response["results"]))
 
         return response
 
     def do_reglist(self) -> Optional[Dict[str, Any]]:
         """List agents from Registrar"""
         if not self.registrar_ip or not self.registrar_port:
             raise UserError("registrar_ip and registrar_port have both to be set in the configuration")
 
+        self.set_full_id_str()
+
         response = registrar_client.doRegistrarList(
             self.registrar_ip, self.registrar_port, tls_context=self.tls_context
         )
 
+        # Marked for deletion (need to modify the code on CI tests)
         logger.info(
-            "From registrar %s port %s retrieved %s", self.registrar_ip, self.registrar_port, json.dumps(response)
+            "From registrar %s port %s retrieved %s\n", self.registrar_ip, self.registrar_port, json.dumps(response)
         )
+        assert isinstance(response, dict)
+        assert isinstance(response["results"], dict)
+        logger.info("Agent list from %s retrieved: \n%s", self.registrar_fid_str, json.dumps(response["results"]))
+
         return response
 
     def do_regdelete(self) -> Dict[str, Any]:
         """Delete agent from Registrar"""
         if not self.registrar_ip or not self.registrar_port:
             raise UserError("registrar_ip and registrar_port have both to be set in the configuration")
 
@@ -900,106 +965,110 @@
         if regresponse["code"] == 404:
             return regresponse
 
         cvresponse = self.do_cvstatus()
 
         if not isinstance(cvresponse, dict):
             logger.error(
-                "Unexpected response from Cloud Verifier %s on port %s. response %s",
-                self.verifier_ip,
-                self.verifier_port,
+                "Unexpected response from %s: %s",
+                self.verifier_fid_str,
                 str(cvresponse),
             )
             return cvresponse
 
         if regresponse["code"] == 200 and cvresponse["code"] == 200:
             return cvresponse
         if regresponse["code"] == 200 and cvresponse["code"] != 200:
             return regresponse
 
         logger.error(
-            "Unknown inconsistent state between registrar %s on "
-            "port %s and verifier %s on port %s occured. Got "
-            "registrar response %s verifier response %s",
-            self.verifier_ip,
-            self.verifier_port,
-            self.registrar_ip,
-            self.registrar_port,
+            "Unknown inconsistent state between %s and %s occured. Got %s from the former and %s from the latter",
+            self.registrar_fid_str,
+            self.verifier_fid_str,
             str(regresponse),
             str(cvresponse),
         )
 
         return {"registrar": regresponse, "verifier": cvresponse}
 
     def do_cvreactivate(self, verifier_check: bool = True) -> Dict[str, Any]:
         """Reactive Agent."""
         if verifier_check:
-            agent_json = self.do_cvstatus()
-            self.verifier_ip = agent_json["results"][self.agent_uuid]["verifier_ip"]
-            self.verifier_port = agent_json["results"][self.agent_uuid]["verifier_port"]
+            cvresponse = self.do_cvstatus()
+            self.verifier_ip = cvresponse["results"][self.agent_uuid]["verifier_ip"]
+            self.verifier_port = cvresponse["results"][self.agent_uuid]["verifier_port"]
+            self.verifier_id = cvresponse["results"][self.agent_uuid]["verifier_id"]
+
+        self.set_full_id_str()
 
         do_cvreactivate = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
         response = do_cvreactivate.put(
             f"/v{self.api_version}/agents/{self.agent_uuid}/reactivate",
             data=b"",
             timeout=self.request_timeout,
         )
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response.status_code == 503:
             logger.error(
-                "Cannot connect to Verifier at %s with Port %s. Connection refused.",
-                self.verifier_ip,
-                self.verifier_port,
+                "Cannot connect to %s. Connection refused.",
+                self.verifier_fid_str,
             )
             return response_json
         if response.status_code == 504:
-            logger.error("Verifier at %s with Port %s timed out.", self.verifier_ip, self.verifier_port)
+            logger.error("%s timed out.", self.verifier_fid_str)
             return response_json
         if response.status_code == 200:
+            # Marked for deletion (need to modify the code on CI tests)
             logger.info("Agent %s re-activated", self.agent_uuid)
+            logger.info("%s re-activated", self.agent_fid_str)
             return response_json
 
         keylime_logging.log_http_response(logger, logging.ERROR, response_json)
-        logger.error("Reactivate command response: %s Unexpected response from Cloud Verifier.", response.status_code)
+        logger.error(
+            "Reactivate command response: %s Unexpected response from %s.", response.status_code, self.verifier_fid_str
+        )
         return response_json
 
     def do_cvstop(self) -> None:
         """Stop declared active agent"""
         params = f"/v{self.api_version}/agents/{self.agent_uuid}/stop"
         do_cvstop = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
         response = do_cvstop.put(params, data=b"", timeout=self.request_timeout)
 
+        self.set_full_id_str()
+
         if response.status_code == 503:
             logger.error(
-                "Cannot connect to Verifier at %s with Port %s. Connection refused.",
-                self.verifier_ip,
-                self.verifier_port,
+                "Cannot connect to %s. Connection refused.",
+                self.verifier_fid_str,
             )
             sys.exit()
         elif response.status_code == 504:
-            logger.error("Verifier at %s with Port %s timed out.", self.verifier_ip, self.verifier_port)
+            logger.error("%s timed out.", self.verifier_fid_str)
             sys.exit()
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response.status_code != 200:
             keylime_logging.log_http_response(logger, logging.ERROR, response_json)
-            logger.error("Stop command response: %s Unexpected response from Cloud Verifier.", response.status_code)
+            logger.error(
+                "Stop command response: %s Unexpected response from %s.", response.status_code, self.verifier_fid_str
+            )
         else:
-            logger.info("Agent %s stopped", self.agent_uuid)
+            logger.info("%s stopped", self.agent_fid_str)
 
     def do_quote(self) -> None:
         """Perform TPM quote by GET towards Agent
 
         Raises:
             UserError: Connection handler
         """
-        self.nonce = TPM_Utilities.random_password(20)
+        self.nonce = tpm_util.random_password(20)
 
         numtries = 0
         response = None
         # Note: We need a specific retry handler (perhaps in common), no point having localised unless we have too.
         while True:
             try:
                 params = f"/v{self.supported_version}/quotes/identity?nonce=%s" % (self.nonce)
@@ -1009,80 +1078,85 @@
                     with RequestsClient(
                         cloudagent_base_url,
                         self.enable_agent_mtls,
                         tls_context=self.agent_tls_context,
                     ) as do_quote:
                         response = do_quote.get(params, timeout=self.request_timeout)
                 else:
-                    logger.warning("Connecting to agent without using mTLS!")
+                    logger.warning("Connecting to %s without using mTLS!", self.agent_fid_str)
                     do_quote = RequestsClient(cloudagent_base_url, tls_enabled=False)
                     response = do_quote.get(params, timeout=self.request_timeout)
 
                 response_json = Tenant._jsonify_response(response, print_response=True, raise_except=True)
 
             except Exception as e:
                 if response is None or response.status_code in (503, 504):
                     numtries += 1
                     if numtries >= self.maxr:
                         logger.error(
-                            "Tenant cannot establish connection to agent on %s with port %s",
-                            self.agent_ip,
-                            self.agent_port,
+                            "Tenant cannot establish connection to %s",
+                            self.agent_fid_str,
                         )
                         sys.exit()
                     next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                     logger.info(
-                        "Tenant connection to agent at %s refused %s/%s times, trying again in %s seconds...",
-                        self.agent_ip,
+                        "Tenant connection to %s refused %s/%s times, trying again in %s seconds...",
+                        self.agent_fid_str,
                         numtries,
                         self.maxr,
                         next_retry,
                     )
                     time.sleep(next_retry)
                     continue
 
                 raise e
             break
 
         if response is not None and response.status_code != 200:
-            raise UserError(f"Status command response: {response.status_code} Unexpected response from Cloud Agent.")
+            raise UserError(
+                f"Status command response: {response.status_code} Unexpected response from {self.agent_fid_str}."
+            )
 
         if "results" not in response_json:
-            raise UserError(f"Error: unexpected http response body from Cloud Agent: {str(response.status_code)}")
+            raise UserError(
+                f"Error: unexpected http response body from {self.agent_fid_str}: {str(response.status_code)}"
+            )
 
         quote = response_json["results"]["quote"]
-        logger.debug("Agent_quote received quote: %s", quote)
+        logger.debug("Tenant received quote from %s: %s", self.agent_fid_str, quote)
 
         public_key = response_json["results"]["pubkey"]
-        logger.debug("Agent_quote received public key: %s", public_key)
+        logger.debug("Tenant received public key from %s: %s", self.agent_fid_str, public_key)
 
         # Ensure hash_alg is in accept_tpm_hash_algs list
         hash_alg = response_json["results"]["hash_alg"]
-        logger.debug("Agent_quote received hash algorithm: %s", hash_alg)
+        logger.debug("Tenant received hash algorithm from %s: %s", self.agent_fid_str, hash_alg)
         if not algorithms.is_accepted(
             hash_alg, config.getlist("tenant", "accept_tpm_hash_algs")
         ) or not algorithms.Hash.is_recognized(hash_alg):
-            raise UserError(f"TPM Quote is using an unaccepted hash algorithm: {hash_alg}")
+            raise UserError(f"TPM Quote from {self.agent_fid_str} is using an unaccepted hash algorithm: {hash_alg}")
 
         # Ensure enc_alg is in accept_tpm_encryption_algs list
         enc_alg = response_json["results"]["enc_alg"]
-        logger.debug("Agent_quote received encryption algorithm: %s", enc_alg)
+        logger.debug("Tenant received received encryption algorithm from %s: %s", self.agent_fid_str, enc_alg)
         if not algorithms.is_accepted(enc_alg, config.getlist("tenant", "accept_tpm_encryption_algs")):
-            raise UserError(f"TPM Quote is using an unaccepted encryption algorithm: {enc_alg}")
+            raise UserError(
+                f"TPM Quote from {self.agent_fid_str} is using an unaccepted encryption algorithm: {enc_alg}"
+            )
 
         # Ensure sign_alg is in accept_tpm_encryption_algs list
         sign_alg = response_json["results"]["sign_alg"]
-        logger.debug("Agent_quote received signing algorithm: %s", sign_alg)
+        logger.debug("Tenant received signing algorithm from %s: %s", self.agent_fid_str, sign_alg)
         if not algorithms.is_accepted(sign_alg, config.getlist("tenant", "accept_tpm_signing_algs")):
-            raise UserError(f"TPM Quote is using an unaccepted signing algorithm: {sign_alg}")
+            raise UserError(f"TPM Quote from {self.agent_fid_str} is using an unaccepted signing algorithm: {sign_alg}")
 
         if not self.validate_tpm_quote(public_key, quote, algorithms.Hash(hash_alg)):
-            raise UserError(f"TPM Quote from cloud agent is invalid for nonce: {self.nonce}")
+            raise UserError(f"TPM Quote from {self.agent_fid_str} is invalid for nonce: {self.nonce}")
 
-        logger.info("Quote from %s validated", self.agent_ip)
+        logger.info("Quote from %s validated", self.agent_fid_str)
 
         # encrypt U with the public key
         encrypted_U = crypto.rsa_encrypt(crypto.rsa_import_pubkey(public_key), self.U)
 
         b64_encrypted_u = base64.b64encode(encrypted_U)
         logger.debug("b64_encrypted_u: %s", b64_encrypted_u.decode("utf-8"))
         data = {"encrypted_key": b64_encrypted_u.decode("utf-8"), "auth_tag": self.auth_tag}
@@ -1098,36 +1172,37 @@
             with RequestsClient(
                 cloudagent_base_url,
                 self.enable_agent_mtls,
                 tls_context=self.agent_tls_context,
             ) as post_ukey:
                 response = post_ukey.post(params, json=data, timeout=self.request_timeout)
         else:
-            logger.warning("Connecting to agent without using mTLS!")
+            logger.warning("Connecting to %s without using mTLS!", self.agent_fid_str)
             post_ukey = RequestsClient(cloudagent_base_url, tls_enabled=False)
             response = post_ukey.post(params, json=data, timeout=self.request_timeout)
 
         if response.status_code == 503:
             logger.error(
-                "Cannot connect to Agent at %s with Port %s. Connection refused.", self.agent_ip, self.agent_port
+                "Cannot connect to %s to post encrypted U. Connection refused.",
+                self.agent_fid_str,
             )
             sys.exit()
         elif response.status_code == 504:
-            logger.error("Verifier at %s with Port %s timed out.", self.verifier_ip, self.verifier_port)
+            logger.error("%s timed out while posting encrypted U", self.agent_fid_str)
             sys.exit()
 
         if response.status_code != 200:
             keylime_logging.log_http_response(logger, logging.ERROR, response_json)
             raise UserError(
-                f"Posting of Encrypted U to the Cloud Agent failed with response code {response.status_code} ({response.text})"
+                f"Posting of encrypted U to {self.agent_fid_str} failed with response code {response.status_code} ({response.text})"
             )
 
     def do_verify(self) -> None:
         """Perform verify using a random generated challenge"""
-        challenge = TPM_Utilities.random_password(20)
+        challenge = tpm_util.random_password(20)
         numtries = 0
 
         while True:
             response = None
             try:
                 cloudagent_base_url = f"{bracketize_ipv6(self.agent_ip)}:{self.agent_port}"
 
@@ -1138,35 +1213,33 @@
                         tls_context=self.agent_tls_context,
                     ) as do_verify:
                         response = do_verify.get(
                             f"/v{self.supported_version}/keys/verify?challenge={challenge}",
                             timeout=self.request_timeout,
                         )
                 else:
-                    logger.warning("Connecting to agent without using mTLS!")
+                    logger.warning("Connecting to %s without using mTLS!", self.agent_fid_str)
                     do_verify = RequestsClient(cloudagent_base_url, tls_enabled=False)
                     response = do_verify.get(
                         f"/v{self.supported_version}/keys/verify?challenge={challenge}", timeout=self.request_timeout
                     )
 
                 response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
             except Exception as e:
                 if response is not None and response.status_code in (503, 504):
                     numtries += 1
                     if numtries >= self.maxr:
-                        logger.error(
-                            "Cannot establish connection to agent on %s with port %s", self.agent_ip, self.agent_port
-                        )
+                        logger.error("Cannot establish connection to %s", self.agent_fid_str)
                         self.do_cvstop()
                         sys.exit()
                     next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                     logger.info(
-                        "Verifier connection to agent at %s refused %s/%s times, trying again in %s seconds...",
-                        self.agent_ip,
+                        "Connection to %s refused %s/%s times, trying again in %s seconds...",
+                        self.agent_fid_str,
                         numtries,
                         self.maxr,
                         next_retry,
                     )
                     time.sleep(next_retry)
                     continue
                 self.do_cvstop()
@@ -1174,39 +1247,46 @@
 
             mac = ""
             ex_mac = crypto.do_hmac(self.K, challenge)
 
             if response.status_code == 200:
                 if "results" not in response_json or "hmac" not in response_json["results"]:
                     logger.critical(
-                        "Error: unexpected http response body from on agent %s with port %s : %s",
-                        self.agent_ip,
-                        self.agent_port,
+                        "Error: unexpected http response body from %s : %s",
+                        self.agent_fid_str,
                         response.status_code,
                     )
                     self.do_cvstop()
                     break
                 mac = response_json["results"]["hmac"]
 
                 if mac == ex_mac:
-                    logger.info("Agent on %s with port %s successfully derived key", self.agent_ip, self.agent_port)
+                    logger.info("Successful key derivation for %s", self.agent_fid_str)
 
             if mac != ex_mac:
                 if response.status_code != 200:
                     keylime_logging.log_http_response(logger, logging.ERROR, response_json)
                 numtries += 1
                 if numtries >= self.maxr:
-                    logger.error("Agent on %s with port %s failed key derivation", self.agent_ip, self.agent_port)
+                    logger.error(
+                        "Failed key derivation for %s (expected length %d, received %d",
+                        self.agent_fid_str,
+                        len(ex_mac),
+                        len(mac),
+                    )
                     self.do_cvstop()
                     sys.exit()
                 next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                 logger.info(
-                    "Key derivation not yet complete (retry %s/%s), trying again in %s seconds... (Ctrl-C to stop)",
+                    "Key derivation not yet complete for %s at try %d/%d (expected length %d, received length %d) trying again in %d seconds... (Ctrl-C to stop)",
+                    self.agent_fid_str,
                     numtries,
                     self.maxr,
+                    len(ex_mac),
+                    len(mac),
                     next_retry,
                 )
                 time.sleep(next_retry)
                 continue
             break
 
     def __convert_runtime_policy(self, args: Dict[str, str]) -> str:
```

### Comparing `keylime-7.2.5/keylime/tornado_requests.py` & `keylime-7.3.0/keylime/tornado_requests.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/tpm/ec_crypto_helper.py` & `keylime-7.3.0/keylime/tpm/ec_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/tpm/tpm2_objects.py` & `keylime-7.3.0/keylime/tpm/tpm2_objects.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/tpm/tpm2_objects_test.py` & `keylime-7.3.0/keylime/tpm/tpm2_objects_test.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/tpm/tpm_util.py` & `keylime-7.3.0/keylime/tpm/tpm_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
+import string
 import struct
-from typing import Dict, List, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat import backends
 from cryptography.hazmat.primitives import hashes, hmac, serialization
 from cryptography.hazmat.primitives.asymmetric import ec, padding
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePublicKey
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from cryptography.hazmat.primitives.asymmetric.utils import Prehashed
 from cryptography.hazmat.primitives.ciphers import Cipher, modes
 
-from keylime import keylime_logging
+from keylime import config, crypto, json, keylime_logging
 from keylime.tpm import ec_crypto_helper, tpm2_objects
 
 logger = keylime_logging.init_logging("tpm_util")
 
 SupportedKeyTypes = Union[RSAPublicKey, EllipticCurvePublicKey]
 
 
@@ -430,7 +431,49 @@
         if party:
             digest.update(party)
         result += digest.finalize()
 
         size -= hashfunc.digest_size
 
     return result[:size_in_bytes]
+
+
+def check_mask(mask: Optional[str], pcr: int) -> bool:
+    if mask is None:
+        return False
+    return bool(1 << pcr & int(mask, 0))
+
+
+def random_password(length: int = 20) -> str:
+    rand = crypto.generate_random_key(length)
+    chars = string.ascii_uppercase + string.digits + string.ascii_lowercase
+    password = ""
+    for i in range(length):
+        password += chars[(rand[i]) % len(chars)]
+    return password
+
+
+def readPolicy(configval: str) -> Dict[str, Any]:
+    policy: Dict[str, Any] = json.loads(configval)
+
+    # compute PCR mask from tpm_policy
+    mask = 0
+    for key in policy:
+        if not key.isdigit() or int(key) > 24:
+            raise Exception(f"Invalid tpm policy pcr number: {key}")
+
+        if int(key) == config.TPM_DATA_PCR:
+            raise Exception(f"Invalid allowlist PCR number {key}, keylime uses this PCR to bind data.")
+        if int(key) == config.IMA_PCR:
+            raise Exception(f"Invalid allowlist PCR number {key}, this PCR is used for IMA.")
+
+        mask = mask | (1 << int(key))
+
+        # wrap it in a list if it is a singleton
+        if isinstance(policy[key], str):
+            policy[key] = [policy[key]]
+
+        # convert all hash values to lowercase
+        policy[key] = [x.lower() for x in policy[key]]
+
+    policy["mask"] = hex(mask)
+    return policy
```

### Comparing `keylime-7.2.5/keylime/tpm/tpm_util_test.py` & `keylime-7.3.0/keylime/tpm/tpm_util_test.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/keylime/tpm_bootlog_enrich.py` & `keylime-7.3.0/keylime/mba/elparsing/tpm_bootlog_enrich.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,70 +5,66 @@
 
 import argparse
 import json
 import re
 import sys
 import traceback
 from ctypes import CDLL, byref, c_char_p, create_string_buffer
+from typing import Any, Dict
 
 import yaml
 
-try:
-    from yaml import CSafeLoader as SafeLoader
-except ImportError:
-    from yaml import SafeLoader
-
 from keylime import config
 
 ##################################################################################
 #
 # yaml by default outputs numbers in decimal format, and this allows us to
 # represent some numbers in hexadecimal
 #
 ##################################################################################
 
 
 class hexint(int):
     pass
 
 
-def representer(_, data):
+def representer(_: Any, data: int) -> yaml.ScalarNode:
     return yaml.ScalarNode("tag:yaml.org,2002:int", hex(data))
 
 
 yaml.add_representer(hexint, representer)
 
 ##################################################################################
 #
 # These function use efivar C libraries to decode device path and guid
 #
 ##################################################################################
 
 efivarlib_functions = CDLL(config.LIBEFIVAR)
 
 
-def getDevicePath(b, l):
+def getDevicePath(b: bytes, l: int) -> str:
     ret = efivarlib_functions.efidp_format_device_path(0, 0, b, l)
     if ret < 0:
-        raise Exception(f"getDevicePath: efidp_format_device_path({b}) returned {ret}")
+        raise Exception(f"getDevicePath: efidp_format_device_path({str(b)}) returned {ret}")
 
     s = create_string_buffer(ret + 1)
 
     ret = efivarlib_functions.efidp_format_device_path(s, ret + 1, b, l)
     if ret < 0:
-        raise Exception(f"getDevicePath: efidp_format_device_path({b}) returned {ret}")
+        raise Exception(f"getDevicePath: efidp_format_device_path({str(b)}) returned {ret}")
 
     return s.value.decode("utf-8")
 
 
-def getGUID(b):
+def getGUID(b: bytes) -> str:
     s = c_char_p(None)
     ret = efivarlib_functions.efi_guid_to_str(b, byref(s))
     if ret < 0:
-        raise Exception(f"getGUID: efi_guid_to_str({b}) returned {ret}")
+        raise Exception(f"getGUID: efi_guid_to_str({str(b)}) returned {ret}")
     assert isinstance(s.value, bytes)
     return s.value.decode("utf-8")  # pylint: disable=E1101
 
 
 ##################################################################################
 #
 # https://uefi.org/sites/default/files/resources/UEFI%20Spec%202.8B%20May%202020.pdf
@@ -93,15 +89,15 @@
 ##################################################################################
 
 ##################################################################################
 # Parse EFI_SIGNATURE_DATA
 ##################################################################################
 
 
-def getKey(b, start, size):
+def getKey(b: bytes, start: int, size: int) -> Dict[str, Any]:
     key = {}
     signatureOwner = getGUID(b[start : start + 16])
     key["SignatureOwner"] = signatureOwner
 
     signatureData = b[start + 16 : start + size]
     key["SignatureData"] = signatureData.hex()
     return key
@@ -125,91 +121,90 @@
 ##################################################################################
 
 ##################################################################################
 # Parse additional information about variables BootOrder and Boot####
 ##################################################################################
 
 
-def getVar(event, b):
+def getVar(event: Dict[str, Any], b: bytes) -> Any:
     if "UnicodeName" in event:
         if "VariableDataLength" in event:
             varlen = event["VariableDataLength"]
 
             # BootOrder variable
             if event["UnicodeName"] == "BootOrder":
                 if varlen % 2 != 0:
                     raise Exception(f"getVar: VariableDataLength({varlen}) is not divisible by 2")
 
                 l = int(varlen / 2)
-                r = []
+                r1 = []
                 for x in range(l):
                     d = int.from_bytes(b[x * 2 : x * 2 + 2], byteorder="little")
-                    r.append(f"Boot{d:04x}")
-                return r
+                    r1.append(f"Boot{d:04x}")
+                return r1
             # Boot#### variable
             if re.match("Boot[0-9a-fA-F]{4}", event["UnicodeName"]):
-                r = {}
+                r2 = {}
                 i = 0
                 size = 4
                 attributes = b[i : i + size]
                 d = int.from_bytes(attributes, "little") & 1
                 if d == 0:
-                    r["Enabled"] = "No"
+                    r2["Enabled"] = "No"
                 else:
-                    r["Enabled"] = "Yes"
+                    r2["Enabled"] = "Yes"
 
                 i += size
                 size = 2
                 filePathListLength = b[i : i + size]
                 d = int.from_bytes(filePathListLength, "little")
-                r["FilePathListLength"] = d
+                r2["FilePathListLength"] = str(d)
 
                 i += size
                 size = 2
                 description = ""
                 while i < varlen:
                     w = b[i : i + size]
                     i += size
                     if w == b"\x00\x00":
                         break
 
                     c = w.decode("utf-16", errors="ignore")
                     description += c
-                r["Description"] = description
+                r2["Description"] = description
                 devicePath = getDevicePath(b[i:], len(b[i:]))
-                r["DevicePath"] = devicePath
-                return r
+                r2["DevicePath"] = devicePath
+                return r2
     return None
 
 
-def enrich_device_path(d: dict) -> None:
+def enrich_device_path(d: Dict[str, Any]) -> None:
     if isinstance(d.get("DevicePath"), str):
         try:
             b = bytes.fromhex(d["DevicePath"])
             l = int(d["LengthOfDevicePath"])
         except Exception:
             return
         try:
             p = getDevicePath(b, l)
         # Deal with garbage devicePath
         except Exception:
             return
         d["DevicePath"] = p
 
 
-def enrich_boot_variable(d: dict) -> None:
+def enrich_boot_variable(d: Dict[str, Any]) -> None:
     if isinstance(d.get("VariableData"), str):
-        b = {}
         b = bytes.fromhex(d["VariableData"])
         k = getVar(d, b)
         if k is not None:
             d["VariableData"] = k
 
 
-def enrich(log: dict) -> None:
+def enrich(log: Dict[str, Any]) -> None:
     """Make the given BIOS boot log easier to understand and process"""
     if "events" in log:
         events = log["events"]
 
         for event in events:
             if "EventType" in event:
                 t = event["EventType"]
@@ -223,20 +218,23 @@
                         enrich_device_path(d)
                 elif t == "EV_EFI_VARIABLE_BOOT":
                     if "Event" in event:
                         d = event["Event"]
                         enrich_boot_variable(d)
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("infile", nargs="?", type=argparse.FileType("r"), default=sys.stdin)
     parser.add_argument("-o", "--output", choices=("yaml", "json"), default="yaml")
     args = parser.parse_args()
-    log = yaml.load(args.infile, Loader=SafeLoader)
+    try:
+        log = yaml.load(args.infile, Loader=yaml.CSafeLoader)
+    except Exception:
+        log = yaml.load(args.infile, Loader=yaml.SafeLoader)
     try:
         enrich(log)
     except Exception:
         traceback.print_exc(file=sys.stderr)
         sys.exit(1)
     if args.output == "yaml":
         print(yaml.dump(log, default_flow_style=False, line_break=None))
```

### Comparing `keylime-7.2.5/keylime/web_util.py` & `keylime-7.3.0/keylime/web_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     )
 
 
 def echo_json_response(
     handler: Any, code: int, status: Optional[str] = None, results: Optional[Dict[str, Any]] = None
 ) -> bool:
     """Takes a json package and returns it to the user w/ full HTTP headers"""
-    if handler is None or code is None:
+    if handler is None:
         return False
     if status is None:
         status = http.client.responses[code]
     if results is None:
         results = {}
 
     json_res = {"code": code, "status": status, "results": results}
```

### Comparing `keylime-7.2.5/keylime.egg-info/PKG-INFO` & `keylime-7.3.0/keylime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keylime
-Version: 7.2.5
+Version: 7.3.0
 Summary: TPM-based key bootstrapping and system integrity measurement system for cloud
 Home-page: https://keylime.dev
 Author: Keylime Community
 Author-email: keylime@groups.io
 License: Apache-2.0
 Project-URL: Source, https://github.com/keylime/keylime
 Project-URL: Documentation, https://keylime.readthedocs.io/en/latest/
```

### Comparing `keylime-7.2.5/keylime.egg-info/SOURCES.txt` & `keylime-7.3.0/keylime.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 keylime/registrar_client.py
 keylime/registrar_common.py
 keylime/requests_client.py
 keylime/revocation_notifier.py
 keylime/signing.py
 keylime/tenant.py
 keylime/tornado_requests.py
-keylime/tpm_bootlog_enrich.py
 keylime/tpm_ek_ca.py
 keylime/types.py
 keylime/web_util.py
 keylime.egg-info/PKG-INFO
 keylime.egg-info/SOURCES.txt
 keylime.egg-info/dependency_links.txt
 keylime.egg-info/entry_points.txt
@@ -80,24 +79,26 @@
 keylime/dsse/x509.py
 keylime/ima/__init__.py
 keylime/ima/ast.py
 keylime/ima/dm_grammar.py
 keylime/ima/file_signatures.py
 keylime/ima/ima.py
 keylime/ima/ima_dm.py
-keylime/ima/ima_test.py
 keylime/ima/types.py
 keylime/mba/__init__.py
 keylime/mba/mba.py
 keylime/mba/elchecking/__init__.py
 keylime/mba/elchecking/__main__.py
 keylime/mba/elchecking/example.py
 keylime/mba/elchecking/mbpolicy.py
 keylime/mba/elchecking/policies.py
 keylime/mba/elchecking/tests.py
+keylime/mba/elparsing/__init__.py
+keylime/mba/elparsing/tpm2_tools_elparser.py
+keylime/mba/elparsing/tpm_bootlog_enrich.py
 keylime/migrations/__init__.py
 keylime/migrations/alembic.ini
 keylime/migrations/env.py
 keylime/migrations/versions/039322ea079b_add_generator_column.py
 keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
 keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
 keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
@@ -125,15 +126,14 @@
 keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
 keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
 keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
 keylime/tpm/__init__.py
 keylime/tpm/ec_crypto_helper.py
 keylime/tpm/tpm2_objects.py
 keylime/tpm/tpm2_objects_test.py
-keylime/tpm/tpm_abstract.py
 keylime/tpm/tpm_main.py
 keylime/tpm/tpm_util.py
 keylime/tpm/tpm_util_test.py
 keylime/tpm/types.py
 templates/2.0/adjust.py
 templates/2.0/agent.j2
 templates/2.0/ca.j2
@@ -151,16 +151,16 @@
 test/test_convert_config.py
 test/test_crypto.py
 test/test_fs_util.py
 test/test_ima_ast.py
 test/test_ima_dm.py
 test/test_ima_verification.py
 test/test_json.py
+test/test_mba_parsing.py
 test/test_policy_conversion.py
 test/test_registrar_db.py
 test/test_retry_algo.py
 test/test_signing.py
-test/test_tpm.py
 test/test_validators.py
 test/test_verifier_db.py
 test/test_version.py
 test/test_web_util.py
```

### Comparing `keylime-7.2.5/keylime.egg-info/entry_points.txt` & `keylime-7.3.0/keylime.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/pyproject.toml` & `keylime-7.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/setup.cfg` & `keylime-7.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = keylime
-version = 7.2.5
+version = 7.3.0
 description = TPM-based key bootstrapping and system integrity measurement system for cloud
 long_description = file: _pypi-notice.md, README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://keylime.dev
 author = Keylime Community
 author_email = keylime@groups.io
 license = Apache-2.0
```

### Comparing `keylime-7.2.5/setup.py` & `keylime-7.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/templates/2.0/adjust.py` & `keylime-7.3.0/templates/2.0/adjust.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/templates/2.0/agent.j2` & `keylime-7.3.0/templates/2.0/agent.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/templates/2.0/ca.j2` & `keylime-7.3.0/templates/2.0/ca.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/templates/2.0/logging.j2` & `keylime-7.3.0/templates/2.0/logging.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/templates/2.0/mapping.json` & `keylime-7.3.0/templates/2.0/mapping.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999985827664399%*

 * *Differences: {"'components'": "{'agent': {'tpm_ownerpassword': {'default': ''}}}"}*

```diff
@@ -148,15 +148,15 @@
             },
             "tpm_hash_alg": {
                 "default": "sha256",
                 "option": "tpm_hash_alg",
                 "section": "cloud_agent"
             },
             "tpm_ownerpassword": {
-                "default": "keylime",
+                "default": "",
                 "option": "tpm_ownerpassword",
                 "section": "cloud_agent"
             },
             "tpm_signing_alg": {
                 "default": "rsassa",
                 "option": "tpm_signing_alg",
                 "section": "cloud_agent"
```

### Comparing `keylime-7.2.5/templates/2.0/registrar.j2` & `keylime-7.3.0/templates/2.0/registrar.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/templates/2.0/tenant.j2` & `keylime-7.3.0/templates/2.0/tenant.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/templates/2.0/verifier.j2` & `keylime-7.3.0/templates/2.0/verifier.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_algorithms.py` & `keylime-7.3.0/test/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_api_version.py` & `keylime-7.3.0/test/test_api_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_ca_impl_openssl.py` & `keylime-7.3.0/test/test_ca_impl_openssl.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_ca_util.py` & `keylime-7.3.0/test/test_ca_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_cert_utils.py` & `keylime-7.3.0/test/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_config.py` & `keylime-7.3.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_convert_config.py` & `keylime-7.3.0/test/test_convert_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_crypto.py` & `keylime-7.3.0/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_fs_util.py` & `keylime-7.3.0/test/test_fs_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_ima_ast.py` & `keylime-7.3.0/test/test_ima_ast.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_ima_dm.py` & `keylime-7.3.0/test/test_ima_dm.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_ima_verification.py` & `keylime-7.3.0/test/test_ima_verification.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_json.py` & `keylime-7.3.0/test/test_json.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_policy_conversion.py` & `keylime-7.3.0/test/test_policy_conversion.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_registrar_db.py` & `keylime-7.3.0/test/test_registrar_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_retry_algo.py` & `keylime-7.3.0/test/test_retry_algo.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_signing.py` & `keylime-7.3.0/test/test_signing.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_validators.py` & `keylime-7.3.0/test/test_validators.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_verifier_db.py` & `keylime-7.3.0/test/test_verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_version.py` & `keylime-7.3.0/test/test_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.2.5/test/test_web_util.py` & `keylime-7.3.0/test/test_web_util.py`

 * *Files identical despite different names*

