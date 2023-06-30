# Comparing `tmp/unified_planning-0.6.0.94.dev1.tar.gz` & `tmp/unified_planning-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified_planning-0.6.0.94.dev1.tar", last modified: Tue May 30 12:39:20 2023, max compression
+gzip compressed data, was "unified_planning-1.0.0.tar", last modified: Fri Jun 30 14:36:32 2023, max compression
```

## Comparing `unified_planning-0.6.0.94.dev1.tar` & `unified_planning-1.0.0.tar`

### file list

```diff
@@ -1,361 +1,376 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.343699 unified_planning-0.6.0.94.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 12:39:20.343699 unified_planning-0.6.0.94.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:39:20.343699 unified_planning-0.6.0.94.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.239698 unified_planning-0.6.0.94.dev1/unified_planning/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.247698 unified_planning-0.6.0.94.dev1/unified_planning/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.251698 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17039 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/state_invariants_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    20529 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/credits.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    48097 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/meta_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.251698 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/oneshot_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/plan_repairer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/oversubscription_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/pddl_anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19891 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    34287 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.255698 unified_planning-0.6.0.94.dev1/unified_planning/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.255698 unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36383 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34146 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/proto_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    34502 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/proto_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.255698 unified_planning-0.6.0.94.dev1/unified_planning/interop/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/interop/from_tarski.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/interop/to_tarski.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.259698 unified_planning-0.6.0.94.dev1/unified_planning/io/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/anml_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)    41213 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    37842 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/ma_pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    75013 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/pddl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    37231 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.263698 unified_planning-0.6.0.94.dev1/unified_planning/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    28405 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/contingent_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/delta_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/fnode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.267698 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/hierarchical_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/task_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.267698 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/actions_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/agents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/fluents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/initial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/objects_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/time_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/timed_conds_effs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/user_types_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.271698 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/ma_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/ma_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    40918 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/problem_kind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.271698 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/chronicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/scheduling_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.271698 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/type_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.279698 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/any.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/fluents_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/free_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/linear_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/names_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/operators_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/quantifier_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/state_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.283698 unified_planning-0.6.0.94.dev1/unified_planning/plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/contingent_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/hierarchical_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/sequential_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/time_triggered_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    30667 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.295699 unified_planning-0.6.0.94.dev1/unified_planning/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.299699 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/basic.anml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/basic_conditional.anml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/connected_locations.anml
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/constants.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/durative_goals.anml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/forall.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/hydrone.anml
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match.anml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match_int_id.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match_test_parser.anml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/simple_mais.anml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/tils.anml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.235698 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.299699 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.299699 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.303699 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/minimals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    39048 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/realistic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    37275 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/testing_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.239698 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.303699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.303699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.307699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-PCP/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.307699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.307699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.307699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.311699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.311699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.311699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.311699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.315699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.315699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.315699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.315699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.319699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.319699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.319699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.319699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Robot/
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.327699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.327699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.327699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Towers/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.327699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.331699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.331699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.331699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.331699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/problem2.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.335699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.335699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.335699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/matchcellar/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.335699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/miconic/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/miconic/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/miconic/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.339699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/robot_fastener/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.339699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/safe_road/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/safe_road/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/safe_road/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.339699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/sailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/sailing/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/sailing/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.339699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/visit_precedence/
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.343699 unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/jobshop.py
--rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_anytime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_compilers_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_contingent_pddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_credits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_expression_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_htn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_infix_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    33608 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_pddl_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    25081 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_protobuf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_pyperplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_quantifier_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_simulated_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_state_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_tarski_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_trajectory_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.243698 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 12:39:19.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-05-30 12:39:20.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:39:19.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-30 12:39:19.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 12:39:19.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 14:36:29.000000 unified_planning-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 14:36:29.000000 unified_planning-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 14:36:32.167109 unified_planning-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-30 14:36:29.000000 unified_planning-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:36:32.167109 unified_planning-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-30 14:36:29.000000 unified_planning-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.139109 unified_planning-1.0.0/unified_planning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.139109 unified_planning-1.0.0/unified_planning/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/cmd/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/cmd/up.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.143109 unified_planning-1.0.0/unified_planning/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.143109 unified_planning-1.0.0/unified_planning/engines/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/state_invariants_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/compilers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48598 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/meta_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.143109 unified_planning-1.0.0/unified_planning/engines/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/oneshot_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/plan_repairer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/mixins/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/oversubscription_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/pddl_anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18248 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35416 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/engines/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.143109 unified_planning-1.0.0/unified_planning/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/grpc/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.143109 unified_planning-1.0.0/unified_planning/grpc/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/grpc/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/grpc/generated/unified_planning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/grpc/proto_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38783 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/grpc/proto_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.147109 unified_planning-1.0.0/unified_planning/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/interop/from_tarski.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18068 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/interop/to_tarski.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.147109 unified_planning-1.0.0/unified_planning/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/io/anml_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41471 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/io/anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/io/anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39290 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/io/ma_pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77329 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/io/pddl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40589 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/io/pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.147109 unified_planning-1.0.0/unified_planning/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29564 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/contingent_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/delta_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18666 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28717 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/fnode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.147109 unified_planning-1.0.0/unified_planning/model/htn/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/htn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/htn/hierarchical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/htn/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/htn/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/htn/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/htn/task_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13510 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.151109 unified_planning-1.0.0/unified_planning/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/actions_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/agents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/fluents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/initial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/objects_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/time_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/timed_conds_effs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/mixins/user_types_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.151109 unified_planning-1.0.0/unified_planning/model/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/multi_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/multi_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/multi_agent/ma_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19329 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/multi_agent/ma_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/problem_kind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.151109 unified_planning-1.0.0/unified_planning/model/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/scheduling/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/scheduling/chronicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/scheduling/scheduling_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.151109 unified_planning-1.0.0/unified_planning/model/tamp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/tamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/tamp/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/tamp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/tamp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/tamp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.151109 unified_planning-1.0.0/unified_planning/model/walkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/expression_quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/fluents_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/free_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/linear_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/names_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/operators_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/quantifier_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17069 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/state_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24752 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/model/walkers/usertype_fluents_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.155109 unified_planning-1.0.0/unified_planning/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/contingent_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/hierarchical_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/sequential_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plans/time_triggered_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.155109 unified_planning-1.0.0/unified_planning/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plot/causal_graph_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31499 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plot/plan_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30679 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.159109 unified_planning-1.0.0/unified_planning/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.159109 unified_planning-1.0.0/unified_planning/test/anml/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/basic.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/basic_conditional.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/connected_locations.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/constants.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/constants_no_variable_duration.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/durative_goals.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/forall.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/hierarchical_blocks_world.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/hydrone.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/match.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/match_int_id.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/match_test_parser.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/simple_mais.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/anml/tils.anml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.131109 unified_planning-1.0.0/unified_planning/test/contingent_pddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.159109 unified_planning-1.0.0/unified_planning/test/contingent_pddl/colorballs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/contingent_pddl/colorballs/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/contingent_pddl/colorballs/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.159109 unified_planning-1.0.0/unified_planning/test/contingent_pddl/logistic_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.159109 unified_planning-1.0.0/unified_planning/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14619 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/minimals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/realistic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.159109 unified_planning-1.0.0/unified_planning/test/examples/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/scheduling/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/scheduling/jobshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37280 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/examples/testing_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.139109 unified_planning-1.0.0/unified_planning/test/hddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.159109 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.159109 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-PCP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-PCP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Rover/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Rover/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Satellite/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Childsnack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Depots/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Depots/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Factories-simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Hiking/
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Player/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Regular/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Robot/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.163109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Rover-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Snake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Snake/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Towers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Towers/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Woodworking/
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/citycar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/citycar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/citycar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/counters/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/counters/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/counters/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/counters/problem2.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/depot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/depot/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/depot/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/htn-transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/htn-transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/htn-transport/problem.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/matchcellar/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/matchcellar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/matchcellar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/miconic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/miconic/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/miconic/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/robot_fastener/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/robot_fastener/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/robot_fastener/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/safe_road/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/safe_road/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/safe_road/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/sailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/sailing/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/sailing/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.167109 unified_planning-1.0.0/unified_planning/test/pddl/visit_precedence/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/visit_precedence/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/pddl/visit_precedence/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    27054 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_anytime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_compilers_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_contingent_pddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_expression_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17057 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_htn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_infix_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_ma_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_ma_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34650 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_pddl_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18899 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_protobuf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_pyperplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_quantifier_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25431 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_simulated_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_state_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_tarski_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_trajectory_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-30 14:36:29.000000 unified_planning-1.0.0/unified_planning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:36:32.139109 unified_planning-1.0.0/unified_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 14:36:31.000000 unified_planning-1.0.0/unified_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-06-30 14:36:32.000000 unified_planning-1.0.0/unified_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:36:31.000000 unified_planning-1.0.0/unified_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-30 14:36:31.000000 unified_planning-1.0.0/unified_planning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-30 14:36:31.000000 unified_planning-1.0.0/unified_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 14:36:31.000000 unified_planning-1.0.0/unified_planning.egg-info/top_level.txt
```

### Comparing `unified_planning-0.6.0.94.dev1/LICENSE` & `unified_planning-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/PKG-INFO` & `unified_planning-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: unified_planning
-Version: 0.6.0.94.dev1
+Version: 1.0.0
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
-Description: UNKNOWN
+Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: grpc
 Provides-Extra: tarski
 Provides-Extra: pyperplan
 Provides-Extra: tamer
 Provides-Extra: enhsp
 Provides-Extra: fast-downward
 Provides-Extra: lpg
 Provides-Extra: fmap
 Provides-Extra: aries
 Provides-Extra: symk
 Provides-Extra: engines
+Provides-Extra: plot
```

### Comparing `unified_planning-0.6.0.94.dev1/README.md` & `unified_planning-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # The AIPlan4EU Unified Planning Library
 
-[![Actions Status](https://github.com/aiplan4eu/unified-planning/actions/workflows/main.yml/badge.svg)](https://github.com/aiplan4eu/unified-planning/actions)
+[![Actions Status](https://github.com/aiplan4eu/unified-planning/actions/workflows/release.yml/badge.svg)](https://github.com/aiplan4eu/unified-planning/actions)
 [![Coverage Status](https://codecov.io/gh/aiplan4eu/unified-planning/branch/master/graph/badge.svg?token=GBM7HYNDRB)](https://codecov.io/gh/aiplan4eu/unified-planning)
 [![Documentation Status](https://readthedocs.org/projects/unified-planning/badge/?version=latest)](https://unified-planning.readthedocs.io/en/latest/)
 [![PyPI version](https://badge.fury.io/py/unified-planning.svg)](https://pypi.python.org/pypi/unified-planning)
 
 The unified_planning library makes it easy to formulate planning problems and to invoke automated planners.
 
 * Define problems in a *simple*, *intuitive*, and *planner independent* way
```

### Comparing `unified_planning-0.6.0.94.dev1/setup.py` & `unified_planning-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages  # type: ignore
 import unified_planning
 
 
-long_description = """============================================================
- Unified planning: A library that unifies planning frameworks
- ============================================================
-    Insert long description here
-"""
+long_description = "Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners."
 
 setup(
     name="unified_planning",
     version=unified_planning.__version__,
     description="Unified Planning Framework",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author="AIPlan4EU Project",
     author_email="aiplan4eu@fbk.eu",
     url="https://www.aiplan4eu-project.eu",
     packages=find_packages(),
     include_package_data=True,
-    python_requires=">=3.7",  # supported Python ranges
+    python_requires=">=3.8",
     install_requires=["pyparsing", "networkx"],
     extras_require={
         "dev": ["tarski[arithmetic]", "pytest", "pytest-cov", "mypy"],
         "grpc": ["grpcio", "grpcio-tools", "grpc-stubs"],
         "tarski": ["tarski[arithmetic]"],
-        "pyperplan": ["up-pyperplan==0.3.0.4.dev1"],
-        "tamer": ["up-tamer==0.3.1.26.dev1"],
-        "enhsp": ["up-enhsp==0.0.13"],
-        "fast-downward": ["up-fast-downward==0.2.1"],
-        "lpg": ["up-lpg==0.0.6.3"],
-        "fmap": ["up-fmap==0.0.6"],
+        "pyperplan": ["up-pyperplan==1.0.0"],
+        "tamer": ["up-tamer==1.0.0"],
+        "enhsp": ["up-enhsp==0.0.15"],
+        "fast-downward": ["up-fast-downward==0.2.3"],
+        "lpg": ["up-lpg==0.0.7"],
+        "fmap": ["up-fmap==0.0.7"],
         "aries": ["up-aries>=0.0.8"],
         "symk": ["up-symk>=0.0.3"],
         "engines": [
             "tarski[arithmetic]",
-            "up-pyperplan==0.3.0.4.dev1",
-            "up-tamer==0.3.1.26.dev1",
-            "up-enhsp==0.0.13",
-            "up-fast-downward==0.2.1",
-            "up-lpg==0.0.6.3",
-            "up-fmap==0.0.6",
+            "up-pyperplan==1.0.0",
+            "up-tamer==1.0.0",
+            "up-enhsp==0.0.15",
+            "up-fast-downward==0.2.3",
+            "up-lpg==0.0.7",
+            "up-fmap==0.0.7",
             "up-aries>=0.0.8",
             "up-symk>=0.0.3",
         ],
+        "plot": ["plotly", "matplotlib", "kaleido", "pygraphviz", "pandas"],
     },
     license="APACHE",
     keywords="planning logic STRIPS RDDL",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
+    entry_points={
+        "console_scripts": [
+            "up = unified_planning.cmd.up:main",
+        ],
+    },
 )
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/__init__.py` & `unified_planning-1.0.0/unified_planning/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,15 +22,15 @@
 if TYPE_CHECKING:
     # can't actually subclass Any at runtime
     AnyBaseClass = Any
 else:
     AnyBaseClass = object
 
 
-VERSION: Tuple[Union[int, str], ...] = (0, 6, 0)
+VERSION: Tuple[Union[int, str], ...] = (1, 0, 0)
 __version__ = ".".join(str(x) for x in VERSION)
 
 # Try to provide human-readable version of latest commit for dev versions
 # E.g. v0.5.1-4-g49a49f2-wip
 #      * 4 commits after tag v0.5.1
 #      * Latest commit "49a49f2"
 #      * -wip: Working tree is dirty (non committed stuff)
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/__init__.py` & `unified_planning-1.0.0/unified_planning/engines/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/__init__.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/bounded_types_remover.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/bounded_types_remover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -81,16 +81,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/compilers_pipeline.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/compilers_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/conditional_effects_remover.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/conditional_effects_remover.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,23 +20,30 @@
 from unified_planning.engines.mixins.compiler import CompilationKind, CompilerMixin
 from unified_planning.engines.compilers.utils import updated_minimize_action_costs
 from unified_planning.engines.results import CompilerResult
 from unified_planning.exceptions import (
     UPProblemDefinitionError,
     UPConflictingEffectsException,
 )
-from unified_planning.model import Problem, ProblemKind
+from unified_planning.model import (
+    Problem,
+    ProblemKind,
+    Action,
+    InstantaneousAction,
+    DurativeAction,
+    AbstractProblem,
+)
 from unified_planning.engines.compilers.utils import (
     get_fresh_name,
     check_and_simplify_preconditions,
     check_and_simplify_conditions,
     replace_action,
 )
 from unified_planning.utils import powerset
-from typing import List, Dict, Tuple, Optional
+from typing import List, Dict, Tuple, Optional, Iterator
 from functools import partial
 
 
 class ConditionalEffectsRemover(engines.engine.Engine, CompilerMixin):
     """
     Conditional effects remover class: this class offers the capability
     to transform a :class:`~unified_planning.model.Problem` with conditional :class:`Effects <unified_planning.model.Effect>`
@@ -89,16 +96,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
@@ -162,121 +172,30 @@
             for e in el:
                 if e.is_conditional():
                     f, v = e.fluent.fluent(), e.value
                     if not f.type.is_bool_type():
                         raise UPProblemDefinitionError(
                             f"The condition of effect: {e}\ncould not be removed without changing the problem."
                         )
-                    else:
-                        em = env.expression_manager
-                        c = e.condition
-                        nv = simplifier.simplify(
-                            em.Or(em.And(c, v), em.And(em.Not(c), f))
-                        )
-                        new_problem.add_timed_effect(t, e.fluent, nv)
+                    em = env.expression_manager
+                    c = e.condition
+                    nv = simplifier.simplify(em.Or(em.And(c, v), em.And(em.Not(c), f)))
+                    new_problem.add_timed_effect(t, e.fluent, nv, forall=e.forall)
                 else:
                     new_problem._add_effect_instance(t, e.clone())
+
         new_problem.clear_actions()
         for ua in problem.unconditional_actions:
             new_uncond_action = ua.clone()
             new_problem.add_action(new_uncond_action)
             new_to_old[new_uncond_action] = ua
         for action in problem.conditional_actions:
-            if isinstance(action, up.model.InstantaneousAction):
-                cond_effects = action.conditional_effects
-                for p in powerset(range(len(cond_effects))):
-                    new_action = action.clone()
-                    new_action.name = get_fresh_name(new_problem, action.name)
-                    new_action.clear_effects()
-                    for e in action.unconditional_effects:
-                        new_action._add_effect_instance(e.clone())
-                    for i, e in enumerate(cond_effects):
-                        if i in p:
-                            # positive precondition
-                            new_action.add_precondition(e.condition)
-                            ne = up.model.Effect(
-                                e.fluent,
-                                e.value,
-                                env.expression_manager.TRUE(),
-                                e.kind,
-                            )
-                            # We try to add the new effect, but it might be in conflict with exising effects,
-                            # so the action is not added to the problem
-                            try:
-                                new_action._add_effect_instance(ne)
-                            except UPConflictingEffectsException:
-                                continue
-                        else:
-                            # negative precondition
-                            new_action.add_precondition(
-                                env.expression_manager.Not(e.condition)
-                            )
-                    # new action is created, then is checked if it has any impact and if it can be simplified
-                    if len(new_action.effects) > 0:
-                        (
-                            action_is_feasible,
-                            simplified_preconditions,
-                        ) = check_and_simplify_preconditions(
-                            new_problem, new_action, simplifier
-                        )
-                        if action_is_feasible:
-                            new_action._set_preconditions(simplified_preconditions)
-                            new_to_old[new_action] = action
-                            new_problem.add_action(new_action)
-            elif isinstance(action, up.model.DurativeAction):
-                timing_cond_effects: Dict[
-                    "up.model.Timing", List["up.model.Effect"]
-                ] = action.conditional_effects
-                cond_effects_timing: List[
-                    Tuple["up.model.Effect", "up.model.Timing"]
-                ] = [(e, t) for t, el in timing_cond_effects.items() for e in el]
-                for p in powerset(range(len(cond_effects_timing))):
-                    new_action = action.clone()
-                    new_action.name = get_fresh_name(new_problem, action.name)
-                    new_action.clear_effects()
-                    for t, el in action.unconditional_effects.items():
-                        for e in el:
-                            new_action._add_effect_instance(t, e.clone())
-                    for i, (e, t) in enumerate(cond_effects_timing):
-                        if i in p:
-                            # positive precondition
-                            new_action.add_condition(t, e.condition)
-                            ne = up.model.Effect(
-                                e.fluent,
-                                e.value,
-                                env.expression_manager.TRUE(),
-                                e.kind,
-                            )
-                            # We try to add the new effect, but it might be in conflict with exising effects,
-                            # so the action is not added to the problem
-                            try:
-                                new_action._add_effect_instance(t, ne)
-                            except UPConflictingEffectsException:
-                                continue
-                        else:
-                            # negative precondition
-                            new_action.add_condition(
-                                t, env.expression_manager.Not(e.condition)
-                            )
-                    # new action is created, then is checked if it has any impact and if it can be simplified
-                    if len(new_action.effects) > 0:
-                        (
-                            action_is_feasible,
-                            simplified_conditions,
-                        ) = check_and_simplify_conditions(
-                            new_problem, new_action, simplifier
-                        )
-                        if action_is_feasible:
-                            new_action.clear_conditions()
-                            for interval, c in simplified_conditions:
-                                new_action.add_condition(interval, c)
-                            new_to_old[new_action] = action
-                            new_problem.add_action(new_action)
-            else:
-                raise NotImplementedError
+            for new_action in self._create_unconditional_actions(action, new_problem):
+                new_to_old[new_action] = action
+                new_problem.add_action(new_action)
 
         new_problem.clear_quality_metrics()
         for qm in problem.quality_metrics:
             if qm.is_minimize_action_costs():
                 new_problem.add_quality_metric(
                     updated_minimize_action_costs(
                         qm, new_to_old, new_problem.environment
@@ -284,7 +203,111 @@
                 )
             else:
                 new_problem.add_quality_metric(qm)
 
         return CompilerResult(
             new_problem, partial(replace_action, map=new_to_old), self.name
         )
+
+    def _create_unconditional_actions(
+        self, action: Action, new_problem: AbstractProblem
+    ) -> Iterator[Action]:
+        # Takes an action and the new problem and returns a sequence of actions
+        # that must be added to the problem in order to maintain the same semantic
+        # removing the conditional effects.
+        assert (
+            action.is_conditional()
+        ), "This method must be called only on conditional actions"
+        env = new_problem.environment
+        simplifier = env.simplifier
+        if isinstance(action, up.model.InstantaneousAction):
+            cond_effects = action.conditional_effects
+            for p in powerset(range(len(cond_effects))):
+                new_action = action.clone()
+                new_action.name = get_fresh_name(new_problem, action.name)
+                new_action.clear_effects()
+                for e in action.unconditional_effects:
+                    new_action._add_effect_instance(e.clone())
+                for i, e in enumerate(cond_effects):
+                    if i in p:
+                        # positive precondition
+                        new_action.add_precondition(e.condition)
+                        ne = up.model.Effect(
+                            e.fluent,
+                            e.value,
+                            env.expression_manager.TRUE(),
+                            e.kind,
+                            e.forall,
+                        )
+                        # We try to add the new effect, but it might be in conflict with exising effects,
+                        # so the action is not added to the problem
+                        try:
+                            new_action._add_effect_instance(ne)
+                        except UPConflictingEffectsException:
+                            continue
+                    else:
+                        # negative precondition
+                        new_action.add_precondition(
+                            env.expression_manager.Not(e.condition)
+                        )
+                # new action is created, then is checked if it has any impact and if it can be simplified
+                if len(new_action.effects) > 0:
+                    (
+                        action_is_feasible,
+                        simplified_preconditions,
+                    ) = check_and_simplify_preconditions(
+                        new_problem, new_action, simplifier
+                    )
+                    if action_is_feasible:
+                        new_action._set_preconditions(simplified_preconditions)
+                        yield new_action
+        elif isinstance(action, up.model.DurativeAction):
+            timing_cond_effects: Dict[
+                "up.model.Timing", List["up.model.Effect"]
+            ] = action.conditional_effects
+            cond_effects_timing: List[Tuple["up.model.Effect", "up.model.Timing"]] = [
+                (e, t) for t, el in timing_cond_effects.items() for e in el
+            ]
+            for p in powerset(range(len(cond_effects_timing))):
+                new_action = action.clone()
+                new_action.name = get_fresh_name(new_problem, action.name)
+                new_action.clear_effects()
+                for t, el in action.unconditional_effects.items():
+                    for e in el:
+                        new_action._add_effect_instance(t, e.clone())
+                for i, (e, t) in enumerate(cond_effects_timing):
+                    if i in p:
+                        # positive precondition
+                        new_action.add_condition(t, e.condition)
+                        ne = up.model.Effect(
+                            e.fluent,
+                            e.value,
+                            env.expression_manager.TRUE(),
+                            e.kind,
+                            e.forall,
+                        )
+                        # We try to add the new effect, but it might be in conflict with exising effects,
+                        # so the action is not added to the problem
+                        try:
+                            new_action._add_effect_instance(t, ne)
+                        except UPConflictingEffectsException:
+                            continue
+                    else:
+                        # negative precondition
+                        new_action.add_condition(
+                            t, env.expression_manager.Not(e.condition)
+                        )
+                # new action is created, then is checked if it has any impact and if it can be simplified
+                if len(new_action.effects) > 0:
+                    (
+                        action_is_feasible,
+                        simplified_conditions,
+                    ) = check_and_simplify_conditions(
+                        new_problem, new_action, simplifier
+                    )
+                    if action_is_feasible:
+                        new_action.clear_conditions()
+                        for interval, c in simplified_conditions:
+                            new_action.add_condition(interval, c)
+                        yield new_action
+        else:
+            raise NotImplementedError
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/disjunctive_conditions_remover.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,41 +10,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines the dnf remover class."""
 
-from fractions import Fraction
+
 import unified_planning as up
 import unified_planning.engines as engines
 from unified_planning.engines.mixins.compiler import CompilationKind, CompilerMixin
 from unified_planning.engines.compilers.utils import (
     get_fresh_name,
     replace_action,
     updated_minimize_action_costs,
 )
 from unified_planning.engines.results import CompilerResult
-from unified_planning.exceptions import UPProblemDefinitionError
 from unified_planning.model import (
+    AbstractProblem,
     FNode,
     Problem,
     BoolExpression,
     NumericConstant,
     InstantaneousAction,
     DurativeAction,
     TimeInterval,
     Timing,
     Action,
     ProblemKind,
     Oversubscription,
     TemporalOversubscription,
 )
 from unified_planning.model.walkers import Dnf
-from typing import List, Optional, Tuple, Dict, Union, cast
+from typing import Iterator, List, Optional, Tuple, Dict, cast
 from itertools import product
 from functools import partial
 
 
 class DisjunctiveConditionsRemover(engines.engine.Engine, CompilerMixin):
     """
     DisjunctiveConditions remover class: this class offers the capability
@@ -91,16 +91,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
@@ -154,84 +157,46 @@
         new_fluents: List["up.model.Fluent"] = []
 
         new_problem = problem.clone()
         new_problem.name = f"{self.name}_{problem.name}"
         new_problem.clear_actions()
         new_problem.clear_goals()
         new_problem.clear_timed_goals()
+        new_problem.clear_timed_effects()
         new_problem.clear_quality_metrics()
 
         dnf = Dnf(env)
         for a in problem.actions:
-            if isinstance(a, InstantaneousAction):
-                new_precond = dnf.get_dnf_expression(
-                    env.expression_manager.And(a.preconditions)
-                )
-                if new_precond.is_or():
-                    for and_exp in new_precond.args:
-                        na = self._create_new_action_with_given_precond(
-                            new_problem, and_exp, a, dnf
-                        )
-                        if na is not None:
-                            new_to_old[na] = a
-                            new_problem.add_action(na)
-                else:
-                    na = self._create_new_action_with_given_precond(
-                        new_problem, new_precond, a, dnf
-                    )
-                    if na is not None:
-                        new_to_old[na] = a
-                        new_problem.add_action(na)
-            elif isinstance(a, DurativeAction):
-                interval_list: List[TimeInterval] = []
-                conditions: List[List[FNode]] = []
-                # save the timing, calculate the dnf of the and of all the conditions at the same time
-                # and then save it in conditions.
-                # conditions contains lists of Fnodes, where [a,b,c] means a or b or c
-                for i, cl in a.conditions.items():
-                    interval_list.append(i)
-                    new_cond = dnf.get_dnf_expression(env.expression_manager.And(cl))
-                    if new_cond.is_or():
-                        conditions.append(new_cond.args)
-                    else:
-                        conditions.append([new_cond])
-                conditions_tuple = cast(Tuple[List[FNode], ...], product(*conditions))
-                for cond_list in conditions_tuple:
-                    nda = self._create_new_durative_action_with_given_conds_at_given_times(
-                        new_problem, interval_list, cond_list, a, dnf
-                    )
-                    if nda is not None:
-                        new_to_old[nda] = a
-                        new_problem.add_action(nda)
-            else:
-                raise NotImplementedError
+            for na in self._create_non_disjunctive_actions(a, new_problem, dnf):
+                new_to_old[na] = a
+                new_problem.add_action(na)
 
-        # Meaningful action is the list of the actions that modify fluents that are not added
-        # just to remove the disjunction from goals
+        # Meaningful action is the list of the actions that modify fluents; those actions are not
+        # added just to remove the disjunction from goals
         meaningful_actions: List["up.model.Action"] = new_problem.actions[:]
 
         goal_to_add = self._goals_without_disjunctions_adding_new_elements(
             dnf,
             new_problem,
             new_to_old,
             new_fluents,
             problem.goals,
         )
         new_problem.add_goal(goal_to_add)
 
-        for t, gl in problem.timed_goals.items():
+        for i, gl in problem.timed_goals.items():
             goal_to_add = self._goals_without_disjunctions_adding_new_elements(
                 dnf,
                 new_problem,
                 new_to_old,
                 new_fluents,
                 gl,
-                t,
+                i,
             )
-            new_problem.add_timed_goal(t, goal_to_add)
+            new_problem.add_timed_goal(i, goal_to_add)
 
         # Every meaningful action must set to False every new fluent added.
         # For the DurativeActions this must happen every time the action modifies something
         em = env.expression_manager
         # new_effects is the List of effects that must be added to every meaningful action
         new_effects: List["up.model.Effect"] = [
             up.model.Effect(em.FluentExp(f), em.FALSE(), em.TRUE()) for f in new_fluents
@@ -246,14 +211,29 @@
                 for tim in a.effects:
                     for e in new_effects:
                         a._add_effect_instance(tim, e)
             else:
                 raise NotImplementedError
             new_to_old[a] = old_action
 
+        for t, el in problem.timed_effects.items():
+            for e in new_effects:
+                new_problem._add_effect_instance(t, e)
+            for e in el:
+                new_cond = dnf.get_dnf_expression(e.condition)
+                if new_cond.is_or():
+                    for arg in new_cond.args:
+                        ne = e.clone()
+                        ne.set_condition(arg)
+                        new_problem._add_effect_instance(t, ne)
+                else:
+                    ne = e.clone()
+                    ne.set_condition(new_cond)
+                    new_problem._add_effect_instance(t, ne)
+
         for qm in problem.quality_metrics:
             if qm.is_minimize_action_costs():
                 new_problem.add_quality_metric(
                     updated_minimize_action_costs(
                         qm, new_to_old, new_problem.environment
                     )
                 )
@@ -272,19 +252,19 @@
                 )
             elif qm.is_temporal_oversubscription():
                 assert isinstance(qm, TemporalOversubscription)
                 new_temporal_oversubscription: Dict[
                     Tuple["up.model.timing.TimeInterval", "up.model.BoolExpression"],
                     NumericConstant,
                 ] = {}
-                for (t, g), v in qm.goals.items():
+                for (i, g), v in qm.goals.items():
                     new_goal = self._goals_without_disjunctions_adding_new_elements(
                         dnf, new_problem, new_to_old, new_fluents, [g]
                     )
-                    new_temporal_oversubscription[(t, new_goal)] = v
+                    new_temporal_oversubscription[(i, new_goal)] = v
                 new_problem.add_quality_metric(
                     TemporalOversubscription(
                         new_temporal_oversubscription,
                         environment=new_problem.environment,
                     )
                 )
             else:
@@ -323,15 +303,15 @@
             new_fluents.append(fake_fluent)
             return env.expression_manager.FluentExp(fake_fluent)
         else:
             return new_goal
 
     def _create_new_durative_action_with_given_conds_at_given_times(
         self,
-        new_problem: "up.model.Problem",
+        new_problem: "up.model.AbstractProblem",
         interval_list: List[TimeInterval],
         cond_list: List[FNode],
         original_action: DurativeAction,
         dnf: Dnf,
     ) -> Optional[DurativeAction]:
         new_action = original_action.clone()
         new_action.name = get_fresh_name(new_problem, original_action.name)
@@ -363,15 +343,15 @@
                     new_action._add_effect_instance(t, e)
         if len(new_action.effects) == 0:
             return None
         return new_action
 
     def _create_new_action_with_given_precond(
         self,
-        new_problem: "up.model.Problem",
+        new_problem: "up.model.AbstractProblem",
         precond: FNode,
         original_action: InstantaneousAction,
         dnf: Dnf,
     ) -> Optional[InstantaneousAction]:
         new_action = original_action.clone()
         new_action.name = get_fresh_name(new_problem, original_action.name)
         new_action.clear_preconditions()
@@ -397,7 +377,51 @@
                     new_e.set_condition(new_cond)
                     new_action._add_effect_instance(new_e)
             else:
                 new_action._add_effect_instance(e)
         if len(new_action.effects) == 0:
             return None
         return new_action
+
+    def _create_non_disjunctive_actions(
+        self, action: Action, new_problem: AbstractProblem, dnf: Dnf
+    ) -> Iterator[Action]:
+        env = new_problem.environment
+        if isinstance(action, InstantaneousAction):
+            new_precond = dnf.get_dnf_expression(
+                env.expression_manager.And(action.preconditions)
+            )
+            if new_precond.is_or():
+                for and_exp in new_precond.args:
+                    na = self._create_new_action_with_given_precond(
+                        new_problem, and_exp, action, dnf
+                    )
+                    if na is not None:
+                        yield na
+            else:
+                na = self._create_new_action_with_given_precond(
+                    new_problem, new_precond, action, dnf
+                )
+                if na is not None:
+                    yield na
+        elif isinstance(action, DurativeAction):
+            interval_list: List[TimeInterval] = []
+            conditions: List[List[FNode]] = []
+            # save the timing, calculate the dnf of the and of all the conditions at the same time
+            # and then save it in conditions.
+            # conditions contains lists of Fnodes, where [a,b,c] means a or b or c
+            for i, cl in action.conditions.items():
+                interval_list.append(i)
+                new_cond = dnf.get_dnf_expression(env.expression_manager.And(cl))
+                if new_cond.is_or():
+                    conditions.append(new_cond.args)
+                else:
+                    conditions.append([new_cond])
+            conditions_tuple = cast(Tuple[List[FNode], ...], product(*conditions))
+            for cond_list in conditions_tuple:
+                nda = self._create_new_durative_action_with_given_conds_at_given_times(
+                    new_problem, interval_list, cond_list, action, dnf
+                )
+                if nda is not None:
+                    yield nda
+        else:
+            raise NotImplementedError
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/grounder.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/grounder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -258,18 +258,21 @@
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/negative_conditions_remover.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/negative_conditions_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -124,16 +124,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
@@ -316,14 +319,15 @@
                         )
                         new_effects.append(
                             Effect(
                                 env.expression_manager.FluentExp(fneg, tuple(fl.args)),
                                 simplified_not_v,
                                 e.condition,
                                 e.kind,
+                                e.forall,
                             )
                         )
                 for ne in new_effects:
                     new_action._add_effect_instance(ne)
                 new_problem.add_action(new_action)
                 new_to_old[new_action] = action
             elif isinstance(action, DurativeAction):
@@ -343,14 +347,15 @@
                                 Effect(
                                     env.expression_manager.FluentExp(
                                         fneg, tuple(fl.args)
                                     ),
                                     simplified_not_v,
                                     e.condition,
                                     e.kind,
+                                    e.forall,
                                 ),
                             )
                 new_problem.add_action(new_durative_action)
                 new_to_old[new_durative_action] = action
             else:
                 raise NotImplementedError
 
@@ -365,13 +370,14 @@
                     new_problem._add_effect_instance(
                         t,
                         Effect(
                             env.expression_manager.FluentExp(fneg, tuple(fl.args)),
                             simplified_not_v,
                             e.condition,
                             e.kind,
+                            e.forall,
                         ),
                     )
 
         return CompilerResult(
             new_problem, partial(replace_action, map=new_to_old), self.name
         )
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/quantifiers_remover.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/quantifiers_remover.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,34 +11,39 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines the quantifiers remover class."""
 
 
+from itertools import product
 import unified_planning as up
 import unified_planning.engines as engines
 from unified_planning.engines.mixins.compiler import CompilationKind, CompilerMixin
 from unified_planning.engines.results import CompilerResult
 from unified_planning.model import (
     Problem,
     InstantaneousAction,
     DurativeAction,
     Action,
     ProblemKind,
     Oversubscription,
     TemporalOversubscription,
+    Object,
+    Variable,
+    Expression,
+    Effect,
 )
 from unified_planning.model.walkers import ExpressionQuantifiersRemover
 from unified_planning.engines.compilers.utils import (
     get_fresh_name,
     replace_action,
     updated_minimize_action_costs,
 )
-from typing import Dict, Optional
+from typing import Dict, List, Optional, Tuple
 from functools import partial
 
 
 class QuantifiersRemover(engines.engine.Engine, CompilerMixin):
     """
     Quantifiers remover class: this class offers the capability
     to transform a problem with quantifiers into a problem without.
@@ -91,16 +96,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
@@ -129,14 +137,17 @@
     @staticmethod
     def resulting_problem_kind(
         problem_kind: ProblemKind, compilation_kind: Optional[CompilationKind] = None
     ) -> ProblemKind:
         new_kind = ProblemKind(problem_kind.features)
         new_kind.unset_conditions_kind("EXISTENTIAL_CONDITIONS")
         new_kind.unset_conditions_kind("UNIVERSAL_CONDITIONS")
+        new_kind.unset_effects_kind("FORALL_EFFECTS")
+        if problem_kind.has_existential_conditions():
+            new_kind.set_conditions("DISJUNCTIVE_CONDITIONS")
         return new_kind
 
     def _compile(
         self,
         problem: "up.model.AbstractProblem",
         compilation_kind: "up.engines.CompilationKind",
     ) -> CompilerResult:
@@ -164,73 +175,88 @@
         new_problem.clear_goals()
         new_problem.clear_quality_metrics()
 
         for action in new_problem.actions:
             if isinstance(action, InstantaneousAction):
                 original_action = problem.action(action.name)
                 assert isinstance(original_action, InstantaneousAction)
-                action.name = get_fresh_name(new_problem, action.name)
                 action.clear_preconditions()
                 for p in original_action.preconditions:
                     action.add_precondition(
                         expression_quantifier_remover.remove_quantifiers(p, problem)
                     )
-                for e in action.effects:
-                    if e.is_conditional():
-                        e.set_condition(
+                original_effects = action.effects
+                action.clear_effects()
+                for effect in original_effects:
+                    for e in effect.expand_effect(new_problem):
+                        if e.is_conditional():
+                            e.set_condition(
+                                expression_quantifier_remover.remove_quantifiers(
+                                    e.condition, problem
+                                ).simplify()
+                            )
+                        e.set_value(
                             expression_quantifier_remover.remove_quantifiers(
-                                e.condition, problem
+                                e.value, problem
                             )
                         )
-                    e.set_value(
-                        expression_quantifier_remover.remove_quantifiers(
-                            e.value, problem
-                        )
-                    )
+                        if not e.condition.is_false():
+                            action._add_effect_instance(e)
                 new_to_old[action] = original_action
             elif isinstance(action, DurativeAction):
                 original_action = problem.action(action.name)
                 assert isinstance(original_action, DurativeAction)
-                action.name = get_fresh_name(new_problem, action.name)
                 action.clear_conditions()
                 for i, cl in original_action.conditions.items():
                     for c in cl:
                         action.add_condition(
                             i,
                             expression_quantifier_remover.remove_quantifiers(
                                 c, problem
                             ),
                         )
-                for t, el in action.effects.items():
-                    for e in el:
-                        if e.is_conditional():
-                            e.set_condition(
+                original_durative_effects = action.effects
+                action.clear_effects()
+                for t, el in original_durative_effects.items():
+                    for effect in el:
+                        for e in effect.expand_effect(new_problem):
+                            if e.is_conditional():
+                                e.set_condition(
+                                    expression_quantifier_remover.remove_quantifiers(
+                                        e.condition, problem
+                                    ).simplify()
+                                )
+                            e.set_value(
                                 expression_quantifier_remover.remove_quantifiers(
-                                    e.condition, problem
+                                    e.value, problem
                                 )
                             )
-                        e.set_value(
-                            expression_quantifier_remover.remove_quantifiers(
-                                e.value, problem
-                            )
-                        )
+                            if not e.condition.is_false():
+                                action._add_effect_instance(t, e)
                 new_to_old[action] = original_action
             else:
                 raise NotImplementedError
-        for el in new_problem.timed_effects.values():
-            for e in el:
-                if e.is_conditional():
-                    e.set_condition(
+        problem_timed_effects = new_problem.timed_effects
+        new_problem.clear_timed_effects()
+        for t, el in problem_timed_effects.items():
+            for effect in el:
+                for e in effect.expand_effect(new_problem):
+                    if e.is_conditional():
+                        e.set_condition(
+                            expression_quantifier_remover.remove_quantifiers(
+                                e.condition, problem
+                            ).simplify()
+                        )
+                    e.set_value(
                         expression_quantifier_remover.remove_quantifiers(
-                            e.condition, problem
+                            e.value, problem
                         )
                     )
-                e.set_value(
-                    expression_quantifier_remover.remove_quantifiers(e.value, problem)
-                )
+                    if not e.condition.is_false():
+                        new_problem._add_effect_instance(t, e)
         for i, gl in problem.timed_goals.items():
             for g in gl:
                 ng = expression_quantifier_remover.remove_quantifiers(g, problem)
                 new_problem.add_timed_goal(i, ng)
         for tc in problem.trajectory_constraints:
             ngc = expression_quantifier_remover.remove_quantifiers(tc, problem)
             if ngc.is_and():
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/state_invariants_remover.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/state_invariants_remover.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -69,16 +69,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/tarski_grounder.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/tarski_grounder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/trajectory_constraints_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -101,16 +101,18 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/usertype_fluents_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -96,16 +96,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
@@ -514,14 +517,15 @@
                     or positive_condition.bool_constant_value()
                 ):
                     effect = Effect(
                         resulting_effect_fluent,
                         em.TRUE(),
                         positive_condition,
                         effect.kind,
+                        effect.forall,
                     )
                     if effect not in returned_effects:
                         yield effect
                         returned_effects.add(effect)
                 negative_condition = em.And(
                     condition_to_add, em.Not(resulting_effect_value)
                 ).substitute(subs)
@@ -533,28 +537,30 @@
                     or negative_condition.bool_constant_value()
                 ):
                     effect = Effect(
                         resulting_effect_fluent,
                         em.FALSE(),
                         negative_condition,
                         effect.kind,
+                        effect.forall,
                     )
                     if effect not in returned_effects:
                         yield effect
                         returned_effects.add(effect)
             else:
                 subbed_cond = (
                     em.And(new_condition, condition_to_add).substitute(subs).simplify()
                 )
                 if not subbed_cond.is_constant() or subbed_cond.bool_constant_value():
                     effect = Effect(
                         resulting_effect_fluent,
                         resulting_effect_value,
                         subbed_cond,
                         effect.kind,
+                        effect.forall,
                     )
                     if effect not in returned_effects:
                         yield effect
                         returned_effects.add(effect)
 
     def _update_names_in_effect(self, effect: Effect, defined_names: Set[str]):
         """Important NOTE: this method adds elements to the defined_names set."""
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/utils.py` & `unified_planning-1.0.0/unified_planning/engines/compilers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,14 +36,15 @@
     TimePointInterval,
     PlanQualityMetric,
     MinimizeActionCosts,
     MinimizeExpressionOnFinalState,
     MaximizeExpressionOnFinalState,
     Oversubscription,
     TemporalOversubscription,
+    AbstractProblem,
 )
 from unified_planning.plans import ActionInstance
 from typing import (
     Callable,
     Dict,
     Iterable,
     List,
@@ -53,15 +54,15 @@
     Tuple,
     Union,
     cast,
 )
 
 
 def check_and_simplify_conditions(
-    problem: Problem, action: DurativeAction, simplifier
+    problem: AbstractProblem, action: DurativeAction, simplifier
 ) -> Tuple[bool, List[Tuple[TimeInterval, FNode]]]:
     """
     Simplifies conditions and if it is False (a contraddiction)
     returns False, otherwise returns True.
     If the simplification is True (a tautology) removes all conditions at the given timing.
     If the simplification is still an AND rewrites back every "arg" of the AND
     in the conditions
@@ -90,15 +91,15 @@
                     nac.append((i, new_cond))
             else:
                 nac.append((i, cs))
     return (True, nac)
 
 
 def check_and_simplify_preconditions(
-    problem: Problem, action: InstantaneousAction, simplifier
+    problem: AbstractProblem, action: InstantaneousAction, simplifier
 ) -> Tuple[bool, List[FNode]]:
     """
     Simplifies preconditions and if it is False (a contraddiction)
     returns False, otherwise returns True.
     If the simplification is True (a tautology) removes all preconditions.
     If the simplification is still an AND rewrites back every "arg" of the AND
     in the preconditions
@@ -137,15 +138,17 @@
 ) -> Optional[Effect]:
     new_fluent = old_effect.fluent.substitute(subs)
     new_value = old_effect.value.substitute(subs)
     new_condition = simplifier.simplify(old_effect.condition.substitute(subs))
     if new_condition == problem.environment.expression_manager.FALSE():
         return None
     else:
-        return Effect(new_fluent, new_value, new_condition, old_effect.kind)
+        return Effect(
+            new_fluent, new_value, new_condition, old_effect.kind, old_effect.forall
+        )
 
 
 def create_action_with_given_subs(
     problem: Problem,
     old_action: Action,
     simplifier,
     subs: Dict[Expression, Expression],
@@ -247,15 +250,17 @@
             new_durative_action.add_condition(interval, c)
         return new_durative_action
     else:
         raise NotImplementedError
 
 
 def get_fresh_name(
-    problem: Problem, original_name: str, parameters_names: Sequence[str] = tuple()
+    problem: AbstractProblem,
+    original_name: str,
+    parameters_names: Sequence[str] = tuple(),
 ) -> str:
     """This method returns a fresh name for the problem, given a name and an iterable of names in input."""
     name_list = [original_name]
     name_list.extend(parameters_names)
     new_name = "_".join(name_list)
     base_name = new_name
     count = 0
@@ -466,19 +471,21 @@
 
     return new_to_old
 
 
 def _apply_function_to_effect(
     effect: Effect, function: Callable[[FNode], FNode]
 ) -> Effect:
+    auto_promote = effect.environment.expression_manager.auto_promote
     return Effect(
         function(effect.fluent),
         function(effect.value),
         function(effect.condition),
         effect.kind,
+        tuple((exp.variable() for exp in auto_promote(effect.forall))),
     )
 
 
 def updated_minimize_action_costs(
     quality_metric: PlanQualityMetric,
     new_to_old: Union[Dict[Action, Action], Dict[Action, Optional[Action]]],
     environment: Environment,
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/credits.py` & `unified_planning-1.0.0/unified_planning/engines/credits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/engine.py` & `unified_planning-1.0.0/unified_planning/engines/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines the engine interface."""
 
-from unified_planning.model import ProblemKind
+from unified_planning.model.problem_kind import ProblemKind
 from unified_planning.engines.credits import Credits
 from abc import ABCMeta, abstractmethod, ABC
 from enum import Enum
 from typing import Optional
 
 
 class OperationMode(Enum):
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/factory.py` & `unified_planning-1.0.0/unified_planning/engines/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -100,14 +100,22 @@
     ),
     "fast-downward-grounder": ("up_fast_downward", "FastDownwardGrounder"),
     "fast-downward-reachability-grounder": (
         "up_fast_downward",
         "FastDownwardReachabilityGrounder",
     ),
     "up_grounder": ("unified_planning.engines.compilers.grounder", "Grounder"),
+    "up_ma_disjunctive_conditions_remover": (
+        "unified_planning.engines.compilers.ma_disjunctive_conditions_remover",
+        "MADisjunctiveConditionsRemover",
+    ),
+    "up_ma_conditional_effects_remover": (
+        "unified_planning.engines.compilers.ma_conditional_effects_remover",
+        "MAConditionalEffectsRemover",
+    ),
 }
 
 DEFAULT_META_ENGINES = {
     "oversubscription": (
         "unified_planning.engines.oversubscription_planner",
         "OversubscriptionPlanner",
     ),
@@ -129,14 +137,16 @@
     "enhsp-any",
     "tamer",
     "sequential_plan_validator",
     "sequential_simulator",
     "up_bounded_types_remover",
     "up_conditional_effects_remover",
     "up_disjunctive_conditions_remover",
+    "up_ma_disjunctive_conditions_remover",
+    "up_ma_conditional_effects_remover",
     "up_negative_conditions_remover",
     "up_quantifiers_remover",
     "up_state_invariants_remover",
     "up_usertype_fluents_remover",
     "tarski_grounder",
     "fast-downward-reachability-grounder",
     "fast-downward-grounder",
@@ -1029,27 +1039,29 @@
         for engine_name, Engine in self._engines.items():
             if (
                 operation_mode is not None
                 and not getattr(Engine, "is_" + operation_mode.value)()
             ):
                 continue
             credits = Engine.get_credits() if show_credits else None
-            stream.write("---------------------------------------\n")
-            stream.write(f"Engine's factory name: {engine_name}\n")
+            engine_name_str = f"Engine's factory name: {engine_name}\n\n"
+            stream.write("-" * (len(engine_name_str) - 2))
+            stream.write("\n")
+            stream.write(engine_name_str)
             if credits is not None:
                 credits.write_credits(stream, full_credits)
             supported_operation_modes = [
                 om.value for om in OperationMode if getattr(Engine, "is_" + om.value)()
             ]
             stream.write("Supported operation modes:\n    - ")
             stream.write("\n    - ".join(supported_operation_modes))
             stream.write("\n")
             if show_supported_kind:
                 stream.write(
-                    f"This engine supports the following features:\n{str(Engine.supported_kind())}\n"
+                    f"\nThis engine supports the following features:\n{str(Engine.supported_kind())}\n"
                 )
             stream.write("\n")
 
     def get_all_applicable_engines(
         self,
         problem_kind: ProblemKind,
         operation_mode: OperationMode = OperationMode.ONESHOT_PLANNER,
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/meta_engine.py` & `unified_planning-1.0.0/unified_planning/engines/meta_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/__init__.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/anytime_planner.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/anytime_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/compiler.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/oneshot_planner.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/oneshot_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/plan_repairer.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/plan_repairer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/plan_validator.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/plan_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/portfolio.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/replanner.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/replanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/sequential_simulator.py` & `unified_planning-1.0.0/unified_planning/engines/mixins/sequential_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/oversubscription_planner.py` & `unified_planning-1.0.0/unified_planning/engines/oversubscription_planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -76,16 +76,18 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/parallel.py` & `unified_planning-1.0.0/unified_planning/engines/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/pddl_anytime_planner.py` & `unified_planning-1.0.0/unified_planning/engines/pddl_anytime_planner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -167,14 +167,54 @@
         The representation to obtain is:
         ``(action-name param1 param2 ... paramN)`` in each line for SequentialPlans
         ``start-time: (action-name param1 param2 ... paramN) [duration]`` in each line for TimeTriggeredPlans,
         where ``[duration]`` is optional and not specified for InstantaneousActions.
         """
         raise NotImplementedError
 
+    def _generate_last_result(
+        self,
+        solve_result: PlanGenerationResult,
+        last_result: Optional[PlanGenerationResult],
+    ) -> PlanGenerationResult:
+        """
+        IMPORTANT FOR ENGINES IMPLEMENTING THIS CLASS
+
+        This method takes the result returned by the _solve method, the last_plan_found
+        by the engine  and the status of the last plan and returns a new PlanGenerationResult.
+        If the engine writes his last plan to a file there is no need to overwrite this method;
+        but if the engine does not write the last plan on a file or if the last result returned
+        is not correct for some reason; this method allows an easy modification.
+
+        :param solve_result: The PlanGenerationResult returned by the solve method.
+        :param last_plan_found: The last plan found by the engine; obtained parsing the planner's
+            output.
+        :param last_status: The correct status of the last plan returned.
+        :return: The PlanGenerationResult compatible with the engine semantic; defaults to the
+            solve_result given in input.
+        """
+        if last_result is None or solve_result.plan is not None:
+            return solve_result
+
+        if solve_result.status in (
+            PlanGenerationResultStatus.UNSOLVABLE_PROVEN,
+            PlanGenerationResultStatus.UNSOLVABLE_INCOMPLETELY,
+        ):
+            new_status = PlanGenerationResultStatus.SOLVED_SATISFICING
+        else:
+            new_status = solve_result.status
+        res = PlanGenerationResult(
+            new_status,
+            last_result.plan,
+            solve_result.engine_name,
+            solve_result.metrics,
+            solve_result.log_messages,
+        )
+        return res
+
     def _get_solutions(
         self,
         problem: "up.model.AbstractProblem",
         timeout: Optional[float] = None,
         output_stream: Optional[IO[str]] = None,
     ) -> Iterator["up.engines.results.PlanGenerationResult"]:
         import threading
@@ -188,26 +228,22 @@
             )
             q.put(res)
 
         try:
             t = threading.Thread(target=run, daemon=True)
             t.start()
             status = PlanGenerationResultStatus.INTERMEDIATE
+            last_res: Optional[PlanGenerationResult] = None
             while status == PlanGenerationResultStatus.INTERMEDIATE:
                 res = q.get()
                 status = res.status
-                # If there is a timeout return the last plan found
-                if status == PlanGenerationResultStatus.TIMEOUT and res.plan is None:
-                    res = PlanGenerationResult(
-                        status,
-                        cast(Writer, writer).last_plan_found,
-                        res.engine_name,
-                        res.metrics,
-                        res.log_messages,
-                    )
+                if status != PlanGenerationResultStatus.INTERMEDIATE:
+                    res = self._generate_last_result(res, last_res)
+                else:
+                    last_res = res
                 yield res
         finally:
             if self._process is not None:
                 try:
                     self._process.kill()
                 except OSError:
                     pass  # This can happen if the process is already terminated
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/pddl_planner.py` & `unified_planning-1.0.0/unified_planning/engines/pddl_planner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,16 +30,15 @@
 import unified_planning.engines.mixins as mixins
 from unified_planning.engines.results import (
     LogLevel,
     LogMessage,
     PlanGenerationResult,
     PlanGenerationResultStatus,
 )
-from unified_planning.io.pddl_writer import PDDLWriter
-from unified_planning.exceptions import UPException
+from unified_planning.io import PDDLWriter, PDDLReader
 from asyncio.subprocess import PIPE
 from fractions import Fraction
 from typing import IO, Any, Callable, Optional, List, Tuple, Union, cast
 
 # This module implements two different mechanisms to execute a PDDL planner in a
 # subprocess, processing the output in real-time and imposing a timeout.
 # The first one uses the "select" module to process the output and error streams
@@ -114,20 +113,20 @@
             Union[
                 "up.model.Type",
                 "up.model.Action",
                 "up.model.Fluent",
                 "up.model.Object",
                 "up.model.Parameter",
                 "up.model.Variable",
+                "up.model.multi_agent.Agent",
             ],
         ],
     ) -> "up.plans.Plan":
         """
         Takes a problem, a filename and a map of renaming and returns the plan parsed from the file.
-
         :param problem: The up.model.problem.Problem instance for which the plan is generated.
         :param plan_filename: The path of the file in which the plan is written.
         :param get_item_named: A function that takes a name and returns the original up.model element instance
             linked to that renaming.
         :return: The up.plans.Plan corresponding to the parsed plan from the file
         """
         with open(plan_filename) as plan:
@@ -142,69 +141,27 @@
             Union[
                 "up.model.Type",
                 "up.model.Action",
                 "up.model.Fluent",
                 "up.model.Object",
                 "up.model.Parameter",
                 "up.model.Variable",
+                "up.model.multi_agent.Agent",
             ],
         ],
     ) -> "up.plans.Plan":
         """
         Takes a problem, a string and a map of renaming and returns the plan parsed from the string.
-
         :param problem: The up.model.problem.Problem instance for which the plan is generated.
         :param plan_str: The plan in string.
         :param get_item_named: A function that takes a name and returns the original up.model element instance linked to that renaming.
         :return: The up.plans.Plan corresponding to the parsed plan from the string
         """
-        actions: List = []
-        is_tt = False
-        for line in plan_str.splitlines():
-            if re.match(r"^\s*(;.*)?$", line):
-                continue
-            line = line.lower()
-            s_ai = re.match(r"^\s*\(\s*([\w?-]+)((\s+[\w?-]+)*)\s*\)\s*$", line)
-            t_ai = re.match(
-                r"^\s*(\d+)\s*:\s*\(\s*([\w?-]+)((\s+[\w?-]+)*)\s*\)\s*(\[\s*(\d+)\s*\])?\s*$",
-                line,
-            )
-            if s_ai:
-                assert is_tt == False
-                name = s_ai.group(1)
-                params_name = s_ai.group(2).split()
-            elif t_ai:
-                is_tt = True
-                start = Fraction(t_ai.group(1))
-                name = t_ai.group(2)
-                params_name = t_ai.group(3).split()
-                dur = None
-                if t_ai.group(6) is not None:
-                    dur = Fraction(t_ai.group(6))
-            else:
-                raise UPException(
-                    "Error parsing plan generated by " + self.__class__.__name__
-                )
-
-            action = get_item_named(name)
-            assert isinstance(action, up.model.Action), "Wrong plan or renaming."
-            parameters = []
-            for p in params_name:
-                obj = get_item_named(p)
-                assert isinstance(obj, up.model.Object), "Wrong plan or renaming."
-                parameters.append(problem.environment.expression_manager.ObjectExp(obj))
-            act_instance = up.plans.ActionInstance(action, tuple(parameters))
-            if is_tt:
-                actions.append((start, act_instance, dur))
-            else:
-                actions.append(act_instance)
-        if is_tt:
-            return up.plans.TimeTriggeredPlan(actions)
-        else:
-            return up.plans.SequentialPlan(actions)
+        reader = PDDLReader(problem.environment)
+        return reader.parse_plan_string(problem, plan_str, get_item_named)
 
     def _solve(
         self,
         problem: "up.model.AbstractProblem",
         heuristic: Optional[Callable[["up.model.state.State"], Optional[float]]] = None,
         timeout: Optional[float] = None,
         output_stream: Optional[Union[Tuple[IO[str], IO[str]], IO[str]]] = None,
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/plan_validator.py` & `unified_planning-1.0.0/unified_planning/engines/plan_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -99,16 +99,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
@@ -158,14 +161,15 @@
                 str
             ] = f"We cannot establish whether {self.name} can validate this problem!"
             if self.error_on_failed_checks:
                 raise up.exceptions.UPUsageError(msg)
             else:
                 warnings.warn(cast(str, msg))
         prev_state: Optional[State] = simulator.get_initial_state()
+        next_state: Optional[State] = prev_state
         if metric is not None:
             metric_value = evaluate_quality_metric_in_initial_state(simulator, metric)
         msg = None
         for i, ai in zip(range(1, len(plan.actions) + 1), plan.actions):
             assert prev_state is not None
             try:
                 unsat_conds, reason = simulator.get_unsatisfied_conditions(
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/replanner.py` & `unified_planning-1.0.0/unified_planning/engines/replanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/results.py` & `unified_planning-1.0.0/unified_planning/engines/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/engines/sequential_simulator.py` & `unified_planning-1.0.0/unified_planning/engines/sequential_simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 from enum import Enum, auto
 from fractions import Fraction
+from itertools import product
 from warnings import warn
 import unified_planning as up
 from unified_planning.engines.compilers import Grounder, GrounderHelper
 from unified_planning.engines.engine import Engine
 from unified_planning.engines.mixins.sequential_simulator import (
     SequentialSimulatorMixin,
 )
@@ -37,14 +38,16 @@
     ExpressionManager,
     UPState,
     Problem,
     MinimizeActionCosts,
     MinimizeExpressionOnFinalState,
     MaximizeExpressionOnFinalState,
     Oversubscription,
+    Expression,
+    Variable,
 )
 from unified_planning.model.types import _RealType
 from unified_planning.model.walkers import StateEvaluator, ExpressionQuantifiersRemover
 from typing import (
     Callable,
     Dict,
     Iterator,
@@ -277,21 +280,24 @@
             for f, v in zip(
                 grounded_action.simulated_effect.fluents,
                 grounded_action.simulated_effect.function(self._problem, state, {}),
             ):
                 updated_values[f] = v
                 assigned_fluent.add(f)
 
-        for effect in grounded_action.effects:
-            fluent, value = self._evaluate_effect(
-                effect, state, updated_values, assigned_fluent, em
-            )
-            if fluent is not None:
-                assert value is not None
-                updated_values[fluent] = value
+        for e in grounded_action.effects:
+            for effect in e.expand_effect(
+                cast(up.model.mixins.ObjectsSetMixin, self._problem)
+            ):
+                fluent, value = self._evaluate_effect(
+                    effect, state, updated_values, assigned_fluent, em
+                )
+                if fluent is not None:
+                    assert value is not None
+                    updated_values[fluent] = value
 
         new_state = state.make_child(updated_values)
         for si in self._state_invariants:
             if not self._se.evaluate(si, new_state).bool_constant_value():
                 raise UPInvalidActionError(
                     "The given action is not applicable because it violates state invariants.",
                     "Bounded numeric types are checked as state invariants.",
@@ -331,15 +337,15 @@
         :raises UPConflictingEffectsException: If to the same fluent are assigned 2 different
             values.
         """
         evaluate: Callable[[FNode], FNode] = lambda exp: self._se.evaluate(exp, state)
         if evaluated_fluent is not None:
             fluent = evaluated_fluent
         else:
-            fluent = effect.fluent.fluent()(*tuple(map(evaluate, effect.fluent.args)))
+            fluent = effect.fluent.fluent()(*(map(evaluate, effect.fluent.args)))
         if evaluated_condition is None:
             evaluated_condition = (
                 not effect.is_conditional() or evaluate(effect.condition).is_true()
             )
         if evaluated_condition:
             new_value = evaluate(effect.value)
             if effect.is_assignment():
@@ -465,76 +471,87 @@
                 for f, v in zip(
                     sim_eff.fluents,
                     sim_eff.function(self._problem, state, {}),
                 ):
                     updated_values[f] = v
                     assigned_fluent.add(f)
 
-            for e in g_action.conditional_effects:
-                if not e.fluent.type.is_bool_type():
-                    evaluated_condition = evaluate(e.condition).bool_constant_value()
-                    if evaluated_condition:
-                        try:
-                            fluent, value = self._evaluate_effect(
-                                e,
-                                state,
-                                updated_values,
-                                assigned_fluent,
-                                em,
-                                evaluated_condition=evaluated_condition,
-                            )
-                            assert fluent is not None and value is not None
-                            updated_values[fluent] = value
-                        except UPConflictingEffectsException:
-                            reason = InapplicabilityReasons.CONFLICTING_EFFECTS
-                            if early_termination:
-                                return unsatisfied_conditions, reason
+            for effect in g_action.conditional_effects:
+                for e in effect.expand_effect(
+                    cast(up.model.mixins.ObjectsSetMixin, self._problem)
+                ):
+                    if not e.fluent.type.is_bool_type():
+                        evaluated_condition = evaluate(
+                            e.condition
+                        ).bool_constant_value()
+                        if evaluated_condition:
+                            try:
+                                fluent, value = self._evaluate_effect(
+                                    e,
+                                    state,
+                                    updated_values,
+                                    assigned_fluent,
+                                    em,
+                                    evaluated_condition=evaluated_condition,
+                                )
+                                assert fluent is not None and value is not None
+                                updated_values[fluent] = value
+                            except UPConflictingEffectsException:
+                                reason = InapplicabilityReasons.CONFLICTING_EFFECTS
+                                if early_termination:
+                                    return unsatisfied_conditions, reason
 
             if updated_values:
-                for e in g_action.unconditional_effects:
-                    ev_fluent = e.fluent.fluent()(*tuple(map(evaluate, e.fluent.args)))
-                    values = updated_values.get(ev_fluent, None)
-                    if values is not None:
-                        try:
-                            fluent, value = self._evaluate_effect(
-                                e,
-                                state,
-                                updated_values,
-                                assigned_fluent,
-                                em,
-                                evaluated_fluent=ev_fluent,
-                                evaluated_condition=True,
-                            )
-                            assert fluent is not None and value is not None
-                            updated_values[fluent] = value
-                        except UPConflictingEffectsException:
-                            reason = InapplicabilityReasons.CONFLICTING_EFFECTS
-                            if early_termination:
-                                return unsatisfied_conditions, reason
-
-            for e in g_action.effects:
-                if e.fluent.fluent() in self._fluents_in_state_invariants:
-                    ev_fluent = e.fluent.fluent()(*tuple(map(evaluate, e.fluent.args)))
-                    if ev_fluent in self._fluent_exps_in_state_invariants:
-                        if ev_fluent not in updated_values:
+                for effect in g_action.unconditional_effects:
+                    for e in effect.expand_effect(
+                        cast(up.model.mixins.ObjectsSetMixin, self._problem)
+                    ):
+                        ev_fluent = e.fluent.fluent()(*(map(evaluate, e.fluent.args)))
+                        values = updated_values.get(ev_fluent, None)
+                        if values is not None:
                             try:
                                 fluent, value = self._evaluate_effect(
                                     e,
                                     state,
                                     updated_values,
                                     assigned_fluent,
                                     em,
                                     evaluated_fluent=ev_fluent,
+                                    evaluated_condition=True,
                                 )
                                 assert fluent is not None and value is not None
                                 updated_values[fluent] = value
                             except UPConflictingEffectsException:
-                                raise UPUnreachableCodeError(
-                                    "Conflicting effects should be caught above"
-                                )
+                                reason = InapplicabilityReasons.CONFLICTING_EFFECTS
+                                if early_termination:
+                                    return unsatisfied_conditions, reason
+
+            for effect in g_action.effects:
+                for e in effect.expand_effect(
+                    cast(up.model.mixins.ObjectsSetMixin, self._problem)
+                ):
+                    if e.fluent.fluent() in self._fluents_in_state_invariants:
+                        ev_fluent = e.fluent.fluent()(*(map(evaluate, e.fluent.args)))
+                        if ev_fluent in self._fluent_exps_in_state_invariants:
+                            if ev_fluent not in updated_values:
+                                try:
+                                    fluent, value = self._evaluate_effect(
+                                        e,
+                                        state,
+                                        updated_values,
+                                        assigned_fluent,
+                                        em,
+                                        evaluated_fluent=ev_fluent,
+                                    )
+                                    assert fluent is not None and value is not None
+                                    updated_values[fluent] = value
+                                except UPConflictingEffectsException:
+                                    raise UPUnreachableCodeError(
+                                        "Conflicting effects should be caught above"
+                                    )
 
             if not isinstance(state, up.model.UPState):
                 raise UPUsageError(
                     f"The UPSequentialSimulator uses the UPState but {type(state).__name__} is given."
                 )
             new_partial_state = state.make_child(updated_values)
             for si in self._state_invariants:
@@ -599,16 +616,19 @@
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/environment.py` & `unified_planning-1.0.0/unified_planning/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -27,15 +27,15 @@
 
 class Environment:
     """
     Represents the environment in the `unified_planning` library.
 
     The `Environment` is a structure that contains multiple
     singleton objects that are used throughout the system,
-    such as the :func:`ExpressionManager <unified_planning.Environment.expression_manager>`, :func:`TypeChecker <unified_planning.Environment.type_checker>`, :func:`ExpressionManager <unified_planning.Environment.expression_manager>`, :func:`TypeManager <unified_planning.Environment.type_manager>`.
+    such as the :func:`ExpressionManager <unified_planning.Environment.expression_manager>`, :func:`TypeChecker <unified_planning.Environment.type_checker>`, :func:`Factory <unified_planning.Environment.factory>`, :func:`TypeManager <unified_planning.Environment.type_manager>`.
 
     """
 
     def __init__(self):
         import unified_planning.model
         import unified_planning.engines
         import unified_planning.model.walkers
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/exceptions.py` & `unified_planning-1.0.0/unified_planning/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/grpc/converter.py` & `unified_planning-1.0.0/unified_planning/grpc/converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py` & `unified_planning-1.0.0/unified_planning/grpc/generated/unified_planning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/grpc/proto_reader.py` & `unified_planning-1.0.0/unified_planning/grpc/proto_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,15 +18,15 @@
 import fractions
 from typing import OrderedDict
 
 import unified_planning.grpc.generated.unified_planning_pb2 as proto
 from unified_planning.exceptions import UPException
 from unified_planning import Environment
 from unified_planning import model
-from unified_planning.model import metrics
+from unified_planning.model import metrics, TimePointInterval, GlobalEndTiming
 import unified_planning.plans
 from unified_planning.grpc.converter import Converter, handles
 from unified_planning.model import (
     DurativeAction,
     Effect,
     InstantaneousAction,
     Parameter,
@@ -296,15 +296,17 @@
             return problem.environment.type_manager.UserType(
                 name=msg.type_name, father=father
             )
 
     @handles(proto.Problem)
     def _convert_problem(
         self, msg: proto.Problem, environment: Optional[Environment] = None
-    ) -> Problem:
+    ) -> model.AbstractProblem:
+        if msg.HasField("scheduling_extension"):
+            return self._convert_scheduling_problem(msg, environment)
         problem_name = str(msg.problem_name) if str(msg.problem_name) != "" else None
         if msg.HasField("hierarchy"):
             problem = model.htn.HierarchicalProblem(
                 name=problem_name, environment=environment
             )
         else:
             problem = Problem(name=problem_name, environment=environment)
@@ -321,30 +323,25 @@
                 else None,
             )
         for f in msg.actions:
             problem.add_action(self.convert(f, problem))
         for eff in msg.timed_effects:
             ot = self.convert(eff.occurrence_time, problem)
             effect = self.convert(eff.effect, problem)
-            problem.add_timed_effect(
-                timing=ot,
-                fluent=effect.fluent,
-                value=effect.value,
-                condition=effect.condition,
-            )
+            problem._add_effect_instance(ot, effect)
 
         for assign in msg.initial_state:
             problem.set_initial_value(
                 fluent=self.convert(assign.fluent, problem),
                 value=self.convert(assign.value, problem),
             )
 
         for g in msg.goals:
             goal = self.convert(g.goal, problem)
-            if str(g.timing) == "":
+            if not g.HasField("timing"):
                 problem.add_goal(goal)
             else:
                 timing = self.convert(g.timing)
                 problem.add_timed_goal(interval=timing, goal=goal)
 
         for tc in msg.trajectory_constraints:
             problem.add_trajectory_constraint(self.convert(tc, problem))
@@ -360,16 +357,88 @@
             problem._initial_task_network = self.convert(
                 msg.hierarchy.initial_task_network, problem
             )
 
         problem.discrete_time = msg.discrete_time
         problem.self_overlapping = msg.self_overlapping
         if msg.HasField("epsilon"):
-            value = msg.epsilon
-            problem.epsilon = fractions.Fraction(value.numerator, value.denominator)
+            problem.epsilon = self.convert(msg.epsilon)
+
+        return problem
+
+    def _convert_scheduling_problem(
+        self, msg: proto.Problem, environment: Optional[Environment] = None
+    ) -> model.scheduling.SchedulingProblem:
+        problem_name = str(msg.problem_name) if str(msg.problem_name) != "" else None
+        problem = model.scheduling.SchedulingProblem(
+            name=problem_name, environment=environment
+        )
+
+        for t in msg.types:
+            problem._add_user_type(self.convert(t, problem))
+        for obj in msg.objects:
+            problem.add_object(self.convert(obj, problem))
+        for f in msg.fluents:
+            problem.add_fluent(
+                self.convert(f, problem),
+                default_initial_value=self.convert(f.default_value, problem)
+                if f.HasField("default_value")
+                else None,
+            )
+        for eff in msg.timed_effects:
+            ot = self.convert(eff.occurrence_time, problem)
+            effect = self.convert(eff.effect, problem)
+            problem._base._add_effect_instance(timing=ot, effect=effect)
+        for assign in msg.initial_state:
+            problem.set_initial_value(
+                fluent=self.convert(assign.fluent, problem),
+                value=self.convert(assign.value, problem),
+            )
+
+        for g in msg.goals:
+            goal = self.convert(g.goal, problem)
+            if not g.HasField("timing"):
+                problem.add_condition(TimePointInterval(GlobalEndTiming()), goal)
+            else:
+                timing = self.convert(g.timing)
+                problem.add_condition(self.convert(timing), goal)
+
+        for c in msg.scheduling_extension.constraints:
+            problem.add_constraint(self.convert(c, problem))
+
+        assert len(msg.trajectory_constraints) == 0
+
+        for metric in msg.metrics:
+            problem.add_quality_metric(self.convert(metric, problem))
+
+        assert not msg.HasField("hierarchy")
+        ext = msg.scheduling_extension
+        for pa in ext.activities:
+            a = problem.add_activity(pa.name)
+            a._set_duration_constraint(self._convert_duration(pa.duration, problem))
+            for p in pa.parameters:
+                prefix = pa.name + "."
+                assert p.name.startswith(prefix)
+                name = p.name[len(prefix) :]  # remove prefix
+                a.add_parameter(name, convert_type_str(p.type, problem))
+            for cond in pa.conditions:
+                a.add_condition(
+                    self.convert(cond.span, problem), self.convert(cond.cond, problem)
+                )
+            for eff in pa.effects:
+                timing = self._convert_timing(eff.occurrence_time)
+                effect = self._convert_effect(eff.effect, problem)
+                a._add_effect_instance(timing, effect)
+            for c in pa.constraints:
+                a.add_constraint(self.convert(c, problem))
+
+        problem.discrete_time = msg.discrete_time
+        problem.self_overlapping = msg.self_overlapping
+        if msg.HasField("epsilon"):
+            problem.epsilon = self.convert(msg.epsilon)
 
         return problem
 
     @handles(proto.AbstractTaskDeclaration)
     def _convert_abstract_task(
         self, msg: proto.AbstractTaskDeclaration, problem: Problem
     ):
@@ -516,29 +585,33 @@
             effects.append((eff, time))
 
         if isinstance(action, DurativeAction):
             for c, span in conditions:
                 action.add_condition(span, c)
             for e, ot in effects:
                 if e.kind == EffectKind.ASSIGN:
-                    action.add_effect(ot, e.fluent, e.value, e.condition)
+                    action.add_effect(ot, e.fluent, e.value, e.condition, e.forall)
                 elif e.kind == EffectKind.DECREASE:
-                    action.add_decrease_effect(ot, e.fluent, e.value, e.condition)
+                    action.add_decrease_effect(
+                        ot, e.fluent, e.value, e.condition, e.forall
+                    )
                 elif e.kind == EffectKind.INCREASE:
-                    action.add_increase_effect(ot, e.fluent, e.value, e.condition)
+                    action.add_increase_effect(
+                        ot, e.fluent, e.value, e.condition, e.forall
+                    )
         elif isinstance(action, InstantaneousAction):
             for c, _ in conditions:
                 action.add_precondition(c)
             for e, _ in effects:
                 if e.kind == EffectKind.ASSIGN:
-                    action.add_effect(e.fluent, e.value, e.condition)
+                    action.add_effect(e.fluent, e.value, e.condition, e.forall)
                 elif e.kind == EffectKind.DECREASE:
-                    action.add_decrease_effect(e.fluent, e.value, e.condition)
+                    action.add_decrease_effect(e.fluent, e.value, e.condition, e.forall)
                 elif e.kind == EffectKind.INCREASE:
-                    action.add_increase_effect(e.fluent, e.value, e.condition)
+                    action.add_increase_effect(e.fluent, e.value, e.condition, e.forall)
 
         return action
 
     @handles(proto.EffectExpression)
     def _convert_effect(
         self, msg: proto.EffectExpression, problem: Problem
     ) -> model.Effect:
@@ -551,38 +624,43 @@
             kind = EffectKind.ASSIGN
 
         return Effect(
             fluent=self.convert(msg.fluent, problem),
             value=self.convert(msg.value, problem),
             condition=self.convert(msg.condition, problem),
             kind=kind,
+            forall=(self.convert(var, problem).variable() for var in msg.forall),
         )
 
     @handles(proto.Duration)
     def _convert_duration(
         self, msg: proto.Duration, problem: Problem
     ) -> model.timing.DurationInterval:
         return model.timing.DurationInterval(
             lower=self.convert(msg.controllable_in_bounds.lower, problem),
             upper=self.convert(msg.controllable_in_bounds.upper, problem),
             is_left_open=bool(msg.controllable_in_bounds.is_left_open),
             is_right_open=bool(msg.controllable_in_bounds.is_right_open),
         )
 
     @handles(proto.TimeInterval)
-    def _convert_timed_interval(self, msg: proto.TimeInterval) -> model.TimeInterval:
+    def _convert_timed_interval(
+        self, msg: proto.TimeInterval, _problem: Optional[Problem] = None
+    ) -> model.TimeInterval:
         return model.TimeInterval(
             lower=self.convert(msg.lower),
             upper=self.convert(msg.upper),
             is_left_open=msg.is_left_open,
             is_right_open=msg.is_right_open,
         )
 
     @handles(proto.Timing)
-    def _convert_timing(self, msg: proto.Timing) -> model.timing.Timing:
+    def _convert_timing(
+        self, msg: proto.Timing, _problem: Optional[Problem] = None
+    ) -> model.timing.Timing:
         return model.Timing(
             delay=self.convert(msg.delay)
             if msg.HasField("delay")
             else fractions.Fraction(0),
             timepoint=self.convert(msg.timepoint),
         )
 
@@ -605,14 +683,18 @@
         container = msg.container_id if msg.container_id != "" else None
         return model.timing.Timepoint(kind, container)
 
     @handles(proto.Plan)
     def _convert_plan(
         self, msg: proto.Plan, problem: Problem
     ) -> unified_planning.plans.Plan:
+        if msg.HasField("schedule"):
+            assert not msg.HasField("hierarchy")
+            assert len(msg.actions) == 0
+            return self._convert_schedule(msg.schedule, problem)
         actions = [self._convert_action_instance(a, problem) for a in msg.actions]
         if all(a[2] is not None for a in actions):
             # If all actions have temporal term, we can assume that they are
             # (id, action, (absolute start time, duration))
             time_triggered_actions = [
                 (start, action, duration) for _, action, (start, duration) in actions
             ]
@@ -689,14 +771,37 @@
                 id,
                 action_instance,
                 (start_time, None if duration == 0 else duration),
             )
         else:
             return id, action_instance, None
 
+    def _convert_schedule(
+        self, msg: proto.Schedule, problem: model.scheduling.SchedulingProblem
+    ) -> unified_planning.plans.Schedule:
+        activities = [problem.get_activity(act_name) for act_name in msg.activities]
+        assignment = {}
+        for var, val in msg.variable_assignments.items():
+            if "." in var:
+                activity_name, parameter_name = var.split(".")
+                activity = problem.get_activity(activity_name)
+                if parameter_name == "start":
+                    param = activity.start
+                elif parameter_name == "end":
+                    param = activity.end
+                else:
+                    param = activity.get_parameter(parameter_name)
+            else:
+                param = problem.get_variable(var)
+            val = self._convert_atom(val, problem)
+            assignment[param] = val
+        return unified_planning.plans.Schedule(
+            assignment=assignment, activities=activities
+        )
+
     @handles(proto.PlanGenerationResult)
     def _convert_plan_generation_result(
         self, result: proto.PlanGenerationResult, problem: Problem
     ) -> unified_planning.engines.PlanGenerationResult:
         if result.status == proto.PlanGenerationResult.Status.Value(
             "SOLVED_SATISFICING"
         ):
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/grpc/proto_writer.py` & `unified_planning-1.0.0/unified_planning/grpc/proto_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,14 +19,15 @@
 
 import unified_planning.grpc.generated.unified_planning_pb2 as proto
 from unified_planning import model
 import unified_planning.engines
 import unified_planning.model.htn
 import unified_planning.engines
 import unified_planning.plans
+from unified_planning.environment import get_environment
 from unified_planning.plans.hierarchical_plan import *
 import unified_planning.model.walkers as walkers
 import unified_planning.plans
 from unified_planning.model.types import domain_size, domain_item
 from unified_planning.exceptions import UPException
 from unified_planning.grpc.converter import Converter, handles
 from unified_planning.model.operators import (
@@ -350,20 +351,21 @@
             kind = proto.EffectExpression.EffectKind.Value("ASSIGN")
         elif effect.is_increase():
             kind = proto.EffectExpression.EffectKind.Value("INCREASE")
         elif effect.is_decrease():
             kind = proto.EffectExpression.EffectKind.Value("DECREASE")
         else:
             raise ValueError(f"Unsupported effect: {effect}")
-
+        auto_promote = effect.environment.expression_manager.auto_promote
         return proto.EffectExpression(
             kind=kind,
             fluent=self.convert(effect.fluent),
             value=self.convert(effect.value),
             condition=self.convert(effect.condition),
+            forall=[self.convert(exp) for exp in auto_promote(effect.forall)],
         )
 
     @handles(model.InstantaneousAction)
     def _convert_instantaneous_action(
         self, a: model.InstantaneousAction
     ) -> proto.Action:
         effects = []
@@ -386,42 +388,62 @@
             duration=None,
             conditions=conditions,
             effects=effects,
         )
 
     @handles(model.DurativeAction)
     def _convert_durative_action(self, a: model.DurativeAction) -> proto.Action:
-        effects = []
+        return proto.Action(
+            name=a.name,
+            parameters=[self.convert(p) for p in a.parameters],
+            duration=self.convert(a.duration),
+            conditions=self._convert_timed_conditions(a.conditions),
+            effects=self._convert_timed_effects(a.effects),
+        )
+
+    def _convert_timed_conditions(
+        self, conds: Dict[model.timing.TimeInterval, List[model.fnode.FNode]]
+    ) -> List[proto.Condition]:
         conditions = []
 
-        for span, cond in a.conditions.items():
+        for span, cond in conds.items():
             span = self.convert(span)
             for c in cond:
                 conditions.append(
                     proto.Condition(
                         cond=self.convert(c),
                         span=span,
                     )
                 )
-        for ot, eff in a.effects.items():
-            ot = self.convert(ot)
+        return conditions
+
+    def _convert_timed_effects(
+        self, effs: Dict[model.timing.Timing, List[model.effect.Effect]]
+    ) -> List[proto.Effect]:
+        effects = []
+        for ot, eff in effs.items():
+            ot = self._convert_timing(ot)
             for e in eff:
                 effects.append(
                     proto.Effect(
                         effect=self.convert(e),
                         occurrence_time=ot,
                     )
                 )
+        return effects
 
-        return proto.Action(
+    @handles(model.scheduling.Activity)
+    def _convert_activity(self, a: model.scheduling.Activity) -> proto.Activity:
+        return proto.Activity(
             name=a.name,
             parameters=[self.convert(p) for p in a.parameters],
             duration=self.convert(a.duration),
-            conditions=conditions,
-            effects=effects,
+            conditions=self._convert_timed_conditions(a.conditions),
+            effects=self._convert_timed_effects(a.effects),
+            constraints=[self.convert(c) for c in a.constraints],
         )
 
     @handles(model.timing.Timepoint)
     def _convert_timepoint(self, tp: model.timing.Timepoint) -> proto.Timepoint:
         if tp.kind == TimepointKind.START:
             kind = proto.Timepoint.TimepointKind.Value("START")
         elif tp.kind == TimepointKind.END:
@@ -527,41 +549,45 @@
     def _convert_task_network(self, tn: model.htn.TaskNetwork) -> proto.TaskNetwork:
         return proto.TaskNetwork(
             variables=[self.convert(v) for v in tn.variables],
             subtasks=[self.convert(st) for st in tn.subtasks],
             constraints=[self.convert(c) for c in tn.constraints],
         )
 
-    def build_hierarchy(
+    def _build_hierarchy(
         self, problem: model.htn.HierarchicalProblem
     ) -> proto.Hierarchy:
         return proto.Hierarchy(
             initial_task_network=self.convert(problem.task_network),
             abstract_tasks=[self.convert(t) for t in problem.tasks],
             methods=[self.convert(m) for m in problem.methods],
         )
 
+    def _build_scheduling(
+        self, problem: model.scheduling.SchedulingProblem
+    ) -> proto.SchedulingExtension:
+        return proto.SchedulingExtension(
+            activities=[self.convert(a) for a in problem.activities],
+            variables=[self.convert(v) for v in problem.base_variables],
+            constraints=[self.convert(c) for c in problem.base_constraints],
+        )
+
     @handles(model.Problem, model.htn.HierarchicalProblem)
     def _convert_problem(self, problem: model.Problem) -> proto.Problem:
         goals = [proto.Goal(goal=self.convert(g)) for g in problem.goals]
         for t, gs in problem.timed_goals.items():
             goals += [
                 proto.Goal(goal=self.convert(g), timing=self.convert(t)) for g in gs
             ]
 
         problem_name = str(problem.name) if problem.name is not None else ""
         hierarchy = None
         if isinstance(problem, model.htn.HierarchicalProblem):
-            hierarchy = self.build_hierarchy(problem)
-        epsilon = None
-        if problem.epsilon is not None:
-            epsilon = proto.Real(
-                numerator=problem.epsilon.numerator,
-                denominator=problem.epsilon.denominator,
-            )
+            hierarchy = self._build_hierarchy(problem)
+
         return proto.Problem(
             domain_name=problem_name + "_domain",
             problem_name=problem_name,
             types=[self.convert(t) for t in problem.user_types],
             fluents=[self.convert(f, problem) for f in problem.fluents],
             objects=[self.convert(o) for o in problem.all_objects],
             actions=[self.convert(a) for a in problem.actions],
@@ -575,15 +601,62 @@
             metrics=[self.convert(m) for m in problem.quality_metrics],
             hierarchy=hierarchy,
             trajectory_constraints=[
                 self.convert(tc) for tc in problem.trajectory_constraints
             ],
             discrete_time=problem.discrete_time,
             self_overlapping=problem.self_overlapping,
-            epsilon=epsilon,
+            epsilon=self.convert(problem.epsilon)
+            if problem.epsilon is not None
+            else None,
+        )
+
+    @handles(model.scheduling.SchedulingProblem)
+    def _convert_scheduling_problem(
+        self, problem: model.scheduling.SchedulingProblem
+    ) -> proto.Problem:
+        problem_name = str(problem.name) if problem.name is not None else ""
+        goals = [
+            proto.Goal(goal=self.convert(g), timing=self.convert(t))
+            for t, g in problem.base_conditions
+        ]
+
+        sched = proto.SchedulingExtension(
+            activities=[self.convert(a) for a in problem.activities],
+            variables=[self.convert(v) for v in problem.base_variables],
+            constraints=[self.convert(c) for c in problem.base_constraints],
+        )
+
+        return proto.Problem(
+            domain_name=problem_name + "_domain",
+            problem_name=problem_name,
+            types=[self.convert(t) for t in problem.user_types],
+            fluents=[self.convert(f, problem) for f in problem.fluents],
+            objects=[self.convert(o) for o in problem.all_objects],
+            initial_state=[
+                proto.Assignment(fluent=self.convert(x), value=self.convert(v))
+                for (x, v) in problem.initial_values.items()
+            ],
+            timed_effects=[
+                proto.TimedEffect(
+                    occurrence_time=self.convert(timing), effect=self.convert(eff)
+                )
+                for (timing, eff) in problem.base_effects
+            ],
+            goals=goals,
+            features=[map_feature(feature) for feature in problem.kind.features],
+            metrics=[self.convert(m) for m in problem.quality_metrics],
+            hierarchy=None,
+            scheduling_extension=sched,
+            trajectory_constraints=None,
+            discrete_time=problem.discrete_time,
+            self_overlapping=problem.self_overlapping,
+            epsilon=self.convert(problem.epsilon)
+            if problem.epsilon is not None
+            else None,
         )
 
     @handles(model.metrics.MinimizeActionCosts)
     def _convert_minimize_action_costs(
         self, metric: model.metrics.MinimizeActionCosts
     ) -> proto.Metric:
         action_costs = {}
@@ -766,14 +839,37 @@
 
         plan = proto.Plan(
             actions=flat_plan.actions,
             hierarchy=proto.PlanHierarchy(root_tasks=root_tasks, methods=methods),
         )
         return plan
 
+    @handles(unified_planning.plans.Schedule)
+    def _convert_schedule(self, schedule: unified_planning.plans.Schedule):
+        assignments = {}
+        for var, val in schedule.assignment.items():
+            if isinstance(var, model.Timepoint):
+                if var.kind == TimepointKind.START:
+                    var = f"{var.container}.start"
+                elif var.kind == TimepointKind.END:
+                    var = f"{var.container}.end"
+                else:
+                    raise ValueError(f"Invalid timepoint in assignment: {var}")
+            else:
+                assert isinstance(var, model.Parameter)
+                var = var.name
+            (val,) = get_environment().expression_manager.auto_promote(val)
+            assignments[var] = self.convert(val).atom
+
+        schedule = proto.Schedule(
+            activities=[a.name for a in schedule.activities],
+            variable_assignments=assignments,
+        )
+        return proto.Plan(schedule=schedule)
+
     @handles(unified_planning.engines.PlanGenerationResult)
     def _convert_plan_generation_result(
         self, result: unified_planning.engines.PlanGenerationResult
     ) -> proto.PlanGenerationResult:
         log_messages = None
         if result.log_messages is not None:
             log_messages = [self.convert(log) for log in result.log_messages]
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/interop/__init__.py` & `unified_planning-1.0.0/unified_planning/interop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/interop/from_tarski.py` & `unified_planning-1.0.0/unified_planning/interop/from_tarski.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/interop/to_tarski.py` & `unified_planning-1.0.0/unified_planning/interop/to_tarski.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/io/anml_grammar.py` & `unified_planning-1.0.0/unified_planning/io/anml_grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/io/anml_reader.py` & `unified_planning-1.0.0/unified_planning/io/anml_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -69,15 +69,15 @@
     Timing,
     TimeInterval,
     Type,
     Parameter,
     Variable,
 )
 from fractions import Fraction
-from typing import Dict, Set, Tuple, Union, Callable, List, Optional
+from typing import Dict, Sequence, Set, Tuple, Union, Callable, List, Optional
 from pyparsing import ParseResults
 from unified_planning.io.utils import parse_string, parse_file
 
 
 class ANMLReader:
     """
     Class that offers the capability, with the :func:`parse_problem <unified_planning.io.ANMLReader.parse_problem>`, to create a :class:`~unified_planning.model.Problem` from an
@@ -194,32 +194,38 @@
                     types_map,
                     global_start,
                     global_end,
                 )
         return self._problem
 
     def parse_problem(
-        self, problem_filename: str, problem_name: Optional[str] = None
+        self,
+        problem_filename: Union[str, Sequence[str]],
+        problem_name: Optional[str] = None,
     ) -> "up.model.Problem":
         """
         Takes in input a filename containing an `ANML` problem and returns the parsed `Problem`.
 
         Check the class documentation for the assumptions made for this parser to work.
 
-        :param problem_filename: The path to the file containing the `ANML` problem.
+        :param problem_filename: The path to the file containing the `ANML` problem
+            or to the files to concatenate to obtain the complete problem.
         :param problem_name: Optionally, the name to give to the created problem; if it is None,
             `problem_filename` will be set as the problem name.
         :return: The `Problem` parsed from the given anml file.
         """
 
         # create the grammar and populate it's data structures
         grammar = ANMLGrammar()
         parse_file(grammar.problem, problem_filename, parse_all=True)
         if problem_name is None:
-            problem_name = problem_filename
+            if isinstance(problem_filename, str):
+                problem_name = problem_filename
+            else:
+                problem_name = "_".join(problem_filename)
         self._problem = self._parse_problem(grammar, problem_name)
         return self._problem
 
     def parse_problem_string(
         self, problem_str: str, problem_name: Optional[str] = None
     ) -> "up.model.Problem":
         """
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/io/anml_writer.py` & `unified_planning-1.0.0/unified_planning/io/anml_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/io/ma_pddl_writer.py` & `unified_planning-1.0.0/unified_planning/io/ma_pddl_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,65 +28,66 @@
     DurativeAction,
     Fluent,
     Parameter,
     Problem,
     Object,
 )
 from unified_planning.model.multi_agent.agent import Agent
+from unified_planning.model.multi_agent.ma_problem import MultiAgentProblem
 from unified_planning.exceptions import (
     UPTypeError,
     UPProblemDefinitionError,
     UPException,
 )
 from unified_planning.model.types import _UserType
-from typing import Callable, Dict, IO, List, Optional, Set, Union, cast
+from typing import Callable, Dict, List, Optional, Set, Union, cast
 from io import StringIO
-from functools import reduce
 from unified_planning.io.pddl_writer import (
     ObjectsExtractor,
     ConverterToPDDLString,
     PDDL_KEYWORDS,
     INITIAL_LETTER,
     _write_effect,
 )
 
 
 class ConverterToMAPDDLString(ConverterToPDDLString):
     """Expression converter to a MA-PDDL string."""
 
     def __init__(
         self,
-        env: "up.environment.Environment",
+        problem: MultiAgentProblem,
         get_mangled_name: Callable[
             [
                 Union[
                     "up.model.Type",
                     "up.model.Action",
                     "up.model.Fluent",
                     "up.model.Object",
                     "up.model.multi_agent.Agent",
                 ]
             ],
             str,
         ],
         agent: Optional["up.model.multi_agent.Agent"],
     ):
-        ConverterToPDDLString.__init__(self, env, get_mangled_name)
-        self.agent = agent
+        ConverterToPDDLString.__init__(self, problem.environment, get_mangled_name)
+        self._problem = problem
+        self._agent = agent
 
     def walk_dot(self, expression, args):
-        agent = expression.agent()
+        agent = self._problem.agent(expression.agent())
         fluent = expression.args[0].fluent()
         objects = expression.args[0].args
         return f'(a_{self.get_mangled_name(fluent)} {self.get_mangled_name(agent)} {" ".join([self.convert(obj) for obj in objects])})'
 
     def walk_fluent_exp(self, expression, args):
         fluent = expression.fluent()
-        if self.agent is not None and fluent in self.agent.fluents:
-            return f'(a_{self.get_mangled_name(fluent)} ?{self.agent.name}{" " if len(args) > 0 else ""}{" ".join(args)})'
+        if self._agent is not None and fluent in self._agent.fluents:
+            return f'(a_{self.get_mangled_name(fluent)} ?{self._agent.name}{" " if len(args) > 0 else ""}{" ".join(args)})'
         else:
             return f'({self.get_mangled_name(fluent)}{" " if len(args) > 0 else ""}{" ".join(args)})'
 
 
 class MAPDDLWriter:
     """
     This class can be used to write a :class:`~unified_planning.model.MultiAgentProblem` in `MA-PDDL`.
@@ -95,20 +96,22 @@
     rewrite_bool_assignments determines if this writer will write
     non constant boolean assignment as conditional effects.
     """
 
     def __init__(
         self,
         problem: "up.model.multi_agent.MultiAgentProblem",
+        explicit_false_initial_states: Optional[bool] = False,
         needs_requirements: bool = True,
         rewrite_bool_assignments: bool = False,
     ):
         self._env = problem.environment
         self.problem = problem
         self.problem_kind = self.problem.kind
+        self.explicit_false_initial_states = explicit_false_initial_states
         self.needs_requirements = needs_requirements
         self.rewrite_bool_assignments = rewrite_bool_assignments
         # otn represents the old to new renamings
         self.otn_renamings: Dict[
             Union[
                 "up.model.Type",
                 "up.model.Action",
@@ -291,30 +294,30 @@
             functions_agent_goal = []
             for g in self.problem.goals:
                 if g.is_dot():
                     f = g.args[0].fluent()
                     agent = g.agent()
                     # args = g.args
                     # objects = g.args[0].args
-                    if f not in ag.fluents:
+                    if f not in ag.fluents and f not in self.all_public_fluents:
                         if f.type.is_bool_type():
                             params = []
                             i = 0
                             for param in f.signature:
                                 if param.type.is_user_type():
                                     params.append(
                                         f" {self._get_mangled_name(param)} - {self._get_mangled_name(param.type)}"
                                     )
                                     i += 1
                                 else:
                                     raise UPTypeError(
                                         "MA-PDDL supports only user type parameters"
                                     )
                             predicates_agent_goal.append(
-                                f'(a_{self._get_mangled_name(f)} ?agent - {self._get_mangled_name(agent) + "_type"}{"".join(params)})'
+                                f'(a_{self._get_mangled_name(f)} ?agent - {"ag"}{"".join(params)})'
                             )
                         elif f.type.is_int_type() or f.type.is_real_type():
                             params = []
                             i = 0
                             for param in f.signature:
                                 if param.type.is_user_type():
                                     params.append(
@@ -322,15 +325,15 @@
                                     )
                                     i += 1
                                 else:
                                     raise UPTypeError(
                                         "MA-PDDL supports only user type parameters"
                                     )
                             functions_agent_goal.append(
-                                f'(a_{self._get_mangled_name(f)} ?agent - {self._get_mangled_name(agent) + "_type"}{"".join(params)})'
+                                f'(a_{self._get_mangled_name(f)} ?agent - {"ag"}{"".join(params)})'
                             )
                         else:
                             raise UPTypeError(
                                 "MA-PDDL supports only boolean and numerical fluents"
                             )
 
             nl = "\n  "
@@ -339,21 +342,21 @@
                 if len(predicates_environment) > 0
                 or len(predicates_agent) > 0
                 or len(predicates_agent_goal) > 0
                 or len(predicates_public_agent) > 0
                 else ""
             )
             out.write(
-                f" {nl.join(predicates_environment)}\n"
-                if len(predicates_environment) > 0
+                f"  {nl.join(predicates_agent_goal)}\n"
+                if len(predicates_agent_goal) > 0
                 else ""
             )
             out.write(
-                f"  {nl.join(predicates_agent_goal)}\n"
-                if len(predicates_agent_goal) > 0
+                f" {nl.join(predicates_environment)}\n"
+                if len(predicates_environment) > 0
                 else ""
             )
             out.write(
                 f"  {nl.join(predicates_public_agent)}\n"
                 if len(predicates_public_agent) > 0
                 else ""
             )
@@ -407,15 +410,15 @@
                 or len(functions_agent) > 0
                 or len(functions_agent_goal) > 0
                 or len(functions_public_agent) > 0
                 else ""
             )
 
             converter = ConverterToMAPDDLString(
-                self.problem.environment, self._get_mangled_name, ag
+                self.problem, self._get_mangled_name, ag
             )
             costs: dict = {}
             for a in ag.actions:
                 if isinstance(a, up.model.InstantaneousAction):
                     out.write(f" (:action {self._get_mangled_name(a)}")
                     out.write(f"\n  :parameters (")
                     out.write(
@@ -442,14 +445,15 @@
                         for e in a.effects:
                             _write_effect(
                                 e,
                                 None,
                                 out,
                                 converter,
                                 self.rewrite_bool_assignments,
+                                self._get_mangled_name,
                             )
 
                         if a in costs:
                             out.write(
                                 f"   (increase (total-cost) {converter.convert(costs[a])})"
                             )
                         out.write(")")
@@ -503,14 +507,15 @@
                             for e in el:
                                 _write_effect(
                                     e,
                                     t,
                                     out,
                                     converter,
                                     self.rewrite_bool_assignments,
+                                    self._get_mangled_name,
                                 )
                         if a in costs:
                             out.write(
                                 f" (at end (increase (total-cost) {converter.convert(costs[a])}))"
                             )
                         out.write(")")
                     out.write(")\n")
@@ -567,40 +572,57 @@
                             f'\n   {self._get_mangled_name(agent)} - {self._get_mangled_name(agent) + "_type"}'
                         )
                     else:
                         out.write(f"")
 
             out.write("\n )\n")
             converter = ConverterToMAPDDLString(
-                self.problem.environment, self._get_mangled_name, ag
+                self.problem, self._get_mangled_name, ag
             )
             out.write(" (:init")
 
             for f, v in self.problem.initial_values.items():
                 if v.is_true():
                     if f.is_dot():
                         fluent = f.args[0].fluent()
                         args = f.args
                         if (
                             fluent in self.all_public_fluents
                             or fluent in ag.fluents
-                            and f.agent().name == ag.name
+                            and f.agent() == ag.name
                         ):
                             out.write(f"\n  {converter.convert(f)}")
-                        elif (
-                            f.agent().name != ag.name
-                            and fluent in self.all_public_fluents
-                        ):
+                        elif f.agent() != ag.name and fluent in self.all_public_fluents:
                             out.write(f"\n  {converter.convert(f)}")
                         else:
                             out.write(f"")
                     else:
                         out.write(f"\n  {converter.convert(f)}")
                 elif v.is_false():
-                    pass
+                    if self.explicit_false_initial_states:
+                        if f.is_dot():
+                            fluent = f.args[0].fluent()
+                            args = f.args
+                            if (
+                                fluent in self.all_public_fluents
+                                or fluent in ag.fluents
+                                and f.agent() == ag.name
+                            ):
+                                out.write(f"\n  (not {converter.convert(f)})")
+                            elif (
+                                f.agent() != ag.name
+                                and fluent in self.all_public_fluents
+                            ):
+                                out.write(f"\n  (not {converter.convert(f)})")
+                            else:
+                                out.write(f"")
+                        else:
+                            out.write(f"\n  (not {converter.convert(f)})")
+                    else:
+                        pass
                 else:
                     out.write(f"\n  (= {converter.convert(f)} {converter.convert(v)})")
             if self.problem.kind.has_actions_cost():
                 out.write(f" (= (total-cost) 0)")
             out.write(")\n")
             out.write(f" (:goal (and")
             for p in self.problem.goals:
@@ -733,29 +755,32 @@
             if self.problem_kind.has_hierarchical_typing() and tmp_name == "object":
                 tmp_name = f"{tmp_name}_"
         else:
             original_name = item.name
             tmp_name = _get_pddl_name(item)
         # if the ma-pddl valid name is the same of the original one and it does not create conflicts,
         # it can be returned
-        if tmp_name == original_name and tmp_name not in self.nto_renamings:
-            new_name = tmp_name
+        if not isinstance(item, up.model.multi_agent.Agent):
+            if tmp_name == original_name and tmp_name not in self.nto_renamings:
+                new_name = tmp_name
+            else:
+                count = 0
+                new_name = tmp_name
+                while self.problem.has_name(new_name) or new_name in self.nto_renamings:
+                    new_name = f"{tmp_name}_{count}"
+                    count += 1
+            assert (
+                new_name not in self.nto_renamings
+                and new_name not in self.otn_renamings.values()
+            )
+
         else:
-            count = 0
             new_name = tmp_name
-            while self.problem.has_name(new_name) or new_name in self.nto_renamings:
-                new_name = f"{tmp_name}_{count}"
-                count += 1
-        assert (
-            new_name not in self.nto_renamings
-            and new_name not in self.otn_renamings.values()
-        )
         self.otn_renamings[item] = new_name
         self.nto_renamings[new_name] = item
-
         return new_name
 
     def get_item_named(
         self, name: str
     ) -> Union[
         "up.model.Type",
         "up.model.Action",
@@ -826,15 +851,17 @@
         import unified_planning.model.walkers as walkers
 
         get_dots = walkers.AnyGetter(lambda x: x.is_dot())
         for a in agent.actions:
             if isinstance(a, up.model.InstantaneousAction):
                 for p in a.preconditions:
                     for d in get_dots.get(p):
-                        _update_domain_objects_ag(self.domain_objects_agents, d.agent())
+                        _update_domain_objects_ag(
+                            self.domain_objects_agents, self.problem.agent(d.agent())
+                        )
                     _update_domain_objects(self.domain_objects, obe.get(p))
                 for e in a.effects:
                     if e.is_conditional():
                         _update_domain_objects(
                             self.domain_objects, obe.get(e.condition)
                         )
                     _update_domain_objects(self.domain_objects, obe.get(e.fluent))
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/io/pddl_reader.py` & `unified_planning-1.0.0/unified_planning/io/pddl_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from itertools import product
+
+from collections import OrderedDict
+from fractions import Fraction
+import re
+from typing import Dict, Union, Callable, List, cast, Tuple
+import typing
 import unified_planning as up
 import unified_planning.model.htn as htn
 import unified_planning.model.walkers
-import typing
 from unified_planning.model import ContingentProblem
 from unified_planning.environment import Environment, get_environment
-from unified_planning.exceptions import UPUsageError
+from unified_planning.exceptions import (
+    UPUsageError,
+    UPException,
+    UPUnsupportedProblemTypeError,
+)
 from unified_planning.io.utils import parse_string, set_results_name, Located
-from collections import OrderedDict
-from fractions import Fraction
-from typing import Dict, Union, Callable, List, cast
 
 import pyparsing
 from pyparsing import ParseResults
 from pyparsing import CharsNotIn, Empty, col, lineno
 from pyparsing import Word, alphanums, alphas, ZeroOrMore, OneOrMore, Keyword
 from pyparsing import Suppress, Group, Optional, Forward
 
@@ -383,15 +388,14 @@
         self,
         problem: up.model.Problem,
         act: typing.Optional[Union[up.model.Action, htn.Method, htn.TaskNetwork]],
         types_map: TypesMap,
         var: Dict[str, up.model.Variable],
         exp: CustomParseResults,
         complete_str: str,
-        assignments: Dict[str, "up.model.Object"] = {},
     ) -> up.model.FNode:
         stack = [(var, exp, False)]
         solved: List[up.model.FNode] = []
         while len(stack) > 0:
             var, exp, status = stack.pop()
             if status:
                 if exp[0].value == "-" and len(exp) == 2:  # unary minus
@@ -421,17 +425,14 @@
                         end_line, end_col = exp.line_end(complete_str), exp.col_end(
                             complete_str
                         )
                         raise SyntaxError(
                             repr(e)
                             + f"\nError from line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
                         )
-                elif exp[0].value in assignments:  # quantified assignment variable
-                    assert len(exp) == 1
-                    solved.append(self._em.ObjectExp(assignments[exp[0].value]))
                 else:
                     start_line, start_col = exp.line_start(complete_str), exp.col_start(
                         complete_str
                     )
                     end_line, end_col = exp.line_end(complete_str), exp.col_end(
                         complete_str
                     )
@@ -483,17 +484,14 @@
                         stack.append((var, exp, True))
                         for i in range(1, len(exp)):
                             stack.append((var, exp[i], False))
                     elif problem.has_fluent(exp[0].value):  # fluent reference
                         stack.append((var, exp, True))
                         for i in range(1, len(exp)):
                             stack.append((var, exp[i], False))
-                    elif exp[0].value in assignments:  # quantified assignment variable
-                        assert len(exp) == 1
-                        stack.append((var, exp, True))
                     elif len(exp) == 1:  # expand an element inside brackets
                         stack.append((var, exp[0], False))
                     else:
                         start_line, start_col = exp.line_start(
                             complete_str
                         ), exp.col_start(complete_str)
                         end_line, end_col = exp.line_end(complete_str), exp.col_end(
@@ -503,23 +501,21 @@
                             f"Not able to handle: {complete_str[exp.locn_start: exp.locn_end]} found at line: {start_line}, col {start_col} to line: {end_line}, col {end_col}"
                         )
                 elif isinstance(exp.value, str):
                     if (
                         exp.value[0] == "?" and exp.value[1:] in var
                     ):  # variable in a quantifier expression
                         solved.append(self._em.VariableExp(var[exp.value[1:]]))
-                    elif exp.value in assignments:  # quantified assignment variable
-                        solved.append(self._em.ObjectExp(assignments[exp.value]))
                     elif exp.value[0] == "?":  # action parameter
                         assert act is not None
                         try:
                             solved.append(
                                 self._em.ParameterExp(act.parameter(exp.value[1:]))
                             )
-                        except KeyError:
+                        except ValueError:
                             start_line, start_col = exp.line_start(
                                 complete_str
                             ), exp.col_start(complete_str)
                             end_line, end_col = exp.line_end(complete_str), exp.col_end(
                                 complete_str
                             )
                             raise SyntaxError(
@@ -561,97 +557,107 @@
         return solved.pop()
 
     def _add_effect(
         self,
         problem: up.model.Problem,
         act: Union[up.model.InstantaneousAction, up.model.DurativeAction],
         types_map: TypesMap,
-        universal_assignments: typing.Optional[
-            Dict["up.model.Action", List[CustomParseResults]]
-        ],
         exp: CustomParseResults,
         complete_str: str,
         cond: Union[up.model.FNode, bool] = True,
         timing: typing.Optional[up.model.Timing] = None,
-        assignments: Dict[str, "up.model.Object"] = {},
+        forall_variables: typing.Optional[Dict[str, up.model.Variable]] = None,
     ):
-        to_add = [(exp, cond)]
+        if forall_variables is None:
+            forall_variables = {}
+        to_add = [(exp, cond, forall_variables)]
         while to_add:
-            exp, cond = to_add.pop(0)
+            exp, cond, forall_variables = to_add.pop(0)
+            assert forall_variables is not None
             if len(exp) == 0:
                 continue  # ignore the case where the effect list is empty, e.g., `:effect ()`
             op = exp[0].value
             if op == "and":
                 for i in range(1, len(exp)):
-                    to_add.append((exp[i], cond))
+                    to_add.append((exp[i], cond, forall_variables))
             elif op == "when":
                 cond = self._parse_exp(
-                    problem, act, types_map, {}, exp[1], complete_str, assignments
+                    problem, act, types_map, forall_variables, exp[1], complete_str
                 )
                 cond = cond.simplify()
                 if not cond.is_false():
-                    to_add.append((exp[2], cond))
+                    to_add.append((exp[2], cond, forall_variables))
             elif op == "not":
                 exp = exp[1]
-                eff = (
+                eff: Tuple[
+                    up.model.FNode, up.model.FNode, Union[up.model.FNode, bool]
+                ] = (
                     self._parse_exp(
-                        problem, act, types_map, {}, exp, complete_str, assignments
+                        problem, act, types_map, forall_variables, exp, complete_str
                     ),
                     self._em.FALSE(),
                     cond,
                 )
-                act.add_effect(*eff if timing is None else (timing, *eff))  # type: ignore
+                act.add_effect(*eff if timing is None else (timing, *eff), forall=tuple(forall_variables.values()))  # type: ignore
             elif op == "assign":
                 eff = (
                     self._parse_exp(
-                        problem, act, types_map, {}, exp[1], complete_str, assignments
+                        problem, act, types_map, forall_variables, exp[1], complete_str
                     ),
                     self._parse_exp(
-                        problem, act, types_map, {}, exp[2], complete_str, assignments
+                        problem, act, types_map, forall_variables, exp[2], complete_str
                     ),
                     cond,
                 )
-                act.add_effect(*eff if timing is None else (timing, *eff))  # type: ignore
+                act.add_effect(*eff if timing is None else (timing, *eff), forall=tuple(forall_variables.values()))  # type: ignore
             elif op == "increase":
                 eff = (
                     self._parse_exp(
-                        problem, act, types_map, {}, exp[1], complete_str, assignments
+                        problem, act, types_map, forall_variables, exp[1], complete_str
                     ),
                     self._parse_exp(
-                        problem, act, types_map, {}, exp[2], complete_str, assignments
+                        problem, act, types_map, forall_variables, exp[2], complete_str
                     ),
                     cond,
                 )
                 act.add_increase_effect(*eff if timing is None else (timing, *eff))  # type: ignore
             elif op == "decrease":
                 eff = (
                     self._parse_exp(
-                        problem, act, types_map, {}, exp[1], complete_str, assignments
+                        problem, act, types_map, forall_variables, exp[1], complete_str
                     ),
                     self._parse_exp(
-                        problem, act, types_map, {}, exp[2], complete_str, assignments
+                        problem, act, types_map, forall_variables, exp[2], complete_str
                     ),
                     cond,
                 )
                 act.add_decrease_effect(*eff if timing is None else (timing, *eff))  # type: ignore
             elif op == "forall":
                 assert isinstance(exp, CustomParseResults)
-                # Get the list of universal_assignments linked to this action. If it does not exist, default it to the empty list
-                assert universal_assignments is not None
-                action_assignments = universal_assignments.setdefault(act, [])
-                action_assignments.append(exp)
+                if forall_variables:
+                    raise UPUnsupportedProblemTypeError(
+                        "Nested forall on effects are not supported."
+                    )
+                forall_variables = forall_variables.copy()
+                vars_string = " ".join([e.value for e in exp[1]])
+                vars_res = self._pp_parameters.parseString(vars_string)
+                for g in vars_res["params"]:
+                    t = types_map[g.value[1] if len(g.value) > 1 else Object]
+                    for o in g.value[0]:
+                        forall_variables[o] = up.model.Variable(o, t)
+                to_add.append((exp[2], cond, forall_variables))
             else:
                 eff = (
                     self._parse_exp(
-                        problem, act, types_map, {}, exp, complete_str, assignments
+                        problem, act, types_map, forall_variables, exp, complete_str
                     ),
                     self._em.TRUE(),
                     cond,
                 )
-                act.add_effect(*eff if timing is None else (timing, *eff))  # type: ignore
+                act.add_effect(*eff if timing is None else (timing, *eff), forall=tuple(forall_variables.values()))  # type: ignore
 
     def _add_condition(
         self,
         problem: up.model.Problem,
         act: up.model.DurativeAction,
         exp: CustomParseResults,
         types_map: TypesMap,
@@ -738,54 +744,60 @@
                 )
 
     def _add_timed_effects(
         self,
         problem: up.model.Problem,
         act: up.model.DurativeAction,
         types_map: TypesMap,
-        universal_assignments: typing.Optional[
-            Dict["up.model.Action", List[CustomParseResults]]
-        ],
         eff: CustomParseResults,
         complete_str: str,
-        assignments: Dict[str, "up.model.Object"] = {},
     ):
-        to_add = [eff]
+        to_add: List[Tuple[CustomParseResults, Dict[str, up.model.Variable]]] = [
+            (eff, {})
+        ]
         while to_add:
-            eff = to_add.pop(0)
+            eff, forall_variables = to_add.pop(0)
             op = eff[0].value
             if op == "and":
                 for i in range(1, len(eff)):
-                    to_add.append(eff[i])
+                    to_add.append((eff[i], forall_variables))
             elif len(eff) == 3 and op == "at" and eff[1].value == "start":
                 self._add_effect(
                     problem,
                     act,
                     types_map,
-                    universal_assignments,
                     eff[2],
                     complete_str,
                     timing=up.model.StartTiming(),
-                    assignments=assignments,
+                    forall_variables=forall_variables,
                 )
             elif len(eff) == 3 and op == "at" and eff[1].value == "end":
                 self._add_effect(
                     problem,
                     act,
                     types_map,
-                    universal_assignments,
                     eff[2],
                     complete_str,
                     timing=up.model.EndTiming(),
-                    assignments=assignments,
+                    forall_variables=forall_variables,
                 )
             elif len(eff) == 3 and op == "forall":
-                assert universal_assignments is not None
-                action_assignments = universal_assignments.setdefault(act, [])
-                action_assignments.append(eff)
+                assert isinstance(eff, CustomParseResults)
+                if forall_variables:
+                    raise UPUnsupportedProblemTypeError(
+                        "Nested forall on effects are not supported."
+                    )
+                forall_variables = forall_variables.copy()
+                vars_string = " ".join([e.value for e in eff[1]])
+                vars_res = self._pp_parameters.parseString(vars_string)
+                for g in vars_res["params"]:
+                    t = types_map[g.value[1] if len(g.value) > 1 else Object]
+                    for o in g.value[0]:
+                        forall_variables[o] = up.model.Variable(o, t)
+                to_add.append((eff[2], forall_variables))
             else:
                 start_line, start_col = eff.line_start(complete_str), eff.col_start(
                     complete_str
                 )
                 end_line, end_col = eff.line_end(complete_str), eff.col_end(
                     complete_str
                 )
@@ -973,15 +985,14 @@
                 domain_res["name"],
                 self._env,
                 initial_defaults={self._tm.BoolType(): self._em.FALSE()},
             )
 
         types_map: TypesMap = {}
         object_type_needed: bool = self._check_if_object_type_is_needed(domain_res)
-        universal_assignments: Dict["up.model.Action", List[CustomParseResults]] = {}
 
         # extract all type declarations into a dictionary
         type_declarations: Dict[str, typing.Optional[str]] = {}
         for type_line in domain_res.get("types", []):
             father_name = None if len(type_line) <= 1 else str(type_line[1])
             if father_name is None and object_type_needed:
                 father_name = Object
@@ -1187,17 +1198,15 @@
                     raise SyntaxError(
                         f"Not able to handle duration constraint of action {n}"
                         + f"Line: {dur.line_start(domain_str)}, col: {dur.col_start(domain_str)}",
                     )
                 cond = CustomParseResults(a["cond"][0])
                 self._add_condition(problem, dur_act, cond, types_map, domain_str)
                 eff = CustomParseResults(a["eff"][0])
-                self._add_timed_effects(
-                    problem, dur_act, types_map, universal_assignments, eff, domain_str
-                )
+                self._add_timed_effects(problem, dur_act, types_map, eff, domain_str)
                 problem.add_action(dur_act)
                 has_actions_cost = has_actions_cost and self._durative_action_has_cost(
                     dur_act
                 )
             else:
                 act: typing.Optional[
                     Union[up.model.SensingAction, up.model.InstantaneousAction]
@@ -1237,15 +1246,14 @@
                         )
                     )
                 if "eff" in a:
                     self._add_effect(
                         problem,
                         act,
                         types_map,
-                        universal_assignments,
                         CustomParseResults(a["eff"][0]),
                         domain_str,
                     )
                 problem.add_action(act)
                 has_actions_cost = (
                     has_actions_cost and self._instantaneous_action_has_cost(act)
                 )
@@ -1329,58 +1337,14 @@
             problem.name = problem_res["name"]
 
             for g in problem_res.get("objects", []):
                 t = types_map[g[1] if len(g) > 1 else Object]
                 for o in g[0]:
                     problem.add_object(up.model.Object(o, t, problem.environment))
 
-            for action, eff_list in universal_assignments.items():
-                for eff in eff_list:
-                    # Parse the variable definition part and create 2 lists, the first one with the variable names,
-                    # the second one with the variable types.
-                    vars_string = " ".join([e.value for e in eff[1]])
-                    vars_res = self._pp_parameters.parseString(vars_string)
-                    var_names: List[str] = []
-                    var_types: List["up.model.Type"] = []
-                    for g in vars_res["params"]:
-                        t = types_map[g.value[1] if len(g.value) > 1 else Object]
-                        for o in g.value[0]:
-                            var_names.append(f"?{o}")
-                            var_types.append(t)
-                    # for each variable type, get all the objects of that type and calculate the cartesian
-                    # product between all the given objects and iterate over them, changing the variable assignments
-                    # in the added effect
-                    for objects in product(*(problem.objects(t) for t in var_types)):
-                        assert len(var_names) == len(objects)
-                        assignments = {
-                            name: obj for name, obj in zip(var_names, objects)
-                        }
-                        if isinstance(action, up.model.InstantaneousAction):
-                            self._add_effect(
-                                problem,
-                                action,
-                                types_map,
-                                None,
-                                eff[2],
-                                domain_str,
-                                assignments=assignments,
-                            )
-                        elif isinstance(action, up.model.DurativeAction):
-                            self._add_timed_effects(
-                                problem,
-                                action,
-                                types_map,
-                                None,
-                                eff[2],
-                                domain_str,
-                                assignments=assignments,
-                            )
-                        else:
-                            raise NotImplementedError
-
             tasknet = problem_res.get("htn", None)
             if tasknet is not None:
                 assert isinstance(problem, htn.HierarchicalProblem)
 
                 for tn_variables in tasknet.get("params", []):
                     tn_var_type = types_map[
                         tn_variables.value[1] if len(tn_variables.value) > 1 else Object
@@ -1640,19 +1604,14 @@
                             )
                         elif optimization == "maximize":
                             problem.add_quality_metric(
                                 up.model.metrics.MaximizeExpressionOnFinalState(
                                     metric_exp
                                 )
                             )
-        else:
-            if len(universal_assignments) != 0:
-                raise UPUsageError(
-                    "The domain has quantified assignments. In the unified_planning library this is compatible only if the problem is given and not only the domain."
-                )
         return problem
 
     def parse_problem(
         self, domain_filename: str, problem_filename: typing.Optional[str] = None
     ) -> "up.model.Problem":
         """
         Takes in input a filename containing the `PDDL` domain and optionally a filename
@@ -1701,7 +1660,120 @@
         if problem_str is not None:
             problem_str = problem_str.replace("\t", " ").lower()
             problem_res = parse_string(self._pp_problem, problem_str, parse_all=True)
         else:
             problem_res = None
 
         return self._parse_problem(domain_res, domain_str, problem_res, problem_str)
+
+    def parse_plan(
+        self,
+        problem: "up.model.Problem",
+        plan_filename: str,
+        get_item_named: typing.Optional[
+            Callable[
+                [str],
+                Union[
+                    "up.model.Type",
+                    "up.model.Action",
+                    "up.model.Fluent",
+                    "up.model.Object",
+                    "up.model.Parameter",
+                    "up.model.Variable",
+                    "up.model.multi_agent.Agent",
+                ],
+            ]
+        ] = None,
+    ) -> "up.plans.Plan":
+        """
+        Takes a problem, a filename and optionally a map of renaming and returns the plan parsed from the file.
+
+        :param problem: The up.model.problem.Problem instance for which the plan is generated.
+        :param plan_filename: The path of the file in which the plan is written.
+        :param get_item_named: A function that takes a name and returns the original up.model element instance
+            linked to that renaming; if None the problem is used to retrieve the actions and objects in the
+            plan from their name.
+        :return: The up.plans.Plan corresponding to the parsed plan from the file
+        """
+        with open(plan_filename) as plan:
+            return self.parse_plan_string(problem, plan.read(), get_item_named)
+
+    def parse_plan_string(
+        self,
+        problem: "up.model.Problem",
+        plan_str: str,
+        get_item_named: typing.Optional[
+            Callable[
+                [str],
+                Union[
+                    "up.model.Type",
+                    "up.model.Action",
+                    "up.model.Fluent",
+                    "up.model.Object",
+                    "up.model.Parameter",
+                    "up.model.Variable",
+                    "up.model.multi_agent.Agent",
+                ],
+            ]
+        ] = None,
+    ) -> "up.plans.Plan":
+        """
+        Takes a problem, a string and optionally a map of renaming and returns the plan parsed from the string.
+
+        :param problem: The up.model.problem.Problem instance for which the plan is generated.
+        :param plan_str: The plan in string.
+        :param get_item_named: A function that takes a name and returns the original up.model element instance
+            linked to that renaming; if None the problem is used to retrieve the actions and objects in the
+            plan from their name.:return: The up.plans.Plan corresponding to the parsed plan from the string
+        """
+        actions: List = []
+        is_tt = False
+        for line in plan_str.splitlines():
+            if re.match(r"^\s*(;.*)?$", line):
+                continue
+            line = line.lower()
+            s_ai = re.match(r"^\s*\(\s*([\w?-]+)((\s+[\w?-]+)*)\s*\)\s*$", line)
+            t_ai = re.match(
+                r"^\s*(\d+)\s*:\s*\(\s*([\w?-]+)((\s+[\w?-]+)*)\s*\)\s*(\[\s*(\d+)\s*\])?\s*$",
+                line,
+            )
+            if s_ai:
+                assert is_tt == False
+                name = s_ai.group(1)
+                params_name = s_ai.group(2).split()
+            elif t_ai:
+                is_tt = True
+                start = Fraction(t_ai.group(1))
+                name = t_ai.group(2)
+                params_name = t_ai.group(3).split()
+                dur = None
+                if t_ai.group(6) is not None:
+                    dur = Fraction(t_ai.group(6))
+            else:
+                raise UPException(
+                    "Error parsing plan generated by " + self.__class__.__name__
+                )
+
+            action = (
+                get_item_named(name)
+                if get_item_named is not None
+                else problem.action(name)
+            )
+            assert isinstance(action, up.model.Action), "Wrong plan or renaming."
+            parameters = []
+            for p in params_name:
+                obj = (
+                    get_item_named(p)
+                    if get_item_named is not None
+                    else problem.object(p)
+                )
+                assert isinstance(obj, up.model.Object), "Wrong plan or renaming."
+                parameters.append(problem.environment.expression_manager.ObjectExp(obj))
+            act_instance = up.plans.ActionInstance(action, tuple(parameters))
+            if is_tt:
+                actions.append((start, act_instance, dur))
+            else:
+                actions.append(act_instance)
+        if is_tt:
+            return up.plans.TimeTriggeredPlan(actions)
+        else:
+            return up.plans.SequentialPlan(actions)
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/io/pddl_writer.py` & `unified_planning-1.0.0/unified_planning/io/pddl_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,14 +36,20 @@
 )
 from unified_planning.exceptions import (
     UPTypeError,
     UPProblemDefinitionError,
     UPException,
 )
 from unified_planning.model.types import _UserType
+from unified_planning.plans import (
+    SequentialPlan,
+    TimeTriggeredPlan,
+    Plan,
+    ActionInstance,
+)
 from typing import Callable, Dict, IO, List, Optional, Set, Union, cast
 from io import StringIO
 from functools import reduce
 
 PDDL_KEYWORDS = {
     "define",
     "domain",
@@ -173,14 +179,15 @@
         get_mangled_name: Callable[
             [
                 Union[
                     "up.model.Type",
                     "up.model.Action",
                     "up.model.Fluent",
                     "up.model.Object",
+                    "up.model.multi_agent.Agent",
                 ]
             ],
             str,
         ],
     ):
         walkers.DagWalker.__init__(self)
         self.get_mangled_name = get_mangled_name
@@ -341,27 +348,29 @@
             Union[
                 "up.model.Type",
                 "up.model.Action",
                 "up.model.Fluent",
                 "up.model.Object",
                 "up.model.Parameter",
                 "up.model.Variable",
+                "up.model.multi_agent.Agent",
             ],
             str,
         ] = {}
         # nto represents the new to old renamings
         self.nto_renamings: Dict[
             str,
             Union[
                 "up.model.Type",
                 "up.model.Action",
                 "up.model.Fluent",
                 "up.model.Object",
                 "up.model.Parameter",
                 "up.model.Variable",
+                "up.model.multi_agent.Agent",
             ],
         ] = {}
         # those 2 maps are "simmetrical", meaning that "(otn[k] == v) implies (nto[v] == k)"
         self.domain_objects: Optional[Dict[_UserType, Set[Object]]] = None
 
     def _write_domain(self, out: IO[str]):
         if self.problem_kind.has_intermediate_conditions_and_effects():
@@ -536,26 +545,32 @@
                         out.write(
                             f" {self._get_mangled_name(ap)} - {self._get_mangled_name(ap.type)}"
                         )
                     else:
                         raise UPTypeError("PDDL supports only user type parameters")
                 out.write(")")
                 if len(a.preconditions) > 0:
-                    out.write(
-                        f'\n  :precondition (and {" ".join([converter.convert(p) for p in (c.simplify() for c in a.preconditions) if not p.is_true()])})'
-                    )
+                    precond_str: List[str] = []
+                    for p in (c.simplify() for c in a.preconditions):
+                        if not p.is_true():
+                            if p.is_and():
+                                precond_str.extend(map(converter.convert, p.args))
+                            else:
+                                precond_str.append(converter.convert(p))
+                    out.write(f'\n  :precondition (and {" ".join(precond_str)})')
                 if len(a.effects) > 0:
                     out.write("\n  :effect (and")
                     for e in a.effects:
                         _write_effect(
                             e,
                             None,
                             out,
                             converter,
                             self.rewrite_bool_assignments,
+                            self._get_mangled_name,
                         )
 
                     if a in costs:
                         out.write(
                             f" (increase (total-cost) {converter.convert(costs[a])})"
                         )
                     out.write(")")
@@ -613,14 +628,15 @@
                         for e in el:
                             _write_effect(
                                 e,
                                 t,
                                 out,
                                 converter,
                                 self.rewrite_bool_assignments,
+                                self._get_mangled_name,
                             )
                     if a in costs:
                         out.write(
                             f" (at end (increase (total-cost) {converter.convert(costs[a])}))"
                         )
                     out.write(")")
                 out.write(")\n")
@@ -668,17 +684,21 @@
             elif v.is_false():
                 pass
             else:
                 out.write(f" (= {converter.convert(f)} {converter.convert(v)})")
         if self.problem.kind.has_actions_cost():
             out.write(f" (= (total-cost) 0)")
         out.write(")\n")
-        out.write(
-            f' (:goal (and {" ".join([converter.convert(p) for p in self.problem.goals])}))\n'
-        )
+        goals_str: List[str] = []
+        for g in (c.simplify() for c in self.problem.goals):
+            if g.is_and():
+                goals_str.extend(map(converter.convert, g.args))
+            else:
+                goals_str.append(converter.convert(g))
+        out.write(f' (:goal (and {" ".join(goals_str)}))\n')
         if len(self.problem.trajectory_constraints) > 0:
             out.write(
                 f' (:constraints {" ".join([converter.convert(c) for c in self.problem.trajectory_constraints])})\n'
             )
         metrics = self.problem.quality_metrics
         if len(metrics) == 1:
             metric = metrics[0]
@@ -705,53 +725,90 @@
             out.write(")\n")
         elif len(metrics) > 1:
             raise up.exceptions.UPUnsupportedProblemTypeError(
                 "Only one metric is supported!"
             )
         out.write(")\n")
 
+    def _write_plan(self, plan: Plan, out: IO[str]):
+        def _format_action_instance(action_instance: ActionInstance) -> str:
+            param_str = ""
+            if action_instance.actual_parameters:
+                param_str = f" {' '.join((p.object().name for p in action_instance.actual_parameters))}"
+            return f"({action_instance.action.name}{param_str})"
+
+        if isinstance(plan, SequentialPlan):
+            for ai in plan.actions:
+                out.write(f"{_format_action_instance(ai)}\n")
+        elif isinstance(plan, TimeTriggeredPlan):
+            for s, ai, dur in plan.timed_actions:
+                start = s.numerator if s.denominator == 1 else float(s)
+                out.write(f"{start}: {_format_action_instance(ai)}")
+                if dur is not None:
+                    duration = dur.numerator if dur.denominator == 1 else float(dur)
+                    out.write(f"[{duration}]")
+                out.write("\n")
+        else:
+            raise NotImplementedError
+
     def print_domain(self):
         """Prints to std output the `PDDL` domain."""
         self._write_domain(sys.stdout)
 
     def print_problem(self):
         """Prints to std output the `PDDL` problem."""
         self._write_problem(sys.stdout)
 
+    def print_plan(self, plan: Plan):
+        """Prints to std output the `PDDL` plan."""
+        self._write_plan(plan, sys.stdout)
+
     def get_domain(self) -> str:
         """Returns the `PDDL` domain."""
         out = StringIO()
         self._write_domain(out)
         return out.getvalue()
 
     def get_problem(self) -> str:
         """Returns the `PDDL` problem."""
         out = StringIO()
         self._write_problem(out)
         return out.getvalue()
 
+    def get_plan(self, plan: Plan) -> str:
+        """Returns the `PDDL` plan."""
+        out = StringIO()
+        self._write_plan(plan, out)
+        return out.getvalue()
+
     def write_domain(self, filename: str):
         """Dumps to file the `PDDL` domain."""
         with open(filename, "w") as f:
             self._write_domain(f)
 
     def write_problem(self, filename: str):
         """Dumps to file the `PDDL` problem."""
         with open(filename, "w") as f:
             self._write_problem(f)
 
+    def write_plan(self, plan: Plan, filename: str):
+        """Dumps to file the `PDDL` plan."""
+        with open(filename, "w") as f:
+            self._write_plan(plan, f)
+
     def _get_mangled_name(
         self,
         item: Union[
             "up.model.Type",
             "up.model.Action",
             "up.model.Fluent",
             "up.model.Object",
             "up.model.Parameter",
             "up.model.Variable",
+            "up.model.multi_agent.Agent",
         ],
     ) -> str:
         """This function returns a valid and unique PDDL name."""
 
         # If we already encountered this item, return it
         if item in self.otn_renamings:
             return self.otn_renamings[item]
@@ -789,14 +846,15 @@
     ) -> Union[
         "up.model.Type",
         "up.model.Action",
         "up.model.Fluent",
         "up.model.Object",
         "up.model.Parameter",
         "up.model.Variable",
+        "up.model.multi_agent.Agent",
     ]:
         """
         Since `PDDL` has a stricter set of possible naming compared to the `unified_planning`, when writing
         a :class:`~unified_planning.model.Problem` it is possible that some things must be renamed. This is why the `PDDLWriter`
         offers this method, that takes a `PDDL` name and returns the original `unified_planning` data structure that corresponds
         to the `PDDL` entity with the given name.
 
@@ -871,14 +929,15 @@
         "up.model.Type",
         "up.model.Action",
         "up.model.Fluent",
         "up.model.Object",
         "up.model.Parameter",
         "up.model.Variable",
         "up.model.Problem",
+        "up.model.multi_agent.Agent",
     ]
 ) -> str:
     """This function returns a pddl name for the chosen item"""
     name = item.name  # type: ignore
     assert name is not None
     name = name.lower()
     regex = re.compile(r"^[a-zA-Z]+.*")
@@ -908,14 +967,28 @@
 
 def _write_effect(
     effect: Effect,
     timing: Optional[Timing],
     out: IO[str],
     converter: ConverterToPDDLString,
     rewrite_bool_assignments: bool,
+    get_mangled_name: Callable[
+        [
+            Union[
+                "up.model.Type",
+                "up.model.Action",
+                "up.model.Fluent",
+                "up.model.Object",
+                "up.model.Parameter",
+                "up.model.Variable",
+                "up.model.multi_agent.Agent",
+            ]
+        ],
+        str,
+    ],
 ):
     simplified_cond = effect.condition.simplify()
     # check for non-constant-bool-assignment
     non_const_bool_ass = (
         effect.value.type.is_bool_type()
         and not effect.value.is_true()
         and not effect.value.is_false()
@@ -923,51 +996,67 @@
     if non_const_bool_ass and not rewrite_bool_assignments:
         raise UPProblemDefinitionError(
             "The problem has non-constant boolean assignments.This can't be directly written ",
             "in PDDL, but it can be translated into a conditional effect maintaining the ",
             "semantic. To enable this feature, set the flag rewrite_bool_assignments",
             " to True in the PDDLWriter constructor.",
         )
+    forall_str = ""
+    if effect.is_forall():
+        mid_str = " ".join(
+            (
+                f"{get_mangled_name(v)} - {get_mangled_name(v.type)}"
+                for v in effect.forall
+            )
+        )
+        forall_str = f"(forall ({mid_str})"
     simplified_cond = effect.condition.simplify()
     if non_const_bool_ass:
         assert effect.is_assignment()
         positive_cond = (simplified_cond & effect.value).simplify()
         if not positive_cond.is_false():
+            out.write(forall_str)
             if timing is not None:
                 if timing.is_from_start():
                     out.write(f" (at start")
                 else:
                     out.write(f" (at end")
             if positive_cond.is_true():
                 out.write(f" {converter.convert(effect.fluent)}")
             else:
                 out.write(
                     f" (when {converter.convert(positive_cond)} {converter.convert(effect.fluent)})"
                 )
             if timing is not None:
                 out.write(")")
+            if effect.is_forall():
+                out.write(")")
         negative_cond = (simplified_cond & effect.value.Not()).simplify()
         if not negative_cond.is_false():
+            out.write(forall_str)
             if timing is not None:
                 if timing.is_from_start():
                     out.write(f" (at start")
                 else:
                     out.write(f" (at end")
             if negative_cond.is_true():
                 out.write(f" {converter.convert(effect.fluent)}")
             else:
                 out.write(
                     f" (when {converter.convert(negative_cond)} (not {converter.convert(effect.fluent)}))"
                 )
             if timing is not None:
                 out.write(")")
+            if effect.is_forall():
+                out.write(")")
         return
 
     if simplified_cond.is_false():
         return
+    out.write(forall_str)
     if timing is not None:
         if timing.is_from_start():
             out.write(f" (at start")
         else:
             out.write(f" (at end")
     if not simplified_cond.is_true():
         out.write(f" (when {converter.convert(effect.condition)}")
@@ -988,7 +1077,9 @@
         out.write(
             f" (assign {converter.convert(effect.fluent)} {converter.convert(simplified_value)})"
         )
     if not simplified_cond.is_true():
         out.write(")")
     if timing is not None:
         out.write(")")
+    if effect.is_forall():
+        out.write(")")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/io/utils.py` & `unified_planning-1.0.0/unified_planning/io/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,28 +11,37 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 import pyparsing
+from typing import Union, Sequence, List
 
 
 def parse_string(obj, problem_str, parse_all):
     if pyparsing.__version__ < "3.0.0":
         return obj.parseString(problem_str, parseAll=parse_all)
     else:
         return obj.parse_string(problem_str, parse_all=parse_all)
 
 
-def parse_file(obj, problem_str, parse_all):
-    if pyparsing.__version__ < "3.0.0":
-        return obj.parseFile(problem_str, parseAll=parse_all)
+def parse_file(obj, problem_filename: Union[str, Sequence[str]], parse_all):
+    if isinstance(problem_filename, str):
+        if pyparsing.__version__ < "3.0.0":
+            return obj.parseFile(problem_filename, parseAll=parse_all)
+        else:
+            return obj.parse_file(problem_filename, parse_all=parse_all)
     else:
-        return obj.parse_file(problem_str, parse_all=parse_all)
+        problem_parts: List[str] = []
+        for filename in problem_filename:
+            assert isinstance(filename, str), "Typing not respected"
+            with open(filename) as file:
+                problem_parts.append(file.read())
+        return parse_string(obj, "\n".join(problem_parts), parse_all)
 
 
 def set_results_name(obj, name):
     if pyparsing.__version__ < "3.0.0":
         return obj.setResultsName(name)
     else:
         return obj.set_results_name(name)
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/__init__.py` & `unified_planning-1.0.0/unified_planning/model/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/abstract_problem.py` & `unified_planning-1.0.0/unified_planning/model/abstract_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/action.py` & `unified_planning-1.0.0/unified_planning/model/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,15 +25,15 @@
     UPTypeError,
     UPUnboundedVariablesError,
     UPProblemDefinitionError,
     UPUsageError,
 )
 from unified_planning.model.mixins.timed_conds_effs import TimedCondsEffs
 from abc import ABC, abstractmethod
-from typing import Dict, List, Set, Union, Optional, Iterable
+from typing import Any, Dict, List, Set, Union, Optional, Iterable
 from collections import OrderedDict
 
 
 class Action(ABC):
     """This is the `Action` interface."""
 
     def __init__(
@@ -70,14 +70,27 @@
     def __eq__(self, oth: object) -> bool:
         raise NotImplementedError
 
     @abstractmethod
     def __hash__(self) -> int:
         raise NotImplementedError
 
+    def __call__(
+        self,
+        *args: "up.model.Expression",
+        agent: Optional["up.model.multi_agent.Agent"] = None,
+        motion_paths: Optional[
+            Dict["up.model.tamp.MotionConstraint", "up.model.tamp.Path"]
+        ] = None,
+    ) -> "up.plans.plan.ActionInstance":
+        params = tuple(args)
+        return up.plans.plan.ActionInstance(
+            self, params, agent=agent, motion_paths=motion_paths
+        )
+
     @abstractmethod
     def clone(self):
         raise NotImplementedError
 
     @property
     def environment(self) -> Environment:
         """Returns this `Action` `Environment`."""
@@ -303,22 +316,25 @@
             self._preconditions.append(precondition_exp)
 
     def add_effect(
         self,
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         Adds the given `assignment` to the `action's effects`.
 
         :param fluent: The `fluent` of which `value` is modified by the `assignment`.
         :param value: The `value` to assign to the given `fluent`.
         :param condition: The `condition` in which this `effect` is applied; the default
             value is `True`.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
         ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
         if not fluent_exp.is_fluent_exp() and not fluent_exp.is_dot():
@@ -329,36 +345,43 @@
             raise UPTypeError("Effect condition is not a Boolean condition!")
         if not fluent_exp.type.is_compatible(value_exp.type):
             # Value is not assignable to fluent (its type is not a subset of the fluent's type).
             raise UPTypeError(
                 f"InstantaneousAction effect has an incompatible value type. Fluent type: {fluent_exp.type} // Value type: {value_exp.type}"
             )
         self._add_effect_instance(
-            up.model.effect.Effect(fluent_exp, value_exp, condition_exp)
+            up.model.effect.Effect(fluent_exp, value_exp, condition_exp, forall=forall)
         )
 
     def add_increase_effect(
         self,
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         Adds the given `increase effect` to the `action's effects`.
 
         :param fluent: The `fluent` which `value` is increased.
         :param value: The given `fluent` is incremented by the given `value`.
         :param condition: The `condition` in which this `effect` is applied; the default
             value is `True`.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
-        ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
+        ) = self._environment.expression_manager.auto_promote(
+            fluent,
+            value,
+            condition,
+        )
         if not fluent_exp.is_fluent_exp() and not fluent_exp.is_dot():
             raise UPUsageError(
                 "fluent field of add_increase_effect must be a Fluent or a FluentExp or a Dot."
             )
         if not condition_exp.type.is_bool_type():
             raise UPTypeError("Effect condition is not a Boolean condition!")
         if not fluent_exp.type.is_compatible(value_exp.type):
@@ -369,30 +392,34 @@
             raise UPTypeError("Increase effects can be created only on numeric types!")
         self._add_effect_instance(
             up.model.effect.Effect(
                 fluent_exp,
                 value_exp,
                 condition_exp,
                 kind=up.model.effect.EffectKind.INCREASE,
+                forall=forall,
             )
         )
 
     def add_decrease_effect(
         self,
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         Adds the given `decrease effect` to the `action's effects`.
 
         :param fluent: The `fluent` which value is decreased.
         :param value: The given `fluent` is decremented by the given `value`.
         :param condition: The `condition` in which this `effect` is applied; the default
             value is `True`.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
         ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
         if not fluent_exp.is_fluent_exp() and not fluent_exp.is_dot():
@@ -409,14 +436,15 @@
             raise UPTypeError("Decrease effects can be created only on numeric types!")
         self._add_effect_instance(
             up.model.effect.Effect(
                 fluent_exp,
                 value_exp,
                 condition_exp,
                 kind=up.model.effect.EffectKind.DECREASE,
+                forall=forall,
             )
         )
 
     def _add_effect_instance(self, effect: "up.model.effect.Effect"):
         assert (
             effect.environment == self._environment
         ), "effect does not have the same environment of the action"
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/contingent_problem.py` & `unified_planning-1.0.0/unified_planning/model/contingent_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/delta_stn.py` & `unified_planning-1.0.0/unified_planning/model/delta_stn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/effect.py` & `unified_planning-1.0.0/unified_planning/model/effect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,21 +15,23 @@
 """
 This module defines the `Effect` class.
 A basic `Effect` has a `fluent` and an `expression`.
 A `condition` can be added to make it a `conditional effect`.
 """
 
 
+from itertools import product
 import unified_planning as up
 from unified_planning.exceptions import (
     UPConflictingEffectsException,
     UPProblemDefinitionError,
+    UPUnboundedVariablesError,
 )
 from enum import Enum, auto
-from typing import List, Callable, Dict, Optional, Set, Union
+from typing import List, Callable, Dict, Optional, Set, Union, Iterable, Tuple, Iterator
 
 
 class EffectKind(Enum):
     """
     The `Enum` representing the possible `Effects` in the `unified_planning`.
 
     The semantic is the following of an `effect` with fluent `F`, value `V` and condition `C`:
@@ -52,33 +54,61 @@
 
     def __init__(
         self,
         fluent: "up.model.fnode.FNode",
         value: "up.model.fnode.FNode",
         condition: "up.model.fnode.FNode",
         kind: EffectKind = EffectKind.ASSIGN,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         fve = fluent.environment.free_vars_extractor
         fluents_in_fluent = fve.get(fluent)
         fluents_in_fluent.remove(fluent)
         if fluents_in_fluent:
             raise UPProblemDefinitionError(
                 f"The fluent: {fluent} contains other fluents in his arguments: {fluents_in_fluent}"
             )
         self._fluent = fluent
         self._value = value
         self._condition = condition
         self._kind = kind
+        fvo = fluent.environment.free_vars_oracle
+        free_vars: Set["up.model.variable.Variable"] = fvo.get_free_variables(fluent)
+        free_vars.update(fvo.get_free_variables(value))
+        free_vars.update(fvo.get_free_variables(condition))
+
+        def free_vars_without_duplicates() -> Iterator["up.model.variable.Variable"]:
+            # store seen variables to avoid duplicates
+            seen: Set["up.model.variable.Variable"] = set()
+            for v in forall:
+                if v in free_vars and not v in seen:
+                    seen.add(v)
+                    assert isinstance(
+                        v, up.model.variable.Variable
+                    ), "Typing not respected"
+                    yield v
+            unbounded_vars = free_vars.difference(seen)
+            if unbounded_vars:
+                raise UPUnboundedVariablesError(
+                    f"Some variables in the effect are unbounded: {unbounded_vars}"
+                )
+
+        self._forall: Tuple["up.model.variable.Variable", ...] = tuple(
+            free_vars_without_duplicates()
+        )
         assert (
             fluent.environment == value.environment
             and value.environment == condition.environment
+            and all(fluent.environment == v.environment for v in self._forall)
         ), "Effect expressions have different environment."
 
     def __repr__(self) -> str:
         s = []
+        if self.is_forall():
+            s.append(f"forall {', '.join(str(v) for v in self._forall)}")
         if self.is_conditional():
             s.append(f"if {str(self._condition)} then")
         s.append(f"{str(self._fluent)}")
         if self.is_assignment():
             s.append(":=")
         elif self.is_increase():
             s.append("+=")
@@ -90,30 +120,40 @@
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, Effect):
             return (
                 self._fluent == oth._fluent
                 and self._value == oth._value
                 and self._condition == oth._condition
                 and self._kind == oth._kind
+                and set(self._forall) == set(oth._forall)
             )
         else:
             return False
 
     def __hash__(self) -> int:
         return (
             hash(self._fluent)
             + hash(self._value)
             + hash(self._condition)
             + hash(self._kind)
+            + sum(map(hash, self._forall))
         )
 
     def clone(self):
-        new_effect = Effect(self._fluent, self._value, self._condition, self._kind)
+        new_effect = Effect(
+            self._fluent, self._value, self._condition, self._kind, self._forall
+        )
         return new_effect
 
+    def is_forall(self) -> bool:
+        """
+        Returns `True` if the `Effect` is a `forall` effect; this means that the `Effect`
+        is applied for the instances of all the specified `Variables`."""
+        return len(self._forall) > 0
+
     def is_conditional(self) -> bool:
         """
         Returns `True` if the `Effect` condition is not `True`; this means that the `Effect` might
         not always be applied but depends on the runtime evaluation of it's :func:`condition <unified_planning.model.Effect.condition>`.
         """
         return not self._condition.is_true()
 
@@ -150,14 +190,47 @@
 
     @property
     def kind(self) -> EffectKind:
         """Returns the `kind` of this `Effect`."""
         return self._kind
 
     @property
+    def forall(self) -> Tuple["up.model.variable.Variable", ...]:
+        """Returns the `Variables` that are universally quantified in this `Effect`."""
+        return self._forall
+
+    def expand_effect(
+        self, objects_set: "up.model.mixins.objects_set.ObjectsSetMixin"
+    ) -> Iterator["up.model.Effect"]:
+        """
+        Expands this effect removing the forall and returns all the effects
+        that are needed in order to maintain semantic equivalence with self.
+
+        :param objects_set: The container of the objects needed to expand this effect.
+        :return: The Iterator over all the effects needed to maintain semantic
+            equivalence with self.
+        """
+        if self.is_forall():
+            for objects in product(
+                *(objects_set.objects(v.type) for v in self._forall)
+            ):
+                assert len(self._forall) == len(objects)
+                subs: Dict[
+                    "up.model.expression.Expression", "up.model.expression.Expression"
+                ] = dict(zip(self._forall, objects))
+                yield up.model.Effect(
+                    fluent=self.fluent.substitute(subs),
+                    value=self.value.substitute(subs),
+                    condition=self.condition.substitute(subs),
+                    kind=self.kind,
+                )
+        else:
+            yield self
+
+    @property
     def environment(self) -> "up.environment.Environment":
         """Returns this `Effect's Environment`."""
         return self._fluent.environment
 
     def is_assignment(self) -> bool:
         """Returns `True` if the :func:`kind <unified_planning.model.Effect.kind>` of this `Effect` is an `assignment`, `False` otherwise."""
         return self._kind == EffectKind.ASSIGN
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/expression.py` & `unified_planning-1.0.0/unified_planning/model/expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -34,22 +34,29 @@
     "up.model.fnode.FNode",
     "up.model.fluent.Fluent",
     "up.model.parameter.Parameter",
     "up.model.variable.Variable",
     bool,
 ]
 NumericConstant = Union[int, float, Fraction, str]
-NumericExpression = Union["up.model.fnode.FNode", NumericConstant]
+NumericExpression = Union[NumericConstant, "up.model.fnode.FNode"]
 ConstantExpression = Union[
     NumericExpression,
     "up.model.object.Object",
     bool,
 ]
-Expression = Union[
+TimeExpression = Union[
     "up.model.timing.Timing",
+    "up.model.timing.Timepoint",
+    int,
+    float,
+    Fraction,
+]
+Expression = Union[
+    TimeExpression,
     BoolExpression,
     ConstantExpression,
 ]
 
 
 def uniform_numeric_constant(value: NumericConstant) -> Union[Fraction, int]:
     """Utility method to handle NumericConstant polymorphism."""
@@ -130,14 +137,16 @@
             elif isinstance(e, up.model.object.Object):
                 assert (
                     e.environment == self.environment
                 ), "Object has a different environment of the expression manager"
                 res.append(self.ObjectExp(e))
             elif isinstance(e, up.model.timing.Timing):
                 res.append(self.TimingExp(e))
+            elif isinstance(e, up.model.timing.Timepoint):
+                res.append(self.TimingExp(up.model.timing.Timing(delay=0, timepoint=e)))
             elif isinstance(e, bool):
                 res.append(self.Bool(e))
             elif (
                 isinstance(e, int)
                 or isinstance(e, float)
                 or isinstance(e, Fraction)
                 or isinstance(e, str)
@@ -162,15 +171,15 @@
         payload: Optional[
             Union[
                 "up.model.fluent.Fluent",
                 "up.model.object.Object",
                 "up.model.parameter.Parameter",
                 "up.model.variable.Variable",
                 "up.model.timing.Timing",
-                "up.model.multi_agent.Agent",
+                str,
                 bool,
                 int,
                 Fraction,
                 Tuple["up.model.variable.Variable", ...],
             ]
         ] = None,
     ) -> "up.model.fnode.FNode":
@@ -206,15 +215,15 @@
         | This function has polymorphic n-arguments:
 
             * ``And(a,b,c)``
             * ``And([a,b,c])``
 
         | Restriction: Arguments must be ``boolean``.
 
-        :param \*args: Either an ``Iterable`` of ``boolean`` expressions, like ``[a, b, c]``, or an unpacked version
+        :param \\*args: Either an ``Iterable`` of ``boolean`` expressions, like ``[a, b, c]``, or an unpacked version
             of it, like ``a, b, c``.
         :return: The ``AND`` expression created.
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.TRUE()
@@ -231,15 +240,15 @@
         | This function has polymorphic n-arguments:
 
             * ``Or(a,b,c)``
             * ``Or([a,b,c])``
 
         | Restriction: Arguments must be ``boolean``
 
-        :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+        :param \\*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
             of it, like ``a, b, c``.
         :return: The ``OR`` expression created.
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.FALSE()
@@ -256,15 +265,15 @@
         | This function has polimorphic n-arguments:
 
             * XOr(a,b,c)
             * XOr([a,b,c])
 
         | Restriction: Arguments must be boolean
 
-        :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+        :param \\*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
             of it, like ``a, b, c``.
         :return: The exclusive disjunction in CNF form.
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.FALSE()
@@ -334,15 +343,15 @@
             ``Exists (var[0]... var[n]) | expression``
 
         Restriction: expression must be of ``boolean type`` and
         vars must be of ``Variable`` type
 
         :param expression: The main expression of the ``existential``. The expression should contain
             the given ``variables``.
-        :param \*vars: All the ``Variables`` appearing in the ``existential`` expression.
+        :param \\*vars: All the ``Variables`` appearing in the ``existential`` expression.
         :return: The created ``Existential`` expression.
         """
         expressions = tuple(self.auto_promote(expression))
         if len(vars) == 0:
             raise UPExpressionDefinitionError(
                 f"Exists of expression: {str(expression)} must be created with at least one variable, otherwise it is not needed."
             )
@@ -360,15 +369,15 @@
             ``Forall (var[0]... var[n]) | expression``
 
         Restriction: expression must be of ``boolean type`` and
         vars must be of ``Variable`` type
 
         :param expression: The main expression of the ``universal`` quantifier. The expression should contain
             the given ``variables``.
-        :param \*vars: All the ``Variables`` appearing in the ``universal`` expression.
+        :param \\*vars: All the ``Variables`` appearing in the ``universal`` expression.
         :return: The created ``Forall`` expression.
         """
         expressions = tuple(self.auto_promote(expression))
         if len(vars) == 0:
             raise UPExpressionDefinitionError(
                 f"Forall of expression: {str(expression)} must be created with at least one variable, otherwise it is not needed."
             )
@@ -466,27 +475,37 @@
             )
         return self.create_node(
             node_type=OperatorKind.FLUENT_EXP, args=tuple(params_exp), payload=fluent
         )
 
     def Dot(
         self,
-        agent: "up.model.multi_agent.Agent",
+        agent: Union["up.model.multi_agent.Agent", str],
         fluent_exp: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
     ) -> "up.model.fnode.FNode":
         """
         Creates an expression for the given ``agent`` and ``fluent_exp``.
-        Restriction: agent must be of ``agent type`` and fluent_exp must be of ``fluentExp type``
+        Restriction: agent must be of ``agent type`` or the name of an agent and
+        fluent_exp must be of ``fluentExp type``
 
         :param agent: The ``Agent`` that will be set as the ``payload`` of this expression.
         :param fluent_exp: The ``Fluent_exp`` that will be set as the ``args`` of this expression.
         :return: The created ``Dot`` Expression.
         """
-        assert agent.environment == self.environment
         (fluent_exp,) = self.auto_promote(fluent_exp)
+        assert fluent_exp.is_fluent_exp()
+        if not isinstance(agent, str):
+            assert isinstance(agent, up.model.multi_agent.Agent), "Typing not respected"
+            assert agent.environment == self.environment
+            if fluent_exp.fluent() not in agent.fluents:
+                raise UPExpressionDefinitionError(
+                    f"Fluent {fluent_exp.fluent()} does not belong to agent {agent.name}"
+                )
+            agent = agent.name
+        assert isinstance(agent, str)
         return self.create_node(
             node_type=OperatorKind.DOT, args=(fluent_exp,), payload=agent
         )
 
     def ParameterExp(
         self, param: "up.model.parameter.Parameter"
     ) -> "up.model.fnode.FNode":
@@ -587,15 +606,15 @@
     def Plus(
         self, *args: Union[Expression, Iterable[Expression]]
     ) -> "up.model.fnode.FNode":
         """
         Creates an expression of the form:
             ``args[0] + ... + args[n]``
 
-        :param \*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
+        :param \\*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
             of it, like ``a, b, 3``.
         :return: The ``PLUS`` expression created. (like ``a + b + 3``)
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.Int(0)
@@ -618,15 +637,15 @@
     def Times(
         self, *args: Union[Expression, Iterable[Expression]]
     ) -> "up.model.fnode.FNode":
         """
         Creates an expression of the form:
             ``args[0] * ... * args[n]``
 
-        :param \*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
+        :param \\*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
             of it, like ``a, b, 3``.
         :return: The ``TIMES`` expression created. (like ``a * b * 3``)
         """
         tuple_args = tuple(self.auto_promote(*args))
 
         if len(tuple_args) == 0:
             return self.Int(1)
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/fluent.py` & `unified_planning-1.0.0/unified_planning/model/fluent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/fnode.py` & `unified_planning-1.0.0/unified_planning/model/fnode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -70,15 +70,15 @@
         elif self.is_int_constant():
             return str(self.constant_value())
         elif self.is_real_constant():
             return str(self.constant_value())
         elif self.is_fluent_exp():
             return self.fluent().name + self.get_nary_expression_string(", ", self.args)
         elif self.is_dot():
-            return f"{self.agent().name}.{self.arg(0)}"
+            return f"{self.agent()}.{self.arg(0)}"
         elif self.is_parameter_exp():
             return self.parameter().name
         elif self.is_variable_exp():
             return self.variable().name
         elif self.is_object_exp():
             return self.object().name
         elif self.is_timing_exp():
@@ -221,16 +221,16 @@
         return self._content.payload
 
     def timing(self) -> "unified_planning.model.timing.Timing":
         """Return the `Timing` stored in this expression."""
         assert self.is_timing_exp()
         return self._content.payload
 
-    def agent(self) -> "unified_planning.model.multi_agent.Agent":
-        """Return the `Agent` stored in this expression."""
+    def agent(self) -> str:
+        """Return the name of the `Agent` stored in this expression."""
         assert self.is_dot()
         return self._content.payload
 
     def simplify(self) -> "FNode":
         """
         Returns the simplified version of this expression.
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/hierarchical_problem.py` & `unified_planning-1.0.0/unified_planning/model/htn/hierarchical_problem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
-from typing import Optional, List, Union, Dict
+from typing import Optional, List, Union, Dict, Set
 from warnings import warn
 
 import unified_planning as up
 from unified_planning.model.expression import ConstantExpression
 from unified_planning.model.htn.method import Method
 from unified_planning.model.htn.task import Task
 from unified_planning.model.htn.task_network import TaskNetwork, AbstractTaskNetwork
@@ -99,56 +99,75 @@
         new_p._initial_defaults = self._initial_defaults.copy()
         new_p._fluents_defaults = self._fluents_defaults.copy()
         new_p._initial_task_network = self._initial_task_network.clone()
         new_p._methods = self._methods.copy()
         new_p._abstract_tasks = self._abstract_tasks.copy()
         return new_p
 
+    def get_unused_fluents(self):
+        """
+        Returns the set of `fluents` that are never used in the problem.
+        """
+        # from our parents unused fluents, remove all those that appear in methods preconditions and constraints
+        unused_fluents: Set["up.model.fluent.Fluent"] = super().get_unused_fluents()
+        fve = self._env.free_vars_extractor
+        # function that takes an FNode and removes all the fluents contained in the given FNode
+        # from the unused_fluents  set.
+        remove_used_fluents = lambda *exps: unused_fluents.difference_update(
+            (f.fluent() for e in exps for f in fve.get(e))
+        )
+        for m in self.methods:
+            remove_used_fluents(*m.preconditions)
+            remove_used_fluents(*m.constraints)
+        remove_used_fluents(*self.task_network.constraints)
+
+        return unused_fluents
+
     @property
     def kind(self) -> "up.model.problem_kind.ProblemKind":
         """Returns the problem kind of this planning problem.
 
         IMPORTANT NOTE: this property does a lot of computation, so it should be called as
         minimum time as possible."""
-        self._kind = super().kind
-        self._kind.set_problem_class("HIERARCHICAL")
+        factory = self._kind_factory()
+        factory.kind.set_problem_class("HIERARCHICAL")
         (TO, PO, TEMPORAL) = (0, 1, 2)
 
         def lvl(tn: AbstractTaskNetwork):
             """Determines the expressivity level of temporal constraints within a task network"""
             if tn.total_order() is not None:
                 return TO
             elif tn.partial_order() is not None:
                 return PO
             else:
                 return TEMPORAL
 
         ordering_kind = lvl(self.task_network)
         if len(self.task_network.variables) > 0:
-            self._kind.set_hierarchical("INITIAL_TASK_NETWORK_VARIABLES")
+            factory.kind.set_hierarchical("INITIAL_TASK_NETWORK_VARIABLES")
         if len(self.task_network.non_temporal_constraints()) > 0:
-            self._kind.set_hierarchical("TASK_NETWORK_CONSTRAINTS")
+            factory.kind.set_hierarchical("TASK_NETWORK_CONSTRAINTS")
 
-        linear_checker = up.model.walkers.linear_checker.LinearChecker(self)
         for method in self.methods:
             ordering_kind = max(ordering_kind, lvl(method))
             for method_cond in method.preconditions:
-                self._kind.set_hierarchical("METHOD_PRECONDITIONS")
-                self._update_problem_kind_condition(method_cond, linear_checker)
+                factory.kind.set_hierarchical("METHOD_PRECONDITIONS")
+                factory.update_problem_kind_expression(method_cond)
             if len(method.non_temporal_constraints()) > 0:
-                self._kind.set_hierarchical("TASK_NETWORK_CONSTRAINTS")
+                factory.kind.set_hierarchical("TASK_NETWORK_CONSTRAINTS")
 
         if ordering_kind == TO:
-            self._kind.set_hierarchical("TASK_ORDER_TOTAL")
+            factory.kind.set_hierarchical("TASK_ORDER_TOTAL")
         elif ordering_kind == PO:
-            self._kind.set_hierarchical("TASK_ORDER_PARTIAL")
+            factory.kind.set_hierarchical("TASK_ORDER_PARTIAL")
         else:
-            self._kind.set_hierarchical("TASK_ORDER_TEMPORAL")
+            factory.kind.set_hierarchical("TASK_ORDER_TEMPORAL")
+            factory.kind.set_time("CONTINUOUS_TIME")
 
-        return self._kind
+        return factory.finalize()
 
     def has_name(self, name: str) -> bool:
         """
         Returns `True` if the given `name` is already in the `HierarchicalProblem`, `False` otherwise.
 
         :param name: The target name to find in the `HierarchicalProblem`.
         :return: `True` if the given `name` is already in the `HierarchicalProblem`, `False` otherwise."""
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/method.py` & `unified_planning-1.0.0/unified_planning/model/htn/method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -52,15 +52,15 @@
         return hash(self._task) + sum(map(hash, self._params))
 
     @property
     def task(self) -> Task:
         return self._task
 
     @property
-    def parameters(self) -> List[up.model.parameter.Parameter]:
+    def parameters(self) -> List["up.model.parameter.Parameter"]:
         return self._params
 
 
 class Method(AbstractTaskNetwork):
     """HTN Method: encoding of a procedure for achieving a high-level task."""
 
     def __init__(
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/ordering.py` & `unified_planning-1.0.0/unified_planning/model/htn/ordering.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2021-2023 AIPlan4EU project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
 from typing import List, Set, Optional, Tuple, Iterable
 
 from unified_planning.environment import get_environment
 from unified_planning.model import FNode, TimepointKind, Timing, StartTiming, EndTiming
 from unified_planning.model.walkers import AnyChecker
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/task.py` & `unified_planning-1.0.0/unified_planning/model/htn/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/task_network.py` & `unified_planning-1.0.0/unified_planning/model/htn/task_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/metrics.py` & `unified_planning-1.0.0/unified_planning/model/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/__init__.py` & `unified_planning-1.0.0/unified_planning/model/mixins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/actions_set.py` & `unified_planning-1.0.0/unified_planning/model/mixins/actions_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/agents_set.py` & `unified_planning-1.0.0/unified_planning/model/mixins/agents_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project / Technion
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/fluents_set.py` & `unified_planning-1.0.0/unified_planning/model/mixins/fluents_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 # limitations under the License.
 #
 
 from warnings import warn
 import unified_planning as up
 from unified_planning.model.expression import ConstantExpression
 from unified_planning.exceptions import UPProblemDefinitionError, UPValueError
-from typing import Optional, List, Dict, Union, Iterable
+from typing import Optional, List, Dict, Union, Iterable, Set
 
 
 class FluentsSetMixin:
     """
     This class is a mixin that contains a `set` of `fluents` with some related methods.
 
     NOTE: when this mixin is used in combination with other mixins that share some
@@ -190,7 +190,23 @@
     def __hash__(self):
         return sum(map(hash, self._fluents))
 
     def _clone_to(self, other: "FluentsSetMixin"):
         other._fluents = self._fluents.copy()
         other._initial_defaults = self._initial_defaults.copy()
         other._fluents_defaults = self._fluents_defaults.copy()
+
+    def get_static_fluents(self) -> Set["up.model.fluent.Fluent"]:
+        """
+        Returns the set of the `static fluents`.
+
+        `Static fluents` are those who can't change their values because they never
+        appear in the :func:`fluent <unified_planning.model.Effect.fluent>` field of an `Effect`, therefore there are no :func:`Actions <unified_planning.model.Problem.actions>`
+        in the `Problem` that can change their value.
+        """
+        return set()  # conservative default, should be overriden
+
+    def get_unused_fluents(self) -> Set["up.model.fluent.Fluent"]:
+        """
+        Returns the set of `fluents` that are never used in the problem.
+        """
+        return set()  # conservative default, should be overriden
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/initial_state.py` & `unified_planning-1.0.0/unified_planning/model/mixins/initial_state.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright 2021-2023 AIPlan4EU project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
 from typing import Union, Dict, Any
 
 import unified_planning as up
 from unified_planning.exceptions import (
     UPProblemDefinitionError,
     UPTypeError,
     UPExpressionDefinitionError,
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/metrics.py` & `unified_planning-1.0.0/unified_planning/model/mixins/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,23 @@
-from typing import Dict, List, Optional, Set, Tuple
+# Copyright 2021-2023 AIPlan4EU project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
 
+from typing import Dict, List, Optional, Set, Tuple
 
 import unified_planning as up
 from unified_planning.model.metrics import PlanQualityMetric
 from unified_planning.model.problem_kind import ProblemKind
 from unified_planning.model.mixins import ActionsSetMixin
 from unified_planning.exceptions import UPProblemDefinitionError
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/objects_set.py` & `unified_planning-1.0.0/unified_planning/model/mixins/objects_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/time_model.py` & `unified_planning-1.0.0/unified_planning/model/mixins/time_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/timed_conds_effs.py` & `unified_planning-1.0.0/unified_planning/model/mixins/timed_conds_effs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,29 @@
-from typing import Optional, Dict, List, Set, Tuple, Union, cast
+# Copyright 2021-2023 AIPlan4EU project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
+
+from typing import Optional, Dict, List, Set, Union, Iterable
 
 import unified_planning as up
 from unified_planning.environment import Environment, get_environment
-from unified_planning.exceptions import (
-    UPConflictingEffectsException,
-    UPTypeError,
-    UPUsageError,
-)
+from unified_planning.exceptions import UPTypeError, UPUsageError
+from unified_planning.model.timing import Timing
 
 
 class TimedCondsEffs:
     """A set of timed conditions of effects."""
 
     def __init__(self, _env: Optional[Environment] = None):
         self._environment = get_environment(_env)
@@ -159,15 +172,17 @@
 
     def is_conditional(self) -> bool:
         """Returns `True` if the `action` has `conditional effects`, `False` otherwise."""
         return any(e.is_conditional() for l in self._effects.values() for e in l)
 
     def add_condition(
         self,
-        interval: Union["up.model.timing.Timing", "up.model.timing.TimeInterval"],
+        interval: Union[
+            "up.model.expression.TimeExpression", "up.model.timing.TimeInterval"
+        ],
         condition: Union[
             "up.model.fnode.FNode",
             "up.model.fluent.Fluent",
             "up.model.parameter.Parameter",
             bool,
         ],
     ):
@@ -176,16 +191,18 @@
         the given expression must evaluate to `True` during the whole given `interval`.
 
         :param interval: The `interval` in which the given expression must evaluate to `True` for this
             `action` to be applicable.
         :param condition: The expression that must be `True` in the given `interval` for this
             `action` to be applicable.
         """
-        if isinstance(interval, up.model.Timing):
-            interval = up.model.TimePointInterval(interval)
+        if not isinstance(interval, up.model.TimeInterval):
+            # transform from int/float/timepoint... to Timing
+            timing = Timing.from_time(interval)
+            interval = up.model.TimePointInterval(timing)  # and from Timing to Interval
         (condition_exp,) = self._environment.expression_manager.auto_promote(condition)
         assert self._environment.type_checker.get_type(condition_exp).is_bool_type()
         conditions = self._conditions.setdefault(interval, [])
         if condition_exp not in conditions:
             conditions.append(condition_exp)
 
     def _set_conditions(
@@ -193,27 +210,30 @@
         interval: "up.model.timing.TimeInterval",
         conditions: List["up.model.fnode.FNode"],
     ):
         self._conditions[interval] = conditions
 
     def add_effect(
         self,
-        timing: "up.model.timing.Timing",
+        timing: "up.model.expression.TimeExpression",
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         At the given time, adds the given assignment to the `action's effects`.
 
         :param timing: The exact time in which the assignment is applied.
         :param fluent: The `fluent` which value is modified by the assignment.
         :param value: The `value` to assign to the given `fluent`.
         :param condition: The `condition` in which this `effect` is applied; the default
             value is `True`.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
         ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
         if not fluent_exp.is_fluent_exp():
@@ -223,32 +243,36 @@
         if not self._environment.type_checker.get_type(condition_exp).is_bool_type():
             raise UPTypeError("Effect condition is not a Boolean condition!")
         if not fluent_exp.type.is_compatible(value_exp.type):
             raise UPTypeError(
                 f"DurativeAction effect has an incompatible value type. Fluent type: {fluent_exp.type} // Value type: {value_exp.type}"
             )
         self._add_effect_instance(
-            timing, up.model.effect.Effect(fluent_exp, value_exp, condition_exp)
+            timing,
+            up.model.effect.Effect(fluent_exp, value_exp, condition_exp, forall=forall),
         )
 
     def add_increase_effect(
         self,
-        timing: "up.model.timing.Timing",
+        timing: "up.model.expression.TimeExpression",
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         At the given time, adds the given `increment` to the `action's effects`.
 
         :param timing: The exact time in which the increment is applied.
         :param fluent: The `fluent` which value is incremented by the added `effect`.
         :param value: The given `fluent` is incremented by the given `value`.
         :param condition: The `condition` in which this effect is applied; the default
             value is `True`.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
         ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
         if not fluent_exp.is_fluent_exp():
@@ -266,32 +290,36 @@
         self._add_effect_instance(
             timing,
             up.model.effect.Effect(
                 fluent_exp,
                 value_exp,
                 condition_exp,
                 kind=up.model.effect.EffectKind.INCREASE,
+                forall=forall,
             ),
         )
 
     def add_decrease_effect(
         self,
-        timing: "up.model.timing.Timing",
+        timing: "up.model.expression.TimeExpression",
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         At the given time, adds the given `decrement` to the `action's effects`.
 
         :param timing: The exact time in which the `decrement` is applied.
         :param fluent: The `fluent` which value is decremented by the added effect.
         :param value: The given `fluent` is decremented by the given `value`.
         :param condition: The `condition` in which this effect is applied; the default
             value is `True`.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
         ) = self._environment.expression_manager.auto_promote(fluent, value, condition)
         if not fluent_exp.is_fluent_exp():
@@ -309,20 +337,24 @@
         self._add_effect_instance(
             timing,
             up.model.effect.Effect(
                 fluent_exp,
                 value_exp,
                 condition_exp,
                 kind=up.model.effect.EffectKind.DECREASE,
+                forall=forall,
             ),
         )
 
     def _add_effect_instance(
-        self, timing: "up.model.timing.Timing", effect: "up.model.effect.Effect"
+        self,
+        timing: "up.model.expression.TimeExpression",
+        effect: "up.model.effect.Effect",
     ):
+        timing = Timing.from_time(timing)
         assert (
             self._environment == effect.environment
         ), "effect does not have the same environment of the action"
         fluents_assigned = self._fluents_assigned.setdefault(timing, {})
         fluents_inc_dec = self._fluents_inc_dec.setdefault(timing, set())
         simulated_effect = self._simulated_effects.get(timing, None)
         up.model.effect.check_conflicting_effects(
@@ -347,15 +379,15 @@
         timing: "up.model.timing.Timing",
         simulated_effect: "up.model.effect.SimulatedEffect",
     ):
         """
         Sets the given `simulated effect` at the specified `timing`.
 
         :param timing: The time in which the `simulated effect` must be applied.
-        :param simulated effects: The `simulated effect` that must be applied at the given `timing`.
+        :param simulated_effect: The `simulated effect` that must be applied at the given `timing`.
         """
         up.model.effect.check_conflicting_simulated_effects(
             simulated_effect,
             timing,
             self._fluents_assigned.setdefault(timing, {}),
             self._fluents_inc_dec.get(timing, set()),
             f"action or problem: {self.name}",  # type: ignore[attr-defined]
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/user_types_set.py` & `unified_planning-1.0.0/unified_planning/model/mixins/user_types_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/__init__.py` & `unified_planning-1.0.0/unified_planning/model/multi_agent/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/agent.py` & `unified_planning-1.0.0/unified_planning/model/multi_agent/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,14 +17,15 @@
 import unified_planning as up
 from unified_planning.model.mixins import (
     ActionsSetMixin,
     FluentsSetMixin,
 )
 from typing import Optional, List, Union, Iterable
 from unified_planning.model.expression import ConstantExpression
+from unified_planning.exceptions import UPUsageError
 
 
 class Agent(
     FluentsSetMixin,
     ActionsSetMixin,
 ):
     """
@@ -81,14 +82,18 @@
         return self.has_action(name) or self.has_fluent(name)
 
     @property
     def name(self) -> str:
         """Returns the `Agent` `name`."""
         return self._name
 
+    @name.setter
+    def name(self, new_value: str):
+        raise UPUsageError("The name of an Agent is immutable.")
+
     @property
     def environment(self) -> "up.Environment":
         """Returns this `Agent` `Environment`."""
         return self._env
 
     def add_public_fluent(
         self,
@@ -96,14 +101,15 @@
         typename: Optional["up.model.types.Type"] = None,
         *,
         default_initial_value: Optional["ConstantExpression"] = None,
         **kwargs: "up.model.types.Type",
     ) -> "up.model.fluent.Fluent":
         """Adds the given `public fluent` to the `problem`.
         If the first parameter is not a `Fluent`, the parameters will be passed to the `Fluent` constructor to create it.
+
         :param fluent_or_name: `Fluent` instance or `name` of the `fluent` to be constructed.
         :param typename: If only the `name` of the `fluent` is given, this is the `fluent's type` (passed to the `Fluent` constructor).
         :param default_initial_value: If provided, defines the default value taken in initial state by
                                       a state variable of this `fluent` that has no explicit value.
         :param kwargs: If only the `name` of the `fluent` is given, these are the `fluent's parameters` (passed to the `Fluent` constructor).
         :return: The `fluent` passed or constructed.
         """
@@ -122,14 +128,15 @@
         typename: Optional["up.model.types.Type"] = None,
         *,
         default_initial_value: Optional["ConstantExpression"] = None,
         **kwargs: "up.model.types.Type",
     ) -> "up.model.fluent.Fluent":
         """Adds the given `private fluent` to the `problem`.
         If the first parameter is not a `Fluent`, the parameters will be passed to the `Fluent` constructor to create it.
+
         :param fluent_or_name: `Fluent` instance or `name` of the `fluent` to be constructed.
         :param typename: If only the `name` of the `fluent` is given, this is the `fluent's type` (passed to the `Fluent` constructor).
         :param default_initial_value: If provided, defines the default value taken in initial state by
                                       a state variable of this `fluent` that has no explicit value.
         :param kwargs: If only the `name` of the `fluent` is given, these are the `fluent's parameters` (passed to the `Fluent` constructor).
         :return: The `fluent` passed or constructed.
         """
@@ -139,22 +146,24 @@
             default_initial_value=default_initial_value,
             **kwargs,
         )
 
     def add_public_fluents(self, fluents: Iterable["up.model.fluent.Fluent"]):
         """
         Adds the given `public fluents` to the `problem`.
+
         :param fluents: The `public fluents` that must be added to the `problem`.
         """
         for fluent in fluents:
             self.add_public_fluent(fluent)
 
     def add_private_fluents(self, fluents: Iterable["up.model.fluent.Fluent"]):
         """
         Adds the given `private fluents` to the `problem`.
+
         :param fluents: The `private fluents` that must be added to the `problem`.
         """
         for fluent in fluents:
             self.add_private_fluent(fluent)
 
     @property
     def public_fluents(self) -> List["up.model.fluent.Fluent"]:
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/ma_environment.py` & `unified_planning-1.0.0/unified_planning/model/multi_agent/ma_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/ma_problem.py` & `unified_planning-1.0.0/unified_planning/model/multi_agent/ma_problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,14 +26,15 @@
     UPPlanDefinitionError,
 )
 from typing import Optional, List, Dict, Union, cast, Iterable
 from unified_planning.model.mixins import (
     ObjectsSetMixin,
     UserTypesSetMixin,
     AgentsSetMixin,
+    InitialStateMixin,
 )
 from fractions import Fraction
 
 
 class MultiAgentProblem(  # type: ignore[misc]
     AbstractProblem,
     UserTypesSetMixin,
@@ -136,22 +137,26 @@
             res += hash(iv)
         for g in self._goals:
             res += hash(g)
         return res
 
     def clone(self):
         new_p = MultiAgentProblem(self._name, self._env)
-        for f in self.ma_environment.fluents:
-            new_p.ma_environment.add_fluent(f)
+        new_p.ma_environment._fluents = self.ma_environment._fluents.copy()
+        new_p.ma_environment._fluents_defaults = (
+            self.ma_environment._fluents_defaults.copy()
+        )
         for ag in self.agents:
             new_ag = up.model.multi_agent.Agent(ag.name, self)
-            for f in ag.fluents:
-                new_ag.add_fluent(f)
+            new_ag._public_fluents = ag._public_fluents.copy()
+            new_ag._fluents = ag._fluents.copy()
+            new_ag._fluents_defaults = ag._fluents_defaults.copy()
             for a in ag.actions:
                 new_ag.add_action(a.clone())
+            new_p.add_agent(new_ag)
         new_p._user_types = self._user_types[:]
         new_p._user_types_hierarchy = self._user_types_hierarchy.copy()
         new_p._objects = self._objects[:]
         new_p._initial_value = self._initial_value.copy()
         new_p._goals = self._goals[:]
         new_p._initial_defaults = self._initial_defaults.copy()
         return new_p
@@ -231,16 +236,20 @@
             if not a.is_constant():
                 raise UPExpressionDefinitionError(
                     f"Impossible to return the initial value of a fluent expression with no constant arguments: {fluent_exp}."
                 )
         if fluent_exp in self._initial_value:
             return self._initial_value[fluent_exp]
         elif fluent_exp.is_dot():
-            agent = fluent_exp.agent()
+            agent = self.agent(fluent_exp.agent())
             f = fluent_exp.arg(0).fluent()
+            if f not in agent.fluents:
+                raise UPProblemDefinitionError(
+                    f"Expression {fluent_exp} is invalid because {f} does not belong to agent {agent.name}"
+                )
             v = agent.fluents_defaults.get(f, None)
             if v is None:
                 raise UPProblemDefinitionError("Initial value not set!")
             return v
         elif fluent_exp.fluent() in self.ma_environment.fluents_defaults:
             return self.ma_environment.fluents_defaults[fluent_exp.fluent()]
         else:
@@ -313,14 +322,18 @@
         """Returns all the `goals` in the `MultiAgentProblem`."""
         return self._goals
 
     def clear_goals(self):
         """Removes all the `goals` from the `MultiAgentProblem`."""
         self._goals = []
 
+    def clear_agents(self):
+        """Removes all the `goals` from the `MultiAgentProblem`."""
+        self._agents = []
+
     @property
     def kind(self) -> "up.model.problem_kind.ProblemKind":
         """
         Calculates and returns the `problem kind` of this `planning problem`.
         If the `Problem` is modified, this method must be called again in order to be reliable.
 
         IMPORTANT NOTE: this property does a lot of computation, so it should be called as
@@ -340,14 +353,16 @@
             self._update_problem_kind_condition(goal)
         return self._kind
 
     def _update_problem_kind_effect(self, e: "up.model.effect.Effect"):
         if e.is_conditional():
             self._update_problem_kind_condition(e.condition)
             self._kind.set_effects_kind("CONDITIONAL_EFFECTS")
+        if e.is_forall():
+            self._kind.set_effects_kind("FORALL_EFFECTS")
         if e.is_increase():
             self._kind.set_effects_kind("INCREASE_EFFECTS")
         elif e.is_decrease():
             self._kind.set_effects_kind("DECREASE_EFFECTS")
 
     def _update_problem_kind_condition(self, exp: "up.model.fnode.FNode"):
         ops = self._operators_extractor.get(exp)
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/object.py` & `unified_planning-1.0.0/unified_planning/model/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,14 +23,15 @@
 
 
 class Object:
     """
     Represents an `Object` of the `unified_planning` library.
 
     An `Object` contains 2 parts:
+
     - `name`: a string containing the `Object's` :func:`name <unified_planning.model.Object.name>`.
     - `type`: a :class:`~unified_planning.model.Type` representing the planning :func:`user_type <unified_planning.model.Object.type>` associated to this `Object`.
 
     The `Object` class is immutable.
     """
 
     def __init__(
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/operators.py` & `unified_planning-1.0.0/unified_planning/model/operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/parameter.py` & `unified_planning-1.0.0/unified_planning/model/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/problem.py` & `unified_planning-1.0.0/unified_planning/model/problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,14 +14,15 @@
 #
 """This module defines the problem class."""
 
 
 from numbers import Real
 import unified_planning as up
 import unified_planning.model.tamp
+from unified_planning.model import Fluent
 from unified_planning.model.abstract_problem import AbstractProblem
 from unified_planning.model.mixins import (
     ActionsSetMixin,
     TimeModelMixin,
     FluentsSetMixin,
     ObjectsSetMixin,
     UserTypesSetMixin,
@@ -32,15 +33,15 @@
 from unified_planning.model.operators import OperatorKind
 from unified_planning.model.types import _IntType
 from unified_planning.exceptions import (
     UPProblemDefinitionError,
     UPTypeError,
 )
 from fractions import Fraction
-from typing import Optional, List, Dict, Set, Tuple, Union, cast
+from typing import Optional, List, Dict, Set, Tuple, Union, cast, Iterable
 
 
 class Problem(  # type: ignore[misc]
     AbstractProblem,
     UserTypesSetMixin,
     TimeModelMixin,
     FluentsSetMixin,
@@ -74,15 +75,15 @@
             self, self.environment, self._add_user_type, self.has_name
         )
         ObjectsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name
         )
         InitialStateMixin.__init__(self, self, self, self.environment)
         MetricsMixin.__init__(self, self.environment)
-        self._operators_extractor = up.model.walkers.OperatorsExtractor()
+
         self._timed_effects: Dict[
             "up.model.timing.Timing", List["up.model.effect.Effect"]
         ] = {}
         self._timed_goals: Dict[
             "up.model.timing.TimeInterval", List["up.model.fnode.FNode"]
         ] = {}
         self._trajectory_constraints: List["up.model.fnode.FNode"] = list()
@@ -356,14 +357,20 @@
 
         `Static fluents` are those who can't change their values because they never
         appear in the :func:`fluent <unified_planning.model.Effect.fluent>` field of an `Effect`, therefore there are no :func:`Actions <unified_planning.model.Problem.actions>`
         in the `Problem` that can change their value.
         """
         return self._get_static_and_unused_fluents()[0]
 
+    def get_unused_fluents(self) -> Set["up.model.fluent.Fluent"]:
+        """
+        Returns the set of `fluents` that are never used in the problem.
+        """
+        return self._get_static_and_unused_fluents()[1]
+
     @property
     def timed_goals(
         self,
     ) -> Dict["up.model.timing.TimeInterval", List["up.model.fnode.FNode"]]:
         """Returns all the `timed goals` in the `Problem`."""
         return self._timed_goals
 
@@ -409,23 +416,26 @@
 
     def add_timed_effect(
         self,
         timing: "up.model.timing.Timing",
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         Adds the given `timed effect` to the `Problem`; a `timed effect` is an :class:`~unified_planning.model.Effect` applied at a fixed time.
 
         :param timing: The exact time in which the given `Effect` is applied.
         :param fluent: The fluent modified by the `Effect`.
         :param value: The value assigned to the given `fluent` at the given `time`.
         :param condition: The condition that must be evaluated to `True` in order for this `Effect` to be
             actually applied.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         if timing.is_from_end():
             raise UPProblemDefinitionError(
                 f"Timing used in timed effect cannot be EndTiming."
             )
         (
             fluent_exp,
@@ -434,32 +444,36 @@
         ) = self._env.expression_manager.auto_promote(fluent, value, condition)
         assert fluent_exp.is_fluent_exp()
         if not self._env.type_checker.get_type(condition_exp).is_bool_type():
             raise UPTypeError("Effect condition is not a Boolean condition!")
         if not fluent_exp.type.is_compatible(value_exp.type):
             raise UPTypeError("Timed effect has not compatible types!")
         self._add_effect_instance(
-            timing, up.model.effect.Effect(fluent_exp, value_exp, condition_exp)
+            timing,
+            up.model.effect.Effect(fluent_exp, value_exp, condition_exp, forall=forall),
         )
 
     def add_increase_effect(
         self,
         timing: "up.model.timing.Timing",
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         Adds the given `timed increase effect` to the `Problem`; a `timed effect` is an :class:`~unified_planning.model.Effect` applied at a fixed time.
 
         :param timing: The exact time in which the given `Effect` is applied.
         :param fluent: The fluent increased by the `Effect`.
         :param value: The value of which the given `fluent` is increased at the given `time`.
         :param condition: The condition that must be evaluated to `True` in order for this `Effect` to be
             actually applied.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
         ) = self._env.expression_manager.auto_promote(fluent, value, condition)
         assert fluent_exp.is_fluent_exp()
@@ -472,32 +486,36 @@
         self._add_effect_instance(
             timing,
             up.model.effect.Effect(
                 fluent_exp,
                 value_exp,
                 condition_exp,
                 kind=up.model.effect.EffectKind.INCREASE,
+                forall=forall,
             ),
         )
 
     def add_decrease_effect(
         self,
         timing: "up.model.timing.Timing",
         fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"],
         value: "up.model.expression.Expression",
         condition: "up.model.expression.BoolExpression" = True,
+        forall: Iterable["up.model.variable.Variable"] = tuple(),
     ):
         """
         Adds the given timed decrease effect to the problem; a `timed effect` is an :class:`~unified_planning.model.Effect` applied at a fixed time.
 
         :param timing: The exact time in which the given `Effect` is applied.
         :param fluent: The fluent decreased by the `Effect`.
         :param value: The value of which the given `fluent` is decrease at the given `time`.
         :param condition: The condition that must be evaluated to `True` in order for this `Effect` to be
             actually applied.
+        :param forall: The 'Variables' that are universally quantified in this
+            effect; the default value is empty.
         """
         (
             fluent_exp,
             value_exp,
             condition_exp,
         ) = self._env.expression_manager.auto_promote(fluent, value, condition)
         assert fluent_exp.is_fluent_exp()
@@ -510,14 +528,15 @@
         self._add_effect_instance(
             timing,
             up.model.effect.Effect(
                 fluent_exp,
                 value_exp,
                 condition_exp,
                 kind=up.model.effect.EffectKind.DECREASE,
+                forall=forall,
             ),
         )
 
     def _add_effect_instance(
         self, timing: "up.model.timing.Timing", effect: "up.model.effect.Effect"
     ):
         assert (
@@ -626,308 +645,354 @@
         Adds the given ``invariant`` to the problem's state invariants.
         State invariants are added as ``Always`` trajectory constraints.
 
         :param invariant: The invariant expression to add to this problem as a state invariant.
         """
         self.add_trajectory_constraint(self._env.expression_manager.Always(invariant))
 
-    @property
-    def kind(self) -> "up.model.problem_kind.ProblemKind":
-        """
-        Calculates and returns the `problem kind` of this `planning problem`.
-        If the `Problem` is modified, this method must be called again in order to be reliable.
-
-        IMPORTANT NOTE: this property does a lot of computation, so it should be called as
-        seldom as possible.
-        """
-        # Create the needed data structures
-        static_fluents, unused_fluents = self._get_static_and_unused_fluents()
+    def _kind_factory(self) -> "_KindFactory":
+        """Returns an intermediate view for the kind computation.
+        Subclasses can use the result of this method to update the kind"""
+        factory = _KindFactory(
+            self,
+            problem_class="ACTION_BASED",
+            environment=self._env,
+        )
 
-        # Create a simplifier and a linear_checker with the problem, so static fluents can be considered as constants
-        simplifier = up.model.walkers.simplifier.Simplifier(self._env, self)
-        linear_checker = up.model.walkers.linear_checker.LinearChecker(self)
-        self._kind = up.model.problem_kind.ProblemKind()
-        self._kind.set_problem_class("ACTION_BASED")
-        self._kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
-        fluents_to_only_increase, fluents_to_only_decrease = self._update_kind_metric(
-            self._kind, linear_checker, static_fluents
-        )
-        for fluent in self._fluents:
-            self._update_problem_kind_fluent(fluent, unused_fluents)
-        for object in self._objects:
-            self._update_problem_kind_type(object.type)
         for action in self._actions:
-            self._update_problem_kind_action(
-                action,
-                fluents_to_only_increase,
-                fluents_to_only_decrease,
-                static_fluents,
-                simplifier,
-                linear_checker,
-            )
+            factory.update_problem_kind_action(action)
         if len(self._timed_effects) > 0:
-            self._kind.set_time("CONTINUOUS_TIME")
-            self._kind.set_time("TIMED_EFFECTS")
+            factory.kind.set_time("CONTINUOUS_TIME")
+            factory.kind.set_time("TIMED_EFFECTS")
         for effect_list in self._timed_effects.values():
             for effect in effect_list:
-                self._update_problem_kind_effect(
-                    effect,
-                    fluents_to_only_increase,
-                    fluents_to_only_decrease,
-                    static_fluents,
-                    simplifier,
-                    linear_checker,
-                )
+                factory.update_problem_kind_effect(effect)
         if len(self._timed_goals) > 0:
-            self._kind.set_time("TIMED_GOALS")
-            self._kind.set_time("CONTINUOUS_TIME")
+            factory.kind.set_time("TIMED_GOALS")
+            factory.kind.set_time("CONTINUOUS_TIME")
         for tc in self._trajectory_constraints:
             if tc.is_always():
-                self._kind.set_constraints_kind("STATE_INVARIANTS")
+                factory.kind.set_constraints_kind("STATE_INVARIANTS")
             else:
-                self._kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
+                factory.kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         for goal_list in self._timed_goals.values():
             for goal in goal_list:
-                self._update_problem_kind_condition(goal, linear_checker)
+                factory.update_problem_kind_expression(goal)
         for goal in self._goals:
-            self._update_problem_kind_condition(goal, linear_checker)
+            factory.update_problem_kind_expression(goal)
+
+        return factory
+
+    @property
+    def kind(self) -> "up.model.problem_kind.ProblemKind":
+        """
+        Calculates and returns the `problem kind` of this `planning problem`.
+        If the `Problem` is modified, this method must be called again in order to be reliable.
+
+        IMPORTANT NOTE: this property does a lot of computation, so it should be called as
+        seldom as possible.
+        """
+        return self._kind_factory().finalize()
+
+
+class _KindFactory:
+    """Utility class to help analyze the kind of `AbstractProblem` subclass."""
+
+    def __init__(
+        self,
+        pb: AbstractProblem,
+        problem_class: str,
+        environment: "unified_planning.Environment",
+    ):
+        assert isinstance(pb, MetricsMixin)
+        assert isinstance(pb, FluentsSetMixin)
+        assert isinstance(pb, ObjectsSetMixin)
+        assert isinstance(pb, UserTypesSetMixin)
+        assert isinstance(pb, TimeModelMixin)
+
+        # WARNING: self.pb may in fact be any subclass of AbstractProblem that has the above mixins.
+        # We declare it as a Problem to avoid limitations of the python type system
+        self.pb: up.model.Problem = pb
+        self.static_fluents: Set[Fluent] = pb.get_static_fluents()
+        self.unused_fluents: Set[Fluent] = pb.get_unused_fluents()
+
+        self.environment: unified_planning.Environment = environment
+        self.kind: up.model.ProblemKind = up.model.ProblemKind()
+
+        self.kind.set_problem_class(problem_class)
+
+        # set optimistically and remove if we encounter a counter example
+        self.kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
+
+        # Create a simplifier and a linear_checker with the problem, so static fluents can be considered as constants
+        self.simplifier: up.model.walkers.simplifier.Simplifier = (
+            up.model.walkers.simplifier.Simplifier(self.environment, self.pb)
+        )
+        self.linear_checker: up.model.walkers.linear_checker.LinearChecker = (
+            up.model.walkers.linear_checker.LinearChecker(self.pb, self.environment)
+        )
+        self.operators_extractor: up.model.walkers.OperatorsExtractor = (
+            up.model.walkers.OperatorsExtractor()
+        )
+
+        (
+            fluents_to_only_increase,
+            fluents_to_only_decrease,
+        ) = self.pb._update_kind_metric(
+            self.kind, self.linear_checker, self.static_fluents
+        )
+        # fluents that can only be increased (resp. decreased) for the problem to be SIMPLE_NUMERIC_PLANNING
+        self.fluents_to_only_increase: Set[Fluent] = fluents_to_only_increase
+        self.fluents_to_only_decrease: Set[Fluent] = fluents_to_only_decrease
+
+        for fluent in self.pb.fluents:
+            self.update_problem_kind_fluent(fluent)
+        for object in self.pb.all_objects:
+            self.update_problem_kind_type(object.type)
+
+    def finalize(self) -> "up.model.ProblemKind":
+        """Once all features have been added, remove unnecessary features that were added preventively."""
         if (
-            not self._kind.has_continuous_numbers()
-            and not self._kind.has_discrete_numbers()
+            not self.kind.has_continuous_numbers()
+            and not self.kind.has_discrete_numbers()
         ):
-            self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+            self.kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
         else:
-            if not self._kind.has_simple_numeric_planning():
-                self._kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
-        if self._kind.has_continuous_time() and self.discrete_time:
-            self._kind.set_time("DISCRETE_TIME")
-            self._kind.unset_time("CONTINUOUS_TIME")
-        if self._self_overlapping and (
-            self._kind.has_continuous_time() or self._kind.has_discrete_time()
+            if not self.kind.has_simple_numeric_planning():
+                self.kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
+        if self.kind.has_continuous_time() and self.pb.discrete_time:
+            self.kind.set_time("DISCRETE_TIME")
+            self.kind.unset_time("CONTINUOUS_TIME")
+        if self.pb.self_overlapping and (
+            self.kind.has_continuous_time() or self.kind.has_discrete_time()
         ):
-            self._kind.set_time("SELF_OVERLAPPING")
-        return self._kind
+            self.kind.set_time("SELF_OVERLAPPING")
+        return self.kind
+
+    def update_problem_kind_type(self, type: "up.model.types.Type"):
+        if type.is_user_type():
+            self.kind.set_typing("FLAT_TYPING")
+            if cast(up.model.types._UserType, type).father is not None:
+                self.kind.set_typing("HIERARCHICAL_TYPING")
+        elif type.is_int_type():
+            self.kind.set_numbers("DISCRETE_NUMBERS")
+        elif type.is_real_type():
+            self.kind.set_numbers("CONTINUOUS_NUMBERS")
 
-    def _update_problem_kind_effect(
+    def update_problem_kind_effect(
         self,
         e: "up.model.effect.Effect",
-        fluents_to_only_increase: Set["up.model.fluent.Fluent"],
-        fluents_to_only_decrease: Set["up.model.fluent.Fluent"],
-        static_fluents: Set["up.model.fluent.Fluent"],
-        simplifier: "up.model.walkers.simplifier.Simplifier",
-        linear_checker: "up.model.walkers.linear_checker.LinearChecker",
     ):
-        value = simplifier.simplify(e.value)
+        value = self.simplifier.simplify(e.value)
+        fluents_in_value = self.environment.free_vars_extractor.get(value)
         if e.is_conditional():
-            self._update_problem_kind_condition(e.condition, linear_checker)
-            self._kind.set_effects_kind("CONDITIONAL_EFFECTS")
+            self.update_problem_kind_expression(e.condition)
+            self.kind.set_effects_kind("CONDITIONAL_EFFECTS")
+        if e.is_forall():
+            self.kind.set_effects_kind("FORALL_EFFECTS")
         if e.is_increase():
-            self._kind.set_effects_kind("INCREASE_EFFECTS")
+            self.kind.set_effects_kind("INCREASE_EFFECTS")
             # If the value is a number (int or real) and it violates the constraint
             # on the "fluents_to_only_increase" or on "fluents_to_only_decrease",
             # unset simple_numeric_planning
             if (  # value is a constant number
                 value.is_int_constant() or value.is_real_constant()
             ):
                 if (
-                    e.fluent in fluents_to_only_increase and value.constant_value() < 0
+                    e.fluent in self.fluents_to_only_increase
+                    and value.constant_value() < 0
                 ) or (
-                    e.fluent in fluents_to_only_decrease and value.constant_value() > 0
+                    e.fluent in self.fluents_to_only_decrease
+                    and value.constant_value() > 0
                 ):
-                    self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+                    self.kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
             else:
-                self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+                self.kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+                if any(f in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+                if any(f not in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         elif e.is_decrease():
-            self._kind.set_effects_kind("DECREASE_EFFECTS")
+            self.kind.set_effects_kind("DECREASE_EFFECTS")
             # If the value is a number (int or real) and it violates the constraint
             # on the "fluents_to_only_increase" or on "fluents_to_only_decrease",
             # unset simple_numeric_planning
             if (  # value is a constant number
                 value.is_int_constant() or value.is_real_constant()
             ):
                 if (
-                    e.fluent in fluents_to_only_increase and value.constant_value() > 0
+                    e.fluent in self.fluents_to_only_increase
+                    and value.constant_value() > 0
                 ) or (
-                    e.fluent in fluents_to_only_decrease and value.constant_value() < 0
+                    e.fluent in self.fluents_to_only_decrease
+                    and value.constant_value() < 0
                 ):
-                    self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+                    self.kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
             else:
-                self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+                self.kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+                if any(f in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+                if any(f not in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         elif e.is_assignment():
             value_type = value.type
-            value = e.value
-            fluents_in_value = self._env.free_vars_extractor.get(value)
             if (
                 value_type.is_int_type() or value_type.is_real_type()
             ):  # the value is a number
                 if (  # if the fluent has increase/decrease constraints or the value assigned is not a constant,
                     # unset "SIMPLE_NUMERIC_PLANNING"
-                    e.fluent in fluents_to_only_increase
-                    or e.fluent in fluents_to_only_decrease
+                    e.fluent in self.fluents_to_only_increase
+                    or e.fluent in self.fluents_to_only_decrease
                     or not value.is_constant()
                 ):
-                    self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
-            if any(f in static_fluents for f in fluents_in_value):
-                self._kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
-            if any(f not in static_fluents for f in fluents_in_value):
-                self._kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+                    self.kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+                if any(f in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
+                if any(f not in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
             elif value.type.is_bool_type():
-                if any(f in static_fluents for f in fluents_in_value):
-                    self._kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
-                if any(f not in static_fluents for f in fluents_in_value):
-                    self._kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+                if any(f in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+                if any(f not in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
+            elif value.type.is_user_type():
+                if any(f in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS")
+                if any(f not in self.static_fluents for f in fluents_in_value):
+                    self.kind.set_effects_kind("FLUENTS_IN_OBJECT_ASSIGNMENTS")
 
-    def _update_problem_kind_condition(
+    def update_problem_kind_expression(
         self,
         exp: "up.model.fnode.FNode",
-        linear_checker: "up.model.walkers.linear_checker.LinearChecker",
     ):
-        ops = self._operators_extractor.get(exp)
+        ops = self.operators_extractor.get(exp)
         if OperatorKind.EQUALS in ops:
-            self._kind.set_conditions_kind("EQUALITIES")
+            self.kind.set_conditions_kind("EQUALITIES")
         if OperatorKind.NOT in ops:
-            self._kind.set_conditions_kind("NEGATIVE_CONDITIONS")
+            self.kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         if OperatorKind.OR in ops:
-            self._kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
+            self.kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         if OperatorKind.EXISTS in ops:
-            self._kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
+            self.kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         if OperatorKind.FORALL in ops:
-            self._kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
-        is_linear, _, _ = linear_checker.get_fluents(exp)
+            self.kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
+        is_linear, _, _ = self.linear_checker.get_fluents(exp)
         if not is_linear:
-            self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
+            self.kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
 
-    def _update_problem_kind_type(self, type: "up.model.types.Type"):
-        if type.is_user_type():
-            self._kind.set_typing("FLAT_TYPING")
-            if cast(up.model.types._UserType, type).father is not None:
-                self._kind.set_typing("HIERARCHICAL_TYPING")
-        elif type.is_int_type():
-            self._kind.set_numbers("DISCRETE_NUMBERS")
-        elif type.is_real_type():
-            self._kind.set_numbers("CONTINUOUS_NUMBERS")
-
-    def _update_problem_kind_fluent(
+    def update_problem_kind_fluent(
         self,
         fluent: "up.model.fluent.Fluent",
-        unused_fluents: Set["up.model.fluent.Fluent"],
     ):
         type = fluent.type
-        if fluent not in unused_fluents or (
+        if fluent not in self.unused_fluents or (
             not type.is_int_type() and not type.is_real_type()
         ):
-            self._update_problem_kind_type(type)
+            self.update_problem_kind_type(type)
         if fluent.type.is_int_type() or type.is_real_type():
             numeric_type = type
             assert isinstance(
                 numeric_type, (up.model.types._RealType, up.model.types._IntType)
             )
             if (
                 numeric_type.lower_bound is not None
                 or numeric_type.upper_bound is not None
             ):
-                self._kind.set_numbers("BOUNDED_TYPES")
-            if fluent not in unused_fluents:
-                self._kind.set_fluents_type("NUMERIC_FLUENTS")
+                self.kind.set_numbers("BOUNDED_TYPES")
+            if fluent not in self.unused_fluents:
+                self.kind.set_fluents_type("NUMERIC_FLUENTS")
         elif type.is_user_type():
-            self._kind.set_fluents_type("OBJECT_FLUENTS")
+            self.kind.set_fluents_type("OBJECT_FLUENTS")
         for param in fluent.signature:
             pt = param.type
-            self._update_problem_kind_type(pt)
+            self.update_problem_kind_type(pt)
             if pt.is_bool_type():
-                self._kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+                self.kind.set_parameters("BOOL_FLUENT_PARAMETERS")
             elif pt.is_int_type():
-                self._kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+                self.kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+
+    def update_action_parameter(self, param: "up.model.Parameter"):
+        pt = param.type
+        self.update_problem_kind_type(pt)
+        if pt.is_bool_type():
+            self.kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        elif pt.is_real_type():
+            self.kind.set_parameters("REAL_ACTION_PARAMETERS")
+        elif pt.is_int_type():
+            if (
+                cast(_IntType, pt).lower_bound is None
+                or cast(_IntType, pt).upper_bound is None
+            ):
+                self.kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+            else:
+                self.kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+
+    def update_action_duration(self, duration: "up.model.DurationInterval"):
+        lower, upper = duration.lower, duration.upper
+        if lower != upper:
+            self.kind.set_time("DURATION_INEQUALITIES")
+        free_vars = self.environment.free_vars_extractor.get(
+            lower
+        ) | self.environment.free_vars_extractor.get(upper)
+        if len(free_vars) > 0:
+            only_static = True
+            for fv in free_vars:
+                if fv.fluent() not in self.static_fluents:
+                    only_static = False
+                    break
+            if only_static:
+                self.kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
+            else:
+                self.kind.set_expression_duration("FLUENTS_IN_DURATIONS")
+
+    def update_action_timed_condition(
+        self, span: "up.model.TimeInterval", cond: "up.model.FNode"
+    ):
+        if span.lower.delay != 0 or span.upper.delay != 0:
+            for t in [span.lower, span.upper]:
+                if (t.is_from_start() and t.delay > 0) or (
+                    t.is_from_end() and t.delay < 0
+                ):
+                    self.kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
+                else:
+                    self.kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
+        self.update_problem_kind_expression(cond)
 
-    def _update_problem_kind_action(
+    def update_action_timed_effect(self, t: "up.model.Timing", eff: "up.model.Effect"):
+        if t.delay != 0:
+            if (t.is_from_start() and t.delay > 0) or (t.is_from_end() and t.delay < 0):
+                self.kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
+            else:
+                self.kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
+        self.update_problem_kind_effect(eff)
+
+    def update_problem_kind_action(
         self,
         action: "up.model.action.Action",
-        fluents_to_only_increase: Set["up.model.fluent.Fluent"],
-        fluents_to_only_decrease: Set["up.model.fluent.Fluent"],
-        static_fluents: Set["up.model.fluent.Fluent"],
-        simplifier: "up.model.walkers.simplifier.Simplifier",
-        linear_checker: "up.model.walkers.linear_checker.LinearChecker",
     ):
         for param in action.parameters:
-            pt = param.type
-            self._update_problem_kind_type(pt)
-            if pt.is_bool_type():
-                self._kind.set_parameters("BOOL_ACTION_PARAMETERS")
-            elif pt.is_real_type():
-                self._kind.set_parameters("REAL_ACTION_PARAMETERS")
-            elif pt.is_int_type():
-                if (
-                    cast(_IntType, pt).lower_bound is None
-                    or cast(_IntType, pt).upper_bound is None
-                ):
-                    self._kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
-                else:
-                    self._kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+            self.update_action_parameter(param)
         if isinstance(action, up.model.action.SensingAction):
-            self._kind.set_problem_class("CONTINGENT")
+            self.kind.set_problem_class("CONTINGENT")
         if isinstance(action, up.model.tamp.InstantaneousMotionAction):
             if len(action.motion_constraints) > 0:
-                self._kind.set_problem_class("TAMP")
+                self.kind.set_problem_class("TAMP")
         if isinstance(action, up.model.action.InstantaneousAction):
             for c in action.preconditions:
-                self._update_problem_kind_condition(c, linear_checker)
+                self.update_problem_kind_expression(c)
             for e in action.effects:
-                self._update_problem_kind_effect(
-                    e,
-                    fluents_to_only_increase,
-                    fluents_to_only_decrease,
-                    static_fluents,
-                    simplifier,
-                    linear_checker,
-                )
+                self.update_problem_kind_effect(e)
             if action.simulated_effect is not None:
-                self._kind.set_simulated_entities("SIMULATED_EFFECTS")
+                self.kind.set_simulated_entities("SIMULATED_EFFECTS")
         elif isinstance(action, up.model.action.DurativeAction):
-            lower, upper = action.duration.lower, action.duration.upper
-            if lower != upper:
-                self._kind.set_time("DURATION_INEQUALITIES")
-            free_vars = self.environment.free_vars_extractor.get(
-                lower
-            ) | self.environment.free_vars_extractor.get(upper)
-            if len(free_vars) > 0:
-                only_static = True
-                for fv in free_vars:
-                    if fv.fluent() not in static_fluents:
-                        only_static = False
-                        break
-                if only_static:
-                    self._kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
-                else:
-                    self._kind.set_expression_duration("FLUENTS_IN_DURATIONS")
+            self.update_action_duration(action.duration)
             for i, lc in action.conditions.items():
-                if i.lower.delay != 0 or i.upper.delay != 0:
-                    for t in [i.lower, i.upper]:
-                        if (t.is_from_start() and t.delay > 0) or (
-                            t.is_from_end() and t.delay < 0
-                        ):
-                            self._kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-                        else:
-                            self._kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
                 for c in lc:
-                    self._update_problem_kind_condition(c, linear_checker)
+                    self.update_action_timed_condition(i, c)
             for t, le in action.effects.items():
-                if t.delay != 0:
-                    if (t.is_from_start() and t.delay > 0) or (
-                        t.is_from_end() and t.delay < 0
-                    ):
-                        self._kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
-                    else:
-                        self._kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
                 for e in le:
-                    self._update_problem_kind_effect(
-                        e,
-                        fluents_to_only_increase,
-                        fluents_to_only_decrease,
-                        static_fluents,
-                        simplifier,
-                        linear_checker,
-                    )
+                    self.update_action_timed_effect(t, e)
             if len(action.simulated_effects) > 0:
-                self._kind.set_simulated_entities("SIMULATED_EFFECTS")
-            self._kind.set_time("CONTINUOUS_TIME")
+                self.kind.set_simulated_entities("SIMULATED_EFFECTS")
+            self.kind.set_time("CONTINUOUS_TIME")
         else:
             raise NotImplementedError
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/problem_kind.py` & `unified_planning-1.0.0/unified_planning/model/problem_kind.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -50,16 +50,19 @@
     ],
     "EFFECTS_KIND": [
         "CONDITIONAL_EFFECTS",
         "INCREASE_EFFECTS",
         "DECREASE_EFFECTS",
         "STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS",
         "STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS",
+        "STATIC_FLUENTS_IN_OBJECT_ASSIGNMENTS",
         "FLUENTS_IN_BOOLEAN_ASSIGNMENTS",
         "FLUENTS_IN_NUMERIC_ASSIGNMENTS",
+        "FLUENTS_IN_OBJECT_ASSIGNMENTS",
+        "FORALL_EFFECTS",
     ],
     "TYPING": ["FLAT_TYPING", "HIERARCHICAL_TYPING"],
     "PARAMETERS": [
         "BOOL_FLUENT_PARAMETERS",
         "BOUNDED_INT_FLUENT_PARAMETERS",
         "BOOL_ACTION_PARAMETERS",
         "BOUNDED_INT_ACTION_PARAMETERS",
@@ -122,15 +125,15 @@
     This class represents the main interesting feature that a :class:`planning Problem <unified_planning.model.AbstractProblem>` can have in order to understand
     if an :class:`~unified_planning.engines.Engine` is capable of solving the `Problem` or not; some features might also help the `Engine`, allowing
     some assumptions to be made.
 
     The `ProblemKind` of a `Problem` is calculated by it's :func:`kind <unified_planning.model.Problem.kind>` property.
     """
 
-    def __init__(self, features: Set[str] = set()):
+    def __init__(self, features: Set[str] = set(), version=None):
         self._features: Set[str] = set(features)
 
     def __repr__(self) -> str:
         features_gen = (f"'{feature}'" for feature in self._features)
         return f'ProblemKind([{", ".join(features_gen)}])'
 
     def __str__(self) -> str:
@@ -159,14 +162,18 @@
         return res
 
     def __le__(self, oth: object):
         if not isinstance(oth, ProblemKind):
             raise ValueError(f"Unable to compare a ProblemKind with a {type(oth)}")
         return self._features.issubset(oth._features)
 
+    def get_version(self):
+        """Currently an empty placeholder, intended to support backward compatible problem kind extensions."""
+        return None
+
     @property
     def features(self) -> Set[str]:
         """Returns the features contained by this `ProblemKind`."""
         return self._features
 
     def union(self, oth: "ProblemKind") -> "ProblemKind":
         """
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/activity.py` & `unified_planning-1.0.0/unified_planning/model/scheduling/activity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,60 @@
-from typing import Optional
+# Copyright 2021-2023 AIPlan4EU project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
 
+from typing import Optional, Union
+
+from unified_planning.model.expression import NumericExpression
+
+from unified_planning.model.fnode import FNode
 from unified_planning.environment import get_environment, Environment
 from unified_planning.exceptions import UPProblemDefinitionError
 from unified_planning.model import (
     Timepoint,
     Timing,
     TimepointKind,
     Fluent,
     NumericConstant,
 )
 import unified_planning as up
 from unified_planning.model.scheduling.chronicle import Chronicle
 
 
 class Activity(Chronicle):
-    """Activity is essentially an interval with start and end timing that facilitates defining constraints in the
-    associated SchedulingProblem"""
+    """Activity is essentially an interval with start and end timepoint that facilitates defining constraints in the
+    associated :class:`SchedulingProblem`"""
 
     def __init__(
         self, name: str, duration: int = 0, _env: Optional[Environment] = None
     ):
         Chronicle.__init__(self, name, _env=_env)
-        start_tp = Timepoint(TimepointKind.START, container=name)
-        end_tp = Timepoint(TimepointKind.END, container=name)
-        self._start = Timing(0, start_tp)
-        self._end = Timing(0, end_tp)
+        self._start = Timepoint(TimepointKind.START, container=name)
+        self._end = Timepoint(TimepointKind.END, container=name)
 
         self.set_fixed_duration(duration)
 
     @property
-    def start(self) -> Timing:
+    def start(self) -> Timepoint:
         """Returns a reference to the start time of this activity."""
         return self._start
 
     @property
-    def end(self) -> Timing:
+    def end(self) -> Timepoint:
         """Returns a reference to the start time of this activity."""
         return self._end
 
     @property
     def duration(self) -> "up.model.timing.DurationInterval":
         """Returns the `activity` `duration interval`."""
         return self._duration
@@ -93,22 +109,42 @@
             )
         ):
             raise UPProblemDefinitionError(
                 f"{duration} is an empty interval duration of action: {self.name}."
             )
         self._duration = duration
 
-    def uses(self, resource: Fluent, amount: NumericConstant = 1):
+    def uses(self, resource: Union[Fluent, FNode], amount: NumericExpression = 1):
         """Asserts that the activity borrows a given amount (1 by default) of the resource.
         The borrowed resources will be reusable by another activity at the time epoch immediately
-         succeeding the activity end.
+        succeeding the activity end.
+
+        :param resource: Fluent expression that denotes the resource taht is used.
+        :param amount: Quantity of the resource that is borrowed over the course of the activity.
         """
         self.add_decrease_effect(self.start, resource, amount)
         self.add_increase_effect(self.end, resource, amount)
 
-    def set_release_date(self, date: int):
-        """Set the earliest date at which the activity can be started."""
+    def add_release_date(self, date: NumericExpression):
+        """Sets the earliest date at which the activity can be started."""
         self.add_constraint(get_environment().expression_manager.LE(date, self.start))
 
-    def set_deadline(self, date: int):
-        """Set the latest date at which the activity might end."""
+    def add_deadline(self, date: NumericExpression):
+        """Sets the latest date at which the activity might end."""
         self.add_constraint(get_environment().expression_manager.LE(self.end, date))
+
+    def clone(self):
+        """Generates a copy of this activity."""
+        new = Activity(self.name, _env=self._environment)
+        self._clone_to(new)
+        new._duration = self._duration
+        return new
+
+    def __hash__(self):
+        return Chronicle.__hash__(self) + hash(self._duration)
+
+    def __eq__(self, other):
+        return (
+            isinstance(other, Activity)
+            and Chronicle.__eq__(self, other)
+            and self._duration == other._duration
+        )
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/chronicle.py` & `unified_planning-1.0.0/unified_planning/model/scheduling/chronicle.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,34 @@
+# Copyright 2021-2023 AIPlan4EU project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
 from typing import Optional, List, OrderedDict, Union
 
+from unified_planning.model.fnode import FNode
 import unified_planning as up
 from unified_planning import Environment
 from unified_planning.model import Parameter
 from unified_planning.model.mixins.timed_conds_effs import TimedCondsEffs
 from unified_planning.model.types import Type
 
 
 class Chronicle(TimedCondsEffs):
-    """Core structure to represent a set of timed conditions and effects."""
+    """Core structure to represent a set of variables, constraints, timed conditions and effects in scheduling problems."""
 
     def __init__(
         self,
         name: str,
         _parameters: Optional["OrderedDict[str, up.model.types.Type]"] = None,
         _env: Optional[Environment] = None,
         **kwargs: "up.model.types.Type",
@@ -41,25 +57,19 @@
                 self._parameters[n] = up.model.parameter.Parameter(
                     n, t, self._environment
                 )
 
     def __repr__(self) -> str:
         s = []
         s.append(f"{self.name}")
-        first = True
-        for p in self.parameters:
-            if first:
-                s.append("(")
-                first = False
-            else:
-                s.append(", ")
-            s.append(str(p))
-        if not first:
-            s.append(")")
+        if len(self.parameters) > 0:
+            s += ["(", ", ".join(map(str, self.parameters)), ")"]
         s.append(" {\n")
+        if hasattr(self, "duration"):
+            s.append(f"    duration = {str(self.duration)}\n")
         if len(self._constraints) > 0:
             s.append("    constraints = [\n")
             for c in self._constraints:
                 s.append(f"      {str(c)}\n")
             s.append("    ]\n")
         if len(self.conditions) > 0:
             s.append("    conditions = [\n")
@@ -101,34 +111,49 @@
         return res
 
     @property
     def name(self) -> str:
         """Returns the `Chronicle` `name`."""
         return self._name
 
+    def _clone_to(self, other: "Chronicle"):  # type: ignore[override]
+        other._parameters = self._parameters.copy()
+        other._constraints = self._constraints.copy()
+        TimedCondsEffs._clone_to(self, other)
+
     def clone(self):
         new = Chronicle(self._name, _env=self._environment)
-        new._parameters = self._parameters.copy()
-        new._constraints = self._constraints.copy()
-        TimedCondsEffs._clone_to(self, new)
+        self._clone_to(new)
         return new
 
     def add_parameter(self, name: str, tpe: Type) -> Parameter:
         """Adds a new decision variable associated to this activity.
         The resulting parameter's identifier will be prefixed with the activity's name but may be
         used outside the activity itself. For instance, it could appear in global constraints or
         constraints involving more than one activity."""
-        assert ":" not in name, f"Usage of ':' is forbidden in names: {name}"
-        scoped_name = f"{self.name}:{name}"
+        assert "." not in name, f"Usage of '.' is forbidden in names: {name}"
+        assert name not in [
+            "start",
+            "end",
+        ], f"Usage of parameter name {name} is reserved"
+        scoped_name = f"{self.name}.{name}"
         if name in self._parameters:
             raise ValueError(f"Name '{name}' already used in chronicle '{self.name}'")
         param = Parameter(scoped_name, tpe)
         self._parameters[name] = param
         return param
 
+    def get_parameter(self, name: str) -> Parameter:
+        """Returns the parameter with the given name."""
+        if name not in self._parameters:
+            raise ValueError(
+                f"Unknown parameter '{name}. Available parameters: {list(self._parameters.keys())}"
+            )
+        return self._parameters[name]
+
     @property
     def parameters(self) -> List["up.model.parameter.Parameter"]:
         """Returns the `list` of the `Action parameters`."""
         return list(self._parameters.values())
 
     def add_constraint(
         self,
@@ -144,7 +169,11 @@
         """
         (constraint_exp,) = self._environment.expression_manager.auto_promote(
             constraint
         )
         assert self._environment.type_checker.get_type(constraint_exp).is_bool_type()
         if constraint_exp not in self._constraints:
             self._constraints.append(constraint_exp)
+
+    @property
+    def constraints(self) -> List[FNode]:
+        return self._constraints
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/state.py` & `unified_planning-1.0.0/unified_planning/model/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/__init__.py` & `unified_planning-1.0.0/unified_planning/model/tamp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/action.py` & `unified_planning-1.0.0/unified_planning/model/tamp/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/objects.py` & `unified_planning-1.0.0/unified_planning/model/tamp/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/path.py` & `unified_planning-1.0.0/unified_planning/model/tamp/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/types.py` & `unified_planning-1.0.0/unified_planning/model/tamp/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/timing.py` & `unified_planning-1.0.0/unified_planning/model/timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 from unified_planning.environment import Environment
 from unified_planning.model.fnode import FNode
-from unified_planning.model.expression import NumericConstant, uniform_numeric_constant
+from unified_planning.model.expression import (
+    NumericConstant,
+    uniform_numeric_constant,
+    TimeExpression,
+)
 from abc import ABC
 from enum import Enum, auto
 from fractions import Fraction
 from typing import Union, Optional
 
 
 class TimepointKind(Enum):
@@ -36,19 +40,25 @@
     GLOBAL_START = auto()
     GLOBAL_END = auto()
     START = auto()
     END = auto()
 
 
 class Timepoint:
-    """Class used to define the point in the time from which a :class:`~unified_planning.model.Timing` is considered."""
+    """Temporal point of interest, one of:
+
+     - global start: temporal origin (time 0) at which the initial state is defined
+     - global end: plan horizon, at which the plan goals must hold.
+     - start time or end time of an action, activity or task/method.
+
+    Used to define the point in the time from which a :class:`~unified_planning.model.timing.Timing` is considered."""
 
     def __init__(self, kind: TimepointKind, container: Optional[str] = None):
         """
-        Creates a new `Timepoint`.
+        Creates a new :class:`Timepoint`.
 
         It is typically used to refer to:
          - the start/end of the containing action or method, or
          - to the start/end of a subtasks in a method
 
         Parameters
         ----------
@@ -88,38 +98,41 @@
         return Timing(delay, self)
 
     def __sub__(self, delay: Union[int, Fraction]) -> "Timing":
         return Timing(-delay, self)
 
     @property
     def kind(self) -> TimepointKind:
-        """Returns the `kind` of this `Timepoint`; the `kind` defines the semantic of the `Timepoint`."""
+        """Returns the `kind` of this :class:`Timepoint`; the `kind` defines the semantic of the `Timepoint`."""
         return self._kind
 
     @property
     def container(self):
         """Returns the `container` in which this `Timepoint` is defined or `None` if it refers to the enclosing `action/method`."""
         return self._container
 
 
 class Timing:
-    """
-    Class that used a :class:`~unified_planning.model.Timepoint` to define from when this `Timing` is considered and a :func:`delay <unified_planning.model.Timing.delay>`,
+    """Time defined relatively to a :class:`Timepoint`.
+
+    Class that used a :class:`~unified_planning.model.timing.Timepoint` to define from when this `Timing` is considered and a :func:`delay <unified_planning.model.Timing.delay>`,
     representing the distance from the given `Timepoint`.
-    For example:
-    A `GLOBAL_START Timepoint` with a `delay` of `5` means `5` units of time after the start of the `Plan`.
+    For instance:
+    A `GLOBAL_START Timepoint` with a `delay` of `5` means `5` units of time after the initial state.
     """
 
     def __init__(self, delay: NumericConstant, timepoint: Timepoint):
         self._timepoint = timepoint
         self._delay = uniform_numeric_constant(delay)
 
     def __repr__(self):
         if self._delay == 0:
             return f"{self._timepoint}"
+        elif self._delay < 0:
+            return f"{self._timepoint} - {-self._delay}"
         else:
             return f"{self._timepoint} + {self._delay}"
 
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, Timing):
             return self._delay == oth._delay and self._timepoint == oth._timepoint
         else:
@@ -161,14 +174,29 @@
             or self._timepoint.kind == TimepointKind.GLOBAL_START
         )
 
     def is_from_end(self) -> bool:
         """Returns `True` if this `Timing` is from the end, `False` if it is from the start."""
         return not self.is_from_start()
 
+    @staticmethod
+    def from_time(time: TimeExpression) -> "Timing":
+        """Converts any supported time expression into its canonical Timing representation."""
+        if (
+            isinstance(time, int)
+            or isinstance(time, float)
+            or isinstance(time, Fraction)
+        ):
+            return GlobalStartTiming() + time
+        elif isinstance(time, Timepoint):
+            return Timing(timepoint=time, delay=0)
+        else:
+            assert isinstance(time, Timing)
+            return time
+
 
 def StartTiming(delay: NumericConstant = 0, container: Optional[str] = None) -> Timing:
     """
     Returns the start timing of an :class:`~unified_planning.model.Action`.
     Created with a delay > 0 represents "delay" time
     after the start of the `Action`.
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/type_manager.py` & `unified_planning-1.0.0/unified_planning/model/type_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/types.py` & `unified_planning-1.0.0/unified_planning/model/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/variable.py` & `unified_planning-1.0.0/unified_planning/model/variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/__init__.py` & `unified_planning-1.0.0/unified_planning/model/walkers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/any.py` & `unified_planning-1.0.0/unified_planning/model/walkers/any.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/dag.py` & `unified_planning-1.0.0/unified_planning/model/walkers/dag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/dnf.py` & `unified_planning-1.0.0/unified_planning/model/walkers/dnf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py` & `unified_planning-1.0.0/unified_planning/model/walkers/expression_quantifiers_remover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/fluents_substituter.py` & `unified_planning-1.0.0/unified_planning/model/walkers/fluents_substituter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/free_vars.py` & `unified_planning-1.0.0/unified_planning/model/walkers/free_vars.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/generic.py` & `unified_planning-1.0.0/unified_planning/model/walkers/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/identitydag.py` & `unified_planning-1.0.0/unified_planning/model/walkers/identitydag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/linear_checker.py` & `unified_planning-1.0.0/unified_planning/model/walkers/linear_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/names_extractor.py` & `unified_planning-1.0.0/unified_planning/model/walkers/names_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -62,15 +62,15 @@
     def walk_variable_exp(self, expression: FNode, args: List[Set[str]]) -> Set[str]:
         return self._args_merge_in_place(args, {expression.variable().name})
 
     def walk_object_exp(self, expression: FNode, args: List[Set[str]]) -> Set[str]:
         return self._args_merge_in_place(args, {expression.object().name})
 
     def walk_dot(self, expression: FNode, args: List[Set[str]]) -> Set[str]:
-        return self._args_merge_in_place(args, {expression.agent().name})
+        return self._args_merge_in_place(args, {expression.agent()})
 
     @walkers.handles(
         op.OperatorKind.AND,
         op.OperatorKind.OR,
         op.OperatorKind.NOT,
         op.OperatorKind.IMPLIES,
         op.OperatorKind.IFF,
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/operators_extractor.py` & `unified_planning-1.0.0/unified_planning/model/walkers/operators_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/quantifier_simplifier.py` & `unified_planning-1.0.0/unified_planning/model/walkers/quantifier_simplifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/simplifier.py` & `unified_planning-1.0.0/unified_planning/model/walkers/simplifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/state_evaluator.py` & `unified_planning-1.0.0/unified_planning/model/walkers/state_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/substituter.py` & `unified_planning-1.0.0/unified_planning/model/walkers/substituter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/type_checker.py` & `unified_planning-1.0.0/unified_planning/model/walkers/type_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -367,19 +367,13 @@
         return BOOL
 
     @walkers.handles(OperatorKind.DOT)
     def walk_dot(
         self, expression: FNode, args: List["unified_planning.model.types.Type"]
     ) -> Optional["unified_planning.model.types.Type"]:
         assert expression.is_dot()
-        a = expression.agent()
         t = expression.args[0]
-        f = t.fluent().name
-        if args[0] is None:
-            return None
         if len(args) != 1:
             return None
         if not t.is_fluent_exp():
             return None
-        if not a.fluent(f):
-            return None
         return args[0]
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/usertype_fluents_walker.py` & `unified_planning-1.0.0/unified_planning/model/walkers/usertype_fluents_walker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/plans/__init__.py` & `unified_planning-1.0.0/unified_planning/plans/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,23 +13,26 @@
 # limitations under the License.
 #
 
 from unified_planning.plans.plan import Plan, ActionInstance, PlanKind
 from unified_planning.plans.sequential_plan import SequentialPlan
 from unified_planning.plans.time_triggered_plan import TimeTriggeredPlan
 from unified_planning.plans.partial_order_plan import PartialOrderPlan
-from unified_planning.plans.contingent_plan import ContingentPlan
+from unified_planning.plans.contingent_plan import ContingentPlanNode, ContingentPlan
 from unified_planning.plans.stn_plan import STNPlanNode, STNPlan
 from unified_planning.plans.hierarchical_plan import HierarchicalPlan
+from unified_planning.plans.schedule import Schedule
 
 __all__ = [
     "Plan",
     "PlanKind",
     "ActionInstance",
     "SequentialPlan",
     "TimeTriggeredPlan",
     "PartialOrderPlan",
+    "ContingentPlanNode",
     "ContingentPlan",
     "STNPlanNode",
     "STNPlan",
     "HierarchicalPlan",
+    "Schedule",
 ]
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/plans/contingent_plan.py` & `unified_planning-1.0.0/unified_planning/plans/contingent_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -235,23 +235,24 @@
         """
         if plan_kind == self._kind:
             return self
         else:
             raise UPUsageError(f"{type(self)} can't be converted to {plan_kind}.")
 
 
-def visit_tree(root_node: ContingentPlanNode) -> Iterator[ContingentPlanNode]:
+def visit_tree(root_node: Optional[ContingentPlanNode]) -> Iterator[ContingentPlanNode]:
     """
     Method to visit all the Tree nodes once.
 
     :param root_node: The starting node of the tree.
     :return: The Iterator over all the Nodes in the tree.
     """
     stack: Deque[ContingentPlanNode] = deque()
-    stack.append(root_node)
+    if root_node is not None:
+        stack.append(root_node)
     already_visited: Set[ContingentPlanNode] = set()
     while stack:
         current_element: ContingentPlanNode = stack.popleft()
         if current_element not in already_visited:
             already_visited.add(current_element)
             get_second_element = lambda x: x[1]
             stack.extend(map(get_second_element, current_element.children))
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/plans/hierarchical_plan.py` & `unified_planning-1.0.0/unified_planning/plans/hierarchical_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Copyright 2021-2023 AIPlan4EU project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
 from dataclasses import dataclass, field
 from typing import Union, Dict, Optional, Tuple, List, OrderedDict, Callable
 
 from unified_planning.model.abstract_problem import AbstractProblem
 
 from unified_planning.exceptions import UPUsageError
 from unified_planning.model.fnode import FNode
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/plans/partial_order_plan.py` & `unified_planning-1.0.0/unified_planning/plans/partial_order_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/plans/plan.py` & `unified_planning-1.0.0/unified_planning/plans/plan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,16 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
 import unified_planning as up
-from unified_planning.environment import Environment, get_environment
 from unified_planning.model import AbstractProblem
+from unified_planning.environment import Environment, get_environment
+from unified_planning.exceptions import UPTypeError
 from abc import ABC, abstractmethod
 from typing import Callable, Optional, Sequence, Tuple, Dict
 from enum import Enum, auto
 
 
 """This module defines the general `Plan` interface and the `ActionInstance` class."""
 
@@ -39,18 +40,29 @@
         params: Sequence["up.model.Expression"] = tuple(),
         agent: Optional["up.model.multi_agent.Agent"] = None,
         motion_paths: Optional[
             Dict["up.model.tamp.MotionConstraint", "up.model.tamp.Path"]
         ] = None,
     ):
         auto_promote = action.environment.expression_manager.auto_promote
+        assert agent is None or isinstance(
+            agent, up.model.multi_agent.Agent
+        ), "Typing not respected"
         self._agent = agent
         self._action = action
         self._params = tuple(auto_promote(params))
         assert len(action.parameters) == len(self._params)
+        for param, assigned_value in zip(action.parameters, self._params):
+            if not param.type.is_compatible(assigned_value.type):
+                raise UPTypeError(
+                    f"Incompatible parameter type assignment. {assigned_value} can't be assigned to: {param}"
+                )
+        assert motion_paths is None or isinstance(
+            motion_paths, dict
+        ), "Typing not respected"
         self._motion_paths = motion_paths
 
     def __repr__(self) -> str:
         s = []
         if len(self._params) > 0:
             s.append("(")
             first = True
@@ -111,14 +123,15 @@
 
     SEQUENTIAL_PLAN = auto()
     TIME_TRIGGERED_PLAN = auto()
     PARTIAL_ORDER_PLAN = auto()
     CONTINGENT_PLAN = auto()
     STN_PLAN = auto()
     HIERARCHICAL_PLAN = auto()
+    SCHEDULE = auto()
 
 
 class Plan(ABC):
     """Represents a generic plan."""
 
     def __init__(
         self, kind: PlanKind, environment: Optional["Environment"] = None
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/plans/sequential_plan.py` & `unified_planning-1.0.0/unified_planning/plans/sequential_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -151,24 +151,25 @@
             lifted_required_fluents: Set[FNode] = set()
             # add free vars of preconditions
             for prec in inst_action.preconditions:
                 lifted_required_fluents |= fve.get(
                     eqr.remove_quantifiers(prec, problem)
                 )
             # add in the required_fluents all the free fluents this action instance deals with
-            for eff in inst_action.effects:
-                lifted_required_fluents |= fve.get(
-                    eqr.remove_quantifiers(eff.condition, problem)
-                )
-                lifted_required_fluents |= fve.get(
-                    eqr.remove_quantifiers(eff.fluent, problem)
-                )
-                lifted_required_fluents |= fve.get(
-                    eqr.remove_quantifiers(eff.value, problem)
-                )
+            for effect in inst_action.effects:
+                for eff in effect.expand_effect(problem):
+                    lifted_required_fluents |= fve.get(
+                        eqr.remove_quantifiers(eff.condition, problem)
+                    )
+                    lifted_required_fluents |= fve.get(
+                        eqr.remove_quantifiers(eff.fluent, problem)
+                    )
+                    lifted_required_fluents |= fve.get(
+                        eqr.remove_quantifiers(eff.value, problem)
+                    )
 
             assignments: Dict[Expression, Expression] = dict(
                 zip(inst_action.parameters, action_instance.actual_parameters)
             )
             for lifted_fluent in lifted_required_fluents:
                 assert lifted_fluent.is_fluent_exp()
                 for (
@@ -192,26 +193,27 @@
                     assert (
                         required_fluent_last_modifier != action_instance
                     )  # sanity check
                     graph.add_edge(required_fluent_last_modifier, action_instance)
 
             # for every effect, set current action instance as the last modifier and the current action instance is ordered
             # after every action instance that requires a fluent the current action instance modifies
-            for eff in inst_action.effects:
-                assert eff.fluent.is_fluent_exp()
-                grounded_fluent = simp.simplify(
-                    subs.substitute(eff.fluent, assignments)
-                )
-                last_modifier[grounded_fluent] = action_instance
-                dependent_action_instance_list = all_required.setdefault(
-                    grounded_fluent, []
-                )
-                for dependent_action_instance in dependent_action_instance_list:
-                    if dependent_action_instance != action_instance:
-                        graph.add_edge(dependent_action_instance, action_instance)
+            for effect in inst_action.effects:
+                for eff in effect.expand_effect(problem):
+                    assert eff.fluent.is_fluent_exp()
+                    grounded_fluent = simp.simplify(
+                        subs.substitute(eff.fluent, assignments)
+                    )
+                    last_modifier[grounded_fluent] = action_instance
+                    dependent_action_instance_list = all_required.setdefault(
+                        grounded_fluent, []
+                    )
+                    for dependent_action_instance in dependent_action_instance_list:
+                        if dependent_action_instance != action_instance:
+                            graph.add_edge(dependent_action_instance, action_instance)
 
         assert nx.is_directed_acyclic_graph(graph)
         # remove redundant edges and return the up.plans.partial_order_plan.PartialOrderPlan structure.
         return up.plans.partial_order_plan.PartialOrderPlan(
             {}, self._environment, nx.transitive_reduction(graph)
         )
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/plans/stn_plan.py` & `unified_planning-1.0.0/unified_planning/plans/stn_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/plans/time_triggered_plan.py` & `unified_planning-1.0.0/unified_planning/plans/time_triggered_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -69,18 +69,18 @@
 
     def __str__(self) -> str:
         def convert_ai(start_ai_dur):
             start, ai, dur = start_ai_dur
             if dur is None:
                 return f"    {float(start)}: {ai}"
             else:
-                return f"    {float(start)}: {ai}: {float(dur)}"
+                return f"    {float(start)}: {ai} [{float(dur)}]"
 
         ret = ["TimeTriggeredPlan:"]
-        ret.extend(map(convert_ai, sorted(self._actions)))
+        ret.extend(map(convert_ai, sorted(self._actions, key=lambda x: x[0])))
         return "\n".join(ret)
 
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, TimeTriggeredPlan) and len(self._actions) == len(
             oth._actions
         ):
             for (s, ai, d), (oth_s, oth_ai, oth_d) in zip(self._actions, oth._actions):
@@ -111,14 +111,15 @@
 
     @property
     def timed_actions(
         self,
     ) -> List[Tuple[Fraction, "plans.plan.ActionInstance", Optional[Fraction]]]:
         """
         Returns the sequence of tuples (`start`, `action_instance`, `duration`) where:
+
         - `start` is when the `ActionInstance` starts;
         - `action_instance` is the `grounded Action` applied;
         - `duration` is the (optional) duration of the `ActionInstance`.
         """
         return self._actions
 
     def replace_action_instances(
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/shortcuts.py` & `unified_planning-1.0.0/unified_planning/shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,15 +42,15 @@
     | This function has polymorphic n-arguments:
 
         * ``And(a,b,c)``
         * ``And([a,b,c])``
 
     | Restriction: Arguments must be ``boolean``.
 
-    :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+    :param \\*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
         of it, like ``a, b, c``.
     :return: The ``AND`` expression created.
     """
     return get_environment().expression_manager.And(*args)
 
 
 def Or(*args: Union[BoolExpression, Iterable[BoolExpression]]) -> FNode:
@@ -59,15 +59,15 @@
     | This function has polymorphic n-arguments:
 
         * ``Or(a,b,c)``
         * ``Or([a,b,c])``
 
     | Restriction: Arguments must be ``boolean``
 
-    :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+    :param \\*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
         of it, like ``a, b, c``.
     :return: The ``OR`` expression created.
     """
     return get_environment().expression_manager.Or(*args)
 
 
 def XOr(*args: Union[BoolExpression, Iterable[BoolExpression]]) -> FNode:
@@ -76,15 +76,15 @@
     | This function has polimorphic n-arguments:
 
         * XOr(a,b,c)
         * XOr([a,b,c])
 
     | Restriction: Arguments must be boolean
 
-    :param \*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
+    :param \\*args: Either an ``Iterable`` of ``boolean expressions``, like ``[a, b, c]``, or an unpacked version
         of it, like ``a, b, c``.
     :return: The exclusive disjunction in CNF form.
     """
     return get_environment().expression_manager.XOr(*args)
 
 
 def Not(expression: BoolExpression) -> FNode:
@@ -137,15 +137,15 @@
         ``Exists (var[0]... var[n]) | expression``
 
     Restriction: expression must be of ``boolean type`` and
     vars must be of ``Variable`` type
 
     :param expression: The main expression of the ``existential``. The expression should contain
         the given ``variables``.
-    :param \*vars: All the ``Variables`` appearing in the ``existential`` expression.
+    :param \\*vars: All the ``Variables`` appearing in the ``existential`` expression.
     :return: The created ``Existential`` expression.
     """
     return get_environment().expression_manager.Exists(expression, *vars)
 
 
 def Forall(
     expression: BoolExpression, *vars: "unified_planning.model.Variable"
@@ -154,15 +154,15 @@
         ``Forall (var[0]... var[n]) | expression``
 
     Restriction: expression must be of ``boolean type`` and
                 vars must be of ``Variable`` type
 
     :param expression: The main expression of the ``universal`` quantifier. The expression should contain
         the given ``variables``.
-    :param \*vars: All the ``Variables`` appearing in the ``universal`` expression.
+    :param \\*vars: All the ``Variables`` appearing in the ``universal`` expression.
     :return: The created ``Forall`` expression.
     """
     return get_environment().expression_manager.Forall(expression, *vars)
 
 
 def FluentExp(
     fluent: "unified_planning.model.Fluent", params: Sequence[Expression] = tuple()
@@ -325,15 +325,15 @@
 
 
 def Plus(*args: Union[Expression, Iterable[Expression]]) -> FNode:
     """
     Creates an expression of the form:
         ``args[0] + ... + args[n]``
 
-    :param \*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
+    :param \\*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
         of it, like ``a, b, 3``.
     :return: The ``PLUS`` expression created. (like ``a + b + 3``)
     """
     return get_environment().expression_manager.Plus(*args)
 
 
 def Minus(left: Expression, right: Expression) -> FNode:
@@ -349,15 +349,15 @@
 
 
 def Times(*args: Union[Expression, Iterable[Expression]]) -> FNode:
     """
     Creates an expression of the form:
         ``args[0] * ... * args[n]``
 
-    :param \*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
+    :param \\*args: Either an ``Iterable`` of expressions, like ``[a, b, 3]``, or an unpacked version
         of it, like ``a, b, 3``.
     :return: The ``TIMES`` expression created. (like ``a * b * 3``)
     """
     return get_environment().expression_manager.Times(*args)
 
 
 def Div(left: Expression, right: Expression) -> FNode:
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/__init__.py` & `unified_planning-1.0.0/unified_planning/test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,15 +18,14 @@
 from functools import wraps
 from importlib.util import find_spec
 from unified_planning.engines import OperationMode
 from unified_planning.environment import get_environment
 from unified_planning.model import ProblemKind
 from unified_planning.test.pddl import enhsp
 from typing import Optional
-import unified_planning.test.scheduling
 
 
 skipIf = unittest.skipIf
 SkipTest = unittest.SkipTest
 
 
 class skipIfEngineNotAvailable(object):
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/connected_locations.anml` & `unified_planning-1.0.0/unified_planning/test/anml/connected_locations.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/constants.anml` & `unified_planning-1.0.0/unified_planning/test/anml/constants.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/constants_no_variable_duration.anml` & `unified_planning-1.0.0/unified_planning/test/anml/constants_no_variable_duration.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/forall.anml` & `unified_planning-1.0.0/unified_planning/test/anml/forall.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml` & `unified_planning-1.0.0/unified_planning/test/anml/hierarchical_blocks_world.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/hydrone.anml` & `unified_planning-1.0.0/unified_planning/test/anml/hydrone.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match.anml` & `unified_planning-1.0.0/unified_planning/test/anml/match.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match_int_id.anml` & `unified_planning-1.0.0/unified_planning/test/anml/match_int_id.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match_test_parser.anml` & `unified_planning-1.0.0/unified_planning/test/anml/match_test_parser.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/simple_mais.anml` & `unified_planning-1.0.0/unified_planning/test/anml/simple_mais.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/contingent_pddl/colorballs/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl` & `unified_planning-1.0.0/unified_planning/test/contingent_pddl/colorballs/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl` & `unified_planning-1.0.0/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/__init__.py` & `unified_planning-1.0.0/unified_planning/test/examples/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,12 +13,13 @@
 # limitations under the License.
 
 
 import unified_planning.test.examples.minimals as minimals
 import unified_planning.test.examples.realistic as realistic
 import unified_planning.test.examples.testing_variants as testing_variants
 import unified_planning.test.examples.hierarchical as hierarchical
+import unified_planning.test.examples.scheduling as scheduling
 
 
 def get_example_problems():
-    sub_modules = [minimals, realistic, testing_variants, hierarchical]
+    sub_modules = [minimals, realistic, testing_variants, hierarchical, scheduling]
     return dict(x for m in sub_modules for x in m.get_example_problems().items())
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/hierarchical.py` & `unified_planning-1.0.0/unified_planning/test/examples/hierarchical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/minimals.py` & `unified_planning-1.0.0/unified_planning/test/examples/minimals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/realistic.py` & `unified_planning-1.0.0/unified_planning/test/examples/realistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from itertools import product
 import unified_planning as up
 from unified_planning.shortcuts import *
 from collections import namedtuple
 
 Example = namedtuple("Example", ["problem", "plan"])
 
 
@@ -943,16 +944,57 @@
     problem.set_initial_value(travel_time(l4, l5), 99)
     problem.set_initial_value(travel_time(l3, l5), 200)
 
     problem.add_goal(is_at(l5))
 
     plan = up.plans.SequentialPlan(
         [
-            up.plans.ActionInstance(move, (ObjectExp(l1), ObjectExp(l3))),
-            up.plans.ActionInstance(move, (ObjectExp(l3), ObjectExp(l4))),
-            up.plans.ActionInstance(move, (ObjectExp(l4), ObjectExp(l5))),
+            move(l1, l3),
+            move(l3, l4),
+            move(l4, l5),
         ]
     )
     travel = Example(problem=problem, plan=plan)
     problems["travel"] = travel
 
+    # safe_road
+    problem = Problem("safe_road")
+
+    Location = UserType("Location")
+
+    safe = Fluent("safe", l_from=Location, l_to=Location)
+    disaster_happened = Fluent("disaster_happened")
+
+    problem.add_fluent(safe, default_initial_value=True)
+    problem.add_fluent(disaster_happened, default_initial_value=False)
+
+    check = InstantaneousAction("check", l_from=Location, l_to=Location)
+    l_from = check.parameter("l_from")
+    l_to = check.parameter("l_to")
+    check.add_effect(safe(l_from, l_to), True)
+    problem.add_action(check)
+
+    natural_disaster = InstantaneousAction("natural_disaster")
+    lx, ly = Variable("lx", Location), Variable("ly", Location)
+    natural_disaster.add_effect(disaster_happened, True)
+    natural_disaster.add_effect(safe(lx, ly), False, forall=[lx, ly])
+    problem.add_action(natural_disaster)
+
+    l1 = Object("l1", Location)
+    l2 = Object("l2", Location)
+    l3 = Object("l3", Location)
+    locations = (l1, l2, l3)
+    problem.add_objects(locations)
+
+    problem.add_goal(disaster_happened)
+    problem.add_goal(Forall(safe(lx, ly), lx, ly))
+
+    def generate_safe_road_plan():
+        yield natural_disaster()
+        for lx, ly in product(locations, repeat=2):
+            yield check(lx, ly)
+
+    plan = up.plans.SequentialPlan(list(generate_safe_road_plan()))
+    safe_road = Example(problem=problem, plan=plan)
+    problems["safe_road"] = safe_road
+
     return problems
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/tamp.py` & `unified_planning-1.0.0/unified_planning/test/examples/tamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -210,17 +210,13 @@
                 ((25.960007356190847, 24.980103867321887, 1.5280187951943522), 0.0),
                 ((25.98183275824111, 25.489999756982453, 1.5280187951943522), 0.0),
                 ((26.0, 26.0, 1.5707963267948966), 0.0),
             ]
         )
     }
 
-    action = up.plans.ActionInstance(
-        move, (ObjectExp(r1), ObjectExp(c1), ObjectExp(c2)), None, motion_paths
-    )
-
-    plan = up.plans.SequentialPlan([action])
+    plan = up.plans.SequentialPlan([move(r1, c1, c2, motion_paths=motion_paths)])
 
     tamp_feasible = Example(problem=problem, plan=plan)
     problems["tamp_feasible"] = tamp_feasible
 
     return problems
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/testing_variants.py` & `unified_planning-1.0.0/unified_planning/test/examples/testing_variants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-PCP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Rover/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Satellite/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Depots/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Hiking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Robot/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Snake/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Towers/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl` & `unified_planning-1.0.0/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/citycar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/problem.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/citycar/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/counters/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/problem2.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/counters/problem2.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/depot/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/problem.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/depot/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/enhsp.py` & `unified_planning-1.0.0/unified_planning/test/pddl/enhsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -125,14 +125,15 @@
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
+        supported_kind.set_effects_kind("FORALL_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/domain.hddl` & `unified_planning-1.0.0/unified_planning/test/pddl/htn-transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/problem.hddl` & `unified_planning-1.0.0/unified_planning/test/pddl/htn-transport/problem.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/matchcellar/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/matchcellar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/miconic/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/miconic/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/robot_fastener/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/safe_road/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/safe_road/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/sailing/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/sailing/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl` & `unified_planning-1.0.0/unified_planning/test/pddl/visit_precedence/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/jobshop.py` & `unified_planning-1.0.0/unified_planning/test/examples/scheduling/jobshop.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-import unified_planning.test.scheduling.examples
+# Copyright 2021-2023 AIPlan4EU project
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
 from unified_planning.shortcuts import *
 from unified_planning.model.scheduling import *
 from typing import List
 
 # Text representation of the FT-O6 instance (Fisher and Thompson)
 FT06 = """nb_jobs nb_machines
 6 6 0 0 0 0
@@ -19,15 +32,15 @@
 3 4 6 1 2 5
 2 1 3 4 5 6
 3 2 5 6 1 4
 2 4 6 1 5 3
 """
 
 
-def parse(instance: str, instance_name: str):
+def parse(instance: str, instance_name: str) -> SchedulingProblem:
     """Parses a job instance and return the corresponding JobShop with 3 operators instance."""
     lines = instance.splitlines()
 
     def ints(line: str) -> List[int]:
         return list(map(int, line.rstrip().split()))
 
     def int_matrix(lines) -> List[List[int]]:
@@ -45,18 +58,18 @@
 
     first_machine_line = last_times_line + 2
     last_machine_line = first_machine_line + num_jobs - 1
     machines = int_matrix(lines[first_machine_line : last_machine_line + 1])
     # print("Machines: ", machines)
 
     problem = unified_planning.model.scheduling.SchedulingProblem(
-        f"sched:jobshop-{instance_name}"
+        f"sched:jobshop-{instance_name}-operators"
     )
     machine_objects = [
-        problem.add_resource(f"m{i}") for i in range(1, num_machines + 1)
+        problem.add_resource(f"m{i}", capacity=1) for i in range(1, num_machines + 1)
     ]
 
     # use the jobshop with operators extension: each activity requires an operator
     # for its duration
     num_operators = 3
     operators = problem.add_resource("operators", capacity=num_operators)
 
@@ -66,12 +79,18 @@
         for t in range(num_machines):
             act = problem.add_activity(f"t_{j}_{t}", duration=times[j][t])
             machine = machine_objects[machines[j][t] - 1]
             act.uses(machine)
             act.uses(operators, amount=1)
 
             if prev_in_job is not None:
-                act.add_constraint(LE(prev_in_job.end, act.start))
+                problem.add_constraint(LE(prev_in_job.end, act.start))
             prev_in_job = act
 
     problem.add_quality_metric(unified_planning.model.metrics.MinimizeMakespan())
     return problem
+
+
+if __name__ == "__main__":
+    pb = parse(FT06, "ft06-operators")
+    print(pb)
+    print(pb.kind)
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_anml_reader.py` & `unified_planning-1.0.0/unified_planning/test/test_anml_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_anml_writer.py` & `unified_planning-1.0.0/unified_planning/test/test_anml_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_anytime.py` & `unified_planning-1.0.0/unified_planning/test/test_anytime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_bounded_types_remover.py` & `unified_planning-1.0.0/unified_planning/test/test_bounded_types_remover.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_compilers_pipeline.py` & `unified_planning-1.0.0/unified_planning/test/test_compilers_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_compilers_quality_metrics.py` & `unified_planning-1.0.0/unified_planning/test/test_compilers_quality_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_conditional_effects_remover.py` & `unified_planning-1.0.0/unified_planning/test/test_conditional_effects_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_contingent_pddl.py` & `unified_planning-1.0.0/unified_planning/test/test_contingent_pddl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_credits.py` & `unified_planning-1.0.0/unified_planning/test/test_credits.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_disjunctive_conditions_remover.py` & `unified_planning-1.0.0/unified_planning/test/test_disjunctive_conditions_remover.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_dnf.py` & `unified_planning-1.0.0/unified_planning/test/test_dnf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_expression_analysis.py` & `unified_planning-1.0.0/unified_planning/test/test_expression_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_factory.py` & `unified_planning-1.0.0/unified_planning/test/test_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_grounder.py` & `unified_planning-1.0.0/unified_planning/test/test_grounder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_htn.py` & `unified_planning-1.0.0/unified_planning/test/test_htn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_infix_notation.py` & `unified_planning-1.0.0/unified_planning/test/test_infix_notation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_model.py` & `unified_planning-1.0.0/unified_planning/test/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -58,14 +58,16 @@
         self.assertEqual(
             str(e.exception),
             "type of the object does not belong to the same environment of the object",
         )
 
     def test_clone_problem_and_action(self):
         for _, (problem, _) in self.problems.items():
+            if problem.kind.has_scheduling():
+                continue
             problem_clone_1 = problem.clone()
             problem_clone_2 = problem.clone()
             for action_1, action_2 in zip(
                 problem_clone_1.actions, problem_clone_2.actions
             ):
                 if isinstance(action_2, InstantaneousAction):
                     action_2._effects = []
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_multi_agent.py` & `unified_planning-1.0.0/unified_planning/test/test_multi_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_negative_conditions_remover.py` & `unified_planning-1.0.0/unified_planning/test/test_negative_conditions_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_partial_order_plan.py` & `unified_planning-1.0.0/unified_planning/test/test_partial_order_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -34,20 +34,23 @@
     def test_all(self):
         with PlanValidator(name="sequential_plan_validator") as validator:
             assert validator is not None
             for problem, plan in self.problems.values():
                 if validator.supports(problem.kind):
                     self.assertTrue(isinstance(plan, up.plans.SequentialPlan))
                     pop_plan = plan.convert_to(PlanKind.PARTIAL_ORDER_PLAN, problem)
-                    for sorted_plan in pop_plan.all_sequential_plans():
+                    for i, sorted_plan in enumerate(pop_plan.all_sequential_plans()):
                         validation_result = validator.validate(problem, sorted_plan)
                         self.assertEqual(
                             up.engines.ValidationResultStatus.VALID,
                             validation_result.status,
+                            msg=f"\n{problem}\n{sorted_plan}",
                         )
+                        if i > 100:
+                            break
 
     @skipIfNoOneshotPlannerForProblemKind(basic_classical_kind.union(hierarchical_kind))
     def test_blocks_world(self):
         problem = self.problems["hierarchical_blocks_world"].problem
         with Compiler(
             problem_kind=problem.kind,
             compilation_kinds=[
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_pddl_io.py` & `unified_planning-1.0.0/unified_planning/test/test_pddl_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -478,14 +478,15 @@
                 or kind.has_timed_goals()
                 or kind.has_bool_fluent_parameters()
                 or kind.has_bounded_int_fluent_parameters()
                 or kind.has_bool_action_parameters()
                 or kind.has_bounded_int_action_parameters()
                 or kind.has_unbounded_int_action_parameters()
                 or kind.has_real_action_parameters()
+                or kind.has_scheduling()
             ):
                 continue
             with tempfile.TemporaryDirectory() as tempdir:
                 domain_filename = os.path.join(tempdir, "domain.pddl")
                 problem_filename = os.path.join(tempdir, "problem.pddl")
 
                 w = PDDLWriter(problem)
@@ -750,16 +751,16 @@
         problem = reader.parse_problem(domain_filename, problem_filename)
 
         self.assertTrue(problem is not None)
         self.assertEqual(len(problem.fluents), 1)
         self.assertEqual(len(problem.actions), 2)
         natural_disaster = problem.action("natural_disaster")
         assert isinstance(natural_disaster, InstantaneousAction)
-        # 9 effects because the forall is expanded in 3 * 3 possible locations instantiations
-        self.assertEqual(len(natural_disaster.effects), 9)
+        self.assertEqual(len(natural_disaster.effects), 1)
+        self.assertTrue(natural_disaster.effects[0].is_forall())
         self.assertEqual(len(list(problem.objects(problem.user_type("location")))), 3)
 
     @skipIfNoOneshotPlannerForProblemKind(
         simple_numeric_kind, OptimalityGuarantee.SOLVED_OPTIMALLY
     )
     def test_reading_domain_only(self):
         reader = PDDLReader()
@@ -790,14 +791,39 @@
             problem.add_quality_metric(MinimizeSequentialPlanLength())
             with OneshotPlanner(
                 problem_kind=problem.kind, optimality_guarantee="SOLVED_OPTIMALLY"
             ) as planner:
                 plan = planner.solve(problem).plan
                 self.assertEqual(len(plan.actions), expected_plan_length)
 
+    def test_writer_nested_and(self):
+        x, y, z = Fluent("x"), Fluent("y"), Fluent("z")
+        goals: List[FNode] = [
+            And(x, y),
+            And(x, And(y, z)),
+            And(Or(x, y), And(y, z)),
+        ]
+        expected_goals: List[str] = [
+            "(:goal (and (x) (y)))\n",
+            "(:goal (and (x) (y) (z)))\n",
+            "(:goal (and (or (x) (y)) (y) (z)))\n",
+        ]
+        assert len(goals) == len(
+            expected_goals
+        ), "goals and expected_goals must have the same length"
+        for i, (goal, expected_goal) in enumerate(zip(goals, expected_goals)):
+            problem = Problem(f"test_{i}")
+            problem.add_fluent(x, default_initial_value=False)
+            problem.add_fluent(y, default_initial_value=False)
+            problem.add_fluent(z, default_initial_value=False)
+            problem.add_goal(goal)
+            writer = PDDLWriter(problem)
+            pddl_problem = writer.get_problem()
+            self.assertIn(expected_goal, pddl_problem)
+
 
 def _have_same_user_types_considering_renamings(
     original_problem: unified_planning.model.Problem,
     tested_problem: unified_planning.model.Problem,
     get_item_named,
 ) -> bool:
     for tested_type in tested_problem.user_types:
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_pddl_planner.py` & `unified_planning-1.0.0/unified_planning/test/test_pddl_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_plan_validator.py` & `unified_planning-1.0.0/unified_planning/test/test_plan_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_planner.py` & `unified_planning-1.0.0/unified_planning/test/test_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -186,14 +186,15 @@
                     problem, CompilationKind.QUANTIFIERS_REMOVING
                 )
                 suitable_problem = res.problem
                 final_report = planner.solve(suitable_problem)
                 plan = final_report.plan.replace_action_instances(
                     res.map_back_action_instance
                 )
+
                 self.assertEqual(
                     final_report.status, PlanGenerationResultStatus.SOLVED_SATISFICING
                 )
                 self.assertEqual(len(plan.timed_actions), 2)
                 self.assertEqual((plan.timed_actions[0])[1].action, move)
                 self.assertEqual((plan.timed_actions[1])[1].action, move)
 
@@ -305,14 +306,23 @@
             self.assertEqual(error_msg, str(e.exception))
 
             # Or we can set the check to be completely skipped
             planner.skip_checks = True
             plan = planner.solve(problem).plan
             self.assertIsNotNone(plan)
 
+    @skipIfEngineNotAvailable("opt-pddl-planner")
+    def test_safe_road(self):
+        problem = self.problems["safe_road"].problem
+        with OneshotPlanner(name="opt-pddl-planner") as planner:
+            self.assertTrue(planner.supports(problem.kind))
+            res = planner.solve(problem)
+            plan = res.plan
+            self.assertEqual(len(plan.actions), 10)
+
     def test_engine_class(self):
         with self.assertRaises(TypeError):
             Engine()  # type: ignore[abstract]
 
         class OneshotEnginePartial(Engine, OneshotPlannerMixin):
             @property
             def name(self):
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_problem.py` & `unified_planning-1.0.0/unified_planning/test/test_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -524,20 +524,27 @@
             "robot_decrease",
             "robot_locations_connected",
             "robot_locations_visited",
             "robot_fluent_of_user_type_with_int_id",
             "basic_int_fluent_param",
             "basic_bounded_int_action_param",
             "basic_unbounded_int_action_param",
+            "sched:basic",
+            "sched:resource_set",
+            "sched:jobshop-ft06-operators",
         ]
         for problem, _ in self.problems.values():
             if problem.name in names_of_SNP_problems:
-                self.assertTrue(problem.kind.has_simple_numeric_planning())
+                self.assertTrue(
+                    problem.kind.has_simple_numeric_planning(), problem.name
+                )
             else:
-                self.assertFalse(problem.kind.has_simple_numeric_planning())
+                self.assertFalse(
+                    problem.kind.has_simple_numeric_planning(), problem.name
+                )
 
     def test_simple_numeric_planning_ad_hoc_1(self):
         problem = Problem("ad_hoc_1")
         Location = UserType("Location")
         is_at = Fluent("is_at", position=Location)
         distance = Fluent("distance", IntType(), loc_1=Location, loc_2=Location)
         total_distance = Fluent("total_distance", IntType())
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_protobuf_io.py` & `unified_planning-1.0.0/unified_planning/test/test_protobuf_io.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -127,15 +127,15 @@
 
         problem = self.problems["robot"].problem
 
         problem_pb = self.pb_writer.convert(problem)
         problem_up = self.pb_reader.convert(problem_pb)
 
         pb_features = set(
-            [up_pb2.Feature.Name(feature) for feature in problem_pb.features]
+            [up_pb2.Feature.Name(feature) for feature in problem_pb.features]  # type: ignore[attr-defined]
         )
         self.assertEqual(set(problem.kind.features), pb_features)
         self.assertEqual(problem, problem_up)
 
     def test_action(self):
         problem = self.problems["robot"].problem
         action = problem.action("move")
@@ -274,50 +274,50 @@
         problem_up = self.pb_reader.convert(problem_pb)
 
         self.assertEqual(problem, problem_up)
 
     def test_timing_expressions(self):
         def build(
             timing: Timing, action: Union[Action, None] = None
-        ) -> proto.Expression:
+        ) -> proto.Expression:  # type: ignore[name-defined]
             problem = Problem("test timing")
             if action is not None:
                 problem.add_action(action)
             node = problem.environment.expression_manager.auto_promote(timing)[0]
             node_pb = self.pb_writer.convert(node)
             node_up = self.pb_reader.convert(node_pb, problem)
             self.assertEqual(node, node_up)
             return node_pb
 
         def check(  # pylint: disable = too-many-arguments
-            expr: proto.Expression,
+            expr: proto.Expression,  # type: ignore[name-defined]
             kind: int,
             tpe: str = "",
             length: Union[int, None] = None,
             integer: Union[int, None] = None,
             real: Union[Fraction, None] = None,
             symbol: Union[str, None] = None,
         ) -> None:
             self.assertEqual(expr.kind, kind)
             self.assertEqual(expr.type, tpe)
             if length is not None:
                 self.assertEqual(len(expr.list), length)
             if integer is not None:
-                self.assertEqual(expr.atom, proto.Atom(int=integer))
+                self.assertEqual(expr.atom, proto.Atom(int=integer))  # type: ignore[attr-defined]
             if real is not None:
-                _pr = proto.Real(numerator=real.numerator, denominator=real.denominator)
-                self.assertEqual(expr.atom, proto.Atom(real=_pr))
+                _pr = proto.Real(numerator=real.numerator, denominator=real.denominator)  # type: ignore[attr-defined]
+                self.assertEqual(expr.atom, proto.Atom(real=_pr))  # type: ignore[attr-defined]
             if symbol is not None:
-                self.assertEqual(expr.atom, proto.Atom(symbol=symbol))
+                self.assertEqual(expr.atom, proto.Atom(symbol=symbol))  # type: ignore[attr-defined]
 
         # pylint: disable = invalid-name
-        cont_kind = proto.ExpressionKind.Value("CONTAINER_ID")
-        const_kind = proto.ExpressionKind.Value("CONSTANT")
-        fun_app_kind = proto.ExpressionKind.Value("FUNCTION_APPLICATION")
-        fun_sym_kind = proto.ExpressionKind.Value("FUNCTION_SYMBOL")
+        cont_kind = proto.ExpressionKind.Value("CONTAINER_ID")  # type: ignore[attr-defined]
+        const_kind = proto.ExpressionKind.Value("CONSTANT")  # type: ignore[attr-defined]
+        fun_app_kind = proto.ExpressionKind.Value("FUNCTION_APPLICATION")  # type: ignore[attr-defined]
+        fun_sym_kind = proto.ExpressionKind.Value("FUNCTION_SYMBOL")  # type: ignore[attr-defined]
         cont_type = "up:container"
         int_type = "up:integer"
         real_type = "up:real"
         time_type = "up:time"
         add_symbol = "up:plus"
         start_symbol = "up:start"
         end_symbol = "up:end"
@@ -427,14 +427,16 @@
                     f"[hash] Error on problem {name}: \n\n{problem}\n=====\n{problem_up}",
                 )
 
     def test_all_plans(self):
         for name, example in self.problems.items():
             problem = example.problem
             plan = example.plan
+            if plan is None:
+                continue
             plan_pb = self.pb_writer.convert(plan)
             plan_up = self.pb_reader.convert(plan_pb, problem)
 
             self.assertEqual(plan, plan_up)
             self.assertEqual(hash(plan), hash(plan_up))
 
     @skipIfEngineNotAvailable("tamer")
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_pyperplan.py` & `unified_planning-1.0.0/unified_planning/test/test_pyperplan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_quantifier_remover.py` & `unified_planning-1.0.0/unified_planning/test/test_quantifier_remover.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -215,7 +215,68 @@
         res = qr.compile(problem, CompilationKind.QUANTIFIERS_REMOVING)
         unq_problem = res.problem
         assert unq_problem is not None
         self.assertTrue(problem.kind.has_existential_conditions())
         self.assertTrue(problem.kind.has_universal_conditions())
         self.assertFalse(unq_problem.kind.has_existential_conditions())
         self.assertFalse(unq_problem.kind.has_universal_conditions())
+
+    def test_forall_effects_removing(self):
+        Obj = UserType("Obj")
+        Obj_son = UserType("Obj_son", Obj)
+
+        Obj_objects = list(Object(f"o{i}", Obj) for i in range(3))
+        son_objects = list(Object(f"s{i}", Obj_son) for i in range(2))
+
+        o0, o1, o2 = Obj_objects
+        s0, s1 = son_objects
+
+        x = Fluent("x", Obj, p1=Obj)
+        y = Fluent("y", Obj, p1=Obj, p2=Obj_son)
+
+        v0, v1 = Variable("v0", Obj), Variable("v1", Obj_son)
+        a = InstantaneousAction("a")
+        a.add_effect(x(v0), y(v0, s0), forall=[v0])
+        b = DurativeAction("b")
+        b.add_effect(StartTiming(), y(v0, v1), x(v1), forall=[v0, v1])
+
+        problem = Problem("forall_effects")
+        problem.add_objects(Obj_objects)
+        problem.add_objects(son_objects)
+        problem.add_actions((a, b))
+        qr = QuantifiersRemover()
+        res = qr.compile(problem, CompilationKind.QUANTIFIERS_REMOVING)
+        unq_problem = res.problem
+        assert isinstance(unq_problem, Problem)
+        expected_effects = {
+            a: [
+                (x(o0), y(o0, s0)),
+                (x(o1), y(o1, s0)),
+                (x(o2), y(o2, s0)),
+                (x(s0), y(s0, s0)),
+                (x(s1), y(s1, s0)),
+            ],
+            b: [
+                (y(o0, s0), x(s0)),
+                (y(o0, s1), x(s1)),
+                (y(o1, s0), x(s0)),
+                (y(o1, s1), x(s1)),
+                (y(o2, s0), x(s0)),
+                (y(o2, s1), x(s1)),
+                (y(s0, s0), x(s0)),
+                (y(s0, s1), x(s1)),
+                (y(s1, s0), x(s0)),
+                (y(s1, s1), x(s1)),
+            ],
+        }
+        for action, assignments in expected_effects.items():
+            unq_action = unq_problem.action(action.name)
+            if isinstance(unq_action, InstantaneousAction):
+                effects = unq_action.effects
+            else:
+                assert isinstance(unq_action, DurativeAction)
+                effects = unq_action.effects[StartTiming()]
+            self.assertEqual(len(assignments), len(effects))
+            for fluent, value in assignments:
+                self.assertTrue(
+                    any(e.fluent == fluent and e.value == value for e in effects)
+                )
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_replanner.py` & `unified_planning-1.0.0/unified_planning/test/test_replanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_scheduling.py` & `unified_planning-1.0.0/unified_planning/test/test_scheduling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,15 +24,15 @@
 
 
 FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 
 
 class TestScheduling(TestCase):
     def test_load_all(self):
-        problems = up.test.scheduling.problems()
+        problems = up.test.examples.scheduling.get_example_problems()
         for name, test_case in problems.items():
             problem = test_case.problem
             print(f"======== {name} =============")
             print(problem)
 
             cloned = problem.clone()
             self.assertEqual(problem, cloned)
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_sequential_simulator.py` & `unified_planning-1.0.0/unified_planning/test/test_sequential_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -118,15 +118,15 @@
 
         self.assertTrue(simulator.is_goal(state))
 
         with self.assertRaises(UPUsageError):
             _ = simulator.apply(state, move, (ts_1, block_3, block_2))
         with self.assertRaises(UPUsageError):
             ai = ActionInstance(
-                move, (ObjectExp(ts_1), ObjectExp(block_3), ObjectExp(block_2))
+                move, (ObjectExp(block_3), ObjectExp(ts_1), ObjectExp(block_2))
             )
             _ = simulator.apply(state, ai, (ts_1, block_3, block_2))
 
     def test_with_sequential_simulator_instance(self):
         problem = self.problems["hierarchical_blocks_world"].problem
         simulator = UPSequentialSimulator(problem)
         self.simulate_on_hierarchical_blocks_world(simulator, problem)
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_simplifier.py` & `unified_planning-1.0.0/unified_planning/test/test_simplifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_simulated_effects.py` & `unified_planning-1.0.0/unified_planning/test/test_simulated_effects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_state_invariants.py` & `unified_planning-1.0.0/unified_planning/test/test_state_invariants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_stn_plan.py` & `unified_planning-1.0.0/unified_planning/test/test_stn_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_substituter.py` & `unified_planning-1.0.0/unified_planning/test/test_substituter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_tamp.py` & `unified_planning-1.0.0/unified_planning/test/test_tamp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_tarski_converter.py` & `unified_planning-1.0.0/unified_planning/test/test_tarski_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_tarski_grounder.py` & `unified_planning-1.0.0/unified_planning/test/test_tarski_grounder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_temporal.py` & `unified_planning-1.0.0/unified_planning/test/test_temporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_trajectory_constraint.py` & `unified_planning-1.0.0/unified_planning/test/test_trajectory_constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_trajectory_constraints_remover.py` & `unified_planning-1.0.0/unified_planning/test/test_trajectory_constraints_remover.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_usertype_fluents_remover.py` & `unified_planning-1.0.0/unified_planning/test/test_usertype_fluents_remover.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/test/test_validator.py` & `unified_planning-1.0.0/unified_planning/test/test_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning/utils.py` & `unified_planning-1.0.0/unified_planning/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 AIPlan4EU project
+# Copyright 2021-2023 AIPlan4EU project
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning.egg-info/PKG-INFO` & `unified_planning-1.0.0/unified_planning.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: unified-planning
-Version: 0.6.0.94.dev1
+Version: 1.0.0
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
-Description: UNKNOWN
+Description: Unified Planning: A library that makes it easy to formulate planning problems and to invoke automated planners.
 Keywords: planning logic STRIPS RDDL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: grpc
 Provides-Extra: tarski
 Provides-Extra: pyperplan
 Provides-Extra: tamer
 Provides-Extra: enhsp
 Provides-Extra: fast-downward
 Provides-Extra: lpg
 Provides-Extra: fmap
 Provides-Extra: aries
 Provides-Extra: symk
 Provides-Extra: engines
+Provides-Extra: plot
```

### Comparing `unified_planning-0.6.0.94.dev1/unified_planning.egg-info/SOURCES.txt` & `unified_planning-1.0.0/unified_planning.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 unified_planning/environment.py
 unified_planning/exceptions.py
 unified_planning/shortcuts.py
 unified_planning/utils.py
 unified_planning.egg-info/PKG-INFO
 unified_planning.egg-info/SOURCES.txt
 unified_planning.egg-info/dependency_links.txt
+unified_planning.egg-info/entry_points.txt
 unified_planning.egg-info/requires.txt
 unified_planning.egg-info/top_level.txt
+unified_planning/cmd/__init__.py
+unified_planning/cmd/arg_parser.py
+unified_planning/cmd/up.py
 unified_planning/engines/__init__.py
 unified_planning/engines/credits.py
 unified_planning/engines/engine.py
 unified_planning/engines/factory.py
 unified_planning/engines/meta_engine.py
 unified_planning/engines/oversubscription_planner.py
 unified_planning/engines/parallel.py
@@ -27,14 +31,16 @@
 unified_planning/engines/sequential_simulator.py
 unified_planning/engines/compilers/__init__.py
 unified_planning/engines/compilers/bounded_types_remover.py
 unified_planning/engines/compilers/compilers_pipeline.py
 unified_planning/engines/compilers/conditional_effects_remover.py
 unified_planning/engines/compilers/disjunctive_conditions_remover.py
 unified_planning/engines/compilers/grounder.py
+unified_planning/engines/compilers/ma_conditional_effects_remover.py
+unified_planning/engines/compilers/ma_disjunctive_conditions_remover.py
 unified_planning/engines/compilers/negative_conditions_remover.py
 unified_planning/engines/compilers/quantifiers_remover.py
 unified_planning/engines/compilers/state_invariants_remover.py
 unified_planning/engines/compilers/tarski_grounder.py
 unified_planning/engines/compilers/trajectory_constraints_remover.py
 unified_planning/engines/compilers/usertype_fluents_remover.py
 unified_planning/engines/compilers/utils.py
@@ -133,17 +139,22 @@
 unified_planning/model/walkers/type_checker.py
 unified_planning/model/walkers/usertype_fluents_walker.py
 unified_planning/plans/__init__.py
 unified_planning/plans/contingent_plan.py
 unified_planning/plans/hierarchical_plan.py
 unified_planning/plans/partial_order_plan.py
 unified_planning/plans/plan.py
+unified_planning/plans/schedule.py
 unified_planning/plans/sequential_plan.py
 unified_planning/plans/stn_plan.py
 unified_planning/plans/time_triggered_plan.py
+unified_planning/plot/__init__.py
+unified_planning/plot/causal_graph_plot.py
+unified_planning/plot/plan_plot.py
+unified_planning/plot/utils.py
 unified_planning/test/__init__.py
 unified_planning/test/test_anml_reader.py
 unified_planning/test/test_anml_writer.py
 unified_planning/test/test_anytime.py
 unified_planning/test/test_bounded_types_remover.py
 unified_planning/test/test_compilers_pipeline.py
 unified_planning/test/test_compilers_quality_metrics.py
@@ -153,14 +164,16 @@
 unified_planning/test/test_disjunctive_conditions_remover.py
 unified_planning/test/test_dnf.py
 unified_planning/test/test_expression_analysis.py
 unified_planning/test/test_factory.py
 unified_planning/test/test_grounder.py
 unified_planning/test/test_htn.py
 unified_planning/test/test_infix_notation.py
+unified_planning/test/test_ma_conditional_effects_remover.py
+unified_planning/test/test_ma_disjunctive_conditions_remover.py
 unified_planning/test/test_model.py
 unified_planning/test/test_multi_agent.py
 unified_planning/test/test_negative_conditions_remover.py
 unified_planning/test/test_partial_order_plan.py
 unified_planning/test/test_pddl_io.py
 unified_planning/test/test_pddl_planner.py
 unified_planning/test/test_plan_validator.py
@@ -206,14 +219,17 @@
 unified_planning/test/examples/__init__.py
 unified_planning/test/examples/hierarchical.py
 unified_planning/test/examples/minimals.py
 unified_planning/test/examples/multi_agent.py
 unified_planning/test/examples/realistic.py
 unified_planning/test/examples/tamp.py
 unified_planning/test/examples/testing_variants.py
+unified_planning/test/examples/scheduling/__init__.py
+unified_planning/test/examples/scheduling/examples.py
+unified_planning/test/examples/scheduling/jobshop.py
 unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
 unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
 unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
 unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
 unified_planning/test/hddl/2020-po-PCP/domain.hddl
 unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
 unified_planning/test/hddl/2020-po-Rover/domain.hddl
@@ -284,11 +300,8 @@
 unified_planning/test/pddl/robot_fastener/domain.pddl
 unified_planning/test/pddl/robot_fastener/problem.pddl
 unified_planning/test/pddl/safe_road/domain.pddl
 unified_planning/test/pddl/safe_road/problem.pddl
 unified_planning/test/pddl/sailing/domain.pddl
 unified_planning/test/pddl/sailing/problem.pddl
 unified_planning/test/pddl/visit_precedence/domain.pddl
-unified_planning/test/pddl/visit_precedence/problem.pddl
-unified_planning/test/scheduling/__init__.py
-unified_planning/test/scheduling/examples.py
-unified_planning/test/scheduling/jobshop.py
+unified_planning/test/pddl/visit_precedence/problem.pddl
```

