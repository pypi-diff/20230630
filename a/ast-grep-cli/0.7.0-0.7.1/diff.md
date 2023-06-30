# Comparing `tmp/ast_grep_cli-0.7.0.tar.gz` & `tmp/ast_grep_cli-0.7.1.tar.gz`

## Comparing `ast_grep_cli-0.7.0.tar` & `ast_grep_cli-0.7.1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-dynamic/Cargo.toml
--rw-r--r--   0     1001      123     7552 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-dynamic/src/lib.rs
--rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/Cargo.toml
--rw-r--r--   0     1001      123     1911 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/cpp.rs
--rw-r--r--   0     1001      123     1815 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/csharp.rs
--rw-r--r--   0     1001      123     1515 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/css.rs
--rw-r--r--   0     1001      123     2024 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/go.rs
--rw-r--r--   0     1001      123     8546 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/lib.rs
--rw-r--r--   0     1001      123     2879 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/parsers.rs
--rw-r--r--   0     1001      123     3114 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/python.rs
--rw-r--r--   0     1001      123     2915 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/rust.rs
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/Cargo.toml
--rw-r--r--   0     1001      123     2331 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/language.rs
--rw-r--r--   0     1001      123     3858 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/lib.rs
--rw-r--r--   0     1001      123    14850 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/match_tree.rs
--rw-r--r--   0     1001      123     3480 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/kind.rs
--rw-r--r--   0     1001      123     3783 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs
--rw-r--r--   0     1001      123    10723 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs
--rw-r--r--   0     1001      123      982 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/text.rs
--rw-r--r--   0     1001      123     6540 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher.rs
--rw-r--r--   0     1001      123    11359 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/meta_var.rs
--rw-r--r--   0     1001      123    15431 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/node.rs
--rw-r--r--   0     1001      123    16351 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/ops.rs
--rw-r--r--   0     1001      123     3089 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/pinned.rs
--rw-r--r--   0     1001      123    10936 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/indent.rs
--rw-r--r--   0     1001      123     6181 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/structural.rs
--rw-r--r--   0     1001      123     9380 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/template.rs
--rw-r--r--   0     1001      123     2572 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer.rs
--rw-r--r--   0     1001      123     8489 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/source.rs
--rw-r--r--   0     1001      123    16414 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/traversal.rs
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-lsp/Cargo.toml
--rw-r--r--   0     1001      123    11291 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-lsp/src/lib.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/Cargo.toml
--rw-r--r--   0     1001      123     6946 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/constraints.rs
--rw-r--r--   0     1001      123     6838 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/deserialize_env.rs
--rw-r--r--   0     1001      123     4880 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/lib.rs
--rw-r--r--   0     1001      123     2765 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/maybe.rs
--rw-r--r--   0     1001      123     6514 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/referent_rule.rs
--rw-r--r--   0     1001      123    16160 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
--rw-r--r--   0     1001      123     4138 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
--rw-r--r--   0     1001      123    13151 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule.rs
--rw-r--r--   0     1001      123     6268 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule_collection.rs
--rw-r--r--   0     1001      123    11320 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule_config.rs
--rw-r--r--   0     1001      123     6716 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/transform.rs
--rw-r--r--   0        0        0     1573 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/crates/cli/Cargo.toml
--rw-r--r--   0     1001      123      249 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/bin/ast-grep.rs
--rw-r--r--   0     1001      123    11003 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/config.rs
--rw-r--r--   0     1001      123    10176 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/error.rs
--rw-r--r--   0     1001      123     3596 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/lang.rs
--rw-r--r--   0     1001      123     4996 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/lib.rs
--rw-r--r--   0     1001      123     1015 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/lsp.rs
--rw-r--r--   0     1001      123       94 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/main.rs
--rw-r--r--   0     1001      123    10196 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/new.rs
--rw-r--r--   0     1001      123    22465 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/print/colored_print.rs
--rw-r--r--   0     1001      123     7675 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/print/interactive_print.rs
--rw-r--r--   0     1001      123     9327 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/print/json_print.rs
--rw-r--r--   0     1001      123     3179 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/print/mod.rs
--rw-r--r--   0     1001      123     8424 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/run.rs
--rw-r--r--   0     1001      123    10361 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/scan.rs
--rw-r--r--   0     1001      123     6866 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/utils.rs
--rw-r--r--   0     1001      123    24629 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/src/verify.rs
--rw-r--r--   0     1001      123      593 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/tests/common/mod.rs
--rw-r--r--   0     1001      123      975 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/tests/run_test.rs
--rw-r--r--   0     1001      123     1046 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/tests/verify_test.rs
--rw-r--r--   0     1001      123     1236 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/pyproject.toml
--rw-r--r--   0     1001      123    59913 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/crates/cli/Cargo.lock
--rw-r--r--   0     1001      123     4980 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/README.md
--rw-r--r--   0     1001      123     1077 2023-06-25 08:20:00.000000 ast_grep_cli-0.7.0/LICENSE
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/Cargo.toml
+-rw-r--r--   0     1001      123     1911 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/cpp.rs
+-rw-r--r--   0     1001      123     1815 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/csharp.rs
+-rw-r--r--   0     1001      123     1515 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/css.rs
+-rw-r--r--   0     1001      123     2024 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/go.rs
+-rw-r--r--   0     1001      123     9828 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/lib.rs
+-rw-r--r--   0     1001      123     2990 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/parsers.rs
+-rw-r--r--   0     1001      123     3114 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/python.rs
+-rw-r--r--   0     1001      123     2915 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/rust.rs
+-rw-r--r--   0     1001      123     2041 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/scala.rs
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/Cargo.toml
+-rw-r--r--   0     1001      123     2331 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/language.rs
+-rw-r--r--   0     1001      123     3858 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/lib.rs
+-rw-r--r--   0     1001      123    14850 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/match_tree.rs
+-rw-r--r--   0     1001      123     3480 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/kind.rs
+-rw-r--r--   0     1001      123     3783 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      123    10723 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      123      982 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/text.rs
+-rw-r--r--   0     1001      123     6540 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher.rs
+-rw-r--r--   0     1001      123    11359 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/meta_var.rs
+-rw-r--r--   0     1001      123    15431 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/node.rs
+-rw-r--r--   0     1001      123    16351 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/ops.rs
+-rw-r--r--   0     1001      123     3089 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/pinned.rs
+-rw-r--r--   0     1001      123    10936 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/indent.rs
+-rw-r--r--   0     1001      123     6181 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/structural.rs
+-rw-r--r--   0     1001      123     9380 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/template.rs
+-rw-r--r--   0     1001      123     2572 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer.rs
+-rw-r--r--   0     1001      123     8489 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/source.rs
+-rw-r--r--   0     1001      123    16414 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/traversal.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/Cargo.toml
+-rw-r--r--   0     1001      123     6946 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/constraints.rs
+-rw-r--r--   0     1001      123     6838 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/deserialize_env.rs
+-rw-r--r--   0     1001      123     4880 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/lib.rs
+-rw-r--r--   0     1001      123     2765 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/maybe.rs
+-rw-r--r--   0     1001      123     6514 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/referent_rule.rs
+-rw-r--r--   0     1001      123    16160 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
+-rw-r--r--   0     1001      123     4138 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
+-rw-r--r--   0     1001      123    13151 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule.rs
+-rw-r--r--   0     1001      123     6268 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule_collection.rs
+-rw-r--r--   0     1001      123    11320 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule_config.rs
+-rw-r--r--   0     1001      123     6716 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/transform.rs
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-dynamic/Cargo.toml
+-rw-r--r--   0     1001      123     7730 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-dynamic/src/lib.rs
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-lsp/Cargo.toml
+-rw-r--r--   0     1001      123    11291 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/local_dependencies/ast-grep-lsp/src/lib.rs
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      123      249 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/bin/ast-grep.rs
+-rw-r--r--   0     1001      123    11003 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/config.rs
+-rw-r--r--   0     1001      123    10194 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/error.rs
+-rw-r--r--   0     1001      123     4105 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/lang.rs
+-rw-r--r--   0     1001      123     4996 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      123     1015 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/lsp.rs
+-rw-r--r--   0     1001      123       94 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/main.rs
+-rw-r--r--   0     1001      123    10196 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/new.rs
+-rw-r--r--   0     1001      123    22465 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/print/colored_print.rs
+-rw-r--r--   0     1001      123     7675 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/print/interactive_print.rs
+-rw-r--r--   0     1001      123     9327 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/print/json_print.rs
+-rw-r--r--   0     1001      123     3179 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/print/mod.rs
+-rw-r--r--   0     1001      123     8602 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/run.rs
+-rw-r--r--   0     1001      123    10361 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/scan.rs
+-rw-r--r--   0     1001      123     6866 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/utils.rs
+-rw-r--r--   0     1001      123    24629 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/src/verify.rs
+-rw-r--r--   0     1001      123      593 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/tests/common/mod.rs
+-rw-r--r--   0     1001      123      975 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/tests/run_test.rs
+-rw-r--r--   0     1001      123     1046 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/tests/verify_test.rs
+-rw-r--r--   0     1001      123     1236 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/pyproject.toml
+-rw-r--r--   0     1001      123    60179 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/crates/cli/Cargo.lock
+-rw-r--r--   0     1001      123     4980 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/README.md
+-rw-r--r--   0     1001      123     1077 2023-06-29 23:45:51.000000 ast_grep_cli-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6235 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.1/PKG-INFO
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-dynamic/Cargo.toml` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-dynamic/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.0"
+version= "0.7.1"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 libloading = "0.8"
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-dynamic/src/lib.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-dynamic/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,23 @@
 pub struct DynamicLang {
   index: LangIndex,
   // inline expando char since it is used frequently
   expando: char,
 }
 
 impl DynamicLang {
-  pub fn all_langs() -> Vec<String> {
-    Self::langs().iter().map(|i| i.name.clone()).collect()
+  pub fn all_langs() -> Vec<Self> {
+    Self::langs()
+      .iter()
+      .enumerate()
+      .map(|(index, inner)| DynamicLang {
+        index: index as LangIndex,
+        expando: inner.expando_char,
+      })
+      .collect()
   }
   pub fn file_types(&self) -> Types {
     let mut builder = TypesBuilder::new();
     let inner = self.inner();
     let mapping = unsafe { &LANG_INDEX };
     for (ext, i) in mapping.iter() {
       if *i == self.index {
@@ -61,15 +68,15 @@
     DynamicLang::from_str(&name).map_err(serde::de::Error::custom)
   }
 }
 
 impl FromStr for DynamicLang {
   type Err = String;
   fn from_str(name: &str) -> Result<Self, Self::Err> {
-    let langs = unsafe { &DYNAMIC_LANG };
+    let langs = Self::langs();
     for (i, lang) in langs.iter().enumerate() {
       if lang.name == name {
         return Ok(DynamicLang {
           index: i as LangIndex,
           expando: lang.expando_char,
         });
       }
@@ -150,14 +157,18 @@
       Self::register_one(reg, &mut langs, &mut mapping)?;
     }
     _ = std::mem::replace(&mut DYNAMIC_LANG, langs);
     _ = std::mem::replace(&mut LANG_INDEX, mapping);
     Ok(())
   }
 
+  pub fn name(&self) -> &str {
+    &self.inner().name
+  }
+
   fn register_one(
     reg: Registration,
     langs: &mut Vec<Inner>,
     mapping: &mut Vec<(String, LangIndex)>,
   ) -> Result<(), DynamicLangError> {
     // lib must be retained!!
     let (_lib, lang) = unsafe { load_ts_language(reg.lib_path, reg.symbol)? };
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/Cargo.toml` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.0"
+version= "0.7.1"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 serde= { version = "1.0", features = ["derive"] }
 
@@ -25,14 +25,15 @@
 tree-sitter-html = { version = "0.19.0", optional = true }
 tree-sitter-java = { version = "0.20.0", optional = true }
 tree-sitter-javascript = { version = "0.20.0", optional = true }
 tree-sitter-kotlin = { version = "0.2.11", optional = true }
 tree-sitter-lua = { version = "0.0.18", optional = true }
 tree-sitter-python = { version = "0.20.2", optional = true }
 tree-sitter-rust = { version = "0.20.3", optional = true }
+tree-sitter-scala = { version = "0.20.1", optional = true }
 tree-sitter-swift = { version = "0.3.6", optional = true }
 tree-sitter-thrift = { version = "0.5.0", optional = true }
 tree-sitter-typescript= { version = "0.20.2", optional = true }
 
 [features]
 builtin-parser = [
   "tree-sitter-c",
@@ -44,12 +45,13 @@
   "tree-sitter-html",
   "tree-sitter-java",
   "tree-sitter-javascript",
   "tree-sitter-kotlin",
   "tree-sitter-lua",
   "tree-sitter-python",
   "tree-sitter-rust",
+  "tree-sitter-scala",
   "tree-sitter-swift",
   "tree-sitter-thrift",
   "tree-sitter-typescript",
 ]
 default = ["builtin-parser"]
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/cpp.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/csharp.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/css.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/go.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/lib.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,85 +1,98 @@
+//! This module defines the supported programming languages for ast-grep.
+//! It provides a set of customized languages with expando_char / pre_process_pattern,
+//! and a set of stub languages without preprocessing.
+//! A rule of thumb: if your language does not accept identifiers like `$VAR`.
+//! You need to create a standalone file and implement expando_char / pre_process_pattern.
+//! Otherwise, you can define it as a stub language using `impl_lang!`.
+
 mod cpp;
 mod csharp;
 mod css;
 mod go;
 mod parsers;
 mod python;
 mod rust;
+mod scala;
+
+use ast_grep_core::language::TSLanguage;
+use ast_grep_core::meta_var::MetaVariable;
 use ignore::types::{Types, TypesBuilder};
+use serde::{de, Deserialize, Deserializer, Serialize};
 use std::borrow::Cow;
 use std::fmt;
+use std::fmt::{Display, Formatter};
 use std::path::Path;
+use std::str::FromStr;
 
-pub use cpp::Cpp;
-pub use csharp::CSharp;
-pub use css::Css;
-pub use go::Go;
-pub use python::Python;
-pub use rust::Rust;
+pub use ast_grep_core::Language;
 
 macro_rules! impl_lang {
   ($lang: ident, $func: ident) => {
     #[derive(Clone, Copy)]
     pub struct $lang;
     impl Language for $lang {
       fn get_ts_language(&self) -> TSLanguage {
         parsers::$func().into()
       }
     }
   };
 }
 
+// Customized Language with expando_char / pre_process_pattern
+pub use cpp::Cpp;
+pub use csharp::CSharp;
+pub use css::Css;
+pub use go::Go;
+pub use python::Python;
+pub use rust::Rust;
+pub use scala::Scala;
+
+// Stub Language without preprocessing
 impl_lang!(C, language_c);
 impl_lang!(Dart, language_dart);
 impl_lang!(Html, language_html);
 impl_lang!(Java, language_java);
 impl_lang!(JavaScript, language_javascript);
 impl_lang!(Kotlin, language_kotlin);
 impl_lang!(Lua, language_lua);
 impl_lang!(Swift, language_swift);
 impl_lang!(Thrift, language_thrift);
 impl_lang!(Tsx, language_tsx);
 impl_lang!(TypeScript, language_typescript);
 
-use ast_grep_core::language::TSLanguage;
-use ast_grep_core::meta_var::MetaVariable;
-pub use ast_grep_core::Language;
-use serde::{Deserialize, Serialize};
-use std::fmt::{Display, Formatter};
-use std::str::FromStr;
-
-/// represents a dynamic language
-#[derive(Clone, Copy, Debug, PartialEq, Eq, Serialize, Deserialize, Hash)]
+/// Represents all built-in languages.
+#[derive(Clone, Copy, Debug, PartialEq, Eq, Serialize, Hash)]
 pub enum SupportLang {
   C,
   Cpp,
   CSharp,
   Css,
   Dart,
   Go,
   Html,
   Java,
   JavaScript,
   Kotlin,
   Lua,
   Python,
   Rust,
+  Scala,
   Swift,
   Thrift,
   Tsx,
   TypeScript,
 }
 
 impl SupportLang {
   pub fn all_langs() -> Vec<SupportLang> {
     use SupportLang::*;
     vec![
-      C, Cpp, CSharp, Css, Dart, Go, Html, Java, JavaScript, Kotlin, Lua, Python, Rust, Swift,
-      Thrift, Tsx, TypeScript,
+      C, Cpp, CSharp, Css, Dart, Go, Html, Java, JavaScript, Kotlin, Lua, Python, Rust, Scala,
+      Swift, Thrift, Tsx, TypeScript,
     ]
   }
 
   pub fn file_types(&self) -> Types {
     file_types(self)
   }
 }
@@ -102,35 +115,48 @@
       LanguageNotSupported(lang) => write!(f, "{} is not supported!", lang),
     }
   }
 }
 
 impl std::error::Error for SupportLangErr {}
 
+impl<'de> Deserialize<'de> for SupportLang {
+  fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
+  where
+    D: Deserializer<'de>,
+  {
+    let s = String::deserialize(deserializer)?;
+    FromStr::from_str(&s).map_err(de::Error::custom)
+  }
+}
+
+/// Implements the language names and aliases.
 impl FromStr for SupportLang {
   type Err = SupportLangErr;
   fn from_str(s: &str) -> Result<Self, Self::Err> {
     use SupportLang::*;
-    match s {
+    let normalized = s.to_lowercase();
+    match normalized.as_str() {
       "c" => Ok(C),
       "cc" | "c++" | "cpp" | "cxx" => Ok(Cpp),
       "cs" | "csharp" => Ok(CSharp),
       "css" | "scss" => Ok(Css),
       "dart" => Ok(Dart),
       "go" | "golang" => Ok(Go),
       "html" => Ok(Html),
       "java" => Ok(Java),
-      "js" | "jsx" => Ok(JavaScript),
-      "kt" | "ktm" | "kts" => Ok(Kotlin),
+      "javascript" | "js" | "jsx" => Ok(JavaScript),
+      "kotlin" | "kt" | "ktm" | "kts" => Ok(Kotlin),
       "lua" => Ok(Lua),
       "py" | "python" => Ok(Python),
       "rs" | "rust" => Ok(Rust),
+      "scala" => Ok(Scala),
       "swift" => Ok(Swift),
       "thrift" => Ok(Thrift),
-      "ts" => Ok(TypeScript),
+      "ts" | "typescript" => Ok(TypeScript),
       "tsx" => Ok(Tsx),
       _ => Err(SupportLangErr::LanguageNotSupported(s.to_string())),
     }
   }
 }
 
 macro_rules! execute_lang_method {
@@ -146,14 +172,15 @@
       S::Html => Html.$method($($pname,)*),
       S::Java => Java.$method($($pname,)*),
       S::JavaScript => JavaScript.$method($($pname,)*),
       S::Kotlin => Kotlin.$method($($pname,)*),
       S::Lua => Lua.$method($($pname,)*),
       S::Python => Python.$method($($pname,)*),
       S::Rust => Rust.$method($($pname,)*),
+      S::Scala => Scala.$method($($pname,)*),
       S::Swift => Swift.$method($($pname,)*),
       S::Thrift => Thrift.$method($($pname,)*),
       S::Tsx => Tsx.$method($($pname,)*),
       S::TypeScript => TypeScript.$method($($pname,)*),
     }
   }
 }
@@ -180,14 +207,15 @@
   fn pre_process_pattern<'q>(&self, query: &'q str) -> Cow<'q, str> {
     execute_lang_method! { self, pre_process_pattern, query }
   }
 }
 
 /// Guess which programming language a file is written in
 /// Adapt from `<https://github.com/Wilfred/difftastic/blob/master/src/parse/guess_language.rs>`
+/// N.B do not confuse it with `FromStr` trait. This function is to guess language from file extension.
 fn from_extension(path: &Path) -> Option<SupportLang> {
   use SupportLang::*;
   match path.extension()?.to_str()? {
     "c" | "h" => Some(C),
     "cc" | "hpp" | "cpp" | "c++" | "hh" | "cxx" | "cu" | "ino" => Some(Cpp),
     "cs" => Some(CSharp),
     "css" | "scss" => Some(Css),
@@ -196,14 +224,15 @@
     "html" | "htm" | "xhtml" => Some(Html),
     "java" => Some(Java),
     "cjs" | "js" | "mjs" | "jsx" => Some(JavaScript),
     "kt" | "ktm" | "kts" => Some(Kotlin),
     "lua" => Some(Lua),
     "py" | "py3" | "pyi" | "bzl" => Some(Python),
     "rs" => Some(Rust),
+    "scala" | "sc" | "sbt" => Some(Scala),
     "swift" => Some(Swift),
     "thrift" => Some(Thrift),
     "ts" | "cts" | "mts" => Some(TypeScript),
     "tsx" => Some(Tsx),
     _ => None,
   }
 }
@@ -237,14 +266,15 @@
     L::JavaScript => {
       add_custom_file_type(&mut builder, "myjs", &["*.js", "*.cjs", "*.jsx", "*.mjs"])
     }
     L::Kotlin => builder.select("kotlin"),
     L::Lua => builder.select("lua"),
     L::Python => builder.select("py"),
     L::Rust => builder.select("rust"),
+    L::Scala => builder.select("scala"),
     L::Swift => builder.select("swift"),
     L::Thrift => builder.select("thrift"),
     L::Tsx => {
       builder
         .add("mytsx", "*.tsx")
         .expect("file pattern must compile");
       builder.select("mytsx")
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/parsers.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/parsers.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 //! This mod maintains a list of tree-sitter parsers crate.
 //! When feature flag `builtin-parser` is on, this mod will import all dependent crates.
-//! However, tree-sitter bs cannot be compiled by wasm-pack. In this case, we can use a blank implementation by turning feature flag off.
+//! However, tree-sitter bs cannot be compiled by wasm-pack.
+//! In this case, we can use a blank implementation by turning feature flag off.
 //! And use other implementation.
 
 #[cfg(feature = "builtin-parser")]
 mod parser_implmentation {
   use ast_grep_core::language::TSLanguage;
 
   pub fn language_c() -> TSLanguage {
@@ -42,14 +43,17 @@
   }
   pub fn language_python() -> TSLanguage {
     tree_sitter_python::language().into()
   }
   pub fn language_rust() -> TSLanguage {
     tree_sitter_rust::language().into()
   }
+  pub fn language_scala() -> TSLanguage {
+    tree_sitter_scala::language().into()
+  }
   pub fn language_swift() -> TSLanguage {
     tree_sitter_swift::language().into()
   }
   pub fn language_thrift() -> TSLanguage {
     tree_sitter_thrift::language().into()
   }
   pub fn language_tsx() -> TSLanguage {
@@ -89,14 +93,15 @@
     language_html,
     language_java,
     language_javascript,
     language_kotlin,
     language_lua,
     language_python,
     language_rust,
+    language_scala,
     language_swift,
     language_thrift,
     language_tsx,
     language_typescript,
   );
 }
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/python.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-language/src/rust.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/Cargo.toml` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 edition= "2021"
 homepage= "https://ast-grep.github.io/"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.0"
+version= "0.7.1"
 
 [dependencies]
 bit-set= { version = "0.5.3" }
 regex = { version = "1.8.4" , optional = true }
 thiserror= "1.0.40"
 tree-sitter= { version = "0.9.2", package = "tree-sitter-facade-sg" }
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/language.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/lib.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/match_tree.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/kind.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher/text.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/matcher.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/meta_var.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/node.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/ops.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/pinned.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/indent.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/structural.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer/template.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/replacer.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/source.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-core/src/traversal.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-lsp/Cargo.toml` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-lsp/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "ast-grep-lsp"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
-version= "0.7.0"
+version= "0.7.1"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [dependencies]
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-lsp/src/lib.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-lsp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/Cargo.toml` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.0"
+version= "0.7.1"
 
 [features]
 default = ["regex"]
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
```

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/constraints.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/deserialize_env.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/lib.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/maybe.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/referent_rule.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/relational_rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule_collection.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/rule_config.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/local_dependencies/ast-grep-config/src/transform.rs` & `ast_grep_cli-0.7.1/local_dependencies/ast-grep-config/src/transform.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/Cargo.toml` & `ast_grep_cli-0.7.1/crates/cli/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 categories = ["command-line-utilities", "development-tools", "parsing"]
 default-run = "sg"
 # use relative path because maturin does not recognize
 readme = "../../README.md"
 license-file = "../../LICENSE"
 
-version= "0.7.0"
+version= "0.7.1"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
-license= "MIT"
+# license.workspace = true
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 homepage= "https://ast-grep.github.io/"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [[bin]]
 name = "sg"
```

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/config.rs` & `ast_grep_cli-0.7.1/crates/cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/error.rs` & `ast_grep_cli-0.7.1/crates/cli/src/error.rs`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use std::path::PathBuf;
 
 use crate::utils::ansi_link;
 
 const DOC_SITE_HOST: &str = "https://ast-grep.github.io";
 const PATTERN_GUIDE: Option<&str> = Some("/guide/pattern-syntax.html");
 const CONFIG_GUIDE: Option<&str> = Some("/guide/rule-config.html");
-const TOOL_OVERVIEW: Option<&str> = Some("/guide/tooling-overview.html");
+const TOOL_OVERVIEW: Option<&str> = Some("/guide/tooling-overview.html#parse-code-from-stdin");
 const CLI_USAGE: Option<&str> = Some("/reference/cli.html");
 const TEST_GUIDE: Option<&str> = Some("/guide/test-rule.html");
 const UTIL_GUIDE: Option<&str> = Some("/guide/rule-config/utility-rule.html");
 const EDITOR_INTEGRATION: Option<&str> = Some("/guide/editor-integration.html");
 const PLAYGROUND: Option<&str> = Some("/playground.html");
 
 /// AppError stands for ast-grep command line usage.
@@ -144,15 +144,15 @@
       ParsePattern => Self::new(
         "Cannot parse query as a valid pattern.",
         "The pattern either fails to parse or contains error. Please refer to pattern syntax guide.",
         PATTERN_GUIDE,
       ),
       LanguageNotSpecified => Self::new(
         "Language must be specified for code from StdIn.",
-        "Please use `--language` to specify the code language.",
+        "Please use `--lang` to specify the code language.",
         TOOL_OVERVIEW,
       ),
       StdInIsNotInteractive => Self::new(
         "Interactive mode is incompatible with parsing code from StdIn.",
         "`--interactive` needs StdIn, but it is used as source code. Please use files as input.",
         TOOL_OVERVIEW,
       ),
```

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/lang.rs` & `ast_grep_cli-0.7.1/crates/cli/src/lang.rs`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 use ast_grep_dynamic::{DynamicLang, Registration};
 use ast_grep_language::{Language, SupportLang};
 use ignore::types::Types;
 use serde::{Deserialize, Serialize};
 
 use std::borrow::Cow;
 use std::collections::HashMap;
-use std::fmt::{Display, Formatter};
+use std::fmt::{Debug, Display, Formatter};
 use std::path::{Path, PathBuf};
 use std::str::FromStr;
 
 #[derive(Serialize, Deserialize, Clone)]
 #[serde(rename_all = "camelCase")]
 pub struct CustomLang {
   library_path: PathBuf,
+  /// the dylib symbol to load ts-language, default is tree-sitter-{name}
   language_symbol: Option<String>,
   meta_var_char: Option<char>,
   expando_char: Option<char>,
   extensions: Vec<String>,
 }
 
 #[derive(Copy, Clone, PartialEq, Eq, Serialize, Deserialize)]
@@ -40,14 +41,29 @@
     let registrations = langs
       .into_iter()
       .map(|(name, custom)| custom_lang_to_registration(name, custom, &base))
       .collect();
     // TODO, add error handling
     unsafe { DynamicLang::register(registrations).expect("TODO") }
   }
+
+  pub fn all_langs() -> Vec<Self> {
+    let builtin = SupportLang::all_langs().into_iter().map(Self::Builtin);
+    let customs = DynamicLang::all_langs().into_iter().map(Self::Custom);
+    builtin.chain(customs).collect()
+  }
+}
+
+impl Debug for SgLang {
+  fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+    match self {
+      Builtin(b) => write!(f, "{}", b),
+      Custom(c) => write!(f, "{}", c.name()),
+    }
+  }
 }
 
 fn custom_lang_to_registration(name: String, custom_lang: CustomLang, base: &Path) -> Registration {
   let path = base.join(custom_lang.library_path);
   let sym = custom_lang
     .language_symbol
     .unwrap_or_else(|| format!("tree_sitter_{name}"));
```

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/lib.rs` & `ast_grep_cli-0.7.1/crates/cli/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/lsp.rs` & `ast_grep_cli-0.7.1/crates/cli/src/lsp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/new.rs` & `ast_grep_cli-0.7.1/crates/cli/src/new.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/print/colored_print.rs` & `ast_grep_cli-0.7.1/crates/cli/src/print/colored_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/print/interactive_print.rs` & `ast_grep_cli-0.7.1/crates/cli/src/print/interactive_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/print/json_print.rs` & `ast_grep_cli-0.7.1/crates/cli/src/print/json_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/print/mod.rs` & `ast_grep_cli-0.7.1/crates/cli/src/print/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/run.rs` & `ast_grep_cli-0.7.1/crates/cli/src/run.rs`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 // RunArg has a field of SgLang
 pub fn register_custom_language_if_is_run(args: &[String]) {
   if !args.is_empty() || args[1].starts_with('-') || args[1] == "run" {
     register_custom_language(None);
   }
 }
 
+// TODO: add long_help
+fn lang_help() -> String {
+  format!(
+    "The language of the pattern. Supported languages are:\n{:?}",
+    SgLang::all_langs()
+  )
+}
+
 #[derive(Parser)]
 pub struct RunArg {
   /// AST pattern to match.
   #[clap(short, long)]
   pattern: String,
 
   /// String to replace the matched AST node.
@@ -39,15 +47,15 @@
   rewrite: Option<String>,
 
   /// Print query pattern's tree-sitter AST. Requires lang be set explicitly.
   #[clap(long, requires = "lang")]
   debug_query: bool,
 
   /// The language of the pattern query.
-  #[clap(short, long)]
+  #[clap(short, long, help(lang_help()))]
   lang: Option<SgLang>,
 
   /// Start interactive edit session. Code rewrite only happens inside a session.
   #[clap(short, long)]
   interactive: bool,
 
   /// The paths to search. You can provide multiple paths separated by spaces.
```

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/scan.rs` & `ast_grep_cli-0.7.1/crates/cli/src/scan.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/utils.rs` & `ast_grep_cli-0.7.1/crates/cli/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/src/verify.rs` & `ast_grep_cli-0.7.1/crates/cli/src/verify.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/tests/common/mod.rs` & `ast_grep_cli-0.7.1/crates/cli/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/tests/run_test.rs` & `ast_grep_cli-0.7.1/crates/cli/tests/run_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/crates/cli/tests/verify_test.rs` & `ast_grep_cli-0.7.1/crates/cli/tests/verify_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/pyproject.toml` & `ast_grep_cli-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-cli"
-version = "0.7.0"
+version = "0.7.1"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_cli-0.7.0/crates/cli/Cargo.lock` & `ast_grep_cli-0.7.1/crates/cli/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -131,15 +131,15 @@
  "similar",
  "tempdir",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "serde",
@@ -147,38 +147,38 @@
  "tempdir",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading 0.8.0",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ast-grep-core",
  "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-c",
  "tree-sitter-cpp",
@@ -188,34 +188,35 @@
  "tree-sitter-html",
  "tree-sitter-java",
  "tree-sitter-javascript",
  "tree-sitter-kotlin",
  "tree-sitter-lua",
  "tree-sitter-python",
  "tree-sitter-rust",
+ "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "dashmap",
  "serde",
  "serde_json",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -276,15 +277,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "benches"
-version = "0.7.0"
+version = "0.7.1"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -1921,14 +1922,24 @@
 checksum = "797842733e252dc11ae5d403a18060bf337b822fc2ae5ddfaa6ff4d9cc20bda6"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-scala"
+version = "0.20.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e1f1de7a274c95937c40bc75dcaee97b5f23107ffcc78fc99a7b982d4f745ef"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
 name = "tree-sitter-swift"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eee2dbeb101a88a1d9e4883e3fbda6c799cf676f6a1cf59e4fc3862e67e70118"
 dependencies = [
  "cc",
  "tree-sitter",
```

### Comparing `ast_grep_cli-0.7.0/README.md` & `ast_grep_cli-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/LICENSE` & `ast_grep_cli-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.0/PKG-INFO` & `ast_grep_cli-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-grep-cli
-Version: 0.7.0
+Version: 0.7.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
@@ -15,15 +15,14 @@
 License-File: LICENSE
 Summary: Structural Search and Rewrite code at large scale using precise AST pattern.
 Keywords: ast,pattern,codemod,structural search,rewrite
 Home-Page: https://ast-grep.github.io/
 Author: Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>
 Author-email: Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>
 Maintainer-email: Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>
-License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/ast-grep/ast-grep
 Project-URL: Documentation, https://ast-grep.github.io/
 Project-URL: Changelog, https://github.com/ast-grep/ast-grep/blob/main/CHANGELOG.md
 
 <p align=center>
   <img src="https://ast-grep.github.io/logo.svg" alt="ast-grep"/>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.7.0 Classifier: Development
+Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.7.1 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Rust Classifier: Topic :: Security Classifier: Topic :: Software Development
 :: Quality Assurance Classifier: Topic :: Software Development Classifier:
 Topic :: Text Processing License-File: LICENSE License-File: LICENSE Summary:
 Structural Search and Rewrite code at large scale using precise AST pattern.
 Keywords: ast,pattern,codemod,structural search,rewrite Home-Page: https://ast-
 grep.github.io/ Author: Herrington Darkholme
 <2883231+HerringtonDarkholme@users.noreply.github.com> Author-email: Herrington
 Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com> Maintainer-
 email: Herrington Darkholme
-<2883231+HerringtonDarkholme@users.noreply.github.com> License: MIT
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-
-URL: Repository, https://github.com/ast-grep/ast-grep Project-URL:
-Documentation, https://ast-grep.github.io/ Project-URL: Changelog, https://
-github.com/ast-grep/ast-grep/blob/main/CHANGELOG.md
+<2883231+HerringtonDarkholme@users.noreply.github.com> Description-Content-
+Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Repository, https:
+//github.com/ast-grep/ast-grep Project-URL: Documentation, https://ast-
+grep.github.io/ Project-URL: Changelog, https://github.com/ast-grep/ast-grep/
+blob/main/CHANGELOG.md
                                   [ast-grep]
  [coverage badge] [https://codecov.io/gh/ast-grep/ast-grep/branch/main/graph/
     badge.svg?token=37VX8H2EWV] [Discord] [Badge] [Badge] [GitHub Sponsors]
 ## ast-grep(sg) ast-grep(sg) is a fast and polyglot tool for code structural
 search, lint and rewriting at large scale.. ## Introduction ast-grep is a AST-
 based tool to search code by pattern code. Think it as your old-friend `grep`
 but it matches AST nodes instead of text. You can write patterns as if you are
```

