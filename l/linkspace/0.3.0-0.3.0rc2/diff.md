# Comparing `tmp/linkspace-0.3.0.tar.gz` & `tmp/linkspace-0.3.0rc2.tar.gz`

## Comparing `linkspace-0.3.0.tar` & `linkspace-0.3.0rc2.tar`

### file list

```diff
@@ -1,170 +1,166 @@
--rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/linkspace-core/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/LICENSE
--rw-r--r--   0        0        0       34 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/README.md
--rw-r--r--   0        0        0     1728 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/consts.rs
--rw-r--r--   0        0        0    10960 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/db.rs
--rw-r--r--   0        0        0     5069 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/db_info.rs
--rw-r--r--   0        0        0        0 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/map.rs
--rw-r--r--   0        0        0      645 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/misc.rs
--rw-r--r--   0        0        0     5988 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/mod.rs
--rw-r--r--   0        0        0     4975 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/queries.rs
--rw-r--r--   0        0        0    10064 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/queries2.rs
--rw-r--r--   0        0        0     4840 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/save.rs
--rw-r--r--   0        0        0     5769 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/tree_iter.rs
--rw-r--r--   0        0        0      595 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/mod.rs
--rw-r--r--   0        0        0     1459 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/query_mode.rs
--rw-r--r--   0        0        0     7452 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/tree_key.rs
--rw-r--r--   0        0        0     2020 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/env/write_result.rs
--rw-r--r--   0        0        0     3673 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/eval.rs
--rw-r--r--   0        0        0     1517 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/lib.rs
--rw-r--r--   0        0        0        0 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/lnsroots.pkt
--rw-r--r--   0        0        0        0 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/matcher/matcher2.rs
--rw-r--r--   0        0        0     8686 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/matcher/mod.rs
--rw-r--r--   0        0        0     3092 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/mut_header.rs
--rw-r--r--   0        0        0     4137 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/partial_hash.rs
--rw-r--r--   0        0        0     4043 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/bitset_test.rs
--rw-r--r--   0        0        0     2268 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/builder.rs
--rw-r--r--   0        0        0     9173 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/exprs.rs
--rw-r--r--   0        0        0      471 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/mod.rs
--rw-r--r--   0        0        0    12662 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/pkt_predicates.rs
--rw-r--r--   0        0        0     4890 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/predicate_type.rs
--rw-r--r--   0        0        0     6439 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/test_pkt.rs
--rw-r--r--   0        0        0     1641 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/treekey.rs
--rw-r--r--   0        0        0    15063 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/uint.rs
--rw-r--r--   0        0        0    20779 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/value_test.rs
--rw-r--r--   0        0        0      758 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/prelude.rs
--rw-r--r--   0        0        0     1213 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/pull.rs
--rw-r--r--   0        0        0     7194 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/query.rs
--rw-r--r--   0        0        0    10689 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/stamp_fmt.rs
--rw-r--r--   0        0        0     5270 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-core/src/stamp_range.rs
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/byte-fmt/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/byte-fmt/LICENSE
--rw-r--r--   0        0        0       63 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/byte-fmt/README.md
--rw-r--r--   0        0        0    10893 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/byte-fmt/src/endian_types.rs
--rw-r--r--   0        0        0    15089 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/byte-fmt/src/lib.rs
--rw-r--r--   0        0        0     8551 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/byte-fmt/src/serde.rs
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/linkspace-cryptography/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-cryptography/LICENSE
--rw-r--r--   0        0        0       59 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-cryptography/README.md
--rw-r--r--   0        0        0      969 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-cryptography/src/keygen.rs
--rw-r--r--   0        0        0     2699 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-cryptography/src/lib.rs
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/linkspace/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace/LICENSE
--rw-r--r--   0        0        0       40 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace/README.md
--rw-r--r--   0        0        0     1728 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace/src/conventions/mod.rs
--rw-r--r--   0        0        0     7874 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace/src/conventions/status.rs
--rw-r--r--   0        0        0     2465 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace/src/interop.rs
--rw-r--r--   0        0        0    35868 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace/src/lib.rs
--rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/linkspace-argon2-identity/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-argon2-identity/LICENSE
--rw-r--r--   0        0        0       38 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-argon2-identity/README.md
--rw-r--r--   0        0        0     6020 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-argon2-identity/src/lib.rs
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/LICENSE
--rw-r--r--   0        0        0       45 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/README.md
--rw-r--r--   0        0        0      247 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/benches/spoints.rs
--rw-r--r--   0        0        0     5881 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/asm_tests.rs
--rw-r--r--   0        0        0      351 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/build_info.rs
--rw-r--r--   0        0        0     6488 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/builder.rs
--rw-r--r--   0        0        0     3926 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/byte_segments.rs
--rw-r--r--   0        0        0     3314 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/consts.rs
--rw-r--r--   0        0        0     9867 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/eval.rs
--rw-r--r--   0        0        0      577 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/exprs.rs
--rw-r--r--   0        0        0    21374 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/field_ids.rs
--rw-r--r--   0        0        0    11774 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/ipath.rs
--rw-r--r--   0        0        0    11168 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/lib.rs
--rw-r--r--   0        0        0     2208 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/link.rs
--rw-r--r--   0        0        0     5000 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/header.rs
--rw-r--r--   0        0        0     5830 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/mod.rs
--rw-r--r--   0        0        0     6641 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/netpkt_arc.rs
--rw-r--r--   0        0        0     2301 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/netpkt_parts.rs
--rw-r--r--   0        0        0     7031 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/netpkt_ptr.rs
--rw-r--r--   0        0        0     1658 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/partial.rs
--rw-r--r--   0        0        0     4406 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/reroute.rs
--rw-r--r--   0        0        0     3121 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/slot.rs
--rw-r--r--   0        0        0     3888 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/point.rs
--rw-r--r--   0        0        0     5978 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/point_parts.rs
--rw-r--r--   0        0        0    13570 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/point_ptr.rs
--rw-r--r--   0        0        0     3617 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/read.rs
--rw-r--r--   0        0        0     7605 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/repr.rs
--rw-r--r--   0        0        0    21438 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/spath.rs
--rw-r--r--   0        0        0    11507 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/spath_fmt.rs
--rw-r--r--   0        0        0     2976 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/spath_macro.rs
--rw-r--r--   0        0        0     2986 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/stamp.rs
--rw-r--r--   0        0        0      506 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-pkt/src/utils.rs
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/abe/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/LICENSE
--rw-r--r--   0        0        0       61 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/README.md
--rw-r--r--   0        0        0     1863 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/abe_macro.rs
--rw-r--r--   0        0        0     9010 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/abtxt.rs
--rw-r--r--   0        0        0    16329 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/ast.rs
--rw-r--r--   0        0        0     6637 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/convert.rs
--rw-r--r--   0        0        0    34386 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/eval.rs
--rw-r--r--   0        0        0     2717 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/lib.rs
--rw-r--r--   0        0        0     3570 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/argv.rs
--rw-r--r--   0        0        0     3640 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/base.rs
--rw-r--r--   0        0        0     7210 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/bytes.rs
--rw-r--r--   0        0        0      462 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/comment.rs
--rw-r--r--   0        0        0     3732 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/encode.rs
--rw-r--r--   0        0        0     3627 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/help.rs
--rw-r--r--   0        0        0     2677 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/logic.rs
--rw-r--r--   0        0        0      875 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/mod.rs
--rw-r--r--   0        0        0     5438 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/abe/src/scope/uint.rs
--rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/linkspace-common/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/LICENSE
--rw-r--r--   0        0        0       99 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/README.md
--rw-r--r--   0        0        0     2114 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/bus.rs
--rw-r--r--   0        0        0     8214 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/cli/keys.rs
--rw-r--r--   0        0        0     4817 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/cli/mod.rs
--rw-r--r--   0        0        0     8227 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/cli/opts.rs
--rw-r--r--   0        0        0     8801 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/cli/reader.rs
--rw-r--r--   0        0        0     7337 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/dgp.rs
--rw-r--r--   0        0        0     8569 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/eval.rs
--rw-r--r--   0        0        0     1217 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/lib.rs
--rw-r--r--   0        0        0     2946 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/pkt_reader.rs
--rw-r--r--   0        0        0     2130 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/pkt_stream_utils.rs
--rw-r--r--   0        0        0     4080 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/predicate_aliases.rs
--rw-r--r--   0        0        0      448 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/prelude.rs
--rw-r--r--   0        0        0     5170 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/handshake.rs
--rw-r--r--   0        0        0     5964 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/blob.rs
--rw-r--r--   0        0        0     4257 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkin.rs
--rw-r--r--   0        0        0     3093 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkout.rs
--rw-r--r--   0        0        0     3757 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/blobmap/mod.rs
--rw-r--r--   0        0        0     1029 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/mod.rs
--rw-r--r--   0        0        0     6686 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/admin.rs
--rw-r--r--   0        0        0     6960 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/claim.rs
--rw-r--r--   0        0        0     8286 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/eval.rs
--rw-r--r--   0        0        0      635 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/file_claim.rs
--rw-r--r--   0        0        0     1390 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/local_claim.rs
--rw-r--r--   0        0        0     6873 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/mod.rs
--rw-r--r--   0        0        0     5062 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/name.rs
--rw-r--r--   0        0        0     5898 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/public_claim.rs
--rw-r--r--   0        0        0      950 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/utils.rs
--rw-r--r--   0        0        0      398 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/mod.rs
--rw-r--r--   0        0        0     4386 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/runtime/handlers.rs
--rw-r--r--   0        0        0      292 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/runtime/mod.rs
--rw-r--r--   0        0        0    18969 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/runtime/rx.rs
--rw-r--r--   0        0        0     3089 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/runtime/threads.rs
--rw-r--r--   0        0        0     4830 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/static_env.rs
--rw-r--r--   0        0        0     2843 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/linkspace-common/src/tests.rs
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 linkspace-0.3.0/local_dependencies/ipcbus/Cargo.toml
--rw-r--r--   0        0        0    16725 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/ipcbus/LICENSE
--rw-r--r--   0        0        0       56 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/ipcbus/README.md
--rw-r--r--   0        0        0     4488 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/ipcbus/src/inotify.rs
--rw-r--r--   0        0        0      652 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/ipcbus/src/lib.rs
--rw-r--r--   0        0        0     4642 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/ipcbus/src/udp_multicast.rs
--rw-r--r--   0        0        0     5162 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/ipcbus/src/udp_procbus.rs
--rw-r--r--   0        0        0     1514 2023-06-30 11:33:22.000000 linkspace-0.3.0/local_dependencies/ipcbus/src/wasmbus.rs
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 linkspace-0.3.0/Cargo.toml
--rw-r--r--   0        0        0      811 2023-06-30 11:33:22.000000 linkspace-0.3.0/Makefile
--rw-r--r--   0        0        0      246 2023-06-30 11:33:22.000000 linkspace-0.3.0/README.md
--rw-r--r--   0        0        0      284 2023-06-30 11:33:22.000000 linkspace-0.3.0/build.rs
--rw-r--r--   0        0        0    13868 2023-06-30 11:33:22.000000 linkspace-0.3.0/linkspace.pyi
--rw-r--r--   0        0        0      273 2023-06-30 11:33:22.000000 linkspace-0.3.0/publish.sh
--rw-r--r--   0        0        0      163 2023-06-30 11:33:22.000000 linkspace-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      144 2023-06-30 11:33:22.000000 linkspace-0.3.0/pyrightconfig.json
--rw-r--r--   0        0        0    22252 2023-06-30 11:33:22.000000 linkspace-0.3.0/src/lib.rs
--rw-r--r--   0        0        0     9858 2023-06-30 11:33:22.000000 linkspace-0.3.0/src/pynetpkt.rs
--rw-r--r--   0        0        0      640 2023-06-30 11:33:22.000000 linkspace-0.3.0/tests/nested_watch.py
--rw-r--r--   0        0        0    58894 2023-06-30 12:02:46.000000 linkspace-0.3.0/Cargo.lock
--rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 linkspace-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/LICENSE
+-rw-r--r--   0        0        0       40 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/README.md
+-rw-r--r--   0        0        0      221 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/build.rs
+-rw-r--r--   0        0        0     1728 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/src/conventions/mod.rs
+-rw-r--r--   0        0        0     7874 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/src/conventions/status.rs
+-rw-r--r--   0        0        0     2465 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/src/interop.rs
+-rw-r--r--   0        0        0    35622 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace/src/lib.rs
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/LICENSE
+-rw-r--r--   0        0        0       56 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/README.md
+-rw-r--r--   0        0        0      526 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/src/lib.rs
+-rw-r--r--   0        0        0     6034 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/src/procbus.rs
+-rw-r--r--   0        0        0     4587 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/src/udp_multicast.rs
+-rw-r--r--   0        0        0     1512 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/ipcbus/src/wasmbus.rs
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/LICENSE
+-rw-r--r--   0        0        0       59 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/README.md
+-rw-r--r--   0        0        0      969 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/src/keygen.rs
+-rw-r--r--   0        0        0     2699 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/src/lib.rs
+-rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/LICENSE
+-rw-r--r--   0        0        0       38 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/README.md
+-rw-r--r--   0        0        0     6020 2023-06-21 12:25:29.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/src/lib.rs
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/LICENSE
+-rw-r--r--   0        0        0       34 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/README.md
+-rw-r--r--   0        0        0     1728 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/consts.rs
+-rw-r--r--   0        0        0    19369 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/db.rs
+-rw-r--r--   0        0        0     1171 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/misc.rs
+-rw-r--r--   0        0        0     5828 2023-06-20 15:25:28.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/mod.rs
+-rw-r--r--   0        0        0    10165 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/queries.rs
+-rw-r--r--   0        0        0    10061 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/queries2.rs
+-rw-r--r--   0        0        0     5769 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/tree_iter.rs
+-rw-r--r--   0        0        0      616 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/mod.rs
+-rw-r--r--   0        0        0     1459 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/query_mode.rs
+-rw-r--r--   0        0        0     7034 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/tree_key.rs
+-rw-r--r--   0        0        0     2020 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/write_result.rs
+-rw-r--r--   0        0        0     1883 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/write_trait.rs
+-rw-r--r--   0        0        0     3673 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/eval.rs
+-rw-r--r--   0        0        0     1499 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/lib.rs
+-rw-r--r--   0        0        0        0 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/lnsroots.pkt
+-rw-r--r--   0        0        0        0 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/matcher/matcher2.rs
+-rw-r--r--   0        0        0     8686 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/matcher/mod.rs
+-rw-r--r--   0        0        0     3092 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/mut_header.rs
+-rw-r--r--   0        0        0     4137 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/partial_hash.rs
+-rw-r--r--   0        0        0     4043 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/bitset_test.rs
+-rw-r--r--   0        0        0     2268 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/builder.rs
+-rw-r--r--   0        0        0     9173 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/exprs.rs
+-rw-r--r--   0        0        0      471 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/mod.rs
+-rw-r--r--   0        0        0    12662 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/pkt_predicates.rs
+-rw-r--r--   0        0        0     4890 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/predicate_type.rs
+-rw-r--r--   0        0        0     6439 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/test_pkt.rs
+-rw-r--r--   0        0        0     1641 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/treekey.rs
+-rw-r--r--   0        0        0    15063 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/uint.rs
+-rw-r--r--   0        0        0    20779 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/value_test.rs
+-rw-r--r--   0        0        0      794 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/prelude.rs
+-rw-r--r--   0        0        0     1213 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/pull.rs
+-rw-r--r--   0        0        0     7194 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/query.rs
+-rw-r--r--   0        0        0    10689 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/stamp_fmt.rs
+-rw-r--r--   0        0        0     5270 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/stamp_range.rs
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/LICENSE
+-rw-r--r--   0        0        0       45 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/README.md
+-rw-r--r--   0        0        0      247 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/benches/spoints.rs
+-rw-r--r--   0        0        0     5881 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/asm_tests.rs
+-rw-r--r--   0        0        0     6488 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/builder.rs
+-rw-r--r--   0        0        0     3926 2023-06-20 14:52:26.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/byte_segments.rs
+-rw-r--r--   0        0        0     3314 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/consts.rs
+-rw-r--r--   0        0        0     9167 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/eval.rs
+-rw-r--r--   0        0        0      577 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/exprs.rs
+-rw-r--r--   0        0        0    21374 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/field_ids.rs
+-rw-r--r--   0        0        0    11774 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/ipath.rs
+-rw-r--r--   0        0        0    11232 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/lib.rs
+-rw-r--r--   0        0        0     2208 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/link.rs
+-rw-r--r--   0        0        0     5000 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/header.rs
+-rw-r--r--   0        0        0     5819 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/mod.rs
+-rw-r--r--   0        0        0     6641 2023-06-20 15:07:14.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_arc.rs
+-rw-r--r--   0        0        0     2301 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_parts.rs
+-rw-r--r--   0        0        0     7054 2023-06-20 15:08:46.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_ptr.rs
+-rw-r--r--   0        0        0     1658 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/partial.rs
+-rw-r--r--   0        0        0     4406 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/reroute.rs
+-rw-r--r--   0        0        0     3121 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/slot.rs
+-rw-r--r--   0        0        0     3888 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point.rs
+-rw-r--r--   0        0        0     5978 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point_parts.rs
+-rw-r--r--   0        0        0    13570 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point_ptr.rs
+-rw-r--r--   0        0        0     3617 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/read.rs
+-rw-r--r--   0        0        0     6993 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/repr.rs
+-rw-r--r--   0        0        0    21438 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath.rs
+-rw-r--r--   0        0        0    11507 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath_fmt.rs
+-rw-r--r--   0        0        0     2976 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath_macro.rs
+-rw-r--r--   0        0        0     2986 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/stamp.rs
+-rw-r--r--   0        0        0      506 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/utils.rs
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/LICENSE
+-rw-r--r--   0        0        0       63 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/README.md
+-rw-r--r--   0        0        0    10893 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/endian_types.rs
+-rw-r--r--   0        0        0    15089 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/lib.rs
+-rw-r--r--   0        0        0     8551 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/serde.rs
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/abe/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/LICENSE
+-rw-r--r--   0        0        0       61 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/README.md
+-rw-r--r--   0        0        0     1863 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/abe_macro.rs
+-rw-r--r--   0        0        0     9010 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/abtxt.rs
+-rw-r--r--   0        0        0    16329 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/ast.rs
+-rw-r--r--   0        0        0     6637 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/convert.rs
+-rw-r--r--   0        0        0    34386 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/eval.rs
+-rw-r--r--   0        0        0     2717 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/lib.rs
+-rw-r--r--   0        0        0     3570 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/argv.rs
+-rw-r--r--   0        0        0     3640 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/base.rs
+-rw-r--r--   0        0        0     7210 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/bytes.rs
+-rw-r--r--   0        0        0      462 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/comment.rs
+-rw-r--r--   0        0        0     3732 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/encode.rs
+-rw-r--r--   0        0        0     3627 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/help.rs
+-rw-r--r--   0        0        0     2677 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/logic.rs
+-rw-r--r--   0        0        0      875 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/mod.rs
+-rw-r--r--   0        0        0     5438 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/abe/src/scope/uint.rs
+-rw-r--r--   0        0        0     1585 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/Cargo.toml
+-rw-r--r--   0        0        0    16725 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/LICENSE
+-rw-r--r--   0        0        0       99 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/README.md
+-rw-r--r--   0        0        0     2114 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/bus.rs
+-rw-r--r--   0        0        0     8214 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/keys.rs
+-rw-r--r--   0        0        0     4693 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/mod.rs
+-rw-r--r--   0        0        0     7787 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/opts.rs
+-rw-r--r--   0        0        0     8801 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/reader.rs
+-rw-r--r--   0        0        0     7337 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/dgp.rs
+-rw-r--r--   0        0        0     8479 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/eval.rs
+-rw-r--r--   0        0        0     1217 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/lib.rs
+-rw-r--r--   0        0        0     2946 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/pkt_reader.rs
+-rw-r--r--   0        0        0     2130 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/pkt_stream_utils.rs
+-rw-r--r--   0        0        0     4080 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/predicate_aliases.rs
+-rw-r--r--   0        0        0      448 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/prelude.rs
+-rw-r--r--   0        0        0     5170 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/handshake.rs
+-rw-r--r--   0        0        0     5964 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blob.rs
+-rw-r--r--   0        0        0     4257 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkin.rs
+-rw-r--r--   0        0        0     3093 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkout.rs
+-rw-r--r--   0        0        0     3757 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/mod.rs
+-rw-r--r--   0        0        0     1029 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/mod.rs
+-rw-r--r--   0        0        0     6707 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/admin.rs
+-rw-r--r--   0        0        0     6960 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/claim.rs
+-rw-r--r--   0        0        0     8286 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/eval.rs
+-rw-r--r--   0        0        0      635 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/file_claim.rs
+-rw-r--r--   0        0        0     1390 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/local_claim.rs
+-rw-r--r--   0        0        0     6873 2023-06-21 12:24:07.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/mod.rs
+-rw-r--r--   0        0        0     5062 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/name.rs
+-rw-r--r--   0        0        0     5898 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/public_claim.rs
+-rw-r--r--   0        0        0      950 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/utils.rs
+-rw-r--r--   0        0        0      398 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/mod.rs
+-rw-r--r--   0        0        0     4386 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/handlers.rs
+-rw-r--r--   0        0        0      292 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/mod.rs
+-rw-r--r--   0        0        0    19220 2023-06-23 08:46:36.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/rx.rs
+-rw-r--r--   0        0        0     3089 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/threads.rs
+-rw-r--r--   0        0        0     4895 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/static_env.rs
+-rw-r--r--   0        0        0     2843 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/tests.rs
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/Cargo.toml
+-rw-r--r--   0        0        0      811 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/Makefile
+-rw-r--r--   0        0        0      246 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/README.md
+-rw-r--r--   0        0        0    13672 2023-06-21 12:25:29.000000 linkspace-0.3.0rc2/linkspace.pyi
+-rw-r--r--   0        0        0      273 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/publish.sh
+-rw-r--r--   0        0        0      163 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/pyrightconfig.json
+-rw-r--r--   0        0        0    21874 2023-06-21 12:30:59.000000 linkspace-0.3.0rc2/src/lib.rs
+-rw-r--r--   0        0        0     9858 2023-06-21 12:30:16.000000 linkspace-0.3.0rc2/src/pynetpkt.rs
+-rw-r--r--   0        0        0      640 2023-06-20 14:27:02.000000 linkspace-0.3.0rc2/tests/nested_watch.py
+-rw-r--r--   0        0        0    68124 2023-06-23 09:29:07.000000 linkspace-0.3.0rc2/Cargo.lock
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 linkspace-0.3.0rc2/PKG-INFO
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [package]
 name = "linkspace-core"
 categories = []
 keywords = ["linkspace"]
 description = "linkspace core"
 
-version= "0.3.0-rc2"
+version= "0.3.0-rc1"
 authors= ["Anton Sol <AntonSol919@gmail.com>"]
 edition= "2021"
 license= "MPL-2.0"
 homepage= "https://www.linkspace.dev"
 documentation= "https://www.linkspace.dev/docs/guide/index.html"
 repository= "https://github.com/AntonSol919/linkspace"
 resolver = "2"
@@ -16,28 +16,24 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [features]
 default=["lmdb"]
 lmdb = ["lmdb-rkv", "lmdb-rkv-sys", "libc"]
 
 [dependencies]
 
-linkspace-pkt = { path = "../linkspace-pkt", version="0.3.0-rc2"}
-linkspace-cryptography = { path = "../linkspace-cryptography",version="0.3.0-rc2"}
+linkspace-pkt = { path = "../linkspace-pkt", version="0.3.0-rc1"}
+linkspace-cryptography = { path = "../linkspace-cryptography",version="0.3.0-rc1"}
 
 arrayvec= "=0.7.2  "
 anyhow= "=1.0.71"
 thiserror=  "=1.0.40"
 tracing= {version = "=0.1.37",features=["release_max_level_info"]}
 either= "=1.8.1"
 serde = { version = "=1.0.160", features = ["derive","rc"] }
-libc = { version = "0.2.147", optional =true}
-smallvec= {version="1.10.0",features=["const_new","const_generics","write"]}
+libc = { version = "=0.2.142", optional =true}
 
 dunce = "1.0.2"
 ipcbus = { path = "../ipcbus", version = "0.1.0"}
-lmdb-rkv = { git="https://github.com/AntonSol919/lmdb-rs", optional = true }
-lmdb-rkv-sys = { git="https://github.com/AntonSol919/lmdb-rs" ,optional = true }
-#lmdb-rkv = {path = "../../../lmdb-rs",optional=true}
-#lmdb-rkv-sys = {path = "../../../lmdb-rs/lmdb-sys",optional=true}
-
+lmdb-rkv = { version = "0.14.0", optional = true }
+lmdb-rkv-sys = { version = "0.11", optional = true }
 time = {version="0.3",features=["parsing","formatting"]}
 parse-display = "0.6.0"
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/consts.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/consts.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/mod.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,77 @@
-use std::{sync::{Arc }, path::{Path,PathBuf},fmt::Debug, io::{Write, self} };
+use std::{sync::{Arc, OnceLock}, path::{Path,PathBuf},fmt::Debug, io::{Write, self} };
 
 use anyhow::Context;
 pub use ipcbus::ProcBus;
-use linkspace_pkt::{ Stamp, PUBLIC_GROUP_PKT, NetPkt, AB, NetPktExt, NetPktPtr };
-use lmdb_sys::MDB_envinfo;
+use linkspace_pkt::{ Stamp, PUBLIC_GROUP_PKT, NetPkt, AB, NetPktExt };
 use tracing::instrument;
-use crate::{LNS_ROOTS};
+use crate::{env::write_trait::save_pkt, LNS_ROOTS};
+
+use self::{db::RawBTreeEnv, queries::{IReadTxn, ReadTxn}};
+
+use super::write_trait::SWrite;
 
-use self::{queries::{ ReadTxn}, save::SaveState, db::LMDBEnv, db_info::{DbInfo, LMDBVersion}};
 
 pub mod db;
 pub mod misc;
 pub mod tree_iter;
 pub mod queries;
 pub mod queries2;
-pub mod save;
-pub mod db_info;
 
 /// A [NetPktPtr] and a recv stamp
 
 
+pub type BusCall = Arc<dyn Fn(Stamp) + Send + Sync + 'static>;
+pub static BUS: OnceLock<BusCall> = OnceLock::new();
 #[derive(Clone)]
-pub struct BTreeEnv(pub Arc<Inner>);
-
-pub struct Inner {
-    lmdb: LMDBEnv,
-    location: PathBuf,
-    pub log_head: ProcBus,
+pub struct BTreeEnv {
+    inner: RawBTreeEnv,
+    location: Arc<PathBuf>,
+    pub log_head: Arc<ipcbus::ProcBus>,
 }
 impl Debug for BTreeEnv {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("BTreeEnv").finish()
     }
 }
 impl BTreeEnv {
-    
     pub fn dir(&self) -> &Path {
-        &self.0.location
+        &self.location
     }
     pub fn open(path: PathBuf, make_dir: bool) -> io::Result<BTreeEnv> {
-        let lmdb= db::open(&path, make_dir)?;
-        let location = path.canonicalize()?;
+        let inner = db::open(&path, make_dir)?;
+        let location = Arc::new(path.canonicalize()?);
         tracing::debug!(?location, "Opening BTreeEnv");
-        let log_head = ProcBus::new(&location)?;
-        let env = BTreeEnv(Arc::new(Inner{
-            lmdb,
-            log_head,
+        let log_head = ipcbus::ProcBus::new(inner.uid());
+        let env = BTreeEnv {
+            inner,
+            log_head: Arc::new(log_head),
             location,
-        }));
+        };
         {
-            let new = save_ptr_one(&env, &***PUBLIC_GROUP_PKT)?.is_new();
+            let mut writer = env.inner.write_txn()?;
+            let new = save_pkt(&mut writer, &**PUBLIC_GROUP_PKT)?;
             if new && std::env::var_os("LK_NO_LNS").is_none(){
                 let mut bytes = LNS_ROOTS;
-                let mut roots:Vec<_> = std::iter::from_fn(||{
+                let roots:Vec<_> = std::iter::from_fn(||{
                     if bytes.is_empty() { return None;}
                     let pkt = crate::pkt::read::read_pkt(bytes, true).unwrap();
                     bytes = &bytes[pkt.size() as usize..];
-                    match pkt{
-                        std::borrow::Cow::Borrowed(o) =>Some((o,SaveState::Pending)),
-                        std::borrow::Cow::Owned(_) => panic!(),
-                    }
+                    Some(pkt)
                 }).collect();
-                save_ptr(&env, &mut roots)?;
+                let mut it = roots.iter().map(|p| p.as_ref() as &dyn NetPkt);
+                let (_i,_) = writer.write_many_state(&mut it, None).unwrap();
             }
         }
         Ok(env)
     }
 
     pub fn local_enckey(&self) -> anyhow::Result<String> {
         // TODO this should prob check for read only access
-        Ok(std::fs::read_to_string(self.0.location.join("local_auth"))?.lines().next().context("missing enckey")?.to_owned())
+        Ok(std::fs::read_to_string(self.location.join("local_auth"))?.lines().next().context("missing enckey")?.to_owned())
     }
     #[instrument(ret,skip(bytes))]
     pub fn set_files_data(&self, path: impl AsRef<std::path::Path>+std::fmt::Debug, bytes: &[u8],overwrite:bool) -> anyhow::Result<()>{
         tracing::trace!(bytes=%AB(bytes));
         let path = self.dir().join("files").join(check_path(path.as_ref())?);
         let r: anyhow::Result<()> = try {
             std::fs::create_dir_all(path.parent().unwrap())?;
@@ -94,72 +92,74 @@
         match std::fs::read(&path){
             Ok(k) => Ok(Some(k)),
             Err(e) if !notfound_err && e.kind() == NotFound =>Ok(None),
             Err(e) => Err(e).with_context(|| anyhow::anyhow!("could not open {}",path.to_string_lossy()))
         }
     }
     #[track_caller]
-    pub fn get_reader(&self) -> anyhow::Result<ReadTxn> {
-        Ok(ReadTxn(self.0.lmdb.read_txn()?))
+    pub fn get_reader(&self) -> io::Result<ReadTxn> {
+        let btree_txn = self.inner.read_txn()?;
+        Ok(ReadTxn(IReadTxn::new(btree_txn)))
+    }
+    pub fn get_writer(&self) -> io::Result<WriteTxn2> {
+        tracing::trace!("Open write txn");
+        Ok(WriteTxn2 {
+            txn: Some(self.inner.write_txn()?),
+            update: &self.log_head,
+            last: None,
+        })
     }
 
     pub async fn log_head(&self) -> Stamp {
-        let v = self.0.log_head.next_async().await;
+        let v = self.log_head.next_async().await;
         Stamp::new(v)
     }
-
-    fn save<P:NetPkt>(&self, pkts: &mut [(P,SaveState)]) -> io::Result<usize>{
-        if pkts.is_empty() { return Ok(0);}
-        let (last_idx, total) = self.0.lmdb.save(pkts).map_err(db::as_io)?;
-        tracing::trace!(last_idx,total,"save ok");
-        if total > 0 {
-            let _ = self.0.log_head.emit(last_idx);
+}
+/// TODO fix name
+/// Needs to broadcast updates and expose a ReadTxn ref
+pub struct WriteTxn2<'o> {
+    txn: Option<db::WriteTxn<'o>>,
+    update: &'o ipcbus::ProcBus,
+    last: Option<Stamp>,
+}
+
+impl<'o> WriteTxn2<'o> {
+    pub fn reader(&self) -> queries::IReadTxn<&(impl misc::Cursors + '_)> {
+        tracing::debug!("Peek reader of write txn");
+        IReadTxn::new(self.txn.as_ref().unwrap())
+    }
+    fn set_last(
+        &mut self,
+        result: io::Result<(usize, Option<Stamp>)>,
+    ) -> io::Result<(usize, Option<Stamp>)> {
+        if let Ok((_writes, Some(last_writes))) = &result {
+            self.last = Some(*last_writes);
         }
-        Ok(total)
-    }
-    pub fn real_disk_size(&self) -> io::Result<u64> {
-        self.0.lmdb.real_disk_size()
-    }
-    pub fn env_info(&self) -> MDB_envinfo{
-        self.0.lmdb.env_info()
+        result
     }
-    pub fn db_info(&self) -> DbInfo{
-        self.0.lmdb.db_info().unwrap()
-    }
-    pub fn lmdb_version(&self) -> LMDBVersion{
-        self.0.lmdb.version_info()
+}
+impl<'txn> Drop for WriteTxn2<'txn> {
+    fn drop(&mut self) {
+        std::mem::drop(self.txn.take());
+        if let Some(last) = self.last {
+            let _ = self.update.emit(last.get());
+        }
     }
 }
 
-
-pub fn save_ptr(env: &BTreeEnv,pkts:&mut [(&NetPktPtr,SaveState)]) -> io::Result<usize>{
-    env.save(pkts)
-}
-pub fn save_dyn(env: &BTreeEnv,pkts:&mut [(&dyn NetPkt,SaveState)]) -> io::Result<usize>{
-    env.save(pkts)
-}
-pub fn save_ptr_one(env:&BTreeEnv,pkt:&NetPktPtr) -> io::Result<SaveState>{
-    let mut o = [(pkt,SaveState::Pending)];
-    save_ptr(env,&mut o)?;
-    Ok(o[0].1)
-}
-pub fn save_dyn_one(env:&BTreeEnv,pkt:&dyn NetPkt) -> io::Result<SaveState>{
-    let mut o = [(pkt,SaveState::Pending)];
-    save_dyn(env,&mut o)?;
-    Ok(o[0].1)
-}
-pub fn save_ptr_iter<'o>(env: &BTreeEnv, it : impl Iterator<Item=&'o NetPktPtr>) -> io::Result<usize>{
-    let mut lst = smallvec::SmallVec::<[(&NetPktPtr,SaveState);8]>::new_const();
-    lst.extend(it.map(|o|(o,SaveState::Pending)));
-    save_ptr(env,&mut lst)
-}
-pub fn save_dyn_iter<'o>(env: &BTreeEnv, it : impl Iterator<Item=&'o dyn NetPkt>) -> io::Result<usize>{
-    let mut lst = smallvec::SmallVec::<[(&dyn NetPkt,SaveState);8]>::new_const();
-    lst.extend(it.map(|o|(o,SaveState::Pending)));
-    save_dyn(env,&mut lst)
+impl<'txn> SWrite for WriteTxn2<'txn> {
+    fn write_many_state<'o>(
+        &mut self,
+        pkts: &'o mut dyn Iterator<Item = &'o dyn NetPkt>,
+        out: Option<&'o mut dyn FnMut(&'o dyn NetPkt, bool) -> Result<bool, ()>>,
+    ) -> io::Result<(usize, Option<Stamp>)> {
+        let r = self.txn.as_mut().unwrap().write_many_state(pkts, out);
+        self.set_last(r)
+    }
 }
+
 fn check_path(path:&std::path::Path) -> anyhow::Result<&std::path::Path>{
     if let Some(c) = path.components().find(|v| !matches!(v,std::path::Component::Normal(_))){
         anyhow::bail!("path can not contain a {c:?} component")
     }
     Ok(path)
 }
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/queries2.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/queries2.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,56 +17,56 @@
 - A Small stack machine. Something like  (Mem:[u8;256]) ++ vec![Enum{ChangeField, (TestOp,&[u8])}]
 
 
 */
 use crate::pkt::field_ids::FieldEnum;
 use crate::predicate::pkt_predicates::PktPredicates;
 use either::Either;
-use linkspace_pkt::{Stamp, B64, U256 };
+use linkspace_pkt::{Stamp, B64, U256, PktFmt };
 
 use crate::prelude::TestSet;
 use crate::{
     predicate::{
         exprs::RuleType,
         test_pkt::{compile_predicates, PktStreamTest},
     },
     prelude::{TreeEntryRef}
 };
 
 use crate::env::query_mode::{Mode, Order, Table};
 use crate::env::tree_key::treekey_checked;
 
 use crate::env::RecvPktPtr;
-use super::queries::ReadTxn;
+use super::queries::IReadTxn;
 use super::tree_iter::TreeKeysIter;
 
 
-impl<'txn> ReadTxn<'txn> {
-    pub fn scope_iter(
-        &'txn self,
+impl<C: super::misc::Cursors> IReadTxn<C> {
+    pub fn scope_iter<'o>(
+        &'o self,
         rules: &PktPredicates,
         order: Order,
-    ) -> Option<(TreeEntryRef<'txn>, TreeKeysIter<'txn>)> {
+    ) -> Option<(TreeEntryRef<'o>, TreeKeysIter<'o>)> {
         let req = rules.compile_tree_keys(order.is_asc()).unwrap();
         let lower_bound = req.lower_bound().unwrap();
-        let iter_dup = self.0.tree_cursor().iter_dup(order.is_asc());
+        let iter_dup = self.btree_txn.tree_cursor().iter_dup(order.is_asc());
         let at = iter_dup.set_range(&lower_bound).map(super::tree_iter::spd)?;
         let mut it = TreeKeysIter {
             req,
             iter_dup,
             lower_bound,
         };
         let at = it.set_pointer_at_match(at)?;
         Some((at, it))
     }
     pub fn query_tree_entries(
-        &'txn self,
+        &self,
         rules: &PktPredicates,
         ord: Order,
-    ) -> impl Iterator<Item = TreeEntryRef<'txn>> +'txn {
+    ) -> impl Iterator<Item = TreeEntryRef> {
         let nth_find_set = rules.state.i_branch;
         let mut yields = nth_find_set.iter(0);
         assert!(yields.peek().is_some(), "i_branch is empty");
         let (mut key_ptr, mut keys_iter) = self.scope_iter(rules, ord).unzip();
         let mut cnt = true;
         let pkt_stamp = rules.create;
         let recv_stamp = rules.recv_stamp;
@@ -121,49 +121,49 @@
                         }
                     }
                 }
             }
             None
         })
     }
-    pub fn query_tree(
-        &'txn self,
+    pub fn query_tree<'o>(
+        &'o self,
         ord: Order,
         predicates: &PktPredicates,
-    ) -> impl Iterator<Item = RecvPktPtr<'txn>> + 'txn{
+    ) -> impl Iterator<Item = RecvPktPtr<'o>> {
         let pkt_filter = compile_predicates(predicates)
             .0
             .filter(|(_test, kind)| !treekey_checked(*kind))
             .map(|(test,_)| test)
             .collect::<Vec<_>>();
-        let c1 = self.0.pkt_cursor();
+        let c1 = self.btree_txn.pkt_cursor();
         let it = self
             .query_tree_entries(predicates, ord)
             .map(move |v| {
                 crate::prelude::read_pkt(&c1, v.local_log_ptr())
                     .map_err(|e|("Btree Error - tree query",v.local_log_ptr(),e))
                     .unwrap()
                     .ok_or_else(||("BTree inconsistent - cant find",v.local_log_ptr()))
                     .unwrap()
             })
             .filter(move |pkt| {
                 let ok = pkt_filter.test(pkt);
-                tracing::trace!(ok,pkt=%linkspace_pkt::PktFmtDebug(pkt),"filter tree");
+                tracing::trace!(ok,pkt=%PktFmt(pkt),"filter tree");
                 ok
             });
         let nth_log_set = predicates.state.i_db.iter(0);
 
         it.zip(nth_log_set).filter_map(|(v, ok)| ok.then_some(v))
     }
 
-    pub fn query_log2(
-        &'txn self,
+    pub fn query_log2<'o>(
+        &'o self,
         ord: Order,
-        rules: &'txn PktPredicates,
-    ) -> impl Iterator<Item = RecvPktPtr<'txn>> {
+        rules: &'o PktPredicates,
+    ) -> impl Iterator<Item = RecvPktPtr<'o>> {
         let (it, recv) = compile_predicates(rules);
         let tests = it.map(|(t, _)| t).collect::<Vec<_>>().into_boxed_slice();
         let log_range = recv.stamp_range(ord.is_asc());
         tracing::debug!(?ord, range=?log_range, pre_chks=?tests, "Query Log");
 
         let it = self.log_range(log_range);
 
@@ -174,15 +174,15 @@
             .filter(move |pkt| tests.test(**pkt));
 
         let nth_log_set = rules.state.i_db.iter(0);
         it.zip(nth_log_set).filter_map(|(v, ok)| ok.then_some(v))
     }
 
     pub fn query_hash_entries(
-        &'txn self,
+        &self,
         hashset: TestSet<U256>,
         ord: Order,
     ) -> impl Iterator<Item = Stamp> + '_ {
         use crate::predicate::value_test::*;
         match ord {
             Order::Asc => {
                 let TestSet {
@@ -193,38 +193,38 @@
                         },
                     mask,
                 } = hashset;
                 if mask != Mask::DEFAULT {
                     tracing::warn!("todo impl hash mask jumping");
                 }
                 let greater_eq: B64<[u8; 32]> = greater_eq.into();
-                self.0
+                self.btree_txn
                     .hash_cursor()
                     .range_uniq(&greater_eq)
                     .map(|(hash, stamp)| (B64(*hash).into(), stamp))
                     .take_while(move |(v, _)| *v <= less_eq)
                     .filter(move |(v, _)| mask.test(v))
                     .map(|(_, stamp)| stamp.into())
             }
             Order::Desc => {
                 todo!("hash desc not yet impl");
             }
         }
     }
-    pub fn query_hash(
-        &'txn self,
+    pub fn query_hash<'o>(
+        &'o self,
         ord: Order,
-        rules: &'txn PktPredicates,
-    ) -> impl Iterator<Item = RecvPktPtr<'txn>> {
+        rules: &PktPredicates,
+    ) -> impl Iterator<Item = RecvPktPtr<'o>> {
         let pkt_filter = compile_predicates(rules)
             .0
             .filter(|(_, kind)| *kind != RuleType::Field(FieldEnum::PktHashF))
             .map(|(test, _)| test)
             .collect::<Vec<_>>();
-        let c1 = self.0.pkt_cursor();
+        let c1 = self.btree_txn.pkt_cursor();
         let it = self
             .query_hash_entries(rules.hash, ord)
             .map(move |v| {
                 crate::prelude::read_pkt(&c1, v)
                     .expect("BTree Is inconsistent")
                     .expect("BTree Is inconsistent")
             })
@@ -234,20 +234,20 @@
                 ok
             });
         let nth_log_set = rules.state.i_db.iter(0);
 
         it.zip(nth_log_set).filter_map(|(v, ok)| ok.then_some(v))
     }
 
-    pub fn query(
-        &'txn self,
+    pub fn query<'o>(
+        &'o self,
         mode: Mode,
-        pred: &'txn PktPredicates,
-        nth_pkt: &'txn mut u32,
-    ) -> anyhow::Result<impl Iterator<Item = RecvPktPtr<'txn>>> {
+        pred: &'o PktPredicates,
+        nth_pkt: &'o mut u32,
+    ) -> anyhow::Result<impl Iterator<Item = RecvPktPtr<'o>>> {
         tracing::debug!(?mode,%pred);
 
         match mode.table {
             Table::Hash => {
                 let it = self.query_hash(mode.order, pred);
                 let filter = pred.state.i_query.iter_contains(nth_pkt);
                 let it = it.zip(filter).filter_map(|(v, ok)| ok.then_some(v));
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/env/lmdb/tree_iter.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/lmdb/tree_iter.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/env/query_mode.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/query_mode.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/env/tree_key.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/tree_key.rs`

 * *Files 3% similar despite different names*

```diff
@@ -186,16 +186,14 @@
     }
 }
 impl<K: AsRef<[u8]>, V: AsRef<[u8]>> std::fmt::Debug for TreeEntry<K, V> {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         (&self.btree_key, self.val()).fmt(f)
     }
 }
-
-
 impl<B: AsRef<[u8]>> std::fmt::Debug for TreeKey<B> {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         let (g, d, spd, sp, k) = self.fields();
         let spath = sp
             .check_components()
             .map(|_| format!("{sp}"))
             .map_err(|_e| format!("Invalid{:?}", sp.spath_bytes()));
@@ -205,25 +203,16 @@
             .field(&spd)
             .field(&spath)
             .field(&k.b64_mini())
             .finish()
     }
 }
 
-impl<K: AsRef<[u8]>, V: AsRef<[u8]>> std::fmt::Display for TreeEntry<K, V> {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        let (g,d,spd,sp,k) = self.btree_key.fields();
-        let key = if k == PRIVATE { String::new() } else { k.to_string()};
-        let TreeValue { create, hash, logptr, links_len, data_size }= self.val();
-        write!(f,"{g}:{d}:{spd} {sp} {key} => ({create},{hash},{logptr},{links_len},{data_size})")
-    }
-}
-
 
-/// check if this type can be answered by a treekey
+/// check if this type can be answered by a treekey - currently conservative to simplify tree query impl
 pub const fn treekey_checked(r:RuleType) -> bool {
     match r {
         #[allow(clippy::match_like_matches_macro)]
         RuleType::Field(f) => match f{
             FieldEnum::PktHashF => true,
             FieldEnum::PubKeyF => true,
             FieldEnum::GroupIDF => true,
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/env/write_result.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/env/write_result.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/eval.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 // Copyright Anton Sol
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #![feature(
-    ptr_from_ref,
     extract_if,
     thread_local,
     file_create_new,
     let_chains,
     try_blocks,
     io_error_other,
     const_option_ext,
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/matcher/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/matcher/mod.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/mut_header.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/mut_header.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/partial_hash.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/partial_hash.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/bitset_test.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/bitset_test.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/builder.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/builder.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/exprs.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/exprs.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/pkt_predicates.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/pkt_predicates.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/predicate_type.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/predicate_type.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/test_pkt.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/test_pkt.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/treekey.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/treekey.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/uint.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/uint.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/predicate/value_test.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/predicate/value_test.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/prelude.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/prelude.rs`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 pub use linkspace_pkt::{*,eval,exprs,Error};
 
 pub use crate::consts::*;
 pub use crate::env::lmdb::queries::*;
 pub use crate::env::tree_key::*;
 pub use crate::env::write_result::*;
+pub use crate::env::write_trait::*;
 pub use crate::env::*;
 pub use crate::eval::*;
 pub use crate::matcher::*;
 pub use crate::partial_hash::PartialHash;
 pub use crate::predicate::exprs::*;
 pub use crate::predicate::pkt_predicates::*;
 pub use crate::predicate::test_pkt::*;
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/pull.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/pull.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/query.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/query.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/stamp_fmt.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/stamp_fmt.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-core/src/stamp_range.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/src/stamp_range.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/byte-fmt/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "byte-fmt"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 authors = ["Anton Sol <AntonSol919@gmail.com>"]
 categories = ["encoding","parsing"]
 keywords = ["base64","abe","newtype"]
 description = "B64 and AB newtype for parsing and printing"
 
 edition= "2021"
 license= "MPL-2.0"
@@ -13,15 +13,15 @@
 repository= "https://github.com/AntonSol919/linkspace"
 resolver = "2"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-abe = { path = "../abe", version = "0.3.0-rc2"}
+abe = { path = "../abe", version = "0.3.0-rc1"}
 
 serde= "=1.0.160"
 base64="=0.21"
 tracing= {version = "=0.1.37",features=["release_max_level_info"]}
 
 serde_bytes = "0.11.6"
 ruint = "1.7.0"
```

### Comparing `linkspace-0.3.0/local_dependencies/byte-fmt/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/byte-fmt/src/endian_types.rs` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/endian_types.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/byte-fmt/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/lib.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/byte-fmt/src/serde.rs` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/src/serde.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-cryptography/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "linkspace-cryptography"
 description = "Blake3 and schnorr cryptographic primitives for linkspace"
 
-version= "0.3.0-rc2"
+version= "0.3.0-rc1"
 authors= ["Anton Sol <AntonSol919@gmail.com>"]
 edition= "2021"
 license= "MPL-2.0"
 homepage= "https://www.linkspace.dev"
 documentation= "https://www.linkspace.dev/docs/guide/index.html"
 repository= "https://github.com/AntonSol919/linkspace"
 resolver = "2"
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-cryptography/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-cryptography/src/keygen.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/src/keygen.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-cryptography/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-cryptography/src/lib.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 [package]
 name = "linkspace"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 edition = "2021"
 authors = ["Anton Sol <AntonSol919@gmail.com>"]
 license = "MPL-2.0"
 homepage = "https://antonsol919.github.io/linkspace/"
 documentation = "https://www.linkspace.dev/docs/guide/index.html"
 repository = "https://github.com/AntonSol919/linkspace"
 categories = ["database","network-programming","asynchronous"]
 keywords = ["linkspace", "supernet"]
 description = "linkspace - a general purpose supernet"
 resolver = "2"
 
 
-
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [features]
 default = ["full", "lmdb"]
 lmdb=["linkspace-common/lmdb"]
 full = ["linkspace-common/full"]
 
 
 [dependencies]
 anyhow= "=1.0.71"
 backtrace = "0.3.67"
-linkspace-common = { path = "../linkspace-common", version = "0.3.0-rc2", default-features = false}
+linkspace-common = { path = "../linkspace-common", version = "0.3.0-rc1", default-features = false}
 tracing= {version = "=0.1.37",features=["release_max_level_info"]}
+build-info= { version = "=0.0.31"}
+
+[build-dependencies]
+build-info-build= { version = "=0.0.31"}
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace/src/conventions/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace/src/conventions/mod.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace/src/conventions/status.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace/src/conventions/status.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace/src/interop.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace/src/interop.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -533,15 +533,15 @@
     use crate::abe::ctx::UserData;
 
     use super::*;
     /// Create a new [Query]. Copy from a template. [Q] is the empty query.
     pub fn lk_query(copy_from: &Query) -> Query {
         Query(copy_from.0.clone())
     }
-    /// Create a new [Query] specifically for a hash. Sets the right mode and 'i' count. See [lk_get_hash] if you don't care to watch the db.
+    /// Create a new [Query] specifically for a hash. Sets the right mode and 'i' count.
     pub fn lk_hash_query(hash: LkHash) -> Query {
         Query(linkspace_common::core::query::Query::hash_eq(hash))
     }
 
     /// Add a single statement to a [Query], potentially skipping an encode step.
     /// i.e. fast path for adding a single statement - lk_query_parse(q,"{field}:{op}:{lk_encode(bytes)}")
     ///
@@ -677,18 +677,18 @@
     pub fn lk_inmem() -> std::io::Result<Linkspace> {
         todo!()
     }
     */
 
     /// save a packet. Returns true if new and false if its old.
     pub fn lk_save(lk: &Linkspace, pkt: &dyn NetPkt) -> std::io::Result<bool> {
-        linkspace_common::core::env::lmdb::save_dyn_one(&mut lk.0.env(), pkt).map(|o|o.is_new())
+        linkspace_common::core::env::write_trait::save_pkt(&mut lk.0.get_writer(), pkt)
     }
     pub fn lk_save_all(lk: &Linkspace, pkts: &[&dyn NetPkt]) -> std::io::Result<usize> {
-        linkspace_common::core::env::lmdb::save_dyn_iter(&mut lk.0.env(), pkts.iter().copied())
+        linkspace_common::core::env::write_trait::save_pkts(&mut lk.0.get_writer(), pkts).map(|(i,_)|i)
     }
     
     /// Run callback for every match for the query in the database.
     /// Break early if the callback returns true. 
     /// If break => number of matches
     /// If no break ( cb only returned false ) => -1 * Number of matches
     pub fn lk_get_all(
@@ -723,18 +723,14 @@
     ) -> LkResult<Option<A>> {
         let mode = query.0.get_mode()?;
         let mut i = 0;
         let reader = lk.0.get_reader();
         let opt_pkt = reader.query(mode, &query.0.predicates, &mut i)?.next();
         Ok(opt_pkt.map(|v| (cb)(v)))
     }
-    /** read a single packet from the database by its hash without copying. 
-    This means that [NetPkt::net_header_mut] is unavailable.
-    To mutate the header, wrap the result in [crate::misc::ReroutePkt] or copy with [NetPkt::as_netbox]..
-     **/
     pub fn lk_get_hash<A>(lk:&Linkspace,hash: LkHash,
                        cb: &mut dyn FnMut(RecvPktPtr) -> A,
     ) -> anyhow::Result<Option<A>> {
         let reader = lk.0.get_reader();
         let opt = reader.read(&hash)?;
         Ok(opt.map(|v|(cb)(v)))
     }
@@ -1010,7 +1006,8 @@
     }
 }
 
 // Allow for interop when importing linkspace_common
 #[doc(hidden)]
 pub mod interop;
 
+pub static BUILD_INFO : &str = build_info::format!("{}", $);
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-argon2-identity/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "linkspace-argon2-identity"
 description = "Argon2 encrypted schnorr keys"
 
-version= "0.3.0-rc2"
+version= "0.3.0-rc1"
 authors= ["Anton Sol <AntonSol919@gmail.com>"]
 edition= "2021"
 license= "MPL-2.0"
 homepage= "https://www.linkspace.dev"
 documentation= "https://www.linkspace.dev/docs/guide/index.html"
 repository= "https://github.com/AntonSol919/linkspace"
 resolver = "2"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [dependencies]
-linkspace-cryptography = { path = "../linkspace-cryptography", version="0.3.0-rc2"}
+linkspace-cryptography = { path = "../linkspace-cryptography", version="0.3.0-rc1"}
 
 thiserror=  "=1.0.40"
 base64="=0.21"
 
 rust-argon2 = {version = "1.0.0",default-features=false}
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-argon2-identity/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-core/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-argon2-identity/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-argon2-identity/src/lib.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 [package]
 name = "linkspace-pkt"
 categories = []
 keywords = ["linkspace"]
 description = "Library for reading and writing linkspace packets"
 
-version= "0.3.0-rc2"
+version= "0.3.0-rc1"
 authors= ["Anton Sol <AntonSol919@gmail.com>"]
 edition= "2021"
 license= "MPL-2.0"
 homepage= "https://www.linkspace.dev"
 documentation= "https://www.linkspace.dev/docs/guide/index.html"
 repository= "https://github.com/AntonSol919/linkspace"
 resolver = "2"
 
 [features]
 default = ["abe"]
 abe = []
 [dependencies]
-linkspace-cryptography = { path = "../linkspace-cryptography", version = "0.3.0-rc2"}
-byte-fmt = { path = "../byte-fmt", version = "0.3.0-rc2"}
+linkspace-cryptography = { path = "../linkspace-cryptography", version = "0.3.0-rc1"}
+byte-fmt = { path = "../byte-fmt", version = "0.3.0-rc1"}
 
 serde= "=1.0.160"
 thiserror=  "=1.0.40"
 arrayvec= "=0.7.2  "
 anyhow= "=1.0.71"
 static_assertions= "=1.1.0"
 auto_impl= "=1.0.1"
 bytes= "=1.1.0"
 bstr= {version = "1.5.0" ,default-features=false}
 bitflags= "=1.3.2"
 
 
-triomphe = { version = "0.1.8", git = "https://github.com/AntonSol919/triomphe"}
+triomphe = { version = "0.1.8-fn", git = "https://github.com/AntonSol919/triomphe"}
 
 [target.'cfg(target_arch = "wasm32")'.dependencies]
 wasm-bindgen = "0.2.80"
 
 
-[build-dependencies]
-vergen = { version="8", features = ["git", "gitcl", "rustc"]}
-
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/asm_tests.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/asm_tests.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/builder.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/builder.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/byte_segments.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/byte_segments.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/consts.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/consts.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/eval.rs`

 * *Files 4% similar despite different names*

```diff
@@ -97,20 +97,16 @@
                 let ctx = EvalCtx{scope}.pre_scope(pkt_scope(pkt.0));
                 Ok(abe::eval::eval(&ctx,&DEFAULT_FMT).unwrap().concat())
             }, none),
             ( @C "point",0..=0,Some(true),"TODO default point fmt",|pkt:&Self,_,_,scope| {
                 let ctx = EvalCtx{scope}.pre_scope(pkt_scope(pkt.0));
                 Ok(abe::eval::eval(&ctx,&DEFAULT_FMT).unwrap().concat())
             }, none),
-            ( @C "pkt-quick",0..=2,Some(true),"[add recv? =false , data_limit = max] same as pkt but without dynamic lookup",|pkt:&Self,arg:&[&[u8]],_,_| {
-                let mut buf = String::new();
-                let add_recv_field = !matches!(arg.get(0).copied(), None | Some(b"false") | Some(b""));
-                let data_limit = arg.get(1).map(|o| Ok::<usize,anyhow::Error>(std::str::from_utf8(o)?.parse()?)).transpose()?.unwrap_or(usize::MAX);
-                PktFmt(pkt.0).to_str(&mut buf,add_recv_field,data_limit)?;
-                Ok(buf.into_bytes())
+            ( @C "pkt-quick",0..=0,Some(true),"same as pkt but without dynamic lookup",|pkt:&Self,_,_,_| {
+                Ok(PktFmt(pkt.0).to_string().into_bytes())
             }, none),
 
 
             ( @C "html-quick",0..=0,Some(true),"same as html but without dynamic lookup",|pkt:&Self,_,_,_| {
                 let mut buf = String::new();
                 PktFmt(pkt.0).to_html(&mut buf,true,None)?;
                 Ok(buf.into_bytes())
@@ -210,25 +206,14 @@
                     }
                 }
             )
         ])
     }
 }
 
-fn eval_recv(b: Stamp, args:&[&[u8]]) -> anyhow::Result<Vec<u8>>{
-    let ok = match args.get(0).copied().unwrap_or(b"") {
-        b"abe" => b.to_abe_str().into_bytes(),
-        b"str" => b.to_string().into_bytes(),
-        b"" => b.0.to_vec(),
-        _ => bail!("unexpected fmt expect ?(str|abe)"),
-    };
-    Ok(ok)
-}
-
-
 #[derive(Copy, Clone, Debug)]
 pub struct RecvStamp<'o> {
     pkt: &'o dyn NetPkt,
 }
 impl<'o> EvalScopeImpl for RecvStamp<'o> {
     fn about(&self) -> (String, String) {
         (
@@ -237,29 +222,30 @@
         )
     }
 
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         fncs!([
             (
                 "recv",
-                0..=1,
+                0..=0,
                 Some(true),
-                "recv stamp - returns now if unavailable in context",
-                |t: &Self, args: &[&[u8]]| eval_recv(t.pkt.get_recv(),args)
+                "recv stamp - errors if unavailable in context",
+                |t: &Self, _i: &[&[u8]]| Ok(t.pkt.get_recv().0.to_vec())
             ),
             (
                 "recv_now",
-                0..=1,
+                0..=0,
                 Some(true),
-                "recv stamp - returns an error if not available in context",
-                |t: &Self, args: &[&[u8]]|
-                eval_recv(
-                    t.pkt.recv().context("no recv available in context")?,
-                    args
-                )
+                "recv stamp - recv stamp returns now if unavailable in context",
+                |t: &Self, _i: &[&[u8]]| Ok(t
+                    .pkt
+                    .recv()
+                    .context("no recv available in context")?
+                    .0
+                    .to_vec())
             )
         ])
     }
 }
 
 #[test]
 fn pktfmt() {
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/exprs.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/exprs.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/field_ids.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/field_ids.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/ipath.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/ipath.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 pub mod spath;
 pub mod spath_fmt;
 pub mod spath_macro;
 pub mod utils;
 pub mod read;
 mod builder;
 mod stamp;
-pub mod build_info;
 
 
 
 pub use consts::*;
 pub use byte_segments::*;
 pub use endian_types::*;
 pub use eval::*;
@@ -267,15 +266,17 @@
     fn get_links(&self) -> &[Link] {
         self.links().unwrap_or_default()
     }
     fn select(&self) -> SelectLink{ SelectLink(self.get_links())}
     fn compute_hash(&self) -> LkHash {
         linkspace_cryptography::hash_segments(&self.pkt_segments().0).into()
     }
-    
+    fn aligned_net_pkt_size(&self) -> u16 {
+        self.point_header_ref().size()
+    }
 
     fn check_private(&self) -> Result<(),crate::Error>{
         if self.group().copied() == Some(PRIVATE) { Err(crate::Error::PrivateGroup)}
         else {Ok(())}
     }
 }
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/link.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/link.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/header.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/header.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     fn as_netarc(&self) -> NetPktArc {
         (**self).as_netarc()
     }
     fn net_header_mut(&mut self) -> Option<&mut NetPktHeader> {
         None
     }
     fn recv(&self) -> Option<Stamp> {
-        (**self).recv()
+        None
     }
 }
 
 impl<T: NetPkt + ?Sized> NetPktExt for T {}
 
 #[doc(notable_trait)]
 /// Utilities for [NetPkt]
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/netpkt_arc.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_arc.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/netpkt_parts.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_parts.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/netpkt_ptr.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/netpkt_ptr.rs`

 * *Files 1% similar despite different names*

```diff
@@ -81,23 +81,23 @@
     pub fn reroute(&self, route: NetPktHeader) -> ReroutePkt<&Self> {
         ReroutePkt {
             net_header: route,
             pkt: self,
         }
     }
 
-    pub fn check(&self, skip_hash:bool) -> Result<(), Error> {
+    pub fn check(&self, skip_hash:bool) -> Result<&[u8], Error> {
         let _ = self.point.internal_consitent_length()?;
         if !skip_hash{
             self.point.check_signature()?;
             if self.hash() != self.point.compute_hash() {
                 return Err(Error::HashMismatch);
             }
         }
-        Ok(())
+        Ok(self.as_netpkt_bytes())
     }
     pub fn as_netpkt_bytes(&self) -> &[u8] {
         unsafe { from_raw_parts(ptr::from_ref(self).cast::<u8>(), usize::from(self.size())) }
     }
 }
 
 impl Clone for NetPktBox {
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/partial.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/partial.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/reroute.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/reroute.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/netpkt/slot.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/netpkt/slot.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/point.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/point_parts.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point_parts.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/point_ptr.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/point_ptr.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/read.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/read.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/repr.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/repr.rs`

 * *Files 4% similar despite different names*

```diff
@@ -38,84 +38,70 @@
 
 pub static JSON_PKT: &str = "todo";
 
 
 /// A static packet formatter similar to DEFAULT_PKT without using ABE expressions.
 pub struct PktFmt<'o>(pub &'o dyn NetPkt);
 
-
 impl<'o> core::fmt::Debug for PktFmt<'o>{
     fn fmt(&self, f: &mut Formatter<'_>) -> Result {
-        self.to_str(f,false,usize::MAX)
-    }
-}
-impl<'o> core::fmt::Display for PktFmt<'o> {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
-        core::fmt::Debug::fmt(self,f)
-    }
-}
-pub fn fmt_b64(bytes:&B64, class:&'static str , f:&mut impl fmt::Write) -> Result{
-    let b64 = bytes.b64();
-    let mut use_mini = false;
-    let group_abe = match *bytes{
-        e if e == PRIVATE=> "[#:0]".into(),
-        e if e == PUBLIC=> "[#:pub]".into(),
-        e if e == *TEST_GROUP => "[#:test]".into(),
-        e => {use_mini = true; e.to_abe_str()}
-    };
-    let ccode = bytes.0[14] >> 4;
-    let dcode = bytes.0[15] >> 4;
-    write!(f,"<span lk-{class}='{b64}' class='lk-b64 lk-c{ccode} lk-d{dcode}'>{}</span>",
-            if use_mini{bytes.b64_mini()} else {group_abe})
-}
-impl<'o> PktFmt<'o>{
-    pub fn to_str<F: fmt::Write>(&self, f: &mut F,add_recv:bool,data_limit:usize) -> Result{
         let pkt = self.0;
         let ptype = pkt.as_point().point_header_ref().point_type.as_str();
         let hash = pkt.hash_ref().to_string();
 
         let group = match *pkt.get_group(){
             e if e == PRIVATE=> "[#:0]".into(),
             e if e == PUBLIC=> "[#:pub]".into(),
             e if e == *TEST_GROUP => "[#:test]".into(),
             e => e.to_abe_str()
         };
         let domain = pkt.get_domain().as_str(true);
         let path = pkt.get_path().to_string();
         let pubkey = pkt.get_pubkey().to_abe_str();
         let create = pkt.get_create_stamp().get();
-    
+
         let links_len = pkt.get_links().len();
-        if add_recv {
-            match pkt.recv(){
-                Some(r) => write!(f,"recv\t{}\n",r),
-                None => write!(f,"recv\t???\n")
-            }?;
-        }
+        
         write!(f,"type\t{ptype}
 hash\t{hash}
 group\t{group}
 domain\t{domain}
 path\t{path}
 pubkey\t{pubkey}
 create\t{create}
 links\t{links_len}
 ")?;
         for crate::Link{ptr,tag}in pkt.get_links(){
             write!(f,"\t{} {ptr}\n",tag.as_str(true))?;
         }
-    let data = pkt.data();
-    let data = &data[0..data.len().min(data_limit)];
-    
-        let data = BStr::new(data);
+        let data = BStr::new(pkt.data());
         let data_size = pkt.data().len();
         write!(f,"data\t{data_size}\n{data}")
-
     }
-
+}
+impl<'o> core::fmt::Display for PktFmt<'o> {
+    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+        core::fmt::Debug::fmt(self,f)
+    }
+}
+pub fn fmt_b64(bytes:&B64, class:&'static str , f:&mut impl fmt::Write) -> Result{
+    let b64 = bytes.b64();
+    let mut use_mini = false;
+    let group_abe = match *bytes{
+        e if e == PRIVATE=> "[#:0]".into(),
+        e if e == PUBLIC=> "[#:pub]".into(),
+        e if e == *TEST_GROUP => "[#:test]".into(),
+        e => {use_mini = true; e.to_abe_str()}
+    };
+    let ccode = bytes.0[14] >> 4;
+    let dcode = bytes.0[15] >> 4;
+    write!(f,"<span lk-{class}='{b64}' class='lk-b64 lk-c{ccode} lk-d{dcode}'>{}</span>",
+            if use_mini{bytes.b64_mini()} else {group_abe})
+}
+impl<'o> PktFmt<'o>{
     /** create a html fragment describing the packet
 
     The format is a bit arbitrary. Its designed to be safe to paste into an html document and usable for most usecases. But it is verbose and somewhat opinionated.
     If it doesn't fit your usecase, just build your own template.
     Note: the lk-c[0..31] and lk-d[0..31] class's are derived from the hash and should be used for color coding when appropriate.
     */
     pub fn to_html<F: fmt::Write>(&self, f: &mut F,
@@ -199,15 +185,7 @@
                 '>' =>  f.write_str("&gt")?,
                 o => write!(f,"{o}")?
             }
         }
         Ok(())
     }
 }
-
-// quick hack 
-pub struct PktFmtDebug<'o>(pub &'o dyn NetPkt);
-impl<'o> core::fmt::Display for PktFmtDebug<'o> {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
-        PktFmt(self.0).to_str(f,true,160)
-    }
-}
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/spath.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/spath_fmt.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath_fmt.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/spath_macro.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/spath_macro.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-pkt/src/stamp.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-pkt/src/stamp.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/abe/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 
 name = "abe"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 authors = ["Anton Sol <AntonSol919@gmail.com>"]
 categories = ["encoding","parsing"]
 keywords = ["ascii-byte-expr", "ascii-byte","abe"]
 description = "Ascii-byte-expression : a tiny byte templating language"
 
 edition= "2021"
 license= "MPL-2.0"
```

### Comparing `linkspace-0.3.0/local_dependencies/abe/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/byte-fmt/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/abe_macro.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/abe_macro.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/abtxt.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/abtxt.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/ast.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/ast.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/convert.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/convert.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/eval.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/lib.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/scope/argv.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/scope/argv.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/scope/base.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/scope/base.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/scope/bytes.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/scope/bytes.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/scope/encode.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/scope/encode.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/scope/help.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/scope/help.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/scope/logic.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/scope/logic.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/scope/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/scope/mod.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/abe/src/scope/uint.rs` & `linkspace-0.3.0rc2/local_dependencies/abe/src/scope/uint.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [package]
 name = "linkspace-common"
 categories = []
 keywords = ["linkspace"]
 description = "linkspace common"
 
-version= "0.3.0-rc2"
+version= "0.3.0-rc1"
 authors= ["Anton Sol <AntonSol919@gmail.com>"]
 edition= "2021"
 license= "MPL-2.0"
 homepage= "https://www.linkspace.dev"
 documentation= "https://www.linkspace.dev/docs/guide/index.html"
 repository= "https://github.com/AntonSol919/linkspace"
 resolver = "2"
@@ -19,28 +19,28 @@
 default = ["full", "lmdb"]
 lmdb=["linkspace-core/lmdb"]
 fs=["memmap2", "notify"]
 cli=["clap", "clap/env", "clap/derive", "rpassword"]
 full=["fs", "cli"]
 
 [dependencies]
-abe = { path = "../abe", version = "0.3.0-rc2"}
-byte-fmt = { path = "../byte-fmt", version = "0.3.0-rc2"}
-linkspace-pkt = { path = "../linkspace-pkt", version = "0.3.0-rc2"}
-linkspace-core= { path = "../linkspace-core",default-features=false, version = "0.3.0-rc2"}
-linkspace-argon2-identity = { path = "../linkspace-argon2-identity", version = "0.3.0-rc2"}
+abe = { path = "../abe", version = "0.3.0-rc1"}
+byte-fmt = { path = "../byte-fmt", version = "0.3.0-rc1"}
+linkspace-pkt = { path = "../linkspace-pkt", version = "0.3.0-rc1"}
+linkspace-core= { path = "../linkspace-core",default-features=false, version = "0.3.0-rc1"}
+linkspace-argon2-identity = { path = "../linkspace-argon2-identity", version = "0.3.0-rc1"}
 
 anyhow= "=1.0.71"
 serde= { version = "=1.0.160", features = ["derive"] }
 tracing= {version = "=0.1.37",features=["release_max_level_info"]}
 tracing-subscriber= "=0.3.17"
 thiserror=  "=1.0.40"
 rand= "=0.8.5"
 clap = { version = "=4.3.4", optional = true , features = ["derive"] }
 futures= "=0.3.28"
 either= "=1.8.1"
 
-memmap2 = { version = "0.7.1", optional = true }
+memmap2 = { version = "0.5.5", optional = true }
 notify = { version = "5.0", optional = true }
 rpassword = { version = "7.1" , optional = true }
 async_executors = { version = "0.6.0", features = ["timer","async_global","bindgen","localpool"] }
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/abe/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/bus.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/bus.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/cli/keys.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/keys.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/cli/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 pub use tracing;
 
 use linkspace_core::prelude::{EvalCtx, Scope};
 use std::{
     io::{stderr,  stdout, },
 };
 
+
+
 pub type PreProc = Option<TypedABE<Vec<u8>>>;
 pub fn write_pkt2(
     preproc: &PreProc,
     pkt: impl NetPkt,
     ctx: &EvalCtx<impl Scope>,
     mut out: impl std::io::Write,
 ) -> std::io::Result<()> {
     match preproc {
         None => {
             let bytes = pkt.byte_segments();
             out.write_all_vectored(&mut bytes.io_slices())?;
         }
-        Some(expr) => {
-            let v = expr.eval(&pkt_ctx(ctx.reref(), &pkt));
-            if let Err(err) = &v{
-                tracing::warn!(?err,?expr,"error pre-processing with expression");
-            }
-            let v = v.map_err(std::io::Error::other)?;
+        Some(e) => {
+            let v = e
+                .eval(&pkt_ctx(ctx.reref(), &pkt))
+                .map_err(std::io::Error::other)?;
             out.write_all(&v)?;
         }
     }
     out.flush()
 }
 pub enum Out {
     Fd(Box<dyn std::io::Write + Send + Sync>),
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/cli/opts.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/opts.rs`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 use crate::{
     pkt_reader::NetPktDecoder,
     prelude::*,
     runtime::{handlers::PktStreamHandler, Linkspace},
 };
 use anyhow::Context;
 use clap::Parser;
-use linkspace_core::prelude::lmdb::{BTreeEnv };
+use linkspace_core::prelude::lmdb::BTreeEnv;
 
 use super::{write_pkt2, WriteDest, WriteDestSpec, reader::PktReadOpts};
 #[derive(Parser, Debug, Clone)]
 pub struct CommonOpts {
     #[clap(flatten)]
     pub linkspace: LinkspaceOpts,
     #[clap(flatten)]
@@ -165,63 +165,51 @@
     pub fn read_private(&self) -> Option<bool> {
         if self.io.private {
             Some(true)
         } else {
             self.io.inp.private_read
         }
     }
-    pub fn check_private<S:NetPkt>(&self, pkt:S ) -> Result<Option<S>,linkspace_pkt::Error> {
-        match self.write_private(){
-            Some(false) => pkt.check_private().map_err(|e| {tracing::error!(?e,pkt=%PktFmtDebug(&pkt),"trying to write private");e})?,
-            Some(true) => {},
-            None => {
-                if let Err(e) = pkt.check_private(){
-                    tracing::info!(?e,pkt=%PktFmtDebug(&pkt),"trying to write private - but no --private or --private-write true/false set - ignoring packet");
-                    return Ok(None)
-                }
-            }
-        }
-        Ok(Some(pkt))
+    pub fn check_private<S:NetPkt>(&self, pkt:S ) -> Result<S,linkspace_pkt::Error> {
+        let write_private = self.write_private().unwrap_or(false);
+        if !write_private { pkt.check_private().map_err(|e| {tracing::warn!(?e,pkt=%PktFmt(&pkt),"enable private writing");e})?}
+        Ok(pkt)
     }
     pub fn open(&self, lst: &[WriteDestSpec]) -> std::io::Result<Vec<WriteDest>> {
         let ctx = self.eval_ctx();
         lst.iter()
             .filter_map(|v| v.open(&ctx).transpose())
             .try_collect()
     }
     pub fn write_dest(
         &self,
         dest: &mut WriteDest,
         pkt: &dyn NetPkt,
         buffer: &mut Option<&mut dyn std::io::Write>,
     ) -> std::io::Result<()> {
-        let pkt = match self.check_private(pkt).map_err(linkspace_pkt::Error::io)?{
-            Some(p) => p,
-            None => return Ok(()),
-        };
+        let pkt = self.check_private(pkt).map_err(linkspace_pkt::Error::io)?;
         let out: &mut dyn std::io::Write = match &mut dest.out {
             super::Out::Db => {
-                lmdb::save_dyn_one(self.linkspace.env_io()?,pkt)?;
-                return Ok(())
-            },
+                return save_pkt(&mut self.linkspace.env_io()?.get_writer()?, pkt).map(|_| ())
+            }
             super::Out::Fd(f) => f,
             super::Out::Buffer => buffer
                 .as_mut()
                 .ok_or_else(|| io::Error::other("no buffer in this context"))?,
         };
         write_pkt2(&dest.prep, pkt, &self.eval_ctx(), out)
     }
 
     pub fn write_multi_dest(
         &self,
         mdest: &mut [WriteDest],
         pkt: &dyn NetPkt,
         mut buffer: Option<&mut dyn std::io::Write>,
     ) -> std::io::Result<()> {
-        let _ = tracing::debug_span!("Writing",pkt=%PktFmtDebug(pkt),recv=?pkt.recv() ).entered();
+        let _ = tracing::debug_span!("Writing",pkt=%PktFmt(pkt)).entered();
         for dest in mdest.iter_mut() {
             self.write_dest(dest, pkt, &mut buffer)?;
         }
         tracing::debug!("finish writing");
         Ok(())
     }
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/cli/reader.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/cli/reader.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/dgp.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/dgp.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/eval.rs`

 * *Files 4% similar despite different names*

```diff
@@ -114,16 +114,15 @@
         }
         let path = SPath::from_slice(inp.get(2).copied().unwrap_or(&[]))?.try_ipath()?;
         let key = inp
             .get(3)
             .map(|v| PubKey::try_fit_bytes_or_b64(v))
             .transpose()?
             .unwrap_or(B64([0; 32]));
-        let env = self.0.lk()?;
-        let reader = env.get_reader();
+        let reader =self.0.lk()?.get_reader();
 
         let predicates = Query::dgpk(domain, group, path, key).predicates;
         let pkt = reader
             .query_tree(query_mode::Order::Desc, &predicates)
             .next()
             .context("no matching packet")?;
         let id = inp.get(4).copied().unwrap_or(b"pkt");
@@ -144,16 +143,15 @@
 funcs evaluate as if [/[func + args]:[rest]]. (e.g. [/readhash:HASH:[group:str]] == [readhash:..:group:str])".into())
     }
     fn list_funcs(&self) -> &[ScopeFunc<&Self>] {
         &[
             ScopeFunc {
                 apply : |this:&Self,inp:&[&[u8]],_,scope|{
                     let hash = B64::try_fit_slice(inp[0])?;
-                    let env = this.0.lk()?;
-                    let reader = env.get_reader();
+                    let reader = this.0.lk()?.get_reader();
                     let pkt = reader.read(&hash)?.with_context(||format!("could not find pkt {}",hash))?;
                     let (id, args) = inp[1..].split_first().unwrap_or((&{b"pkt" as &[u8]},&[]));
                     let r = pkt_scope(&*pkt).try_apply_func(id, args, true,scope);
                     drop(reader);
                     r
                 },
                 info: ScopeFuncInfo {
@@ -182,16 +180,15 @@
                 let _empty = it.next().context("arg delimited with ':'")?;
                 ast::exact::<0>(_empty)?;
                 let hash = it.next().context("missing hash")?;
                 let expr = it.next().context("missing expr")?;
                 let alt = it.next();
                 let hash = eval(&ctx, hash)?.concat();
                 let hash: LkHash = LkHash::try_fit_slice(&hash)?;
-                let env = this.0.lk()?;
-                let reader = env.get_reader();
+                let reader = this.0.lk()?.get_reader();
                 match reader.read(&hash)? {
                     None => {
                         let alt = alt.with_context(|| format!("could not find pkt {}", hash))?;
                         it.next().context("to many args?")?;
                         let r = eval(&ctx, alt)?.concat();
                         ApplyResult::Value(r)
                     }
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/lib.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/pkt_reader.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/pkt_reader.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/pkt_stream_utils.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/pkt_stream_utils.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/predicate_aliases.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/predicate_aliases.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/handshake.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/handshake.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/blob.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blob.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkin.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkin.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkout.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/checkout.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/blobmap/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/blobmap/mod.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/impex/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/impex/mod.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/admin.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/admin.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 /// The lns:[#:0] lookup entries.
 
 use crate::{prelude::*, protocols::lns::{GROUP_TAG, LNS, BY_TAG_P, PUBKEY_TAG}};
-use linkspace_core::prelude::{query_mode::Order, RecvPktPtr, lmdb::save_dyn_iter};
+use linkspace_core::prelude::{query_mode::Order, RecvPktPtr};
 use tracing::instrument;
 
 use super::claim::Claim;
 
 
 // only call this with a valid claim
 #[instrument(ret,skip(lk),level="debug")]
 pub(crate) fn save_private_claim(lk: &Linkspace,new_claim:&Claim,admin:Option<&SigningKey>,and: &[&dyn NetPkt],priority:bool) -> anyhow::Result<bool>{
+    let wr = lk.get_writer();
     let read = lk.get_reader();
     let admin_k = admin.map(|v| v.pubkey());
     let now = now();
     // This claim is being overwritten. This means its old by-tag ptrs must be removed as well. 
     let old_claim = super::lookup_claim(lk, &new_claim.name)?;
     let old_claim = old_claim.as_ref();
     let old_chash = old_claim.map(|o|o.pkt.hash());
@@ -68,31 +69,32 @@
     fn as_p(p:&Option<NetPktBox>) -> Option<&dyn NetPkt> {
         match &p {
             Some(o) => Some(o as &dyn NetPkt),
             None => None,
         }
     }
 
-    let it = [&new_claim.pkt as &dyn NetPkt].into_iter()
+    let txn : Vec<&dyn NetPkt>= [&new_claim.pkt as &dyn NetPkt].into_iter()
         .chain(as_p(&drop_old_group))
         .chain(as_p(&add_new_group))
         .chain(as_p(&drop_old_pubkey))
         .chain(as_p(&add_new_pubkey))
-        .chain(and.iter().copied());
-    save_dyn_iter(lk.env(), it)?;
+        .chain(and.iter().copied())
+        .collect();
+    save_pkts(wr, &txn)?;
     Ok(true)
 }
 
 #[instrument(ret,skip(reader),level="debug")]
 pub fn ptr_lookup(reader: &ReadTxn, tag: Tag, ptr: LkHash,admin:Option<PubKey>) -> ApplyResult<Claim> {
     let ple = ptr_lookup_entry(reader, tag, ptr, admin);
     read_claims(reader, ple.into_ok()??.pkt, now()).find_map(|(_,p)| p.ok()?).into()
 }
 #[instrument(ret,skip(reader),level="debug")]
-pub fn ptr_lookup_entry<'o>(reader: &'o ReadTxn, tag: Tag, ptr: LkHash,admin:Option<PubKey>) -> ApplyResult<RecvPktPtr<'o>> {
+pub fn ptr_lookup_entry(reader: &ReadTxn, tag: Tag, ptr: LkHash,admin:Option<PubKey>) -> ApplyResult<RecvPktPtr> {
     let path = BY_TAG_P.into_spathbuf().push(tag).push(ptr);
     let mut preds = PktPredicates::from_gd(PRIVATE, LNS).path(path)?.create_before(now()).unwrap();
     // entries have the form /by-tag/TAG/PTR
     if let Some(v) = admin {
         preds.pubkey.add(TestOp::Equal, v.into())
     }
     tracing::debug!(%preds,"by-tag");
@@ -104,15 +106,15 @@
 fn read_claims<'o>(reader: &'o ReadTxn,pkt: &'o impl NetPkt,valid_at:Stamp) -> impl Iterator<Item=TaggedClaim> +'o{
     pkt.get_links().iter()
         .map(|v| (rtag(v.tag),v.ptr))
         .filter(move |((until,_),_)| *until > valid_at)
         .map(|(rt,p)| (rt,Claim::read(reader,&p)))
 }
 
-pub fn list_ptr_lookups<'o>(reader: &'o ReadTxn, tag: AB<[u8; 16]>,ptr:Option<LkHash>,admin:Option<PubKey>) -> impl Iterator<Item=Vec<TaggedClaim>> +'o {
+pub fn list_ptr_lookups(reader: &ReadTxn, tag: AB<[u8; 16]>,ptr:Option<LkHash>,admin:Option<PubKey>) -> impl Iterator<Item=Vec<TaggedClaim>> +'_ {
     let path = BY_TAG_P.into_spathbuf().push(tag);
     let path = if let Some(p) = ptr { path.push(*p)} else { path}; 
     let mut preds = PktPredicates::from_gd(PRIVATE, LNS).create_before(now()).unwrap();
     preds.prefix(path).unwrap();
     preds.path_len.add(TestOp::Equal,3);
     preds.state.i_branch.add(TestOp::Equal,0);
     if let Some(v) = admin {
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/claim.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/claim.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/eval.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/eval.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/file_claim.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/file_claim.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/local_claim.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/local_claim.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/mod.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/mod.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/name.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/name.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/public_claim.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/public_claim.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/protocols/lns/utils.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/protocols/lns/utils.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/runtime/handlers.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/handlers.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/runtime/rx.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/rx.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 //
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this
 // file, You can obtain one at https://mozilla.org/MPL/2.0/.
 use super::handlers::{FollowHandler, PktStreamHandler, SinglePktHandler, StopReason};
 use anyhow::{bail, Context};
 pub use async_executors::{Timer, TimerExt};
+use futures::future::Either;
 pub use futures::task::{LocalSpawn, LocalSpawnExt};
-use linkspace_core::prelude::{*, lmdb::{BTreeEnv  }};
+use linkspace_core::prelude::{*, lmdb::{BTreeEnv, WriteTxn2, misc::Refreshable}};
 use linkspace_pkt::reroute::ShareArcPkt;
 use std::{
     borrow::{Borrow, Cow},
     cell::{Cell, OnceCell, RefCell},
     ops::{ ControlFlow},
-    rc::{Rc },
+    rc::{Rc, Weak},
     time::{Duration, Instant},
 };
 use tracing::{warn, Span, debug_span, instrument};
 
 pub type PktStream = Box<dyn PktStreamHandler + 'static>;
 pub type Matcher = linkspace_core::matcher::Matcher<PktStream>;
 /// [WatchEntry] with an associated callback (Box<dyn [PktStreamHandler]>)
@@ -37,43 +38,57 @@
 }
 enum Pending {
     PostWatch { cb: PostTxnHandler, span: Span },
     NewWatch { watch_entry: RxEntry },
     Close { id: QueryID, range: bool },
 }
 
+struct _ExecutorTxn {
+    last: Stamp,
+    txn: Either<Rc<ReadTxn>, Weak<ReadTxn>>,
+}
+
 impl Borrow<BTreeEnv> for Linkspace {
     fn borrow(&self) -> &BTreeEnv {
         self.env()
     }
 }
 
 pub(crate) struct Executor {
     env: BTreeEnv,
     written: Cell<bool>,
     cbs: RefCell<(Matcher, PostTxnList)>,
     pending: RefCell<Vec<Pending>>,
-    process_txn: RefCell<Rc<ReadTxn<'static>>>,
+    process_txn: RefCell<Rc<ReadTxn>>,
     process_upto: Cell<Stamp>,
     is_running: Cell<bool>,
     pub spawner: OnceCell<Rc<dyn LocalAsync>>,
 }
 
 impl Linkspace {
-    pub fn get_reader<'env:'txn,'txn>(&'env self) -> Rc<ReadTxn<'txn>> {
+    pub fn get_reader(&self) -> Rc<ReadTxn> {
+        //Rc::new(self.exec.env.get_reader().unwrap())
         self.exec.process_txn.borrow().clone()
     }
-    
+    pub fn get_writer(&self) -> WriteTxn2 {
+        if !self.exec.written.get() {
+            tracing::trace!("Set Written true")
+        }
+        self.exec.written.set(true);
+        self.exec.env.get_writer().unwrap()
+    }
     pub fn env(&self) -> &BTreeEnv {
         &self.exec.env
     }
     pub fn spawner(&self) -> &OnceCell<Rc<dyn LocalAsync>> {
         &self.exec.spawner
     }
+}
 
+impl Linkspace {
     fn rt_log_head(&self) -> Stamp {
         self.exec.process_upto.get()
     }
     /** return when next to process.
      Ok(None) means immediatly, Ok(Some(stamp)) means at stamp a watch can be dropped, Err means no current watches
     **/
     #[instrument(skip(self),ret)]
@@ -89,16 +104,15 @@
         self.exec.cbs.borrow_mut().0.gc(now()).ok_or(()).map(Some)
     }
     pub fn new(env: BTreeEnv, spawner: Rc<dyn LocalAsync>) -> Linkspace {
         Self::new_opt_rt(env, OnceCell::from(spawner))
     }
 
     pub fn new_opt_rt(env: BTreeEnv, spawner: OnceCell<Rc<dyn LocalAsync>>) -> Linkspace {
-        let reader : ReadTxn<'_>= env.get_reader().unwrap();
-        let reader : ReadTxn<'static> = unsafe { std::mem::transmute(reader)};
+        let reader = env.get_reader().unwrap();
         let at = reader.log_head();
         Linkspace {
             exec: Rc::new(Executor {
                 env,
                 written: Cell::new(false),
                 cbs: Default::default(),
                 pending: Default::default(),
@@ -140,23 +154,23 @@
             }
         }
     }
     pub async fn poll(&self) -> Stamp {
         loop {
             self.process();
             let rt_head = self.rt_log_head();
-            let env_head = self.env().log_head().await;
+            let env_head = self.inner().log_head().await;
             if env_head == rt_head {
                 return env_head;
             }
         }
     }
     pub fn run(&self) -> ! {
         loop {
-            if let Some(v) = self.env().0.log_head.next_d(None) {
+            if let Some(v) = self.inner().log_head.next_d(None) {
                 if self.rt_log_head().get() < v {
                     self.process();
                 }
             }
         }
     }
 
@@ -245,39 +259,38 @@
                 Err(_) => {
                     tracing::debug!("no more callbacks");
                     return Ok(1);
                 }
             };
 
             tracing::debug!(wakeup=?d(next_check), "waiting for new event");
-            self.env().0.log_head.next_d(Some(next_check));
+            self.inner().log_head.next_d(Some(next_check));
         }
     }
 
     /// check the log for new packets and execute callbacks
     #[instrument(skip(self))]
     pub fn process(&self) -> Stamp {
         self.exec.written.set(false);
         let this = self.clone();
         let (txn, from, upto): (Rc<ReadTxn>, Stamp, Stamp) = {
             let mut txn = self.exec.process_txn.borrow_mut();
             let rx_last = self.exec.process_upto.get();
             match Rc::get_mut(&mut txn) {
                 Some(txn) => {
                     tracing::trace!(?rx_last, "refresh txn");
-                    txn.refresh();
+                    Refreshable::refresh(txn);
                 }
                 None => {
-                    tracing::warn!("holding a read txn across callbacks!");
-                    // the transmute sets the lifetime - but the open txn can eat up memory
-                    *txn = Rc::new(unsafe{std::mem::transmute(self.exec.env.get_reader().unwrap())});
+                    tracing::warn!("holding a txn across callbacks!");
+                    *txn = Rc::new(self.exec.env.get_reader().unwrap());
                 }
             }
             let txn_last = txn.log_head();
-            if rx_last >= txn_last {
+            if rx_last > txn_last {
                 tracing::debug!(?txn_last, ?rx_last, "Already processed");
                 return rx_last;
             }
             (txn.clone(), rx_last, txn_last)
         };
         let _g = tracing::error_span!("Processing txn", ?from, ?upto).entered();
         let txn = txn;
@@ -293,15 +306,15 @@
             }
             count = Rc::strong_count(&txn)
         };
         for pkt in txn.pkts_after(from) {
             if pkt.net_header().flags.contains(NetFlags::SILENT) {
                 tracing::trace!("(not) skipping silent pkt - TODO make this a option");
             }
-            let _g = tracing::error_span!("Matching",pkt=%PktFmtDebug(&pkt)).entered();
+            let _g = tracing::error_span!("Matching",logptr=?pkt.recv,pkt=%PktFmt(&pkt.pkt)).entered();
             tracing::debug!("Testing New Pkt");
 
             let pkt = ShareArcPkt {
                 arc: OnceCell::new(),
                 pkt,
             };
 
@@ -423,15 +436,15 @@
             let local_span = tracing::debug_span!(parent: &span, "DB Callback").entered();
             tracing::trace!(?mode);
             let reader = self.get_reader();
             let r = reader
                 .query(mode, &q.predicates, &mut counter)?
                 .try_for_each(|dbp| {
                     let _g = local_span.enter();
-                    tracing::debug!(pkt=%PktFmtDebug(&dbp.pkt), recv=%dbp.recv().unwrap(),"Match");
+                    tracing::debug!(pkt=%PktFmt(&dbp.pkt),"Match");
                     onmatch.handle_pkt(&dbp, self)
                 });
             if Rc::strong_count(&reader) > 2 {
                 warn!("Holding txn open");
             }
             tracing::debug!(?r,"Done with DB");
             if matches!(r, ControlFlow::Break(_)) {
@@ -457,15 +470,17 @@
             Err(_) => self
                 .exec
                 .pending
                 .borrow_mut()
                 .push(Pending::PostWatch { cb, span }),
         }
     }
-    
+    pub fn inner(&self) -> &BTreeEnv {
+        &self.exec.env
+    }
     pub fn close(&self, id: impl AsRef<QueryIDRef>) {
         match self.exec.cbs.try_borrow_mut() {
             Ok(mut lk) => {
                 lk.0.deregister(id.as_ref(), false, |w| {
                     drop_watch(w, self, StopReason::Closed)
                 });
             }
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/runtime/threads.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/runtime/threads.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/static_env.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/static_env.rs`

 * *Files 19% similar despite different names*

```diff
@@ -9,23 +9,32 @@
 use std::cell::OnceCell;
 /// static btreeenv, shares one receiver thread and database session.
 /// With thread local linkspace's
 /// TODO: allow multiple
 use std::io;
 use std::path::{Path, PathBuf};
 use std::sync::OnceLock;
+use std::thread::JoinHandle;
+
+
+
+
+
+
+
 pub static ROOT_PATH: OnceLock<PathBuf> = OnceLock::new();
 static ENV: OnceLock<BTreeEnv> = OnceLock::new();
+static IPC_THREAD: OnceLock<JoinHandle<()>> = OnceLock::new();
 
 #[thread_local]
 static LINKSPACE: OnceCell<Linkspace> = OnceCell::new();
 pub fn get_env(root: &Path, mkdir: bool) -> io::Result<&'static BTreeEnv> {
     ENV.get_or_try_init(|| -> io::Result<BTreeEnv> {
         let mut env = BTreeEnv::open(root.to_owned(), mkdir)?;
-        Arc::get_mut(&mut env.0).unwrap().log_head.init();
+        env.log_head.init_udp();
         ROOT_PATH.set(root.canonicalize()?).unwrap();
         Ok(env)
     })
 }
 
 pub fn find_linkspace(root: Option<&Path>) -> io::Result<PathBuf> {
     match ROOT_PATH.get() {
@@ -51,90 +60,77 @@
             Ok(path)
         }
     }
 }
 
 pub fn open_linkspace_dir(root: Option<&Path>, new: bool) -> io::Result<Linkspace> {
     let path = find_linkspace(root)?;
-    LINKSPACE
-        .get_or_try_init(|| {
+    LINKSPACE.get_or_try_init(|| {
+            // ensure the IPC thread is propery enabled.
+            if ENV.get().is_none() != IPC_THREAD.get().is_none() {
+                return Err(io::Error::other(
+                    "use get_linkspace before get_env if both are required",
+                ));
+            };
             let env = get_env(&path, new)?;
             let rt = Linkspace::new_opt_rt(env.clone(), Default::default());
-            rt.env().0.log_head.init();
+            IPC_THREAD.get_or_init(|| rt.env().log_head.setup_ipc_thread());
             Ok(rt)
         })
         .map(|r| r.clone())
 }
 
+
+
 #[thread_local]
 static GROUP: OnceCell<GroupID> = OnceCell::new();
-pub fn set_group(group: GroupID) {
-    assert_eq!(
-        *GROUP.get_or_init(|| group),
-        group,
-        "user bug: the default group can only be set once per thread"
-    );
+pub fn set_group(group:GroupID){
+    assert_eq!(*GROUP.get_or_init(|| group), group, "user bug: the default group can only be set once per thread");
 }
 /** [Thread Local]: get the 'default' group. from [set_group] || $LK_GROUP || [#:pub]
 
 If the LK_GROUP expression requires LNS evaluation this will use the thread local linkspace or open the default.
 **/
-pub fn group() -> GroupID {
+pub fn group() -> GroupID{
     use std::env::*;
-    *GROUP.get_or_init(|| match std::env::var("LK_GROUP") {
+    *GROUP.get_or_init(|| match std::env::var("LK_GROUP"){
         Err(VarError::NotPresent) => PUBLIC,
         Ok(o) => {
-            let expr: GroupExpr = o.parse().expect("cant parse LK_GROUP");
-            let ctx = std_ctx_v(
-                || {
-                    if let Some(o) = LINKSPACE.get() {
-                        return Ok(o.clone());
-                    }
-                    tracing::info!("opening default linkspace to read evaluate LK_GROUP variable");
-                    Ok(open_linkspace_dir(None, false)?)
-                },
-                EVAL0_1,
-                true,
-            );
+            let expr : GroupExpr = o.parse().expect("cant parse LK_GROUP");
+            let ctx = std_ctx_v(|| {
+                if let Some(o) = LINKSPACE.get(){ return Ok(o.clone())}
+                tracing::info!("opening default linkspace to read evaluate LK_GROUP variable");
+                Ok(open_linkspace_dir(None, false)?)
+            }, EVAL0_1,true);
             expr.eval(&ctx).expect("can't eval LK_GROUP")
-        }
-        _ => panic!("can't read LK_DOMAIN as utf8"),
+        },
+        _ => panic!("can't read LK_DOMAIN as utf8")
     })
 }
 
 #[thread_local]
-static DOMAIN: OnceCell<Domain> = OnceCell::new();
+static DOMAIN : OnceCell<Domain> = OnceCell::new();
 
 /// set the result for [domain]
-pub fn set_domain(domain: Domain) {
-    assert_eq!(
-        *DOMAIN.get_or_init(|| domain),
-        domain,
-        "user bug: the standard domain can only be set once per thread"
-    );
+pub fn set_domain(domain:Domain) {
+    assert_eq!(*DOMAIN.get_or_init(|| domain), domain, "user bug: the standard domain can only be set once per thread");
 }
 /** [Thread Local]: get the 'default' domain. from [set_domain] || $LK_DOMAIN || [0;16]
 
 If the LK_DOMAIN expression requires LNS evaluation this will use the thread local linkspace or open the default.
 **/
-pub fn domain() -> Domain {
+pub fn domain() -> Domain{
     use std::env::*;
-    *DOMAIN.get_or_init(|| match std::env::var("LK_DOMAIN") {
+    *DOMAIN.get_or_init(|| match std::env::var("LK_DOMAIN"){
         Err(VarError::NotPresent) => ab(b""),
         Ok(o) => {
-            let expr: DomainExpr = o.parse().expect("cant parse LK_DOMAIN");
-            let ctx = std_ctx_v(
-                || {
-                    if let Some(o) = LINKSPACE.get() {
-                        return Ok(o.clone());
-                    }
-                    tracing::info!("opening default linkspace to read evaluate LK_DOMAIN variable");
-                    Ok(open_linkspace_dir(None, false)?)
-                },
-                EVAL0_1,
-                true,
-            );
+            let expr : DomainExpr = o.parse().expect("cant parse LK_DOMAIN");
+            let ctx = std_ctx_v(|| {
+                if let Some(o) = LINKSPACE.get(){ return Ok(o.clone())}
+                tracing::info!("opening default linkspace to read evaluate LK_DOMAIN variable");
+                Ok(open_linkspace_dir(None, false)?)
+            }, EVAL0_1,true);
             expr.eval(&ctx).expect("can't eval LK_DOMAIN")
         }
-        _ => panic!("can't read LK_DOMAIN as utf8"),
+        _ => panic!("can't read LK_DOMAIN as utf8")
     })
 }
```

### Comparing `linkspace-0.3.0/local_dependencies/linkspace-common/src/tests.rs` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/src/tests.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/ipcbus/Cargo.toml` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -9,25 +9,21 @@
 keywords = []
 description = "Cross platform IPC bus"
 resolver = "2"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [features]
 default = []
-inotify = ["nix/inotify","memmap2"]
 [dependencies]
 
 tracing= {version = "=0.1.37",features=["release_max_level_info"]}
-anyhow= "=1.0.71"
+libc= "=0.2.142"
 
 socket2 = { version = "0.4.4", features = ["all"]}
+nix = "0.24.1"
 event-listener = "2.5.2"
 
 [target.'cfg(target_arch = "wasm32")'.dependencies]
-futures= "=0.3.28"
+futures = "0.3.21"
 
 [target.'cfg(not(target_arch = "wasm32"))'.dependencies]
 fslock = {version="0.2.1"}
-libc= "0.2.147"
-
-nix = { version = "0.26.2", features = ["socket"] }
-memmap2 = { version = "0.7.1", optional =true}
```

### Comparing `linkspace-0.3.0/local_dependencies/ipcbus/LICENSE` & `linkspace-0.3.0rc2/local_dependencies/linkspace-common/LICENSE`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/local_dependencies/ipcbus/src/udp_multicast.rs` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/src/udp_multicast.rs`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     bind_to_device(&mut send_socket);
 
     let mut recv_socket = Socket::new(Domain::IPV4, Type::DGRAM, Some(Protocol::UDP)).unwrap();
     bind_to_device(&mut recv_socket);
     recv_socket.set_reuse_address(true).unwrap();
     reuse_port(&mut recv_socket);
 
-    let listen_addr: SocketAddr = (addr, port).into();
+    let listen_addr: SocketAddr = ([0, 0, 0, 0], port).into();
     recv_socket.bind(&listen_addr.into()).unwrap();
     recv_socket.set_reuse_address(true).unwrap();
     recv_socket
         .join_multicast_v4(&Ipv4Addr::from(addr), &Ipv4Addr::LOCALHOST)
         .unwrap();
     (
         recv_socket,
@@ -127,13 +127,13 @@
     use std::os::unix::prelude::AsRawFd;
     let dev = std::ffi::OsString::from("lo");
     if let Err(e) = nix::sys::socket::setsockopt(
         socket.as_raw_fd(),
         nix::sys::socket::sockopt::BindToDevice,
         &dev,
     ) {
-        tracing::info!(e=?e,"could not bind to loopback device. Nothing bad will happen - setcap cap_net_raw=+eip [executable path] might fix this error")
+        tracing::info!(e=?e,"could not bind to loopback device. Nothing bad will happen. ")
     }
 }
 
 #[cfg(windows)]
 pub fn bind_to_device(_socket: &mut Socket) {}
```

### Comparing `linkspace-0.3.0/local_dependencies/ipcbus/src/wasmbus.rs` & `linkspace-0.3.0rc2/local_dependencies/ipcbus/src/wasmbus.rs`

 * *Files 0% similar despite different names*

```diff
@@ -48,9 +48,7 @@
         }
         *old = last;
         let v = rx.next().await.unwrap();
         *old = old.max(v);
         return *old;
     }
 }
-
-
```

### Comparing `linkspace-0.3.0/Cargo.toml` & `linkspace-0.3.0rc2/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 [package]
 name = "linkspace-py"
 
-version = "0.3.0"
+version ="0.3.0-rc2"
 authors= ["Anton Sol <AntonSol919@gmail.com>"]
 edition= "2021"
 license= "MPL-2.0"
 homepage= "https://www.linkspace.dev"
 documentation= "https://www.linkspace.dev/docs/guide/index.html"
 repository= "https://github.com/AntonSol919/linkspace"
-build = "../../build_env.rs"
 resolver = "2"
 
 [lib]
 name = "linkspace"
 crate-type = ["cdylib"]
 
 [dependencies]
-linkspace = { path = "local_dependencies/linkspace", version ="0.3.0-rc2"}
-linkspace-pkt = { path = "local_dependencies/linkspace-pkt", version ="0.3.0-rc2"}
+linkspace = { path = "local_dependencies/linkspace", version ="0.3.0-rc1"}
 
-smallvec= {version="1.10.0",features=["const_new","const_generics","write"]}
 anyhow= "=1.0.71"
 tracing= {version = "=0.1.37",features=["release_max_level_info"]}
 tracing-subscriber = { version = "=0.3.17", features = ["env-filter"] }
 
-pyo3 = { version = "0.19.0", features = ["extension-module","anyhow","abi3","serde","abi3-py38"]  }
-[build-dependencies]
-vergen = { version = "=8.2.1", features = ["git", "gitcl", "rustc"] }
-
+pyo3 = { version = "0.18.2", features = ["extension-module","anyhow","abi3","serde","abi3-py38"]  }
+smallvec = {version="1.10.0",features=["const_new","const_generics","write"]}
```

### Comparing `linkspace-0.3.0/Makefile` & `linkspace-0.3.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/linkspace.pyi` & `linkspace-0.3.0rc2/linkspace.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -135,25 +135,16 @@
             - ``pkt``: Pkt
             Returns: bool,optional
     Returns:
         If cb returned True, returns number of packets matching the query. Otherwise -1 * number of matches.
     
     """
     ...
-
-def lk_get_hash(lk:Linkspace,hash:str|bytes) -> Pkt | None:
-    """Read a single packet hash from the database"""
-    ...
-
-
 def lk_hash_query(hash:str|bytes) -> Query:
-    """
-    Shorthand for building a query that matches a single hash
-    Use lk_get_hash if you do not care to watch the database
-    """
+    """Shorthand for building a query that matches a single hash"""
     ...
 
 def lk_info(lk:Linkspace) -> LkInfo:
     """Misc info about the linkspace instance"""
     ...
 
 def lk_key(lk:Linkspace,password:bytes|None=None,name:str|None=None,create:bool=False) -> SigningKey:
```

### Comparing `linkspace-0.3.0/src/lib.rs` & `linkspace-0.3.0rc2/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -390,20 +390,14 @@
         cb_err = call_cont_py(py, &cb, (pkt,)).map(|c| breaks = c);
         breaks
     })?;
     cb_err?;
     Ok(count)
 }
 #[pyfunction]
-pub fn lk_get_hash(lk: &Linkspace, hash:  &PyAny) -> anyhow::Result<Option<Pkt>> {
-    let hash = LkHash::try_fit_bytes_or_b64(bytelike(hash)?)?;
-    linkspace_rs::runtime::lk_get_hash(&lk.0, hash, &mut |pkt| Pkt::from_dyn(&pkt))
-}
-
-#[pyfunction]
 pub fn lk_watch(
     py: Python,
     lk: &Linkspace,
     query: &Query,
     on_match: Option<PyFunc>,
     on_close: Option<PyFunc>,
     on_err: Option<PyFunc>,
@@ -584,15 +578,14 @@
     m.add_function(wrap_pyfunction!(crate::lk_query_clear, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_open, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_save, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_save_all, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_get, m)?)?;
-    m.add_function(wrap_pyfunction!(crate::lk_get_hash, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_get_all, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_watch, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_process, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_process_while, m)?)?;
 
     m.add_function(wrap_pyfunction!(crate::lk_list_watches, m)?)?;
     m.add_function(wrap_pyfunction!(crate::lk_info, m)?)?;
@@ -615,16 +608,14 @@
     m.add_function(wrap_pyfunction!(crate::domain, m)?)?;
     m.add_function(wrap_pyfunction!(crate::set_domain, m)?)?;
 
     m.add("PRIVATE", PyBytes::new(py, &consts::PRIVATE.0))?;
     m.add("TEST_GROUP", PyBytes::new(py, &**consts::TEST_GROUP))?;
     m.add("PUBLIC", PyBytes::new(py, &consts::PUBLIC.0))?;
     m.add("DEFAULT_PKT", abe::DEFAULT_PKT)?;
-    linkspace_pkt::build_info!();
-    m.add("VERSION",BUILD_INFO)?;
 
     Ok(())
 }
 
 #[pyfunction]
 #[pyo3(signature=(bytes,mini=false))]
 pub fn b64<'o>(bytes:&[u8], mini:bool) -> String{
```

### Comparing `linkspace-0.3.0/src/pynetpkt.rs` & `linkspace-0.3.0rc2/src/pynetpkt.rs`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/tests/nested_watch.py` & `linkspace-0.3.0rc2/tests/nested_watch.py`

 * *Files identical despite different names*

### Comparing `linkspace-0.3.0/Cargo.lock` & `linkspace-0.3.0rc2/Cargo.lock`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "abe"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
  "arrayvec",
  "base64 0.21.2",
  "bstr",
  "hex",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "addr2line"
-version = "0.20.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+checksum = "a76fd60b23679b7d19bd066031410fb7e458ccc5e958eb5c325888ce4baedc97"
 dependencies = [
  "gimli",
 ]
 
 [[package]]
 name = "adler"
 version = "1.0.2"
@@ -36,14 +36,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "anstream"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
@@ -200,17 +215,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "backtrace"
-version = "0.3.68"
+version = "0.3.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+checksum = "233d376d6d185f2a3093e58f283f60f880315b6c60075b01f36b3b85154564ca"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -253,20 +268,14 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "bitflags"
-version = "2.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
-
-[[package]]
 name = "blake2b_simd"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c2f0dc9a68c6317d884f97cc36cf5a3d20ba14ce404227df55e1af708ab04bc"
 dependencies = [
  "arrayref",
  "arrayvec",
@@ -328,22 +337,87 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a246e68bb43f6cd9db24bea052a53e40405417c5fb372e3d1a8a7f770a564ef5"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "build-info"
+version = "0.0.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b301350c1c448e35b896f32b68c49c8ecd969a71978fbafc4ebd09ec3f4eee2"
+dependencies = [
+ "build-info-common",
+ "build-info-proc",
+ "once_cell",
+]
+
+[[package]]
+name = "build-info-build"
+version = "0.0.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b314717755dd6a06fc11ad3f7909ba4c0ae2ab516f5cb0404fe924c71bfc7d0"
+dependencies = [
+ "anyhow",
+ "base64 0.21.2",
+ "bincode",
+ "build-info-common",
+ "cargo_metadata",
+ "chrono",
+ "git2",
+ "glob",
+ "once_cell",
+ "pretty_assertions",
+ "rustc_version",
+ "serde_json",
+ "xz2",
+]
+
+[[package]]
+name = "build-info-common"
+version = "0.0.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5e040d36472d40ec9424c36a7b54be589072e605596b6f20b0c56c5230b460cc"
+dependencies = [
+ "chrono",
+ "derive_more",
+ "semver",
+ "serde",
+]
+
+[[package]]
+name = "build-info-proc"
+version = "0.0.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffd5f241ddd417436c48d35da9869480891449ddd1ae3fd483bbcfbae741a422"
+dependencies = [
+ "anyhow",
+ "base64 0.21.2",
+ "bincode",
+ "build-info-common",
+ "chrono",
+ "num-bigint",
+ "num-traits",
+ "proc-macro-error",
+ "proc-macro2",
+ "quote",
+ "serde_json",
+ "syn 2.0.18",
+ "xz2",
+]
+
+[[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "byte-fmt"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "abe",
  "base64 0.21.2",
  "bytemuck",
  "ruint",
  "serde",
  "serde_bytes",
@@ -363,15 +437,15 @@
 name = "bytemuck_derive"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
@@ -379,26 +453,74 @@
 [[package]]
 name = "bytes"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4872d67bab6358e59559027aa3b9157c53d9358c51423c17554809a8858e0f8"
 
 [[package]]
+name = "camino"
+version = "1.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c530edf18f37068ac2d977409ed5cd50d53d73bc653c7647b48eb78976ac9ae2"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "cargo-platform"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cbdb825da8a5df079a43676dbe042702f1707b1109f713a01420fbb4cc71fa27"
+dependencies = [
+ "serde",
+]
+
+[[package]]
+name = "cargo_metadata"
+version = "0.15.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eee4243f1f26fc7a42710e7439c149e2b10b05472f88090acce52632f231a73a"
+dependencies = [
+ "camino",
+ "cargo-platform",
+ "semver",
+ "serde",
+ "serde_json",
+ "thiserror",
+]
+
+[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+dependencies = [
+ "jobserver",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "chrono"
+version = "0.4.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
+dependencies = [
+ "android-tzdata",
+ "iana-time-zone",
+ "num-traits",
+ "serde",
+ "winapi",
+]
+
+[[package]]
 name = "clap"
 version = "4.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80672091db20273a15cf9fdd4e47ed43b5091ec9841bf4c6145c9dfbbcae09ed"
 dependencies = [
  "clap_builder",
  "clap_derive",
@@ -409,29 +531,29 @@
 name = "clap_builder"
 version = "4.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1458a1df40e1e2afebb7ab60ce55c1fa8f431146205aa5f4887e0b111c27636"
 dependencies = [
  "anstream",
  "anstyle",
- "bitflags 1.3.2",
+ "bitflags",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
 version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
@@ -449,17 +571,17 @@
 checksum = "62ec6771ecfa0762d24683ee5a32ad78487a3d3afdc0fb8cae19d2c5deb50b7c"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "const-oid"
-version = "0.9.3"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6340df57935414636969091153f35f68d9f00bbc8fb4a9c6054706c213e6c6bc"
+checksum = "520fbf3c07483f94e3e3ca9d0cfd913d7718ef2483d2cfd91c0d9e91474ab913"
 
 [[package]]
 name = "constant_time_eq"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "245097e9a4535ee1e3e3931fcfcd55a796a44c643e8596ff6566d68f09b87bbc"
 
@@ -472,14 +594,20 @@
 [[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
+name = "core-foundation-sys"
+version = "0.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+
+[[package]]
 name = "cpufeatures"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
@@ -522,18 +650,28 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
+name = "ctor"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
+dependencies = [
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "der"
-version = "0.7.7"
+version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c7ed52955ce76b1554f509074bb357d3fb8ac9b51288a65a3fd480d1dfba946"
+checksum = "56acb310e15652100da43d130af8d97b509e95af61aab1c5a7939ef24337ee17"
 dependencies = [
  "const-oid",
  "zeroize",
 ]
 
 [[package]]
 name = "derive_more"
@@ -545,14 +683,20 @@
  "proc-macro2",
  "quote",
  "rustc_version",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "diff"
+version = "0.1.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
+
+[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "const-oid",
@@ -660,14 +804,23 @@
  "cfg-if",
  "libc",
  "redox_syscall 0.2.16",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "form_urlencoded"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+dependencies = [
+ "percent-encoding",
+]
+
+[[package]]
 name = "fsevent-sys"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76ee7a02da4d231650c7cea31349b889be2f45ddb3ef3032d2ec8185f6313fd2"
 dependencies = [
  "libc",
 ]
@@ -749,15 +902,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -805,17 +958,17 @@
  "typenum",
  "version_check",
  "zeroize",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -823,14 +976,33 @@
 [[package]]
 name = "gimli"
 version = "0.27.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
 
 [[package]]
+name = "git2"
+version = "0.17.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b989d6a7ca95a362cf2cfc5ad688b3a467be1f87e480b8dad07fee8c79b0044"
+dependencies = [
+ "bitflags",
+ "libc",
+ "libgit2-sys",
+ "log",
+ "url",
+]
+
+[[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "gloo-timers"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b995a66bb87bebce9a0f4a95aed01daca4872c050bfcb21653361c03bc35e5c"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -873,26 +1045,59 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.57"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
+name = "idna"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inotify"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8069d3ec154eb856955c1c0fbffefbf5f3c40a104ec912d4797314c1801abff"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "inotify-sys",
  "libc",
 ]
 
 [[package]]
 name = "inotify-sys"
 version = "0.1.5"
@@ -908,46 +1113,65 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "io-lifetimes"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "ipcbus"
 version = "0.1.0"
 dependencies = [
- "anyhow",
  "event-listener",
  "fslock",
  "futures",
  "libc",
- "memmap2",
  "nix",
  "socket2",
  "tracing",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.8"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi",
+ "io-lifetimes",
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
+name = "jobserver"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "js-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
@@ -978,201 +1202,226 @@
 
 [[package]]
 name = "kqueue-sys"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8367585489f01bc55dd27404dcf56b95e6da061a256a666ab23be9ba96a2e587"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "libc",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.147"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+
+[[package]]
+name = "libgit2-sys"
+version = "0.15.2+1.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a80df2e11fb4a61f4ba2ab42dbe7f74468da143f1a75c74e11dee7c813f694fa"
+dependencies = [
+ "cc",
+ "libc",
+ "libz-sys",
+ "pkg-config",
+]
+
+[[package]]
+name = "libz-sys"
+version = "1.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+ "vcpkg",
+]
 
 [[package]]
 name = "linkspace"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
  "backtrace",
+ "build-info",
+ "build-info-build",
  "linkspace-common",
  "tracing",
 ]
 
 [[package]]
 name = "linkspace-argon2-identity"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "base64 0.21.2",
  "linkspace-cryptography",
  "rust-argon2",
  "thiserror",
 ]
 
 [[package]]
 name = "linkspace-cli"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
+ "build-info",
+ "build-info-build",
  "crossbeam-channel",
  "either",
  "linkspace",
  "linkspace-common",
- "memmap2",
+ "memmap2 0.6.2",
  "serde_json",
  "tracing",
  "tracing-subscriber",
- "vergen",
 ]
 
 [[package]]
 name = "linkspace-common"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "abe",
  "anyhow",
  "async_executors",
  "byte-fmt",
  "clap",
  "either",
  "futures",
  "linkspace-argon2-identity",
  "linkspace-core",
  "linkspace-pkt",
- "memmap2",
+ "memmap2 0.5.10",
  "notify",
  "rand",
  "rand_chacha",
  "rpassword",
  "serde",
  "thiserror",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "linkspace-core"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
  "arrayvec",
  "dunce",
  "either",
  "ipcbus",
  "libc",
  "linkspace-cryptography",
  "linkspace-pkt",
  "lmdb-rkv",
  "lmdb-rkv-sys",
  "parse-display",
  "serde",
- "smallvec",
  "thiserror",
  "time",
  "tracing",
 ]
 
 [[package]]
 name = "linkspace-cryptography"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "blake3",
  "getrandom",
  "k256",
  "rand",
  "rand_chacha",
  "rand_core",
  "thiserror",
 ]
 
 [[package]]
 name = "linkspace-handshake"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "linkspace",
  "linkspace-common",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "linkspace-lns"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "linkspace",
  "linkspace-common",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "linkspace-pkt"
-version = "0.3.0-rc2"
+version = "0.3.0-rc1"
 dependencies = [
  "anyhow",
  "arrayvec",
  "auto_impl",
  "bincode",
- "bitflags 1.3.2",
+ "bitflags",
  "bstr",
  "byte-fmt",
  "bytes",
  "linkspace-cryptography",
  "serde",
  "serde_json",
  "static_assertions",
  "thiserror",
  "triomphe",
- "vergen",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "linkspace-py"
-version = "0.3.0"
+version = "0.3.0-rc2"
 dependencies = [
  "anyhow",
  "linkspace",
- "linkspace-pkt",
  "pyo3",
  "smallvec",
  "tracing",
  "tracing-subscriber",
- "vergen",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.3"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lmdb-rkv"
-version = "0.15.1"
-source = "git+https://github.com/AntonSol919/lmdb-rs#5c0e86e3e169c00e48c8849a38702e9137b3521a"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "447a296f7aca299cfbb50f4e4f3d49451549af655fb7215d7f8c0c3d64bad42b"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "byteorder",
  "libc",
  "lmdb-rkv-sys",
 ]
 
 [[package]]
 name = "lmdb-rkv-sys"
-version = "0.15.1"
-source = "git+https://github.com/AntonSol919/lmdb-rs#5c0e86e3e169c00e48c8849a38702e9137b3521a"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "61b9ce6b3be08acefa3003c57b7565377432a89ec24476bbe72e11d101f852fe"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
@@ -1188,14 +1437,25 @@
 [[package]]
 name = "log"
 version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
+name = "lzma-sys"
+version = "0.1.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5fda04ab3764e6cde78b9974eec4f779acaba7c4e84b36eca3cf77c581b85d27"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+]
+
+[[package]]
 name = "matchers"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
  "regex-automata",
 ]
@@ -1204,44 +1464,53 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
-version = "0.7.1"
+version = "0.5.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
+checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "memmap2"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d28bba84adfe6646737845bc5ebbfa2c08424eb1c37e94a1fd2a82adb56a872"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.8"
@@ -1252,33 +1521,31 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "nix"
-version = "0.26.2"
+version = "0.24.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
+checksum = "fa52e972a9a719cecb6864fb88568781eb706bac2cd1d4f04a648542dbf78069"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "cfg-if",
  "libc",
- "memoffset 0.7.1",
- "pin-utils",
- "static_assertions",
+ "memoffset 0.6.5",
 ]
 
 [[package]]
 name = "notify"
 version = "5.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "729f63e1ca555a43fe3efa4f3efdf4801c479da85b432242a7b726f353c88486"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "crossbeam-channel",
  "filetime",
  "fsevent-sys",
  "inotify",
  "kqueue",
  "libc",
  "mio",
@@ -1293,29 +1560,68 @@
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
+name = "num-bigint"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
+name = "num-traits"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "object"
-version = "0.31.1"
+version = "0.30.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+checksum = "03b4680b86d9cfafba8fc491dc9b6df26b68cf40e9e6cd73909194759a63c385"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
+name = "output_vt100"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "628223faebab4e3e40667ee0b2336d34a5b960ff60ea743ddfdbcf7770bcfb66"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "parking"
@@ -1339,15 +1645,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall 0.3.5",
  "smallvec",
- "windows-targets 0.48.1",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "parse-display"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b25af4ef94a8528b41fb49a696e361dc6ef975c782417268072d987ac327964"
@@ -1369,31 +1675,37 @@
  "regex",
  "regex-syntax 0.6.29",
  "structmeta",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "percent-encoding"
+version = "2.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+
+[[package]]
 name = "pin-project"
-version = "1.1.1"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e138fdd8263907a2b0e1b4e80b7e58c721126479b6e6eedfb1b402acea7b9bd"
+checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.1"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1fef411b303e3e12d534fb6e7852de82da56edd937d895125821fb7c09436c7"
+checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -1423,14 +1735,26 @@
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "pretty_assertions"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a25e9bcb20aa780fd0bb16b72403a9064d6b3f22f026946029acb941a50af755"
+dependencies = [
+ "ctor",
+ "diff",
+ "output_vt100",
+ "yansi",
+]
+
+[[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
@@ -1448,88 +1772,88 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.63"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.9.0",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.29"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1562,24 +1886,24 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "regex"
 version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
@@ -1683,32 +2007,27 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.1"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbc6396159432b5c8490d4e301d8c705f61860b8b6c863bf79942ce5401968f3"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
- "bitflags 2.3.3",
+ "bitflags",
  "errno",
+ "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "rustversion"
-version = "1.0.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
-
-[[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
@@ -1740,14 +2059,17 @@
 ]
 
 [[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "send_wrapper"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f638d531eccd6e23b980caf34876660d38e265409d8e99b397ab71eb3612fad0"
 
@@ -1773,22 +2095,22 @@
 name = "serde_derive"
 version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1912,17 +2234,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.22"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1944,15 +2266,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -1985,34 +2307,49 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
+]
+
+[[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
  "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.26"
+version = "0.1.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
+checksum = "8803eee176538f94ae9a14b55b2804eb7e1441f8210b1c31290b3bccdccff73b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -2062,48 +2399,68 @@
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
+name = "unicode-bidi"
+version = "0.3.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
+name = "unicode-normalization"
+version = "0.1.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+dependencies = [
+ "tinyvec",
+]
+
+[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "url"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
+dependencies = [
+ "form_urlencoded",
+ "idna",
+ "percent-encoding",
+]
+
+[[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
 [[package]]
-name = "vergen"
-version = "8.2.1"
+name = "vcpkg"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b3c89c2c7e50f33e4d35527e5bf9c11d6d132226dbbd1753f0fbe9f19ef88c6"
-dependencies = [
- "anyhow",
- "rustc_version",
- "rustversion",
- "time",
-]
+checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
@@ -2146,15 +2503,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2180,15 +2537,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.22",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -2233,29 +2590,38 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.1",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
@@ -2267,17 +2633,17 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm 0.48.0",
  "windows_aarch64_msvc 0.48.0",
  "windows_i686_gnu 0.48.0",
  "windows_i686_msvc 0.48.0",
  "windows_x86_64_gnu 0.48.0",
  "windows_x86_64_gnullvm 0.48.0",
@@ -2365,11 +2731,26 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
+name = "xz2"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "388c44dc09d76f1536602ead6d325eb532f5c122f17782bd57fb47baeeb767e2"
+dependencies = [
+ "lzma-sys",
+]
+
+[[package]]
+name = "yansi"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09041cd90cf85f7f8b2df60c646f853b7f535ce68f85244eb6731cf89fa498ec"
+
+[[package]]
 name = "zeroize"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
```

### Comparing `linkspace-0.3.0/PKG-INFO` & `linkspace-0.3.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkspace
-Version: 0.3.0
+Version: 0.3.0rc2
 Home-Page: https://www.linkspace.dev
 Author: Anton Sol <AntonSol919@gmail.com>
 Author-email: Anton Sol <AntonSol919@gmail.com>
 License: MPL-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/AntonSol919/linkspace
```

