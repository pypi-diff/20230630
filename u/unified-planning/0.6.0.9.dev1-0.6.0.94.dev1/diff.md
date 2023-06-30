# Comparing `tmp/unified_planning-0.6.0.9.dev1.tar.gz` & `tmp/unified_planning-0.6.0.94.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified_planning-0.6.0.9.dev1.tar", last modified: Thu May  4 15:32:36 2023, max compression
+gzip compressed data, was "unified_planning-0.6.0.94.dev1.tar", last modified: Tue May 30 12:39:20 2023, max compression
```

## Comparing `unified_planning-0.6.0.9.dev1.tar` & `unified_planning-0.6.0.94.dev1.tar`

### file list

```diff
@@ -1,360 +1,361 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.579271 unified_planning-0.6.0.9.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 15:32:36.579271 unified_planning-0.6.0.9.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:32:36.579271 unified_planning-0.6.0.9.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.543269 unified_planning-0.6.0.9.dev1/unified_planning/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.547269 unified_planning-0.6.0.9.dev1/unified_planning/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.547269 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    17677 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    18492 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/credits.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    41064 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/meta_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.547269 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/oneshot_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/plan_repairer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/oversubscription_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.551269 unified_planning-0.6.0.9.dev1/unified_planning/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.551269 unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35468 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/proto_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    33343 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/proto_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.551269 unified_planning-0.6.0.9.dev1/unified_planning/interop/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/interop/from_tarski.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/interop/to_tarski.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.551269 unified_planning-0.6.0.9.dev1/unified_planning/io/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/anml_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)    41213 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    37842 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/ma_pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    74227 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/pddl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    37139 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    26929 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/python_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    28405 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/contingent_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/delta_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/fnode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/hierarchical_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/task_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/actions_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/agents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/fluents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/initial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/objects_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/time_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/timed_conds_effs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/user_types_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/ma_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/ma_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38729 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/problem_kind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/chronicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/scheduling_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/type_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.559270 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/any.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/fluents_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/free_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/linear_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/names_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/operators_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/quantifier_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/state_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.559270 unified_planning-0.6.0.9.dev1/unified_planning/plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/contingent_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/hierarchical_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/sequential_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/time_triggered_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    27425 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.563270 unified_planning-0.6.0.9.dev1/unified_planning/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/basic.anml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/basic_conditional.anml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/connected_locations.anml
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/constants.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/durative_goals.anml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/forall.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/hydrone.anml
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match.anml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match_int_id.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match_test_parser.anml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/simple_mais.anml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/tils.anml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.539269 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/minimals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    38724 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/realistic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30699 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/testing_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.543269 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/problem2.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/matchcellar/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/miconic/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/miconic/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/miconic/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/robot_fastener/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/safe_road/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/safe_road/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/safe_road/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/sailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/sailing/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/sailing/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/visit_precedence/
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/jobshop.py
--rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_anytime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_compilers_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_contingent_pddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_credits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_expression_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_htn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_infix_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    32858 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_pddl_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_protobuf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_pyperplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_python_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_quantifier_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_simulated_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_tarski_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_trajectory_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.543269 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.343699 unified_planning-0.6.0.94.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 12:39:20.343699 unified_planning-0.6.0.94.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:39:20.343699 unified_planning-0.6.0.94.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.239698 unified_planning-0.6.0.94.dev1/unified_planning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.247698 unified_planning-0.6.0.94.dev1/unified_planning/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.251698 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17039 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7771 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/state_invariants_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19514 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20529 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48097 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/meta_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.251698 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/oneshot_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/plan_repairer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/oversubscription_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/pddl_anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19891 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34287 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/engines/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.255698 unified_planning-0.6.0.94.dev1/unified_planning/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.255698 unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36383 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34146 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/proto_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34502 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/grpc/proto_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.255698 unified_planning-0.6.0.94.dev1/unified_planning/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/interop/from_tarski.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/interop/to_tarski.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.259698 unified_planning-0.6.0.94.dev1/unified_planning/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/anml_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41213 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37842 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/ma_pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75013 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/pddl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37231 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.263698 unified_planning-0.6.0.94.dev1/unified_planning/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28405 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/contingent_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/delta_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/fnode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.267698 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/hierarchical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/htn/task_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.267698 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/actions_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/agents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/fluents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/initial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/objects_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/time_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/timed_conds_effs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/user_types_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.271698 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/ma_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/ma_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40918 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/problem_kind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.271698 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/chronicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/scheduling_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.271698 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.279698 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/fluents_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/free_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/linear_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/names_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/operators_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/quantifier_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/state_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.283698 unified_planning-0.6.0.94.dev1/unified_planning/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/contingent_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/hierarchical_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/sequential_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/plans/time_triggered_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30667 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.295699 unified_planning-0.6.0.94.dev1/unified_planning/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.299699 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/basic.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/basic_conditional.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/connected_locations.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/constants.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/durative_goals.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/forall.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/hydrone.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match_int_id.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match_test_parser.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/simple_mais.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/anml/tils.anml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.235698 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.299699 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.299699 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.303699 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/minimals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39048 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/realistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37275 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/examples/testing_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.239698 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.303699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.303699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.307699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-PCP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.307699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.307699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.307699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.311699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.311699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.311699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.311699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.315699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.315699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.315699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.315699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.319699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.319699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.319699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.319699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.323699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.327699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.327699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.327699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Towers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.327699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.331699 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.331699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.331699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.331699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/problem2.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.335699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.335699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.335699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/matchcellar/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.335699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/miconic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/miconic/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/miconic/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.339699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/robot_fastener/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.339699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/safe_road/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/safe_road/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/safe_road/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.339699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/sailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/sailing/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/sailing/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.339699 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/visit_precedence/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.343699 unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/jobshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_anytime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_compilers_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_contingent_pddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_expression_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_htn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_infix_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33608 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_pddl_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25081 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_protobuf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_pyperplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_quantifier_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_simulated_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_state_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_tarski_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_trajectory_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-30 12:39:16.000000 unified_planning-0.6.0.94.dev1/unified_planning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:39:20.243698 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 12:39:19.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-05-30 12:39:20.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:39:19.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-30 12:39:19.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 12:39:19.000000 unified_planning-0.6.0.94.dev1/unified_planning.egg-info/top_level.txt
```

### Comparing `unified_planning-0.6.0.9.dev1/LICENSE` & `unified_planning-0.6.0.94.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/PKG-INFO` & `unified_planning-0.6.0.94.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified_planning
-Version: 0.6.0.9.dev1
+Version: 0.6.0.94.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: UNKNOWN
 Keywords: planning logic STRIPS RDDL
@@ -25,8 +25,9 @@
 Provides-Extra: pyperplan
 Provides-Extra: tamer
 Provides-Extra: enhsp
 Provides-Extra: fast-downward
 Provides-Extra: lpg
 Provides-Extra: fmap
 Provides-Extra: aries
+Provides-Extra: symk
 Provides-Extra: engines
```

### Comparing `unified_planning-0.6.0.9.dev1/README.md` & `unified_planning-0.6.0.94.dev1/README.md`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/setup.py` & `unified_planning-0.6.0.94.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,29 +22,31 @@
     python_requires=">=3.7",  # supported Python ranges
     install_requires=["pyparsing", "networkx"],
     extras_require={
         "dev": ["tarski[arithmetic]", "pytest", "pytest-cov", "mypy"],
         "grpc": ["grpcio", "grpcio-tools", "grpc-stubs"],
         "tarski": ["tarski[arithmetic]"],
         "pyperplan": ["up-pyperplan==0.3.0.4.dev1"],
-        "tamer": ["up-tamer==0.3.1.22.dev1"],
+        "tamer": ["up-tamer==0.3.1.26.dev1"],
         "enhsp": ["up-enhsp==0.0.13"],
         "fast-downward": ["up-fast-downward==0.2.1"],
         "lpg": ["up-lpg==0.0.6.3"],
         "fmap": ["up-fmap==0.0.6"],
         "aries": ["up-aries>=0.0.8"],
+        "symk": ["up-symk>=0.0.3"],
         "engines": [
             "tarski[arithmetic]",
             "up-pyperplan==0.3.0.4.dev1",
-            "up-tamer==0.3.1.22.dev1",
+            "up-tamer==0.3.1.26.dev1",
             "up-enhsp==0.0.13",
             "up-fast-downward==0.2.1",
             "up-lpg==0.0.6.3",
             "up-fmap==0.0.6",
             "up-aries>=0.0.8",
+            "up-symk>=0.0.3",
         ],
     },
     license="APACHE",
     keywords="planning logic STRIPS RDDL",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from unified_planning.engines.engine import Engine, OperationMode
 from unified_planning.engines.meta_engine import MetaEngine
 from unified_planning.engines.credits import Credits
 from unified_planning.engines.factory import Factory
 from unified_planning.engines.parallel import Parallel
 from unified_planning.engines.pddl_planner import PDDLPlanner
+from unified_planning.engines.pddl_anytime_planner import PDDLAnytimePlanner
 from unified_planning.engines.plan_validator import SequentialPlanValidator
 from unified_planning.engines.oversubscription_planner import OversubscriptionPlanner
 from unified_planning.engines.replanner import Replanner
 from unified_planning.engines.results import (
     Result,
     LogMessage,
     PlanGenerationResult,
@@ -48,14 +49,15 @@
 from unified_planning.engines.mixins.portfolio import PortfolioSelectorMixin
 
 __all__ = [
     "Factory",
     "Grounder",
     "Parallel",
     "PDDLPlanner",
+    "PDDLAnytimePlanner",
     "SequentialPlanValidator",
     "SequentialSimulatorMixin",
     "UPSequentialSimulator",
     "Event",
     "InstantaneousEvent",
     "Engine",
     "OptimalityGuarantee",
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 from unified_planning.engines.compilers.bounded_types_remover import BoundedTypesRemover
 from unified_planning.engines.compilers.conditional_effects_remover import (
     ConditionalEffectsRemover,
 )
 from unified_planning.engines.compilers.disjunctive_conditions_remover import (
     DisjunctiveConditionsRemover,
 )
+from unified_planning.engines.compilers.state_invariants_remover import (
+    StateInvariantsRemover,
+)
 from unified_planning.engines.compilers.grounder import Grounder, GrounderHelper
 from unified_planning.engines.compilers.quantifiers_remover import QuantifiersRemover
 from unified_planning.engines.compilers.negative_conditions_remover import (
     NegativeConditionsRemover,
 )
 from unified_planning.engines.compilers.trajectory_constraints_remover import (
     TrajectoryConstraintsRemover,
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/bounded_types_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/bounded_types_remover.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,20 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("REAL_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
@@ -84,15 +90,17 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/compilers_pipeline.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/conditional_effects_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/conditional_effects_remover.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,20 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("REAL_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
@@ -92,15 +98,17 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,20 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("REAL_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
@@ -94,14 +100,15 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/grounder.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/grounder.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,17 +146,17 @@
         """
         Returns an iterator over all the possible grounded actions of the problem given at construction time.
         Every resulting tuple is made of 3 elements: ``original_action``, ``parameters``, ``grounded_action`` where:
 
         * The ``original_action`` is the `Action` of the ``Problem`` that is grounded.
         * The ``parameters`` is the `Tuple of expressions` used to ground the ``original_action``.
         * The ``grounded_action`` is the `Action` created by grounding the ``original_action`` with the given ``parameters``;
-        the ``grounded_action`` can be ``None`` if the grounding of the ``original_action`` with the given parameters
-        creates an invalid or meaningless `Action` (invalid if it has conflicting `Effects`,
-        meaningless if it has no `effects` or contradicting `conditions`).
+            the ``grounded_action`` can be ``None`` if the grounding of the ``original_action`` with the given parameters
+            creates an invalid or meaningless `Action` (invalid if it has conflicting `Effects`,
+            meaningless if it has no `effects` or contradicting `conditions`).
         """
         for old_action in self._problem.actions:
             for grounded_params in self.get_possible_parameters(old_action):
                 assert isinstance(grounded_params, tuple)
                 new_action = self.ground_action(old_action, grounded_params)
                 yield (old_action, grounded_params, new_action)
 
@@ -239,14 +239,18 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
@@ -265,17 +269,19 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
         supported_kind.set_expression_duration("FLUENTS_IN_DURATIONS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/negative_conditions_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/negative_conditions_remover.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,20 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("REAL_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
@@ -127,14 +133,17 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_time("SELF_OVERLAPPING")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
+        supported_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
@@ -229,14 +238,18 @@
                 ng = fluent_remover.remove_negative_fluents(g)
                 new_problem.add_timed_goal(i, ng)
 
         for g in problem.goals:
             ng = fluent_remover.remove_negative_fluents(g)
             new_problem.add_goal(ng)
 
+        for tc in problem.trajectory_constraints:
+            ntc = fluent_remover.remove_negative_fluents(tc)
+            new_problem.add_trajectory_constraint(ntc)
+
         for qm in problem.quality_metrics:
             if qm.is_minimize_action_costs():
                 new_problem.add_quality_metric(
                     updated_minimize_action_costs(
                         qm, new_to_old, new_problem.environment
                     )
                 )
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/quantifiers_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/quantifiers_remover.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,20 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("REAL_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
@@ -94,15 +100,18 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
+        supported_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
@@ -218,14 +227,21 @@
                 e.set_value(
                     expression_quantifier_remover.remove_quantifiers(e.value, problem)
                 )
         for i, gl in problem.timed_goals.items():
             for g in gl:
                 ng = expression_quantifier_remover.remove_quantifiers(g, problem)
                 new_problem.add_timed_goal(i, ng)
+        for tc in problem.trajectory_constraints:
+            ngc = expression_quantifier_remover.remove_quantifiers(tc, problem)
+            if ngc.is_and():
+                for arg in ngc.args:
+                    new_problem.add_trajectory_constraint(arg)
+            else:
+                new_problem.add_trajectory_constraint(ngc)
         for g in problem.goals:
             ng = expression_quantifier_remover.remove_quantifiers(g, problem)
             new_problem.add_goal(ng)
         for qm in problem.quality_metrics:
             if qm.is_minimize_action_costs():
                 new_problem.add_quality_metric(
                     updated_minimize_action_costs(
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/tarski_grounder.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/tarski_grounder.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         supported_kind.set_typing("HIERARCHICAL_TYPING")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         supported_kind.set_conditions_kind("EQUALITIES")
         supported_kind.set_conditions_kind("EXISTENTIAL_CONDITIONS")
         supported_kind.set_conditions_kind("UNIVERSAL_CONDITIONS")
         supported_kind.set_effects_kind("CONDITIONAL_EFFECTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         return supported_kind
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,24 +69,31 @@
         return compilation_kind == CompilationKind.TRAJECTORY_CONSTRAINTS_REMOVING
 
     @staticmethod
     def resulting_problem_kind(
         problem_kind: ProblemKind, compilation_kind: Optional[CompilationKind] = None
     ) -> ProblemKind:
         new_kind = ProblemKind(problem_kind.features)
-        if new_kind.has_trajectory_constraints():
-            new_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
+        if new_kind.has_trajectory_constraints() or new_kind.has_state_invariants():
+            new_kind.unset_constraints_kind("TRAJECTORY_CONSTRAINTS")
+            new_kind.unset_constraints_kind("STATE_INVARIANTS")
+            new_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
+            new_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
         return new_kind
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
@@ -105,14 +112,15 @@
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         return supported_kind
 
     def _compile(
         self,
         problem: "up.model.AbstractProblem",
         compilation_kind: "up.engines.CompilationKind",
@@ -144,59 +152,69 @@
             if new_c.is_and():
                 C.extend(new_c.args)
             else:
                 C.append(new_c)
         # create a list that contains trajectory_constraints
         # trajectory_constraints can contain quantifiers and need to be remove
         relevancy_dict = self._build_relevancy_dict(env, C)
-        A_prime: List["up.model.effect.Effect"] = list()
+        A_prime: List["up.model.InstantaneousAction"] = list()
         I_prime, F_prime = self._get_monitoring_atoms(env, C, I)
         G_prime = env.expression_manager.And(
             [self._monitoring_atom_dict[c] for c in self._get_landmark_constraints(C)]
         )
         trace_back_map: Dict[Action, Tuple[Action, List[FNode]]] = {}
         assert isinstance(grounding_result.map_back_action_instance, partial)
         map_grounded_action = grounding_result.map_back_action_instance.keywords["map"]
         for a in new_problem.actions:
             map_value = map_grounded_action[a]
             assert isinstance(a, InstantaneousAction)
-            E: List["up.model.effect.Effect"] = list()
+            effects_to_add: List["up.model.effect.Effect"] = []
             # create an empty list to store the new effects for each trajectory constraints
             relevant_constraints = self._get_relevant_constraints(a, relevancy_dict)
             for c in relevant_constraints:
                 # manage the action for each trajectory_constraints that is relevant
                 if c.is_always():
                     precondition, to_add = self._manage_always_compilation(
                         env, c.args[0], a
                     )
                 elif c.is_at_most_once():
                     precondition, to_add = self._manage_amo_compilation(
-                        env, c.args[0], self._monitoring_atom_dict[c], a, E
+                        env, c.args[0], self._monitoring_atom_dict[c], a, effects_to_add
                     )
                 elif c.is_sometime_before():
                     precondition, to_add = self._manage_sb_compilation(
-                        env, c.args[0], c.args[1], self._monitoring_atom_dict[c], a, E
+                        env,
+                        c.args[0],
+                        c.args[1],
+                        self._monitoring_atom_dict[c],
+                        a,
+                        effects_to_add,
                     )
                 elif c.is_sometime():
                     self._manage_sometime_compilation(
-                        env, c.args[0], self._monitoring_atom_dict[c], a, E
+                        env, c.args[0], self._monitoring_atom_dict[c], a, effects_to_add
                     )
                 elif c.is_sometime_after():
                     self._manage_sa_compilation(
-                        env, c.args[0], c.args[1], self._monitoring_atom_dict[c], a, E
+                        env,
+                        c.args[0],
+                        c.args[1],
+                        self._monitoring_atom_dict[c],
+                        a,
+                        effects_to_add,
                     )
                 else:
                     raise Exception(
                         f"ERROR This compiler cannot handle this constraint = {c}"
                     )
                 if c.is_always() or c.is_at_most_once() or c.is_sometime_before():
                     if to_add and not precondition.is_true():
-                        a.preconditions.append(precondition)
-            for eff in E:
-                a.effects.append(eff)
+                        a.add_precondition(precondition)
+            for eff in effects_to_add:
+                a._add_effect_instance(eff)
             if env.expression_manager.FALSE() not in a.preconditions:
                 A_prime.append(a)
             trace_back_map[a] = map_value
         # create new problem to return
         # adding new fluents, goal, initial values and actions
         G_new = (env.expression_manager.And(new_problem.goals, G_prime)).simplify()
         new_problem.clear_goals()
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """This module defines the conditional effects remover class."""
 
 
-from fractions import Fraction
 from itertools import product
 import unified_planning as up
 import unified_planning.engines as engines
 from unified_planning.engines.mixins.compiler import CompilationKind, CompilerMixin
 from unified_planning.engines.results import CompilerResult
 from unified_planning.model import (
     Problem,
@@ -74,14 +73,20 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("REAL_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
@@ -100,25 +105,27 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
         supported_kind.set_expression_duration("FLUENTS_IN_DURATIONS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         return supported_kind
 
     @staticmethod
     def supports(problem_kind):
         return problem_kind <= UsertypeFluentsRemover.supported_kind()
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/utils.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/compilers/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,14 +401,16 @@
         if interval not in new_problem.timed_goals:
             new_problem.add_timed_goal(interval, condition)
 
     new_goal = em.And(*map(function, original_problem.goals), condition).simplify()
     if new_goal.is_and():
         for arg in new_goal.args:
             new_problem.add_goal(arg)
+    else:
+        new_problem.add_goal(new_goal)
 
     for qm in original_problem.quality_metrics:
         if qm.is_minimize_action_costs():
             assert isinstance(qm, MinimizeActionCosts)
             new_costs: Dict["up.model.Action", "up.model.Expression"] = {}
             for new_a, old_a in new_to_old.items():
                 cost = qm.get_action_cost(old_a)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/credits.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/engine.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/factory.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,21 +33,23 @@
 from unified_planning.engines.mixins.portfolio import PortfolioSelectorMixin
 from unified_planning.engines.mixins.replanner import ReplannerMixin
 from unified_planning.engines.mixins.plan_repairer import PlanRepairerMixin
 from unified_planning.engines.mixins.sequential_simulator import (
     SequentialSimulatorMixin,
 )
 from unified_planning.engines.engine import OperationMode
-from typing import IO, Any, Dict, Tuple, Optional, List, Union, Type, Sequence
+from typing import IO, Any, Dict, Tuple, Optional, List, Union, Type, Sequence, cast
 from pathlib import PurePath
 
 
 DEFAULT_ENGINES = {
     "fast-downward": ("up_fast_downward", "FastDownwardPDDLPlanner"),
     "fast-downward-opt": ("up_fast_downward", "FastDownwardOptimalPDDLPlanner"),
+    "symk": ("up_symk", "SymKPDDLPlanner"),
+    "symk-opt": ("up_symk", "SymKOptimalPDDLPlanner"),
     "pyperplan": ("up_pyperplan.engine", "EngineImpl"),
     "pyperplan-opt": ("up_pyperplan.engine", "OptEngineImpl"),
     "enhsp": ("up_enhsp.enhsp_planner", "ENHSPSatEngine"),
     "enhsp-opt": ("up_enhsp.enhsp_planner", "ENHSPOptEngine"),
     "enhsp-any": ("up_enhsp.enhsp_planner", "ENHSPAnytimeEngine"),
     "tamer": ("up_tamer.engine", "EngineImpl"),
     "lpg": ("up_lpg.lpg_planner", "LPGEngine"),
@@ -72,14 +74,18 @@
         "unified_planning.engines.compilers.conditional_effects_remover",
         "ConditionalEffectsRemover",
     ),
     "up_disjunctive_conditions_remover": (
         "unified_planning.engines.compilers.disjunctive_conditions_remover",
         "DisjunctiveConditionsRemover",
     ),
+    "up_state_invariants_remover": (
+        "unified_planning.engines.compilers.state_invariants_remover",
+        "StateInvariantsRemover",
+    ),
     "up_negative_conditions_remover": (
         "unified_planning.engines.compilers.negative_conditions_remover",
         "NegativeConditionsRemover",
     ),
     "up_quantifiers_remover": (
         "unified_planning.engines.compilers.quantifiers_remover",
         "QuantifiersRemover",
@@ -110,27 +116,30 @@
         "Replanner",
     ),
 }
 
 DEFAULT_ENGINES_PREFERENCE_LIST = [
     "fast-downward",
     "fast-downward-opt",
+    "symk",
+    "symk-opt",
     "pyperplan",
     "pyperplan-opt",
     "enhsp",
     "enhsp-opt",
     "enhsp-any",
     "tamer",
     "sequential_plan_validator",
     "sequential_simulator",
     "up_bounded_types_remover",
     "up_conditional_effects_remover",
     "up_disjunctive_conditions_remover",
     "up_negative_conditions_remover",
     "up_quantifiers_remover",
+    "up_state_invariants_remover",
     "up_usertype_fluents_remover",
     "tarski_grounder",
     "fast-downward-reachability-grounder",
     "fast-downward-grounder",
     "up_grounder",
     "lpg",
     "lpg-anytime",
@@ -393,14 +402,85 @@
             module = importlib.import_module(module_name)
             EngineImpl = getattr(module, class_name)
             self._meta_engines[name] = EngineImpl
             self._meta_engines_info.append((name, module_name, class_name))
         if EngineImpl.is_compatible_engine(engine):
             self._engines[f"{name}[{engine_name}]"] = EngineImpl[engine]
 
+    def _engine_satisfies_conditions(
+        self,
+        EngineClass: Type["up.engines.engine.Engine"],
+        operation_mode: "OperationMode",
+        problem_kind: ProblemKind,
+        optimality_guarantee: Optional["OptimalityGuarantee"],
+        compilation_kind: Optional["CompilationKind"],
+        plan_kind: Optional["PlanKind"],
+        anytime_guarantee: Optional["AnytimeGuarantee"],
+    ) -> bool:
+        if not getattr(EngineClass, "is_" + operation_mode.value)():
+            return False
+        if (
+            operation_mode == OperationMode.ONESHOT_PLANNER
+            or operation_mode == OperationMode.REPLANNER
+            or operation_mode == OperationMode.PORTFOLIO_SELECTOR
+        ):
+            assert (
+                issubclass(EngineClass, OneshotPlannerMixin)
+                or issubclass(EngineClass, ReplannerMixin)
+                or issubclass(EngineClass, PortfolioSelectorMixin)
+            )
+            assert anytime_guarantee is None
+            assert compilation_kind is None
+            assert plan_kind is None
+            if optimality_guarantee is not None and not EngineClass.satisfies(
+                optimality_guarantee
+            ):
+                return False
+        elif operation_mode == OperationMode.PLAN_VALIDATOR:
+            assert issubclass(EngineClass, PlanValidatorMixin)
+            assert optimality_guarantee is None
+            assert anytime_guarantee is None
+            assert compilation_kind is None
+            if plan_kind is not None and not EngineClass.supports_plan(plan_kind):
+                return False
+        elif operation_mode == OperationMode.COMPILER:
+            assert issubclass(EngineClass, CompilerMixin)
+            assert optimality_guarantee is None
+            assert anytime_guarantee is None
+            assert plan_kind is None
+            if compilation_kind is not None and not EngineClass.supports_compilation(
+                compilation_kind
+            ):
+                return False
+        elif operation_mode == OperationMode.ANYTIME_PLANNER:
+            assert issubclass(EngineClass, AnytimePlannerMixin)
+            assert optimality_guarantee is None
+            assert compilation_kind is None
+            assert plan_kind is None
+            if anytime_guarantee is not None and not EngineClass.ensures(
+                anytime_guarantee
+            ):
+                return False
+        elif operation_mode == OperationMode.PLAN_REPAIRER:
+            assert issubclass(EngineClass, PlanRepairerMixin)
+            assert anytime_guarantee is None
+            assert compilation_kind is None
+            if plan_kind is not None and not EngineClass.supports_plan(plan_kind):
+                return False
+            if optimality_guarantee is not None and not EngineClass.satisfies(
+                optimality_guarantee
+            ):
+                return False
+        else:
+            assert optimality_guarantee is None
+            assert anytime_guarantee is None
+            assert compilation_kind is None
+            assert plan_kind is None
+        return EngineClass.supports(problem_kind)
+
     def _get_engine_class(
         self,
         operation_mode: "OperationMode",
         name: Optional[str] = None,
         problem_kind: ProblemKind = ProblemKind(),
         optimality_guarantee: Optional["OptimalityGuarantee"] = None,
         compilation_kind: Optional["CompilationKind"] = None,
@@ -414,85 +494,33 @@
                 raise up.exceptions.UPNoRequestedEngineAvailableException
         problem_features = list(problem_kind.features)
         planners_features = []
         # Make sure that optimality guarantees and compilation kind are mutually exclusive
         assert optimality_guarantee is None or compilation_kind is None
         for name in self._preference_list:
             EngineClass = self._engines[name]
-            if getattr(EngineClass, "is_" + operation_mode.value)():
-                if (
-                    operation_mode == OperationMode.ONESHOT_PLANNER
-                    or operation_mode == OperationMode.REPLANNER
-                    or operation_mode == OperationMode.PORTFOLIO_SELECTOR
-                ):
-                    assert (
-                        issubclass(EngineClass, OneshotPlannerMixin)
-                        or issubclass(EngineClass, ReplannerMixin)
-                        or issubclass(EngineClass, PortfolioSelectorMixin)
-                    )
-                    assert anytime_guarantee is None
-                    assert compilation_kind is None
-                    assert plan_kind is None
-                    if optimality_guarantee is not None and not EngineClass.satisfies(
-                        optimality_guarantee
-                    ):
-                        continue
-                elif operation_mode == OperationMode.PLAN_VALIDATOR:
-                    assert issubclass(EngineClass, PlanValidatorMixin)
-                    assert optimality_guarantee is None
-                    assert anytime_guarantee is None
-                    assert compilation_kind is None
-                    if plan_kind is not None and not EngineClass.supports_plan(
-                        plan_kind
-                    ):
-                        continue
-                elif operation_mode == OperationMode.COMPILER:
-                    assert issubclass(EngineClass, CompilerMixin)
-                    assert optimality_guarantee is None
-                    assert anytime_guarantee is None
-                    assert plan_kind is None
-                    if (
-                        compilation_kind is not None
-                        and not EngineClass.supports_compilation(compilation_kind)
-                    ):
-                        continue
-                elif operation_mode == OperationMode.ANYTIME_PLANNER:
-                    assert issubclass(EngineClass, AnytimePlannerMixin)
-                    assert optimality_guarantee is None
-                    assert compilation_kind is None
-                    assert plan_kind is None
-                    if anytime_guarantee is not None and not EngineClass.ensures(
-                        anytime_guarantee
-                    ):
-                        continue
-                elif operation_mode == OperationMode.PLAN_REPAIRER:
-                    assert issubclass(EngineClass, PlanRepairerMixin)
-                    assert anytime_guarantee is None
-                    assert compilation_kind is None
-                    if plan_kind is not None and not EngineClass.supports_plan(
-                        plan_kind
-                    ):
-                        continue
-                    if optimality_guarantee is not None and not EngineClass.satisfies(
-                        optimality_guarantee
-                    ):
-                        continue
-                else:
-                    assert optimality_guarantee is None
-                    assert anytime_guarantee is None
-                    assert compilation_kind is None
-                    assert plan_kind is None
-                if EngineClass.supports(problem_kind):
-                    return EngineClass
-                else:
-                    x = [name] + [
-                        str(EngineClass.supports(ProblemKind({f})))
-                        for f in problem_features
-                    ]
-                    planners_features.append(x)
+            if self._engine_satisfies_conditions(
+                EngineClass,
+                operation_mode,
+                problem_kind,
+                optimality_guarantee,
+                compilation_kind,
+                plan_kind,
+                anytime_guarantee,
+            ):
+                return EngineClass
+            elif getattr(EngineClass, "is_" + operation_mode.value)():
+                # The EngineClass satisfies the given OperationMode but does not
+                # satisfy some other features; add it to the error report features if
+                # no NoSuitableEngineAvailable are found.
+                x = [name] + [
+                    str(EngineClass.supports(ProblemKind({f})))
+                    for f in problem_features
+                ]
+                planners_features.append(x)
         if len(planners_features) > 0:
             header = ["Engine"] + problem_features
             msg = f"No available engine supports all the problem features:\n{format_table(header, planners_features)}"
         elif compilation_kind is not None:
             msg = f"No available engine supports {compilation_kind}"
         elif plan_kind is not None:
             msg = f"No available engine supports {plan_kind}"
@@ -696,15 +724,15 @@
         *   | using ``names`` (list of specific planners name) and ``params`` (list of planner dependent options) to get a ``Parallel`` engine.
             | e.g. ``OneshotPlanner(names=['tamer', 'tamer'], params=[{'heuristic': 'hadd'}, {'heuristic': 'hmax'}])``
         *   | using ``problem_kind`` and ``optimality_guarantee``.
             | e.g. ``OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
         """
         if isinstance(optimality_guarantee, str):
             try:
-                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee.upper()]
             except KeyError:
                 raise UPUsageError(
                     f"{optimality_guarantee} is not a valid OptimalityGuarantee."
                 )
         return self._get_engine(
             OperationMode.ONESHOT_PLANNER,
             name,
@@ -737,15 +765,20 @@
         * optimal (``OPTIMAL_PLANS``);
         * just a different plan, with no specific guarantee (``None``).
 
         It raises an exception if the problem has no optimality metrics and anytime_guarantee
         is equal to ``INCREASING_QUALITY`` or ``OPTIMAL_PLAN``.
         """
         if isinstance(anytime_guarantee, str):
-            anytime_guarantee = AnytimeGuarantee[anytime_guarantee]
+            try:
+                anytime_guarantee = AnytimeGuarantee[anytime_guarantee.upper()]
+            except KeyError:
+                raise UPUsageError(
+                    f"{anytime_guarantee} is not a valid AnytimeGuarantee."
+                )
         return self._get_engine(
             OperationMode.ANYTIME_PLANNER,
             name,
             None,
             params,
             problem_kind,
             anytime_guarantee=anytime_guarantee,
@@ -805,26 +838,32 @@
 
         *   | using ``names`` (the names of the specific compilers), ``params`` (compilers dependent options) and ``compilation_kinds``.
             | e.g. ``Compiler(names=['up_quantifiers_remover', 'up_grounder'], params=[{'opt1': 'val1'}, {'opt2': 'val2'}], compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])``
         *   | using ``problem_kind`` and ``compilation_kinds`` parameters.
             | e.g. ``Compiler(problem_kind=problem.kind, compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])``
         """
         if isinstance(compilation_kind, str):
-            compilation_kind = CompilationKind[compilation_kind]
-
+            try:
+                compilation_kind = CompilationKind[compilation_kind.upper()]
+            except KeyError:
+                raise UPUsageError(
+                    f"{compilation_kind} is not a valid CompilationKind."
+                )
         kinds: Optional[List[CompilationKind]] = None
         if compilation_kinds is not None:
             kinds = []
             for kind in compilation_kinds:
                 if isinstance(kind, str):
-                    kinds.append(CompilationKind[kind])
+                    try:
+                        kinds.append(CompilationKind[kind.upper()])
+                    except KeyError:
+                        raise UPUsageError(f"{kind} is not a valid CompilationKind.")
                 else:
-                    assert isinstance(kind, CompilationKind)
+                    assert isinstance(kind, CompilationKind), "Typing not respected"
                     kinds.append(kind)
-
         return self._get_engine(
             OperationMode.COMPILER,
             name,
             names,
             params,
             problem_kind,
             compilation_kind=compilation_kind,
@@ -869,15 +908,15 @@
         *   | using ``problem`` (with its kind) and ``optimality_guarantee`` parameters.
             | e.g. ``Replanner(problem, optimality_guarantee=SOLVED_OPTIMALLY)``
         *   | using ``name`` (the name of a specific replanner) and ``params`` (replanner dependent options).
             | e.g. ``Replanner(problem, name='replanner[tamer]')``
         """
         if isinstance(optimality_guarantee, str):
             try:
-                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee.upper()]
             except KeyError:
                 raise UPUsageError(
                     f"{optimality_guarantee} is not a valid OptimalityGuarantee."
                 )
         return self._get_engine(
             OperationMode.REPLANNER,
             name,
@@ -902,18 +941,21 @@
 
         *   | using ``name`` (the name of a plan repairer) and eventually ``params``.
             | e.g. ``PlanRepairer(name='xxx')``
         *   | using ``problem_kind``, ``plan_kind`` and ``optimality_guarantee``.
             | e.g. ``PlanRepairer(problem_kind=problem.kind, plan_kind=plan.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
         """
         if isinstance(plan_kind, str):
-            plan_kind = PlanKind[plan_kind]
+            try:
+                plan_kind = PlanKind[plan_kind.upper()]
+            except KeyError:
+                raise UPUsageError(f"{plan_kind} is not a valid PlanKind.")
         if isinstance(optimality_guarantee, str):
             try:
-                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee.upper()]
             except KeyError:
                 raise UPUsageError(
                     f"{optimality_guarantee} is not a valid OptimalityGuarantee."
                 )
         return self._get_engine(
             OperationMode.PLAN_REPAIRER,
             name=name,
@@ -933,36 +975,147 @@
     ) -> "up.engines.engine.Engine":
         """
         Returns a portfolio selector. There are two ways to call this method:
 
         *   | using ``name`` (the name of a specific portfolio) and eventually ``params`` (portfolio dependent options).
             | e.g. ``PortfolioSelector(name='ibacop')``
         *   | using ``problem_kind`` and ``optimality_guarantee``.
-            | e.g. ``OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
+            | e.g. ``PortfolioSelector(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
         """
         if isinstance(optimality_guarantee, str):
             try:
-                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee.upper()]
             except KeyError:
                 raise UPUsageError(
                     f"{optimality_guarantee} is not a valid OptimalityGuarantee."
                 )
         return self._get_engine(
             OperationMode.PORTFOLIO_SELECTOR,
             name=name,
             params=params,
             problem_kind=problem_kind,
             optimality_guarantee=optimality_guarantee,
         )
 
     def print_engines_info(
-        self, stream: IO[str] = sys.stdout, full_credits: bool = True
+        self,
+        stream: IO[str] = sys.stdout,
+        *,
+        operation_mode: Optional[Union[OperationMode, str]] = None,
+        show_supported_kind: bool = True,
+        show_credits: bool = False,
+        full_credits: bool = True,
     ):
+        """
+        Writes the info of all the installed engines in the given stream; the
+        default stream is the stdout.
+
+        :param stream: The ``IO[str]`` where all the engine's info are written;
+            defaults to sys.stdout.
+        :param operation_mode: If specified, writes info about the engines that support
+            that OperationMode.
+        :param show_supported_kind: If ``True`` writes the supported_kind of the engines.
+            defaults to ``True``.
+        :param show_credits: If ``True`` writes the credits of the engines.
+            defaults to ``False``.
+        :param full_credits: If ``True`` writes a longer version of the credits; ignored
+            if ``show_credits`` is ``False``; defaults to ``True``.
+        """
         stream.write("These are the engines currently available:\n")
-        for Engine in self._engines.values():
-            credits = Engine.get_credits()
+        if isinstance(operation_mode, str):
+            try:
+                operation_mode = OperationMode[operation_mode.upper()]
+            except KeyError:
+                raise UPUsageError(f"{operation_mode} is not a valid OperationMode.")
+        for engine_name, Engine in self._engines.items():
+            if (
+                operation_mode is not None
+                and not getattr(Engine, "is_" + operation_mode.value)()
+            ):
+                continue
+            credits = Engine.get_credits() if show_credits else None
+            stream.write("---------------------------------------\n")
+            stream.write(f"Engine's factory name: {engine_name}\n")
             if credits is not None:
-                stream.write("---------------------------------------\n")
                 credits.write_credits(stream, full_credits)
+            supported_operation_modes = [
+                om.value for om in OperationMode if getattr(Engine, "is_" + om.value)()
+            ]
+            stream.write("Supported operation modes:\n    - ")
+            stream.write("\n    - ".join(supported_operation_modes))
+            stream.write("\n")
+            if show_supported_kind:
                 stream.write(
-                    f"This engine supports the following features:\n{str(Engine.supported_kind())}\n\n"
+                    f"This engine supports the following features:\n{str(Engine.supported_kind())}\n"
+                )
+            stream.write("\n")
+
+    def get_all_applicable_engines(
+        self,
+        problem_kind: ProblemKind,
+        operation_mode: OperationMode = OperationMode.ONESHOT_PLANNER,
+        *,
+        optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
+        anytime_guarantee: Optional[Union["AnytimeGuarantee", str]] = None,
+        plan_kind: Optional[Union["PlanKind", str]] = None,
+        compilation_kind: Optional[Union["CompilationKind", str]] = None,
+    ) -> List[str]:
+        """
+        | Returns all the engine names installed that are able to handle all the given
+          requirements.
+
+        | Since the semantic of the parameters given to this function depends on the chosen ``OperationMode``,
+          an user must have clear their meaning in the Operation Mode context.
+
+        :param problem_kind: An engine is returned only if it supports this ``problem_kind``.
+        :param operation_mode: An engine is returned only if it implements this ``operation_mode``; defaults to ``ONESHOT_PLANNER``.
+        :param optimality_guarantee: An engine is returned only if it satisfies this ``optimality_guarantee``. This parameter
+            can be specified only if the ``operation_mode`` is ``ONESHOT_PLANNER``, ``REPLANNER``, ``PLAN_REPAIRER``
+            or ``PORTFOLIO_SELECTOR``.
+        :param anytime_guarantee: An engine is returned only if it satisfies this ``anytime_guarantee``. This parameter
+            can be specified only if the ``operation_mode`` is ``ANYTIME_PLANNER``.
+        :param plan_kind: An engine is returned only if it is able to handle this ``plan_kind``. This parameter
+            can be specified only if the ``operation_mode`` is ``PLAN_VALIDATOR`` or ``PLAN_REPAIRER``.
+        :param compilation_kind: An engine is returned only if it is able to handle this ``compilation_kind``. This
+            parameter can be specified only if the ``operation_mode`` is ``COMPILER``.
+        :return: The list of engines names that satisfy all the given requirements.
+        """
+        if isinstance(optimality_guarantee, str):
+            try:
+                optimality_guarantee = OptimalityGuarantee[optimality_guarantee.upper()]
+            except KeyError:
+                raise UPUsageError(
+                    f"{optimality_guarantee} is not a valid OptimalityGuarantee."
+                )
+        if isinstance(anytime_guarantee, str):
+            try:
+                anytime_guarantee = AnytimeGuarantee[anytime_guarantee.upper()]
+            except KeyError:
+                raise UPUsageError(
+                    f"{anytime_guarantee} is not a valid AnytimeGuarantee."
+                )
+        if isinstance(compilation_kind, str):
+            try:
+                compilation_kind = CompilationKind[compilation_kind.upper()]
+            except KeyError:
+                raise UPUsageError(
+                    f"{compilation_kind} is not a valid CompilationKind."
                 )
+        if isinstance(plan_kind, str):
+            try:
+                plan_kind = PlanKind[plan_kind.upper()]
+            except KeyError:
+                raise UPUsageError(f"{plan_kind} is not a valid PlanKind.")
+        names: List[str] = []
+        for name in self._preference_list:
+            EngineClass = self._engines[name]
+            if self._engine_satisfies_conditions(
+                EngineClass,
+                operation_mode,
+                problem_kind,
+                cast(Optional[OptimalityGuarantee], optimality_guarantee),
+                cast(Optional[CompilationKind], compilation_kind),
+                plan_kind,
+                cast(Optional[AnytimeGuarantee], anytime_guarantee),
+            ):
+                names.append(name)
+        return names
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/meta_engine.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/meta_engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/anytime_planner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/anytime_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return True
 
     @staticmethod
     def ensures(anytime_guarantee: AnytimeGuarantee) -> bool:
         """
         :param anytime_guarantee: The `anytime_guarantee` that must be satisfied.
         :return: `True` if the `AnytimePlannerMixin` implementation ensures the given
-        `anytime_guarantee`, `False` otherwise.
+            `anytime_guarantee`, `False` otherwise.
         """
         return False
 
     def get_solutions(
         self,
         problem: "up.model.AbstractProblem",
         timeout: Optional[float] = None,
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/compiler.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     CONDITIONAL_EFFECTS_REMOVING = auto()
     DISJUNCTIVE_CONDITIONS_REMOVING = auto()
     NEGATIVE_CONDITIONS_REMOVING = auto()
     QUANTIFIERS_REMOVING = auto()
     TRAJECTORY_CONSTRAINTS_REMOVING = auto()
     USERTYPE_FLUENTS_REMOVING = auto()
     BOUNDED_TYPES_REMOVING = auto()
+    STATE_INVARIANTS_REMOVING = auto()
 
 
 class CompilerMixin(ABC):
     """Generic class for a compiler defining it's interface."""
 
     def __init__(self, default: Optional[CompilationKind] = None):
         self._default = default
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/oneshot_planner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/oneshot_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     @staticmethod
     def is_oneshot_planner() -> bool:
         return True
 
     @staticmethod
     def satisfies(optimality_guarantee: OptimalityGuarantee) -> bool:
         """
-        :param optimality_guarantee: The `optimality_guarantee` that must be satisfied.
-        :return: `True` if the `OneshotPlannerMixin` implementation satisfies the given
-        `optimality_guarantee`, `False` otherwise.
+        :param optimality_guarantee: The ``optimality_guarantee`` that must be satisfied.
+        :return: ``True`` if the ``OneshotPlannerMixin`` implementation satisfies the given
+            ``optimality_guarantee``, ``False`` otherwise.
         """
         return False
 
     def solve(
         self,
         problem: "up.model.AbstractProblem",
         heuristic: Optional[Callable[["up.model.state.State"], Optional[float]]] = None,
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/plan_repairer.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/plan_repairer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/plan_validator.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/portfolio.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     @staticmethod
     def satisfies(
         optimality_guarantee: "up.engines.mixins.oneshot_planner.OptimalityGuarantee",
     ) -> bool:
         """
         :param optimality_guarantee: The `optimality_guarantee` that must be satisfied.
         :return: `True` if the `PortfolioSelectorMixin` implementation satisfies the given
-        `optimality_guarantee`, `False` otherwise.
+            `optimality_guarantee`, `False` otherwise.
         """
         return False
 
     def get_best_oneshot_planners(
         self,
         problem: "up.model.AbstractProblem",
         max_planners: Optional[int] = None,
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/replanner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/sequential_simulator.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/mixins/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/oversubscription_planner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/oversubscription_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
+        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
         supported_kind.set_expression_duration("FLUENTS_IN_DURATIONS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         final_supported_kind = supported_kind.intersection(engine.supported_kind())
         final_supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         final_supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         return final_supported_kind
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/parallel.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/parallel.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/pddl_planner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/pddl_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import sys
 import tempfile
 import os
 import re
 import time
 import unified_planning as up
 import unified_planning.engines as engines
+from unified_planning.engines.engine import OperationMode
 import unified_planning.engines.mixins as mixins
 from unified_planning.engines.results import (
     LogLevel,
     LogMessage,
     PlanGenerationResult,
     PlanGenerationResultStatus,
 )
@@ -70,14 +71,15 @@
         :param self: The PDDLEngine instance.
         :param needs_requirements: Flag defining if the Engine needs the PDDL requirements.
         :param rewrite_bool_assignments: Flag defining if the non-constant boolean assignments
             will be rewritten as conditional effects in the PDDL file submitted to the Engine.
         """
         engines.engine.Engine.__init__(self)
         mixins.OneshotPlannerMixin.__init__(self)
+        self._mode_running = OperationMode.ONESHOT_PLANNER
         self._needs_requirements = needs_requirements
         self._rewrite_bool_assignments = rewrite_bool_assignments
         self._process = None
         self._writer = None
 
     @abstractmethod
     def _get_cmd(
@@ -215,15 +217,23 @@
         logs: List["up.engines.results.LogMessage"] = []
         with tempfile.TemporaryDirectory() as tempdir:
             domain_filename = os.path.join(tempdir, "domain.pddl")
             problem_filename = os.path.join(tempdir, "problem.pddl")
             plan_filename = os.path.join(tempdir, "plan.txt")
             self._writer.write_domain(domain_filename)
             self._writer.write_problem(problem_filename)
-            cmd = self._get_cmd(domain_filename, problem_filename, plan_filename)
+            if self._mode_running == OperationMode.ONESHOT_PLANNER:
+                cmd = self._get_cmd(domain_filename, problem_filename, plan_filename)
+            elif self._mode_running == OperationMode.ANYTIME_PLANNER:
+                assert isinstance(
+                    self, up.engines.pddl_anytime_planner.PDDLAnytimePlanner
+                )
+                cmd = self._get_anytime_cmd(
+                    domain_filename, problem_filename, plan_filename
+                )
             if output_stream is None:
                 # If we do not have an output stream to write to, we simply call
                 # a subprocess and retrieve the final output and error with communicate
                 process = subprocess.Popen(
                     cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE
                 )
                 timeout_occurred: bool = False
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/plan_validator.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/plan_validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
-from typing import Optional
+from typing import Optional, cast
+import warnings
 import unified_planning as up
 import unified_planning.environment
 import unified_planning.engines as engines
 import unified_planning.engines.mixins as mixins
 import unified_planning.model.walkers as walkers
 from unified_planning.model import (
     AbstractProblem,
@@ -30,14 +31,15 @@
     ValidationResult,
     ValidationResultStatus,
     LogMessage,
     LogLevel,
     FailedValidationReason,
 )
 from unified_planning.engines.sequential_simulator import (
+    InapplicabilityReasons,
     UPSequentialSimulator,
     evaluate_quality_metric,
     evaluate_quality_metric_in_initial_state,
 )
 from unified_planning.plans import SequentialPlan, PlanKind
 from unified_planning.exceptions import (
     UPConflictingEffectsException,
@@ -76,14 +78,20 @@
 
     @staticmethod
     def supported_kind() -> ProblemKind:
         supported_kind = ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+        supported_kind.set_parameters("REAL_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_conditions_kind("NEGATIVE_CONDITIONS")
         supported_kind.set_conditions_kind("DISJUNCTIVE_CONDITIONS")
@@ -95,15 +103,17 @@
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
+        supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("FINAL_VALUE")
@@ -132,34 +142,52 @@
         if len(problem.quality_metrics) > 0:
             if len(problem.quality_metrics) == 1:
                 metric = problem.quality_metrics[0]
             else:
                 raise UPProblemDefinitionError(
                     "The UP does not support more than one quality metric in the problem."
                 )
-        simulator = UPSequentialSimulator(problem)
+        # To support infinite domain action's parameters the checks on the simulator must be disabled
+        # and, if the problem is not supported for different reasons, re-raise the warning/exception
+        with warnings.catch_warnings(record=True) as _:
+            simulator = UPSequentialSimulator(problem, error_on_failed_checks=False)
+        kind = problem.kind
+        kind.unset_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+        kind.unset_parameters("REAL_ACTION_PARAMETERS")
+        if not self.skip_checks and not simulator.supports(kind):
+            msg: Optional[
+                str
+            ] = f"We cannot establish whether {self.name} can validate this problem!"
+            if self.error_on_failed_checks:
+                raise up.exceptions.UPUsageError(msg)
+            else:
+                warnings.warn(cast(str, msg))
         prev_state: Optional[State] = simulator.get_initial_state()
         if metric is not None:
             metric_value = evaluate_quality_metric_in_initial_state(simulator, metric)
         msg = None
-        for i, ai in enumerate(plan.actions):
+        for i, ai in zip(range(1, len(plan.actions) + 1), plan.actions):
             assert prev_state is not None
             try:
-                unsat_conds = simulator.get_unsatisfied_conditions(prev_state, ai)
+                unsat_conds, reason = simulator.get_unsatisfied_conditions(
+                    prev_state, ai
+                )
                 if unsat_conds:
+                    assert reason == InapplicabilityReasons.VIOLATES_CONDITIONS
                     msg = f"Preconditions {unsat_conds} of {str(i)}-th action instance {str(ai)} are not satisfied."
-            except UPConflictingEffectsException as e:
-                msg = f"{str(i)}-th action instance {str(ai)} creates conflicting effects: {str(e)}"
             except UPUsageError as e:
                 msg = f"{str(i)}-th action instance {str(ai)} creates a UsageError: {str(e)}"
             except UPInvalidActionError as e:
                 msg = f"{str(i)}-th action instance {str(ai)} creates an Invalid Action: {str(e)}"
-            next_state = simulator.apply_unsafe(prev_state, ai)
-            if next_state is None:
-                msg = f"{str(i)}-th action instance {str(ai)} creates conflicting effects."
+            try:
+                next_state = simulator.apply_unsafe(prev_state, ai)
+            except UPInvalidActionError as e:
+                msg = f"{str(i)}-th action instance {str(ai)} creates an Invalid Action: {str(e)}"
+            except UPConflictingEffectsException as e:
+                msg = f"{str(i)}-th action instance {str(ai)} creates Conflicting Effects: {str(e)}"
             if msg is not None:
                 logs = [LogMessage(LogLevel.INFO, msg)]
                 return ValidationResult(
                     ValidationResultStatus.INVALID,
                     self.name,
                     logs,
                     None,
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/replanner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/results.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/results.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from typing import Callable, Dict, Optional, List, Union
 
 
 class ValidationResultStatus(Enum):
     """
-    Enum representing the 2 possible values in the `status` field of a :class:`~unified_planning.engines.ValidationResult`:
-    VALID or INVALID.
+    Enum representing the 3 possible values in the `status` field of a :class:`~unified_planning.engines.ValidationResult`:
+    VALID, INVALID or UNKNOWN.
     """
 
     VALID = (
         auto()
     )  # The plan is valid for the problem, it satisfies all the hard constraints
     INVALID = (
         auto()
     )  # The plan is invalid for the problem, it does not satisfy all the hard constraints
+    UNKNOWN = (
+        auto()
+    )  # The planner can't tell if the plan is valid or invalid for the given problem
 
     def __bool__(self):
         if self == ValidationResultStatus.VALID:
             return True
         else:
             return False
 
@@ -151,14 +154,25 @@
             )
         elif self.status in NEGATIVE_OUTCOMES and self.plan is not None:
             raise UPUsageError(
                 f"The Result status is {str(self.status)} but the plan is {str(self.plan)}.\nWith this status the plan must be None."
             )
         return self
 
+    def __str__(self) -> str:
+        ret = [
+            f"status: {self.status.name}",
+            f"engine: {self.engine_name}",
+        ]
+        if self.plan is not None:
+            ret.append(f"plan: {self.plan}")
+        else:
+            ret.append("plan: None")
+        return "\n".join(ret)
+
     def is_definitive_result(self, *args) -> bool:
         optimality_required = False
         if len(args) > 0:
             optimality_required = (
                 len(args[0].quality_metrics) > 0
             )  # Require optimality if the problem has at least one quality metric.
         return (
@@ -263,22 +277,34 @@
 
     def __post_init__(self):
         assert (
             self.inapplicable_action is None
             or self.reason == FailedValidationReason.INAPPLICABLE_ACTION
         ), "The inapplicable_action can be set only if the reason of the failed plan is an inapplicable action."
 
+    def __str__(self) -> str:
+        ret = [
+            f"status: {self.status.name}",
+            f"engine: {self.engine_name}",
+        ]
+        if self.metric_evaluations is not None:
+            ret.append(f"metrics: ")
+            for metric, value in self.metric_evaluations.items():
+                ret.append(f"    {metric}: {value}")
+        if self.reason is not None:
+            ret.append(f"reason: {self.reason.name}")
+        if self.inapplicable_action is not None:
+            ret.append(f"inapplicable action: {self.inapplicable_action}")
+        return "\n".join(ret)
+
     def is_definitive_result(self, *args) -> bool:
         return True
 
     def __bool__(self):
-        if self.status == ValidationResultStatus.VALID:
-            return True
-        else:
-            return False
+        return bool(self.status)
 
 
 @dataclass
 class CompilerResult(Result):
     """Class that represents the result of a compile call."""
 
     problem: Optional[AbstractProblem]
@@ -295,9 +321,16 @@
                 f"The compiled Problem is None but the map_back_action_instance Callable is not None."
             )
         if self.problem is not None and self.map_back_action_instance is None:
             raise UPUsageError(
                 f"The compiled Problem is {str(self.problem)} but the map_back_action_instance Callable is None."
             )
 
+    def __str__(self) -> str:
+        ret = [
+            f"problem: {self.problem}",
+            f"engine: {self.engine_name}",
+        ]
+        return "\n".join(ret)
+
     def is_definitive_result(self, *args) -> bool:
         return self.problem is not None
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/engines/sequential_simulator.py` & `unified_planning-0.6.0.94.dev1/unified_planning/engines/sequential_simulator.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,41 +10,77 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
+from enum import Enum, auto
 from fractions import Fraction
 from warnings import warn
 import unified_planning as up
 from unified_planning.engines.compilers import Grounder, GrounderHelper
 from unified_planning.engines.engine import Engine
 from unified_planning.engines.mixins.sequential_simulator import (
     SequentialSimulatorMixin,
 )
+from unified_planning.model.fluent import get_all_fluent_exp
 from unified_planning.exceptions import (
     UPUsageError,
     UPConflictingEffectsException,
     UPInvalidActionError,
+    UPUnreachableCodeError,
+    UPProblemDefinitionError,
 )
 from unified_planning.model import (
+    Fluent,
     FNode,
-    Type,
     ExpressionManager,
     UPState,
     Problem,
     MinimizeActionCosts,
     MinimizeExpressionOnFinalState,
     MaximizeExpressionOnFinalState,
     Oversubscription,
 )
 from unified_planning.model.types import _RealType
-from unified_planning.model.walkers import StateEvaluator
-from typing import Dict, Iterator, List, Optional, Sequence, Set, Tuple, Union, cast
+from unified_planning.model.walkers import StateEvaluator, ExpressionQuantifiersRemover
+from typing import (
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Union,
+    cast,
+)
+
+
+class InapplicabilityReasons(Enum):
+    """
+    Represents the possible reasons for an action being inapplicable after the
+    ``SequentialSimulator.is_applicable`` method returns ``True`` but then the
+    ``SequentialSimulator.apply_unsafe`` returns ``None``.
+
+    Possible values:
+
+    *   | ``VIOLATES_CONDITIONS``: The action's conditions don't evaluate to True in the given state;
+        | Generally the most frequent and common cause of action's inapplicability.
+    *   | ``CONFLICTING_EFFECTS``: The action applied in the given state creates conflicting effects;
+        | This generally means that the action gives 2 different values to the same fluent instance.
+    *   | ``VIOLATES_STATE_INVARIANTS``: The new state does not satisfy the state invariants of the problem.
+        | State invariants are the ``Always`` expressions of the trajectory constraints or the bounded types.
+    """
+
+    VIOLATES_CONDITIONS = auto()
+    CONFLICTING_EFFECTS = auto()
+    VIOLATES_STATE_INVARIANTS = auto()
 
 
 class UPSequentialSimulator(Engine, SequentialSimulatorMixin):
     """
     Sequential SequentialSimulatorMixin implementation.
 
     This SequentialSimulator, when considering if a state is goal or not, ignores the
@@ -64,14 +100,51 @@
                 raise UPUsageError(msg)
             else:
                 warn(msg)
         assert isinstance(self._problem, up.model.Problem)
         self._grounder = GrounderHelper(problem)
         self._actions = set(self._problem.actions)
         self._se = StateEvaluator(self._problem)
+        self._initial_state: Optional[UPState] = None
+
+        # Add state invariants without quantifiers to get all the grounded
+        # fluent instances that might modify the state invariants
+        qrm = ExpressionQuantifiersRemover(self._problem.environment)
+        self._state_invariants: List[FNode] = [
+            qrm.remove_quantifiers(si, self._problem).simplify()
+            for si in self._problem.state_invariants
+        ]
+        # Set of all the fluents appearing in the state_invariants. Used to skip checks
+        # if None of this fluent is modified
+        self._fluent_exps_in_state_invariants: Set[FNode] = set()
+        for si in self._state_invariants:
+            self._fluent_exps_in_state_invariants |= (
+                si.environment.free_vars_extractor.get(si)
+            )
+
+        # Add bounded types as state invariants
+        em = self._problem.environment.expression_manager
+        for f in self._problem.fluents:
+            lower_bound, upper_bound = None, None
+            f_type = f.type
+            if f_type.is_int_type() or f_type.is_real_type():
+                f_type = cast(_RealType, f_type)
+                lower_bound, upper_bound = f_type.lower_bound, f_type.upper_bound
+            if lower_bound is not None:
+                for f_e in get_all_fluent_exp(self._problem, f):
+                    self._fluent_exps_in_state_invariants.add(f_e)
+                    self._state_invariants.append(em.LE(lower_bound, f_e))
+            if upper_bound is not None:
+                for f_e in get_all_fluent_exp(self._problem, f):
+                    self._fluent_exps_in_state_invariants.add(f_e)
+                    self._state_invariants.append(em.LE(f_e, upper_bound))
+
+        self._fluents_in_state_invariants: Set[Fluent] = set(
+            (fe.fluent() for fe in self._fluent_exps_in_state_invariants)
+        )
 
     def _ground_action(
         self, action: "up.model.Action", params: Tuple["up.model.FNode", ...]
     ) -> Optional["up.model.InstantaneousAction"]:
         """
         Utility method to ground an action and do the basic checks.
 
@@ -95,15 +168,23 @@
         """
         Returns the problem's initial state.
 
         NOTE: Every method that requires a state assumes that it's the same class
         of the state given here, therefore an up.model.UPState.
         """
         assert isinstance(self._problem, Problem), "supported_kind not respected"
-        return UPState(self._problem.initial_values)
+        if self._initial_state is None:
+            self._initial_state = UPState(self._problem.initial_values)
+            for si in self._state_invariants:
+                if not self._se.evaluate(si, self._initial_state).bool_constant_value():
+                    raise UPProblemDefinitionError(
+                        "The initial state of the problem already violates the state invariants"
+                    )
+        assert self._initial_state is not None
+        return self._initial_state
 
     def _is_applicable(
         self,
         state: "up.model.State",
         action: "up.model.Action",
         parameters: Tuple["up.model.FNode", ...],
     ) -> bool:
@@ -115,22 +196,18 @@
         :param action_or_action_instance: The `ActionInstance` or the `Action` that must be checked
             for applicability.
         :param parameters: The parameters to ground the given `Action`. This param must be `None` if
             an `ActionInstance` is given instead.
         :return: Whether or not the action is applicable in the given `state`.
         """
         try:
-            is_applicable = (
-                len(
-                    self.get_unsatisfied_conditions(
-                        state, action, parameters, early_termination=True
-                    )
-                )
-                == 0
+            _, reason = self.get_unsatisfied_conditions(
+                state, action, parameters, early_termination=True, full_check=True
             )
+            is_applicable = reason is None
         except UPInvalidActionError:
             is_applicable = False
         return is_applicable
 
     def _apply(
         self,
         state: "up.model.State",
@@ -146,90 +223,94 @@
         :param action_or_action_instance: The `ActionInstance` or the `Action` of which conditions are checked
             and effects evaluated.
         :param parameters: The parameters to ground the given `Action`. This param must be `None` if
             an `ActionInstance` is given instead.
         :return: `None` if the `action` is not applicable in the given `state`, the new State generated
             if the action is applicable.
         """
-        if not self.is_applicable(state, action, parameters):
+        _, reason = self.get_unsatisfied_conditions(
+            state, action, parameters, early_termination=True, full_check=False
+        )
+        if reason is not None:
             return None
-        else:
+        try:
             return self.apply_unsafe(state, action, parameters)
+        except (UPInvalidActionError, UPConflictingEffectsException):
+            return None
 
     def apply_unsafe(
         self,
         state: "up.model.State",
         action_or_action_instance: Union["up.model.Action", "up.plans.ActionInstance"],
         parameters: Optional[Sequence["up.model.Expression"]] = None,
-    ) -> Optional["up.model.State"]:
+    ) -> "up.model.State":
         """
         Returns a new `State`, which is a copy of the given `state` but the applicable `effects` of the
         `action` are applied; therefore some `fluent` values are updated.
         IMPORTANT NOTE: Assumes that `self.is_applicable(state, event)` returns `True`.
 
         :param state: The state in which the given action's conditions are checked and the effects evaluated.
         :param action_or_action_instance: The `ActionInstance` or the `Action` of which conditions are checked
             and effects evaluated.
         :param parameters: The parameters to ground the given `Action`. This param must be `None` if
             an `ActionInstance` is given instead.
-        :return: The new `State` created by the given action; `None` if the evaluation of the effects
-            creates conflicting effects.
+        :return: The new `State` created by the given action.
+        :raises UPConflictingEffectsException: If to the same fluent are assigned 2 different
+            values.
+        :raises UPInvalidActionError: If the action is invalid or if it violates some state invariants.
         """
         action, params = self._get_action_and_parameters(
             action_or_action_instance, parameters
         )
         if not isinstance(state, up.model.UPState):
             raise UPUsageError(
                 f"The UPSequentialSimulator uses the UPState but {type(state).__name__} is given."
             )
         grounded_action = self._ground_action(action, params)
         if grounded_action is None:
-            return None
+            raise UPInvalidActionError("Apply_unsafe got an inapplicable action.")
         assert isinstance(action, up.model.InstantaneousAction)
         updated_values: Dict["up.model.FNode", "up.model.FNode"] = {}
         assigned_fluent: Set["up.model.FNode"] = set()
         em = self._problem.environment.expression_manager
-        for effect in grounded_action.effects:
-            try:
-                fluent, value = self._evaluate_effect(
-                    effect, state, updated_values, assigned_fluent, em
-                )
-            except UPConflictingEffectsException:
-                return None
-            if fluent is not None:
-                assert value is not None
-                updated_values[fluent] = value
+
         if grounded_action.simulated_effect is not None:
             for f, v in zip(
                 grounded_action.simulated_effect.fluents,
                 grounded_action.simulated_effect.function(self._problem, state, {}),
             ):
-                old_value = updated_values.get(f, None)
-                # If f was already modified and it was modified by an increase/decrease or with an assign
-                # with a different value
-                if old_value is not None and (
-                    f not in assigned_fluent
-                    or old_value.constant_value() != v.constant_value()
-                ):
-                    if not f.type.is_bool_type():
-                        return None
-                    # solve with add-after-delete logic
-                    elif not old_value.bool_constant_value():
-                        updated_values[f] = v
-                else:
-                    updated_values[f] = v
-        return state.make_child(updated_values)
+                updated_values[f] = v
+                assigned_fluent.add(f)
+
+        for effect in grounded_action.effects:
+            fluent, value = self._evaluate_effect(
+                effect, state, updated_values, assigned_fluent, em
+            )
+            if fluent is not None:
+                assert value is not None
+                updated_values[fluent] = value
+
+        new_state = state.make_child(updated_values)
+        for si in self._state_invariants:
+            if not self._se.evaluate(si, new_state).bool_constant_value():
+                raise UPInvalidActionError(
+                    "The given action is not applicable because it violates state invariants.",
+                    "Bounded numeric types are checked as state invariants.",
+                )
+        return new_state
 
     def _evaluate_effect(
         self,
         effect: "up.model.Effect",
         state: "up.model.State",
         updated_values: Dict["up.model.FNode", "up.model.FNode"],
         assigned_fluent: Set["up.model.FNode"],
         em: ExpressionManager,
+        evaluated_fluent: Optional[FNode] = None,
+        evaluated_condition: Optional[bool] = None,
     ) -> Tuple[Optional[FNode], Optional[FNode]]:
         """
         Evaluates the given effect in the state, and returns the fluent affected
         by this effect and the new value that is assigned to the fluent.
 
         If the effect is conditional and the condition evaluates to False in the state,
         (None, None) is returned.
@@ -237,57 +318,64 @@
         :param effect: The effect to evaluate.
         :param state: The state in which the effect is evaluated.
         :param updated_values: Map from fluents to their value, used to correctly evaluate
             more than one increase/decrease effect on the same fluent.
         :param assigned_fluent: The set containing all the fluents already assigned in the
             event containing this effect.
         :param em: The current environment expression manager.
+        :param evaluated_fluent: In case the fluent is already evaluated outside, pass it to
+            avoid doing the same thing again.
+        :param evaluated_condition: In case the condition is already evaluated outside, pass it to
+            avoid doing the same thing again.
         :return: The Tuple[Fluent, Value], where the fluent is the one affected by the given
             effect and value is the new value assigned to the fluent.
         :raises UPConflictingEffectsException: If to the same fluent are assigned 2 different
             values.
         """
-        evaluated_args = tuple(self._se.evaluate(a, state) for a in effect.fluent.args)
-        fluent = self._problem.environment.expression_manager.FluentExp(
-            effect.fluent.fluent(), evaluated_args
-        )
-        if (not effect.is_conditional()) or self._se.evaluate(
-            effect.condition, state
-        ).is_true():
-            new_value = self._se.evaluate(effect.value, state)
+        evaluate: Callable[[FNode], FNode] = lambda exp: self._se.evaluate(exp, state)
+        if evaluated_fluent is not None:
+            fluent = evaluated_fluent
+        else:
+            fluent = effect.fluent.fluent()(*tuple(map(evaluate, effect.fluent.args)))
+        if evaluated_condition is None:
+            evaluated_condition = (
+                not effect.is_conditional() or evaluate(effect.condition).is_true()
+            )
+        if evaluated_condition:
+            new_value = evaluate(effect.value)
             if effect.is_assignment():
                 old_value = updated_values.get(fluent, None)
                 if (
                     old_value is not None
                     and new_value.constant_value() != old_value.constant_value()
                 ):
                     if not fluent.type.is_bool_type():
                         raise UPConflictingEffectsException(
-                            f"The fluent {fluent} is modified by 2 different assignments in the same event."
+                            f"The fluent {fluent} is modified by 2 different assignments in the same action."
                         )
                     # solve with add-after-delete logic
                     elif not old_value.bool_constant_value():
                         return fluent, new_value
                     else:
                         return None, None
                 elif old_value is not None and fluent not in assigned_fluent:
                     raise UPConflictingEffectsException(
-                        f"The fluent {fluent} is modified by 1 assignments and an increase/decrease in the same event."
+                        f"The fluent {fluent} is modified by 1 assignments and an increase/decrease in the same action."
                     )
                 else:
                     assigned_fluent.add(fluent)
                     return fluent, new_value
             else:
                 if fluent in assigned_fluent:
                     raise UPConflictingEffectsException(
-                        f"The fluent {fluent} is modified by an assignment and an increase/decrease in the same event."
+                        f"The fluent {fluent} is modified by an assignment and an increase/decrease in the same action."
                     )
                 # If the fluent is in updated_values, we take his modified value, (which was modified by another increase or decrease)
                 # otherwise we take it's evaluation in the state as it's value.
-                f_eval = updated_values.get(fluent, self._se.evaluate(fluent, state))
+                f_eval = updated_values.get(fluent, evaluate(fluent))
                 if effect.is_increase():
                     return (
                         fluent,
                         em.auto_promote(
                             f_eval.constant_value() + new_value.constant_value()
                         )[0],
                     )
@@ -318,114 +406,149 @@
 
     def get_unsatisfied_conditions(
         self,
         state: "up.model.State",
         action_or_action_instance: Union["up.model.Action", "up.plans.ActionInstance"],
         parameters: Optional[Sequence["up.model.Expression"]] = None,
         early_termination: bool = False,
-    ) -> List["up.model.FNode"]:
+        full_check: bool = False,
+    ) -> Tuple[List["up.model.FNode"], Optional[InapplicabilityReasons]]:
         """
-        Returns the list of `unsatisfied action's conditions` evaluated in the given `state`.
-        If the flag `early_termination` is set, the method ends and returns at the first `unsatisfied condition`.
+        Returns the list of ``unsatisfied action's conditions`` evaluated in the given ``state``, together with
+        an Optional reason of why the action can't be applied to the given state. If the ``full_check``
+        flag is set, the returned list can be empty but the action can't be applied in the given state,.
+        To be sure that the action is applicable, the ``InapplicabilityReason`` returned must be ``None``.
+        If the flag ``early_termination`` is set, the method ends and returns at the first ``unsatisfied condition``.
         Note that the returned list might also contain conditions that were not originally in the action, if this
-        action violates some other semantic bound (for example bounded types).
+        action violates some other semantic constraints (for example bounded types or state invariants).
 
         :param state: The state in which the given action's conditions are checked.
         :param action_or_action_instance: The `ActionInstance` or the `Action` of which conditions are checked.
         :param parameters: The parameters to ground the given `Action`. This param must be `None` if
             an `ActionInstance` is given instead.
+        :param early_termination: When ``True``, the first error found is returned.
+        :param full_check: When ``True``, fails also if the action applied creates any semantic problems; such as
+            conflicting_effects or violates state_invariants.
         :return: The list of all the `action's conditions` that evaluated to `False` or the list containing the first
             `condition` evaluated to `False` if the flag `early_termination` is set.
         """
         action, params = self._get_action_and_parameters(
             action_or_action_instance,
             parameters,
         )
         g_action = self._ground_action(action, params)
         if g_action is None:
             raise UPInvalidActionError(
                 "The given action grounded with the given parameters does not create a valid action."
             )
+        evaluate: Callable[[FNode], FNode] = lambda exp: self._se.evaluate(exp, state)
+        reason: Optional[InapplicabilityReasons] = None
         unsatisfied_conditions = []
         for c in g_action.preconditions:
-            evaluated_cond = self._se.evaluate(c, state)
+            evaluated_cond = evaluate(c)
             if (
                 not evaluated_cond.is_bool_constant()
                 or not evaluated_cond.bool_constant_value()
             ):
                 unsatisfied_conditions.append(c)
+                reason = InapplicabilityReasons.VIOLATES_CONDITIONS
                 if early_termination:
-                    return unsatisfied_conditions
+                    return unsatisfied_conditions, reason
 
-        # check that the assignments will respect the bound typing
-        new_bounded_types_values: Dict["up.model.FNode", "up.model.FNode"] = {}
+        updated_values: Dict["up.model.FNode", "up.model.FNode"] = {}
         assigned_fluent: Set["up.model.FNode"] = set()
         em = self._problem.environment.expression_manager
-        for effect in g_action.effects:
-            lower_bound, upper_bound = None, None
-            f_type = effect.fluent.type
-            if f_type.is_int_type() or f_type.is_real_type():
-                f_type = cast(_RealType, effect.fluent.type)
-                lower_bound, upper_bound = f_type.lower_bound, f_type.upper_bound
-            if lower_bound is not None or upper_bound is not None:
-                fluent, value = self._evaluate_effect(
-                    effect, state, new_bounded_types_values, assigned_fluent, em
-                )
-                if fluent is not None:
-                    assert value is not None
-                    new_bounded_types_values[fluent] = value
-                    if lower_bound is not None and lower_bound > cast(
-                        Fraction, value.constant_value()
-                    ):
-                        unsatisfied_conditions.append(em.LE(lower_bound, fluent))
-                        if early_termination:
-                            return unsatisfied_conditions
-                    if upper_bound is not None and upper_bound < cast(
-                        Fraction, value.constant_value()
-                    ):
-                        unsatisfied_conditions.append(em.LE(fluent, upper_bound))
-                        if early_termination:
-                            return unsatisfied_conditions
-        if g_action.simulated_effect is not None:
-            to_check = False
-            for f in g_action.simulated_effect.fluents:
-                f_type = cast(_RealType, f.type)
-                if (f_type.is_int_type() or f_type.is_real_type()) and (
-                    f_type.lower_bound is not None or f_type.upper_bound is not None
-                ):
-                    to_check = True
-                    break
-            if to_check:
+
+        if full_check:
+            # Add simulated effects to updated_values and assigned_fluent before other effects
+            sim_eff = g_action.simulated_effect
+            if sim_eff is not None:
                 for f, v in zip(
-                    g_action.simulated_effect.fluents,
-                    g_action.simulated_effect.function(self._problem, state, {}),
+                    sim_eff.fluents,
+                    sim_eff.function(self._problem, state, {}),
                 ):
-                    lower_bound, upper_bound = None, None
-                    if f.type.is_int_type() or f.type.is_real_type():
-                        f_type = cast(_RealType, f.type)
-                        lower_bound, upper_bound = (
-                            f_type.lower_bound,
-                            f_type.upper_bound,
-                        )
-                    if lower_bound is not None or upper_bound is not None:
-                        if (
-                            lower_bound is not None
-                            and cast(Fraction, v.constant_value()) < lower_bound
-                        ):
-                            unsatisfied_conditions.append(em.LE(lower_bound, f))
+                    updated_values[f] = v
+                    assigned_fluent.add(f)
+
+            for e in g_action.conditional_effects:
+                if not e.fluent.type.is_bool_type():
+                    evaluated_condition = evaluate(e.condition).bool_constant_value()
+                    if evaluated_condition:
+                        try:
+                            fluent, value = self._evaluate_effect(
+                                e,
+                                state,
+                                updated_values,
+                                assigned_fluent,
+                                em,
+                                evaluated_condition=evaluated_condition,
+                            )
+                            assert fluent is not None and value is not None
+                            updated_values[fluent] = value
+                        except UPConflictingEffectsException:
+                            reason = InapplicabilityReasons.CONFLICTING_EFFECTS
                             if early_termination:
-                                break
-                        if (
-                            upper_bound is not None
-                            and cast(Fraction, v.constant_value()) > upper_bound
-                        ):
-                            unsatisfied_conditions.append(em.LE(f, upper_bound))
+                                return unsatisfied_conditions, reason
+
+            if updated_values:
+                for e in g_action.unconditional_effects:
+                    ev_fluent = e.fluent.fluent()(*tuple(map(evaluate, e.fluent.args)))
+                    values = updated_values.get(ev_fluent, None)
+                    if values is not None:
+                        try:
+                            fluent, value = self._evaluate_effect(
+                                e,
+                                state,
+                                updated_values,
+                                assigned_fluent,
+                                em,
+                                evaluated_fluent=ev_fluent,
+                                evaluated_condition=True,
+                            )
+                            assert fluent is not None and value is not None
+                            updated_values[fluent] = value
+                        except UPConflictingEffectsException:
+                            reason = InapplicabilityReasons.CONFLICTING_EFFECTS
                             if early_termination:
-                                break
-        return unsatisfied_conditions
+                                return unsatisfied_conditions, reason
+
+            for e in g_action.effects:
+                if e.fluent.fluent() in self._fluents_in_state_invariants:
+                    ev_fluent = e.fluent.fluent()(*tuple(map(evaluate, e.fluent.args)))
+                    if ev_fluent in self._fluent_exps_in_state_invariants:
+                        if ev_fluent not in updated_values:
+                            try:
+                                fluent, value = self._evaluate_effect(
+                                    e,
+                                    state,
+                                    updated_values,
+                                    assigned_fluent,
+                                    em,
+                                    evaluated_fluent=ev_fluent,
+                                )
+                                assert fluent is not None and value is not None
+                                updated_values[fluent] = value
+                            except UPConflictingEffectsException:
+                                raise UPUnreachableCodeError(
+                                    "Conflicting effects should be caught above"
+                                )
+
+            if not isinstance(state, up.model.UPState):
+                raise UPUsageError(
+                    f"The UPSequentialSimulator uses the UPState but {type(state).__name__} is given."
+                )
+            new_partial_state = state.make_child(updated_values)
+            for si in self._state_invariants:
+                if not self._se.evaluate(si, new_partial_state).bool_constant_value():
+                    unsatisfied_conditions.append(si)
+                    if reason is None:
+                        reason = InapplicabilityReasons.VIOLATES_STATE_INVARIANTS
+                    if early_termination:
+                        break
+        return unsatisfied_conditions, reason
 
     def get_unsatisfied_goals(
         self, state: "up.model.State", early_termination: bool = False
     ) -> List["up.model.FNode"]:
         """
         Returns the list of `unsatisfied goals` evaluated in the given `state`.
         If the flag `early_termination` is set, the method ends and returns the first `unsatisfied goal`.
@@ -455,14 +578,18 @@
 
     @staticmethod
     def supported_kind() -> "up.model.ProblemKind":
         supported_kind = up.model.ProblemKind()
         supported_kind.set_problem_class("ACTION_BASED")
         supported_kind.set_typing("FLAT_TYPING")
         supported_kind.set_typing("HIERARCHICAL_TYPING")
+        supported_kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
+        supported_kind.set_parameters("BOOL_ACTION_PARAMETERS")
+        supported_kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
         supported_kind.set_numbers("CONTINUOUS_NUMBERS")
         supported_kind.set_numbers("DISCRETE_NUMBERS")
         supported_kind.set_numbers("BOUNDED_TYPES")
         supported_kind.set_problem_type("SIMPLE_NUMERIC_PLANNING")
         supported_kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         supported_kind.set_fluents_type("NUMERIC_FLUENTS")
         supported_kind.set_fluents_type("OBJECT_FLUENTS")
@@ -475,14 +602,15 @@
         supported_kind.set_effects_kind("INCREASE_EFFECTS")
         supported_kind.set_effects_kind("DECREASE_EFFECTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_BOOLEAN_ASSIGNMENTS")
         supported_kind.set_effects_kind("FLUENTS_IN_NUMERIC_ASSIGNMENTS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
+        supported_kind.set_constraints_kind("STATE_INVARIANTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/environment.py` & `unified_planning-0.6.0.94.dev1/unified_planning/environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/exceptions.py` & `unified_planning-0.6.0.94.dev1/unified_planning/exceptions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/grpc/converter.py` & `unified_planning-0.6.0.94.dev1/unified_planning/grpc/converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2.py` & `unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/unified_planning_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16unified_planning.proto\"i\n\nExpression\x12\x13\n\x04\x61tom\x18\x01 \x01(\x0b\x32\x05.Atom\x12\x19\n\x04list\x18\x02 \x03(\x0b\x32\x0b.Expression\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x1d\n\x04kind\x18\x04 \x01(\x0e\x32\x0f.ExpressionKind\"\\\n\x04\x41tom\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x15\n\x04real\x18\x03 \x01(\x0b\x32\x05.RealH\x00\x12\x11\n\x07\x62oolean\x18\x04 \x01(\x08H\x00\x42\t\n\x07\x63ontent\".\n\x04Real\x12\x11\n\tnumerator\x18\x01 \x01(\x03\x12\x13\n\x0b\x64\x65nominator\x18\x02 \x01(\x03\"9\n\x0fTypeDeclaration\x12\x11\n\ttype_name\x18\x01 \x01(\t\x12\x13\n\x0bparent_type\x18\x02 \x01(\t\"\'\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"n\n\x06\x46luent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nvalue_type\x18\x02 \x01(\t\x12\x1e\n\nparameters\x18\x03 \x03(\x0b\x32\n.Parameter\x12\"\n\rdefault_value\x18\x04 \x01(\x0b\x32\x0b.Expression\"/\n\x11ObjectDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\xcd\x01\n\x10\x45\x66\x66\x65\x63tExpression\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x1c.EffectExpression.EffectKind\x12\x1b\n\x06\x66luent\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x03 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\tcondition\x18\x04 \x01(\x0b\x32\x0b.Expression\"4\n\nEffectKind\x12\n\n\x06\x41SSIGN\x10\x00\x12\x0c\n\x08INCREASE\x10\x01\x12\x0c\n\x08\x44\x45\x43REASE\x10\x02\"M\n\x06\x45\x66\x66\x65\x63t\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"C\n\tCondition\x12\x19\n\x04\x63ond\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1b\n\x04span\x18\x02 \x01(\x0b\x32\r.TimeInterval\"\x8d\x01\n\x06\x41\x63tion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.Duration\x12\x1e\n\nconditions\x18\x04 \x03(\x0b\x32\n.Condition\x12\x18\n\x07\x65\x66\x66\x65\x63ts\x18\x05 \x03(\x0b\x32\x07.Effect\"\x90\x01\n\tTimepoint\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.Timepoint.TimepointKind\x12\x14\n\x0c\x63ontainer_id\x18\x02 \x01(\t\"E\n\rTimepointKind\x12\x10\n\x0cGLOBAL_START\x10\x00\x12\x0e\n\nGLOBAL_END\x10\x01\x12\t\n\x05START\x10\x02\x12\x07\n\x03\x45ND\x10\x03\"=\n\x06Timing\x12\x1d\n\ttimepoint\x18\x01 \x01(\x0b\x32\n.Timepoint\x12\x14\n\x05\x64\x65lay\x18\x02 \x01(\x0b\x32\x05.Real\"o\n\x08Interval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x1a\n\x05lower\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x1a\n\x05upper\x18\x04 \x01(\x0b\x32\x0b.Expression\"k\n\x0cTimeInterval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x16\n\x05lower\x18\x02 \x01(\x0b\x32\x07.Timing\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x16\n\x05upper\x18\x04 \x01(\x0b\x32\x07.Timing\"5\n\x08\x44uration\x12)\n\x16\x63ontrollable_in_bounds\x18\x01 \x01(\x0b\x32\t.Interval\"G\n\x17\x41\x62stractTaskDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\"F\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\ttask_name\x18\x02 \x01(\t\x12\x1f\n\nparameters\x18\x03 \x03(\x0b\x32\x0b.Expression\"\xaf\x01\n\x06Method\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1c\n\rachieved_task\x18\x03 \x01(\x0b\x32\x05.Task\x12\x17\n\x08subtasks\x18\x04 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x05 \x03(\x0b\x32\x0b.Expression\x12\x1e\n\nconditions\x18\x06 \x03(\x0b\x32\n.Condition\"g\n\x0bTaskNetwork\x12\x1d\n\tvariables\x18\x01 \x03(\x0b\x32\n.Parameter\x12\x17\n\x08subtasks\x18\x02 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x03 \x03(\x0b\x32\x0b.Expression\"\x83\x01\n\tHierarchy\x12\x30\n\x0e\x61\x62stract_tasks\x18\x01 \x03(\x0b\x32\x18.AbstractTaskDeclaration\x12\x18\n\x07methods\x18\x02 \x03(\x0b\x32\x07.Method\x12*\n\x14initial_task_network\x18\x03 \x01(\x0b\x32\x0c.TaskNetwork\"@\n\x04Goal\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\"R\n\x0bTimedEffect\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"E\n\nAssignment\x12\x1b\n\x06\x66luent\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression\"B\n\x0eGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x15\n\x06weight\x18\x02 \x01(\x0b\x32\x05.Real\"f\n\x13TimedGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\x12\x15\n\x06weight\x18\x03 \x01(\x0b\x32\x05.Real\"\x9c\x04\n\x06Metric\x12 \n\x04kind\x18\x01 \x01(\x0e\x32\x12.Metric.MetricKind\x12\x1f\n\nexpression\x18\x02 \x01(\x0b\x32\x0b.Expression\x12.\n\x0c\x61\x63tion_costs\x18\x03 \x03(\x0b\x32\x18.Metric.ActionCostsEntry\x12(\n\x13\x64\x65\x66\x61ult_action_cost\x18\x04 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\x05goals\x18\x05 \x03(\x0b\x32\x0f.GoalWithWeight\x12)\n\x0btimed_goals\x18\x06 \x03(\x0b\x32\x14.TimedGoalWithWeight\x1a?\n\x10\x41\x63tionCostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression:\x02\x38\x01\"\xe8\x01\n\nMetricKind\x12\x19\n\x15MINIMIZE_ACTION_COSTS\x10\x00\x12#\n\x1fMINIMIZE_SEQUENTIAL_PLAN_LENGTH\x10\x01\x12\x15\n\x11MINIMIZE_MAKESPAN\x10\x02\x12&\n\"MINIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x03\x12&\n\"MAXIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x04\x12\x14\n\x10OVERSUBSCRIPTION\x10\x05\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10\x06\"\xe2\x02\n\x07Problem\x12\x13\n\x0b\x64omain_name\x18\x01 \x01(\t\x12\x14\n\x0cproblem_name\x18\x02 \x01(\t\x12\x1f\n\x05types\x18\x03 \x03(\x0b\x32\x10.TypeDeclaration\x12\x18\n\x07\x66luents\x18\x04 \x03(\x0b\x32\x07.Fluent\x12#\n\x07objects\x18\x05 \x03(\x0b\x32\x12.ObjectDeclaration\x12\x18\n\x07\x61\x63tions\x18\x06 \x03(\x0b\x32\x07.Action\x12\"\n\rinitial_state\x18\x07 \x03(\x0b\x32\x0b.Assignment\x12#\n\rtimed_effects\x18\x08 \x03(\x0b\x32\x0c.TimedEffect\x12\x14\n\x05goals\x18\t \x03(\x0b\x32\x05.Goal\x12\x1a\n\x08\x66\x65\x61tures\x18\n \x03(\x0e\x32\x08.Feature\x12\x18\n\x07metrics\x18\x0b \x03(\x0b\x32\x07.Metric\x12\x1d\n\thierarchy\x18\x0c \x01(\x0b\x32\n.Hierarchy\"\x80\x01\n\x0e\x41\x63tionInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63tion_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12\x19\n\nstart_time\x18\x04 \x01(\x0b\x32\x05.Real\x12\x17\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x05.Real\"\xae\x01\n\x0eMethodInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12/\n\x08subtasks\x18\x06 \x03(\x0b\x32\x1d.MethodInstance.SubtasksEntry\x1a/\n\rSubtasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x96\x01\n\rPlanHierarchy\x12\x31\n\nroot_tasks\x18\x01 \x03(\x0b\x32\x1d.PlanHierarchy.RootTasksEntry\x12 \n\x07methods\x18\x02 \x03(\x0b\x32\x0f.MethodInstance\x1a\x30\n\x0eRootTasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"K\n\x04Plan\x12 \n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x0f.ActionInstance\x12!\n\thierarchy\x18\x02 \x01(\x0b\x32\x0e.PlanHierarchy\"\x83\x02\n\x0bPlanRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12*\n\x0fresolution_mode\x18\x02 \x01(\x0e\x32\x11.PlanRequest.Mode\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x37\n\x0e\x65ngine_options\x18\x04 \x03(\x0b\x32\x1f.PlanRequest.EngineOptionsEntry\x1a\x34\n\x12\x45ngineOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x04Mode\x12\x0f\n\x0bSATISFIABLE\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\"C\n\x11ValidationRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\"{\n\nLogMessage\x12#\n\x05level\x18\x01 \x01(\x0e\x32\x14.LogMessage.LogLevel\x12\x0f\n\x07message\x18\x02 \x01(\t\"7\n\x08LogLevel\x12\t\n\x05\x44\x45\x42UG\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\t\n\x05\x45RROR\x10\x03\"\xbf\x03\n\x14PlanGenerationResult\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.PlanGenerationResult.Status\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\x12\x33\n\x07metrics\x18\x03 \x03(\x0b\x32\".PlanGenerationResult.MetricsEntry\x12!\n\x0clog_messages\x18\x04 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x05 \x01(\x0b\x32\x07.Engine\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x01\n\x06Status\x12\x16\n\x12SOLVED_SATISFICING\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\x12\x15\n\x11UNSOLVABLE_PROVEN\x10\x02\x12\x1b\n\x17UNSOLVABLE_INCOMPLETELY\x10\x03\x12\x0b\n\x07TIMEOUT\x10\r\x12\n\n\x06MEMOUT\x10\x0e\x12\x12\n\x0eINTERNAL_ERROR\x10\x0f\x12\x17\n\x13UNSUPPORTED_PROBLEM\x10\x10\x12\x10\n\x0cINTERMEDIATE\x10\x11\"\x16\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xba\x01\n\x10ValidationResult\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.ValidationResult.ValidationResultStatus\x12!\n\x0clog_messages\x18\x02 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x03 \x01(\x0b\x32\x07.Engine\"0\n\x16ValidationResultStatus\x12\t\n\x05VALID\x10\x00\x12\x0b\n\x07INVALID\x10\x01\"\xe5\x01\n\x0e\x43ompilerResult\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x37\n\rmap_back_plan\x18\x02 \x03(\x0b\x32 .CompilerResult.MapBackPlanEntry\x12!\n\x0clog_messages\x18\x03 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x04 \x01(\x0b\x32\x07.Engine\x1a\x43\n\x10MapBackPlanEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.ActionInstance:\x02\x38\x01*\xb0\x01\n\x0e\x45xpressionKind\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x43ONSTANT\x10\x01\x12\r\n\tPARAMETER\x10\x02\x12\x0c\n\x08VARIABLE\x10\x07\x12\x11\n\rFLUENT_SYMBOL\x10\x03\x12\x13\n\x0f\x46UNCTION_SYMBOL\x10\x04\x12\x12\n\x0eSTATE_VARIABLE\x10\x05\x12\x18\n\x14\x46UNCTION_APPLICATION\x10\x06\x12\x10\n\x0c\x43ONTAINER_ID\x10\x08*\xbc\t\n\x07\x46\x65\x61ture\x12\x10\n\x0c\x41\x43TION_BASED\x10\x00\x12\x10\n\x0cHIERARCHICAL\x10\x1a\x12\x1b\n\x17SIMPLE_NUMERIC_PLANNING\x10\x1e\x12\x1c\n\x18GENERAL_NUMERIC_PLANNING\x10\x1f\x12\x13\n\x0f\x43ONTINUOUS_TIME\x10\x01\x12\x11\n\rDISCRETE_TIME\x10\x02\x12\'\n#INTERMEDIATE_CONDITIONS_AND_EFFECTS\x10\x03\x12#\n\x1f\x45XTERNAL_CONDITIONS_AND_EFFECTS\x10\'\x12\x11\n\rTIMED_EFFECTS\x10\x04\x12\x0f\n\x0bTIMED_GOALS\x10\x05\x12\x19\n\x15\x44URATION_INEQUALITIES\x10\x06\x12\x1f\n\x1bSTATIC_FLUENTS_IN_DURATIONS\x10\x1b\x12\x18\n\x14\x46LUENTS_IN_DURATIONS\x10\x1c\x12\x16\n\x12\x43ONTINUOUS_NUMBERS\x10\x07\x12\x14\n\x10\x44ISCRETE_NUMBERS\x10\x08\x12\x11\n\rBOUNDED_TYPES\x10&\x12\x17\n\x13NEGATIVE_CONDITIONS\x10\t\x12\x1a\n\x16\x44ISJUNCTIVE_CONDITIONS\x10\n\x12\x0e\n\nEQUALITIES\x10\x0b\x12\x1a\n\x16\x45XISTENTIAL_CONDITIONS\x10\x0c\x12\x18\n\x14UNIVERSAL_CONDITIONS\x10\r\x12\x17\n\x13\x43ONDITIONAL_EFFECTS\x10\x0e\x12\x14\n\x10INCREASE_EFFECTS\x10\x0f\x12\x14\n\x10\x44\x45\x43REASE_EFFECTS\x10\x10\x12)\n%STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS\x10)\x12)\n%STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS\x10*\x12\"\n\x1e\x46LUENTS_IN_BOOLEAN_ASSIGNMENTS\x10+\x12\"\n\x1e\x46LUENTS_IN_NUMERIC_ASSIGNMENTS\x10,\x12\x0f\n\x0b\x46LAT_TYPING\x10\x11\x12\x17\n\x13HIERARCHICAL_TYPING\x10\x12\x12\x13\n\x0fNUMERIC_FLUENTS\x10\x13\x12\x12\n\x0eOBJECT_FLUENTS\x10\x14\x12\x10\n\x0c\x41\x43TIONS_COST\x10\x15\x12\x0f\n\x0b\x46INAL_VALUE\x10\x16\x12\x0c\n\x08MAKESPAN\x10\x17\x12\x0f\n\x0bPLAN_LENGTH\x10\x18\x12\x14\n\x10OVERSUBSCRIPTION\x10\x1d\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10(\x12\"\n\x1eSTATIC_FLUENTS_IN_ACTIONS_COST\x10-\x12\x1b\n\x17\x46LUENTS_IN_ACTIONS_COST\x10.\x12\x15\n\x11SIMULATED_EFFECTS\x10\x19\x12\x18\n\x14METHOD_PRECONDITIONS\x10 \x12\x1c\n\x18TASK_NETWORK_CONSTRAINTS\x10!\x12\"\n\x1eINITIAL_TASK_NETWORK_VARIABLES\x10\"\x12\x14\n\x10TASK_ORDER_TOTAL\x10#\x12\x16\n\x12TASK_ORDER_PARTIAL\x10$\x12\x17\n\x13TASK_ORDER_TEMPORAL\x10%2\xd8\x01\n\x0fUnifiedPlanning\x12\x34\n\x0bplanAnytime\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult0\x01\x12\x32\n\x0bplanOneShot\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult\x12\x35\n\x0cvalidatePlan\x12\x12.ValidationRequest\x1a\x11.ValidationResult\x12$\n\x07\x63ompile\x12\x08.Problem\x1a\x0f.CompilerResultb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16unified_planning.proto\"i\n\nExpression\x12\x13\n\x04\x61tom\x18\x01 \x01(\x0b\x32\x05.Atom\x12\x19\n\x04list\x18\x02 \x03(\x0b\x32\x0b.Expression\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x1d\n\x04kind\x18\x04 \x01(\x0e\x32\x0f.ExpressionKind\"\\\n\x04\x41tom\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x15\n\x04real\x18\x03 \x01(\x0b\x32\x05.RealH\x00\x12\x11\n\x07\x62oolean\x18\x04 \x01(\x08H\x00\x42\t\n\x07\x63ontent\".\n\x04Real\x12\x11\n\tnumerator\x18\x01 \x01(\x03\x12\x13\n\x0b\x64\x65nominator\x18\x02 \x01(\x03\"9\n\x0fTypeDeclaration\x12\x11\n\ttype_name\x18\x01 \x01(\t\x12\x13\n\x0bparent_type\x18\x02 \x01(\t\"\'\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"n\n\x06\x46luent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nvalue_type\x18\x02 \x01(\t\x12\x1e\n\nparameters\x18\x03 \x03(\x0b\x32\n.Parameter\x12\"\n\rdefault_value\x18\x04 \x01(\x0b\x32\x0b.Expression\"/\n\x11ObjectDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\xcd\x01\n\x10\x45\x66\x66\x65\x63tExpression\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x1c.EffectExpression.EffectKind\x12\x1b\n\x06\x66luent\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x03 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\tcondition\x18\x04 \x01(\x0b\x32\x0b.Expression\"4\n\nEffectKind\x12\n\n\x06\x41SSIGN\x10\x00\x12\x0c\n\x08INCREASE\x10\x01\x12\x0c\n\x08\x44\x45\x43REASE\x10\x02\"M\n\x06\x45\x66\x66\x65\x63t\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"C\n\tCondition\x12\x19\n\x04\x63ond\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1b\n\x04span\x18\x02 \x01(\x0b\x32\r.TimeInterval\"\x8d\x01\n\x06\x41\x63tion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.Duration\x12\x1e\n\nconditions\x18\x04 \x03(\x0b\x32\n.Condition\x12\x18\n\x07\x65\x66\x66\x65\x63ts\x18\x05 \x03(\x0b\x32\x07.Effect\"\x90\x01\n\tTimepoint\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.Timepoint.TimepointKind\x12\x14\n\x0c\x63ontainer_id\x18\x02 \x01(\t\"E\n\rTimepointKind\x12\x10\n\x0cGLOBAL_START\x10\x00\x12\x0e\n\nGLOBAL_END\x10\x01\x12\t\n\x05START\x10\x02\x12\x07\n\x03\x45ND\x10\x03\"=\n\x06Timing\x12\x1d\n\ttimepoint\x18\x01 \x01(\x0b\x32\n.Timepoint\x12\x14\n\x05\x64\x65lay\x18\x02 \x01(\x0b\x32\x05.Real\"o\n\x08Interval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x1a\n\x05lower\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x1a\n\x05upper\x18\x04 \x01(\x0b\x32\x0b.Expression\"k\n\x0cTimeInterval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x16\n\x05lower\x18\x02 \x01(\x0b\x32\x07.Timing\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x16\n\x05upper\x18\x04 \x01(\x0b\x32\x07.Timing\"5\n\x08\x44uration\x12)\n\x16\x63ontrollable_in_bounds\x18\x01 \x01(\x0b\x32\t.Interval\"G\n\x17\x41\x62stractTaskDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\"F\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\ttask_name\x18\x02 \x01(\t\x12\x1f\n\nparameters\x18\x03 \x03(\x0b\x32\x0b.Expression\"\xaf\x01\n\x06Method\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1c\n\rachieved_task\x18\x03 \x01(\x0b\x32\x05.Task\x12\x17\n\x08subtasks\x18\x04 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x05 \x03(\x0b\x32\x0b.Expression\x12\x1e\n\nconditions\x18\x06 \x03(\x0b\x32\n.Condition\"g\n\x0bTaskNetwork\x12\x1d\n\tvariables\x18\x01 \x03(\x0b\x32\n.Parameter\x12\x17\n\x08subtasks\x18\x02 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x03 \x03(\x0b\x32\x0b.Expression\"\x83\x01\n\tHierarchy\x12\x30\n\x0e\x61\x62stract_tasks\x18\x01 \x03(\x0b\x32\x18.AbstractTaskDeclaration\x12\x18\n\x07methods\x18\x02 \x03(\x0b\x32\x07.Method\x12*\n\x14initial_task_network\x18\x03 \x01(\x0b\x32\x0c.TaskNetwork\"@\n\x04Goal\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\"R\n\x0bTimedEffect\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"E\n\nAssignment\x12\x1b\n\x06\x66luent\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression\"B\n\x0eGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x15\n\x06weight\x18\x02 \x01(\x0b\x32\x05.Real\"f\n\x13TimedGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\x12\x15\n\x06weight\x18\x03 \x01(\x0b\x32\x05.Real\"\x9c\x04\n\x06Metric\x12 \n\x04kind\x18\x01 \x01(\x0e\x32\x12.Metric.MetricKind\x12\x1f\n\nexpression\x18\x02 \x01(\x0b\x32\x0b.Expression\x12.\n\x0c\x61\x63tion_costs\x18\x03 \x03(\x0b\x32\x18.Metric.ActionCostsEntry\x12(\n\x13\x64\x65\x66\x61ult_action_cost\x18\x04 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\x05goals\x18\x05 \x03(\x0b\x32\x0f.GoalWithWeight\x12)\n\x0btimed_goals\x18\x06 \x03(\x0b\x32\x14.TimedGoalWithWeight\x1a?\n\x10\x41\x63tionCostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression:\x02\x38\x01\"\xe8\x01\n\nMetricKind\x12\x19\n\x15MINIMIZE_ACTION_COSTS\x10\x00\x12#\n\x1fMINIMIZE_SEQUENTIAL_PLAN_LENGTH\x10\x01\x12\x15\n\x11MINIMIZE_MAKESPAN\x10\x02\x12&\n\"MINIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x03\x12&\n\"MAXIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x04\x12\x14\n\x10OVERSUBSCRIPTION\x10\x05\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10\x06\"\xd8\x03\n\x07Problem\x12\x13\n\x0b\x64omain_name\x18\x01 \x01(\t\x12\x14\n\x0cproblem_name\x18\x02 \x01(\t\x12\x1f\n\x05types\x18\x03 \x03(\x0b\x32\x10.TypeDeclaration\x12\x18\n\x07\x66luents\x18\x04 \x03(\x0b\x32\x07.Fluent\x12#\n\x07objects\x18\x05 \x03(\x0b\x32\x12.ObjectDeclaration\x12\x18\n\x07\x61\x63tions\x18\x06 \x03(\x0b\x32\x07.Action\x12\"\n\rinitial_state\x18\x07 \x03(\x0b\x32\x0b.Assignment\x12#\n\rtimed_effects\x18\x08 \x03(\x0b\x32\x0c.TimedEffect\x12\x14\n\x05goals\x18\t \x03(\x0b\x32\x05.Goal\x12\x1a\n\x08\x66\x65\x61tures\x18\n \x03(\x0e\x32\x08.Feature\x12\x18\n\x07metrics\x18\x0b \x03(\x0b\x32\x07.Metric\x12\x1d\n\thierarchy\x18\x0c \x01(\x0b\x32\n.Hierarchy\x12+\n\x16trajectory_constraints\x18\r \x03(\x0b\x32\x0b.Expression\x12\x15\n\rdiscrete_time\x18\x0e \x01(\x08\x12\x18\n\x10self_overlapping\x18\x0f \x01(\x08\x12\x16\n\x07\x65psilon\x18\x10 \x01(\x0b\x32\x05.Real\"\x80\x01\n\x0e\x41\x63tionInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63tion_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12\x19\n\nstart_time\x18\x04 \x01(\x0b\x32\x05.Real\x12\x17\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x05.Real\"\xae\x01\n\x0eMethodInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12/\n\x08subtasks\x18\x06 \x03(\x0b\x32\x1d.MethodInstance.SubtasksEntry\x1a/\n\rSubtasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x96\x01\n\rPlanHierarchy\x12\x31\n\nroot_tasks\x18\x01 \x03(\x0b\x32\x1d.PlanHierarchy.RootTasksEntry\x12 \n\x07methods\x18\x02 \x03(\x0b\x32\x0f.MethodInstance\x1a\x30\n\x0eRootTasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"K\n\x04Plan\x12 \n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x0f.ActionInstance\x12!\n\thierarchy\x18\x02 \x01(\x0b\x32\x0e.PlanHierarchy\"\x83\x02\n\x0bPlanRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12*\n\x0fresolution_mode\x18\x02 \x01(\x0e\x32\x11.PlanRequest.Mode\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x37\n\x0e\x65ngine_options\x18\x04 \x03(\x0b\x32\x1f.PlanRequest.EngineOptionsEntry\x1a\x34\n\x12\x45ngineOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x04Mode\x12\x0f\n\x0bSATISFIABLE\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\"C\n\x11ValidationRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\"{\n\nLogMessage\x12#\n\x05level\x18\x01 \x01(\x0e\x32\x14.LogMessage.LogLevel\x12\x0f\n\x07message\x18\x02 \x01(\t\"7\n\x08LogLevel\x12\t\n\x05\x44\x45\x42UG\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\t\n\x05\x45RROR\x10\x03\"\xbf\x03\n\x14PlanGenerationResult\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.PlanGenerationResult.Status\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\x12\x33\n\x07metrics\x18\x03 \x03(\x0b\x32\".PlanGenerationResult.MetricsEntry\x12!\n\x0clog_messages\x18\x04 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x05 \x01(\x0b\x32\x07.Engine\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x01\n\x06Status\x12\x16\n\x12SOLVED_SATISFICING\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\x12\x15\n\x11UNSOLVABLE_PROVEN\x10\x02\x12\x1b\n\x17UNSOLVABLE_INCOMPLETELY\x10\x03\x12\x0b\n\x07TIMEOUT\x10\r\x12\n\n\x06MEMOUT\x10\x0e\x12\x12\n\x0eINTERNAL_ERROR\x10\x0f\x12\x17\n\x13UNSUPPORTED_PROBLEM\x10\x10\x12\x10\n\x0cINTERMEDIATE\x10\x11\"\x16\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xc7\x01\n\x10ValidationResult\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.ValidationResult.ValidationResultStatus\x12!\n\x0clog_messages\x18\x02 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x03 \x01(\x0b\x32\x07.Engine\"=\n\x16ValidationResultStatus\x12\t\n\x05VALID\x10\x00\x12\x0b\n\x07INVALID\x10\x01\x12\x0b\n\x07UNKNOWN\x10\x02\"\xe5\x01\n\x0e\x43ompilerResult\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x37\n\rmap_back_plan\x18\x02 \x03(\x0b\x32 .CompilerResult.MapBackPlanEntry\x12!\n\x0clog_messages\x18\x03 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x04 \x01(\x0b\x32\x07.Engine\x1a\x43\n\x10MapBackPlanEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.ActionInstance:\x02\x38\x01*\xb0\x01\n\x0e\x45xpressionKind\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x43ONSTANT\x10\x01\x12\r\n\tPARAMETER\x10\x02\x12\x0c\n\x08VARIABLE\x10\x07\x12\x11\n\rFLUENT_SYMBOL\x10\x03\x12\x13\n\x0f\x46UNCTION_SYMBOL\x10\x04\x12\x12\n\x0eSTATE_VARIABLE\x10\x05\x12\x18\n\x14\x46UNCTION_APPLICATION\x10\x06\x12\x10\n\x0c\x43ONTAINER_ID\x10\x08*\xc3\x0b\n\x07\x46\x65\x61ture\x12\x10\n\x0c\x41\x43TION_BASED\x10\x00\x12\x10\n\x0cHIERARCHICAL\x10\x1a\x12\x1b\n\x17SIMPLE_NUMERIC_PLANNING\x10\x1e\x12\x1c\n\x18GENERAL_NUMERIC_PLANNING\x10\x1f\x12\x13\n\x0f\x43ONTINUOUS_TIME\x10\x01\x12\x11\n\rDISCRETE_TIME\x10\x02\x12\'\n#INTERMEDIATE_CONDITIONS_AND_EFFECTS\x10\x03\x12#\n\x1f\x45XTERNAL_CONDITIONS_AND_EFFECTS\x10\'\x12\x11\n\rTIMED_EFFECTS\x10\x04\x12\x0f\n\x0bTIMED_GOALS\x10\x05\x12\x19\n\x15\x44URATION_INEQUALITIES\x10\x06\x12\x14\n\x10SELF_OVERLAPPING\x10/\x12\x1f\n\x1bSTATIC_FLUENTS_IN_DURATIONS\x10\x1b\x12\x18\n\x14\x46LUENTS_IN_DURATIONS\x10\x1c\x12\x16\n\x12\x43ONTINUOUS_NUMBERS\x10\x07\x12\x14\n\x10\x44ISCRETE_NUMBERS\x10\x08\x12\x11\n\rBOUNDED_TYPES\x10&\x12\x17\n\x13NEGATIVE_CONDITIONS\x10\t\x12\x1a\n\x16\x44ISJUNCTIVE_CONDITIONS\x10\n\x12\x0e\n\nEQUALITIES\x10\x0b\x12\x1a\n\x16\x45XISTENTIAL_CONDITIONS\x10\x0c\x12\x18\n\x14UNIVERSAL_CONDITIONS\x10\r\x12\x17\n\x13\x43ONDITIONAL_EFFECTS\x10\x0e\x12\x14\n\x10INCREASE_EFFECTS\x10\x0f\x12\x14\n\x10\x44\x45\x43REASE_EFFECTS\x10\x10\x12)\n%STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS\x10)\x12)\n%STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS\x10*\x12\"\n\x1e\x46LUENTS_IN_BOOLEAN_ASSIGNMENTS\x10+\x12\"\n\x1e\x46LUENTS_IN_NUMERIC_ASSIGNMENTS\x10,\x12\x0f\n\x0b\x46LAT_TYPING\x10\x11\x12\x17\n\x13HIERARCHICAL_TYPING\x10\x12\x12\x13\n\x0fNUMERIC_FLUENTS\x10\x13\x12\x12\n\x0eOBJECT_FLUENTS\x10\x14\x12\x1a\n\x16\x42OOL_FLUENT_PARAMETERS\x10\x32\x12!\n\x1d\x42OUNDED_INT_FLUENT_PARAMETERS\x10\x33\x12\x1a\n\x16\x42OOL_ACTION_PARAMETERS\x10\x34\x12!\n\x1d\x42OUNDED_INT_ACTION_PARAMETERS\x10\x35\x12#\n\x1fUNBOUNDED_INT_ACTION_PARAMETERS\x10\x36\x12\x1a\n\x16REAL_ACTION_PARAMETERS\x10\x37\x12\x10\n\x0c\x41\x43TIONS_COST\x10\x15\x12\x0f\n\x0b\x46INAL_VALUE\x10\x16\x12\x0c\n\x08MAKESPAN\x10\x17\x12\x0f\n\x0bPLAN_LENGTH\x10\x18\x12\x14\n\x10OVERSUBSCRIPTION\x10\x1d\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10(\x12\"\n\x1eSTATIC_FLUENTS_IN_ACTIONS_COST\x10-\x12\x1b\n\x17\x46LUENTS_IN_ACTIONS_COST\x10.\x12\x15\n\x11SIMULATED_EFFECTS\x10\x19\x12\x1a\n\x16TRAJECTORY_CONSTRAINTS\x10\x30\x12\x14\n\x10STATE_INVARIANTS\x10\x31\x12\x18\n\x14METHOD_PRECONDITIONS\x10 \x12\x1c\n\x18TASK_NETWORK_CONSTRAINTS\x10!\x12\"\n\x1eINITIAL_TASK_NETWORK_VARIABLES\x10\"\x12\x14\n\x10TASK_ORDER_TOTAL\x10#\x12\x16\n\x12TASK_ORDER_PARTIAL\x10$\x12\x17\n\x13TASK_ORDER_TEMPORAL\x10%2\xd8\x01\n\x0fUnifiedPlanning\x12\x34\n\x0bplanAnytime\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult0\x01\x12\x32\n\x0bplanOneShot\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult\x12\x35\n\x0cvalidatePlan\x12\x12.ValidationRequest\x1a\x11.ValidationResult\x12$\n\x07\x63ompile\x12\x08.Problem\x1a\x0f.CompilerResultb\x06proto3')
 
 _EXPRESSIONKIND = DESCRIPTOR.enum_types_by_name['ExpressionKind']
 ExpressionKind = enum_type_wrapper.EnumTypeWrapper(_EXPRESSIONKIND)
 _FEATURE = DESCRIPTOR.enum_types_by_name['Feature']
 Feature = enum_type_wrapper.EnumTypeWrapper(_FEATURE)
 UNKNOWN = 0
 CONSTANT = 1
@@ -37,14 +37,15 @@
 CONTINUOUS_TIME = 1
 DISCRETE_TIME = 2
 INTERMEDIATE_CONDITIONS_AND_EFFECTS = 3
 EXTERNAL_CONDITIONS_AND_EFFECTS = 39
 TIMED_EFFECTS = 4
 TIMED_GOALS = 5
 DURATION_INEQUALITIES = 6
+SELF_OVERLAPPING = 47
 STATIC_FLUENTS_IN_DURATIONS = 27
 FLUENTS_IN_DURATIONS = 28
 CONTINUOUS_NUMBERS = 7
 DISCRETE_NUMBERS = 8
 BOUNDED_TYPES = 38
 NEGATIVE_CONDITIONS = 9
 DISJUNCTIVE_CONDITIONS = 10
@@ -58,23 +59,31 @@
 STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS = 42
 FLUENTS_IN_BOOLEAN_ASSIGNMENTS = 43
 FLUENTS_IN_NUMERIC_ASSIGNMENTS = 44
 FLAT_TYPING = 17
 HIERARCHICAL_TYPING = 18
 NUMERIC_FLUENTS = 19
 OBJECT_FLUENTS = 20
+BOOL_FLUENT_PARAMETERS = 50
+BOUNDED_INT_FLUENT_PARAMETERS = 51
+BOOL_ACTION_PARAMETERS = 52
+BOUNDED_INT_ACTION_PARAMETERS = 53
+UNBOUNDED_INT_ACTION_PARAMETERS = 54
+REAL_ACTION_PARAMETERS = 55
 ACTIONS_COST = 21
 FINAL_VALUE = 22
 MAKESPAN = 23
 PLAN_LENGTH = 24
 OVERSUBSCRIPTION = 29
 TEMPORAL_OVERSUBSCRIPTION = 40
 STATIC_FLUENTS_IN_ACTIONS_COST = 45
 FLUENTS_IN_ACTIONS_COST = 46
 SIMULATED_EFFECTS = 25
+TRAJECTORY_CONSTRAINTS = 48
+STATE_INVARIANTS = 49
 METHOD_PRECONDITIONS = 32
 TASK_NETWORK_CONSTRAINTS = 33
 INITIAL_TASK_NETWORK_VARIABLES = 34
 TASK_ORDER_TOTAL = 35
 TASK_ORDER_PARTIAL = 36
 TASK_ORDER_TEMPORAL = 37
 
@@ -464,18 +473,18 @@
   _PLANHIERARCHY_ROOTTASKSENTRY._serialized_options = b'8\001'
   _PLANREQUEST_ENGINEOPTIONSENTRY._options = None
   _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_options = b'8\001'
   _PLANGENERATIONRESULT_METRICSENTRY._options = None
   _PLANGENERATIONRESULT_METRICSENTRY._serialized_options = b'8\001'
   _COMPILERRESULT_MAPBACKPLANENTRY._options = None
   _COMPILERRESULT_MAPBACKPLANENTRY._serialized_options = b'8\001'
-  _EXPRESSIONKIND._serialized_start=5268
-  _EXPRESSIONKIND._serialized_end=5444
-  _FEATURE._serialized_start=5447
-  _FEATURE._serialized_end=6659
+  _EXPRESSIONKIND._serialized_start=5399
+  _EXPRESSIONKIND._serialized_end=5575
+  _FEATURE._serialized_start=5578
+  _FEATURE._serialized_end=7053
   _EXPRESSION._serialized_start=26
   _EXPRESSION._serialized_end=131
   _ATOM._serialized_start=133
   _ATOM._serialized_end=225
   _REAL._serialized_start=227
   _REAL._serialized_end=273
   _TYPEDECLARATION._serialized_start=275
@@ -531,51 +540,51 @@
   _METRIC._serialized_start=2479
   _METRIC._serialized_end=3019
   _METRIC_ACTIONCOSTSENTRY._serialized_start=2721
   _METRIC_ACTIONCOSTSENTRY._serialized_end=2784
   _METRIC_METRICKIND._serialized_start=2787
   _METRIC_METRICKIND._serialized_end=3019
   _PROBLEM._serialized_start=3022
-  _PROBLEM._serialized_end=3376
-  _ACTIONINSTANCE._serialized_start=3379
-  _ACTIONINSTANCE._serialized_end=3507
-  _METHODINSTANCE._serialized_start=3510
-  _METHODINSTANCE._serialized_end=3684
-  _METHODINSTANCE_SUBTASKSENTRY._serialized_start=3637
-  _METHODINSTANCE_SUBTASKSENTRY._serialized_end=3684
-  _PLANHIERARCHY._serialized_start=3687
-  _PLANHIERARCHY._serialized_end=3837
-  _PLANHIERARCHY_ROOTTASKSENTRY._serialized_start=3789
-  _PLANHIERARCHY_ROOTTASKSENTRY._serialized_end=3837
-  _PLAN._serialized_start=3839
-  _PLAN._serialized_end=3914
-  _PLANREQUEST._serialized_start=3917
-  _PLANREQUEST._serialized_end=4176
-  _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_start=4077
-  _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_end=4129
-  _PLANREQUEST_MODE._serialized_start=4131
-  _PLANREQUEST_MODE._serialized_end=4176
-  _VALIDATIONREQUEST._serialized_start=4178
-  _VALIDATIONREQUEST._serialized_end=4245
-  _LOGMESSAGE._serialized_start=4247
-  _LOGMESSAGE._serialized_end=4370
-  _LOGMESSAGE_LOGLEVEL._serialized_start=4315
-  _LOGMESSAGE_LOGLEVEL._serialized_end=4370
-  _PLANGENERATIONRESULT._serialized_start=4373
-  _PLANGENERATIONRESULT._serialized_end=4820
-  _PLANGENERATIONRESULT_METRICSENTRY._serialized_start=4577
-  _PLANGENERATIONRESULT_METRICSENTRY._serialized_end=4623
-  _PLANGENERATIONRESULT_STATUS._serialized_start=4626
-  _PLANGENERATIONRESULT_STATUS._serialized_end=4820
-  _ENGINE._serialized_start=4822
-  _ENGINE._serialized_end=4844
-  _VALIDATIONRESULT._serialized_start=4847
-  _VALIDATIONRESULT._serialized_end=5033
-  _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_start=4985
-  _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_end=5033
-  _COMPILERRESULT._serialized_start=5036
-  _COMPILERRESULT._serialized_end=5265
-  _COMPILERRESULT_MAPBACKPLANENTRY._serialized_start=5198
-  _COMPILERRESULT_MAPBACKPLANENTRY._serialized_end=5265
-  _UNIFIEDPLANNING._serialized_start=6662
-  _UNIFIEDPLANNING._serialized_end=6878
+  _PROBLEM._serialized_end=3494
+  _ACTIONINSTANCE._serialized_start=3497
+  _ACTIONINSTANCE._serialized_end=3625
+  _METHODINSTANCE._serialized_start=3628
+  _METHODINSTANCE._serialized_end=3802
+  _METHODINSTANCE_SUBTASKSENTRY._serialized_start=3755
+  _METHODINSTANCE_SUBTASKSENTRY._serialized_end=3802
+  _PLANHIERARCHY._serialized_start=3805
+  _PLANHIERARCHY._serialized_end=3955
+  _PLANHIERARCHY_ROOTTASKSENTRY._serialized_start=3907
+  _PLANHIERARCHY_ROOTTASKSENTRY._serialized_end=3955
+  _PLAN._serialized_start=3957
+  _PLAN._serialized_end=4032
+  _PLANREQUEST._serialized_start=4035
+  _PLANREQUEST._serialized_end=4294
+  _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_start=4195
+  _PLANREQUEST_ENGINEOPTIONSENTRY._serialized_end=4247
+  _PLANREQUEST_MODE._serialized_start=4249
+  _PLANREQUEST_MODE._serialized_end=4294
+  _VALIDATIONREQUEST._serialized_start=4296
+  _VALIDATIONREQUEST._serialized_end=4363
+  _LOGMESSAGE._serialized_start=4365
+  _LOGMESSAGE._serialized_end=4488
+  _LOGMESSAGE_LOGLEVEL._serialized_start=4433
+  _LOGMESSAGE_LOGLEVEL._serialized_end=4488
+  _PLANGENERATIONRESULT._serialized_start=4491
+  _PLANGENERATIONRESULT._serialized_end=4938
+  _PLANGENERATIONRESULT_METRICSENTRY._serialized_start=4695
+  _PLANGENERATIONRESULT_METRICSENTRY._serialized_end=4741
+  _PLANGENERATIONRESULT_STATUS._serialized_start=4744
+  _PLANGENERATIONRESULT_STATUS._serialized_end=4938
+  _ENGINE._serialized_start=4940
+  _ENGINE._serialized_end=4962
+  _VALIDATIONRESULT._serialized_start=4965
+  _VALIDATIONRESULT._serialized_end=5164
+  _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_start=5103
+  _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_end=5164
+  _COMPILERRESULT._serialized_start=5167
+  _COMPILERRESULT._serialized_end=5396
+  _COMPILERRESULT_MAPBACKPLANENTRY._serialized_start=5329
+  _COMPILERRESULT_MAPBACKPLANENTRY._serialized_end=5396
+  _UNIFIEDPLANNING._serialized_start=7056
+  _UNIFIEDPLANNING._serialized_end=7272
 # @@protoc_insertion_point(module_scope)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py` & `unified_planning-0.6.0.94.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/grpc/proto_reader.py` & `unified_planning-0.6.0.94.dev1/unified_planning/grpc/proto_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # type: ignore
-from abc import ABC
 from functools import partial
 from typing import Tuple, Union, Optional
 import fractions
 from typing import OrderedDict
 
 import unified_planning.grpc.generated.unified_planning_pb2 as proto
 from unified_planning.exceptions import UPException
@@ -43,16 +42,18 @@
 
 def convert_type_str(s: str, problem: Problem) -> model.types.Type:
     if s == "up:bool":
         return problem.environment.type_manager.BoolType()
     elif s == "up:integer":
         return problem.environment.type_manager.IntType()
     elif "up:integer[" in s:
-        lb = int(s.split("[")[1].split(",")[0])
-        ub = int(s.split(",")[1].split("]")[0])
+        str_lb = s.split("[")[1].split(",")[0]
+        lb = None if "-inf" in str_lb else int(str_lb)
+        str_ub = s.split(",")[1].split("]")[0]
+        ub = None if "inf" in str_ub else int(str_ub)
         return problem.environment.type_manager.IntType(lb, ub)
     elif s == "up:real":
         return problem.environment.type_manager.RealType()
     elif "up:real[" in s:
         return problem.environment.type_manager.RealType(
             lower_bound=fractions.Fraction(s.split("[")[1].split(",")[0]),
             upper_bound=fractions.Fraction(s.split(",")[1].split("]")[0]),
@@ -88,15 +89,24 @@
         return OperatorKind.EXISTS
     elif op == "up:forall":
         return OperatorKind.FORALL
     elif op == "up:implies":
         return OperatorKind.IMPLIES
     elif op == "up:iff":
         return OperatorKind.IFF
-
+    elif op == "up:always":
+        return OperatorKind.ALWAYS
+    elif op == "up:at_most_once":
+        return OperatorKind.AT_MOST_ONCE
+    elif op == "up:sometime":
+        return OperatorKind.SOMETIME
+    elif op == "up:sometime_after":
+        return OperatorKind.SOMETIME_AFTER
+    elif op == "up:sometime_before":
+        return OperatorKind.SOMETIME_BEFORE
     raise ValueError(f"Unknown operator `{op}`")
 
 
 class ProtobufReader(Converter):
     """
     ProtobufReader: This class uses the convert method to take the protobuf representation of a
     unified_planning Problem and return the equivalent unified_planning Problem instance.
@@ -332,26 +342,35 @@
             goal = self.convert(g.goal, problem)
             if str(g.timing) == "":
                 problem.add_goal(goal)
             else:
                 timing = self.convert(g.timing)
                 problem.add_timed_goal(interval=timing, goal=goal)
 
+        for tc in msg.trajectory_constraints:
+            problem.add_trajectory_constraint(self.convert(tc, problem))
+
         for metric in msg.metrics:
             problem.add_quality_metric(self.convert(metric, problem))
 
         if msg.HasField("hierarchy"):
             for task in msg.hierarchy.abstract_tasks:
                 problem.add_task(self.convert(task, problem))
             for method in msg.hierarchy.methods:
                 problem.add_method(self.convert(method, problem))
             problem._initial_task_network = self.convert(
                 msg.hierarchy.initial_task_network, problem
             )
 
+        problem.discrete_time = msg.discrete_time
+        problem.self_overlapping = msg.self_overlapping
+        if msg.HasField("epsilon"):
+            value = msg.epsilon
+            problem.epsilon = fractions.Fraction(value.numerator, value.denominator)
+
         return problem
 
     @handles(proto.AbstractTaskDeclaration)
     def _convert_abstract_task(
         self, msg: proto.AbstractTaskDeclaration, problem: Problem
     ):
         return model.htn.Task(
@@ -644,15 +663,17 @@
         else:
             return flat_plan
 
     @handles(proto.ActionInstance)
     def _convert_action_instance(
         self, msg: proto.ActionInstance, problem: Problem
     ) -> Tuple[
-        str, ActionInstance, Optional[Tuple[model.Timing, model.timing.Duration]]
+        str,
+        ActionInstance,
+        Optional[Tuple[fractions.Fraction, Optional[fractions.Fraction]]],
     ]:
         # action instance parameters are atoms but in UP they are FNodes
         # converting to up.model.FNode
         parameters = tuple([self.convert(param, problem) for param in msg.parameters])
 
         id = msg.id
         action_instance = unified_planning.plans.ActionInstance(
@@ -660,15 +681,19 @@
             parameters,
         )
 
         if msg.HasField("start_time") and msg.HasField("end_time"):
             start_time = self.convert(msg.start_time)
             end_time = self.convert(msg.end_time)
             duration = end_time - start_time
-            return id, action_instance, (start_time, duration)
+            return (
+                id,
+                action_instance,
+                (start_time, None if duration == 0 else duration),
+            )
         else:
             return id, action_instance, None
 
     @handles(proto.PlanGenerationResult)
     def _convert_plan_generation_result(
         self, result: proto.PlanGenerationResult, problem: Problem
     ) -> unified_planning.engines.PlanGenerationResult:
@@ -799,14 +824,18 @@
             "VALID"
         ):
             r_status = unified_planning.engines.ValidationResultStatus.VALID
         elif result.status == proto.ValidationResult.ValidationResultStatus.Value(
             "INVALID"
         ):
             r_status = unified_planning.engines.ValidationResultStatus.INVALID
+        elif result.status == proto.ValidationResult.ValidationResultStatus.Value(
+            "UNKNOWN"
+        ):
+            r_status = unified_planning.engines.ValidationResultStatus.UNKNOWN
         else:
             raise UPException(f"Unexpected ValidationResult status: {result.status}")
         return unified_planning.engines.ValidationResult(
             status=r_status,
             engine_name=result.engine.name,
             log_messages=[self.convert(log) for log in result.log_messages],
         )
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/grpc/proto_writer.py` & `unified_planning-0.6.0.94.dev1/unified_planning/grpc/proto_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from unified_planning.exceptions import UPException
 from unified_planning.grpc.converter import Converter, handles
 from unified_planning.model.operators import (
     BOOL_OPERATORS,
     IRA_OPERATORS,
     RELATIONS,
     OperatorKind,
+    TRAJECTORY_CONSTRAINTS,
 )
 from unified_planning.model.timing import TimepointKind
 
 
 def map_operator(op: int) -> str:
     if op == OperatorKind.PLUS:
         return "up:plus"
@@ -63,14 +64,24 @@
         return "up:implies"
     elif op == OperatorKind.IFF:
         return "up:iff"
     elif op == OperatorKind.EXISTS:
         return "up:exists"
     elif op == OperatorKind.FORALL:
         return "up:forall"
+    elif op == OperatorKind.ALWAYS:
+        return "up:always"
+    elif op == OperatorKind.AT_MOST_ONCE:
+        return "up:at_most_once"
+    elif op == OperatorKind.SOMETIME:
+        return "up:sometime"
+    elif op == OperatorKind.SOMETIME_AFTER:
+        return "up:sometime_after"
+    elif op == OperatorKind.SOMETIME_BEFORE:
+        return "up:sometime_before"
     raise ValueError(f"Unknown operator `{op}`")
 
 
 def proto_type(tpe: model.Type) -> str:
     if tpe.is_bool_type():
         return "up:bool"
     elif tpe.is_time_type():
@@ -237,15 +248,19 @@
         return proto.Expression(
             atom=None,
             list=sub_list,
             kind=proto.ExpressionKind.Value("STATE_VARIABLE"),
             type=proto_type(expression.fluent().type),
         )
 
-    @walkers.handles(BOOL_OPERATORS.union(IRA_OPERATORS).union(RELATIONS))
+    @walkers.handles(
+        BOOL_OPERATORS.union(IRA_OPERATORS)
+        .union(RELATIONS)
+        .union(TRAJECTORY_CONSTRAINTS)
+    )
     def walk_operator(
         self, expression: model.FNode, args: List[proto.Expression]
     ) -> proto.Expression:
         sub_list = []
         sub_list.append(
             proto.Expression(
                 atom=proto.Atom(symbol=map_operator(expression.node_type)),
@@ -524,24 +539,29 @@
             abstract_tasks=[self.convert(t) for t in problem.tasks],
             methods=[self.convert(m) for m in problem.methods],
         )
 
     @handles(model.Problem, model.htn.HierarchicalProblem)
     def _convert_problem(self, problem: model.Problem) -> proto.Problem:
         goals = [proto.Goal(goal=self.convert(g)) for g in problem.goals]
-        for t, gs in problem.timed_goals:
+        for t, gs in problem.timed_goals.items():
             goals += [
                 proto.Goal(goal=self.convert(g), timing=self.convert(t)) for g in gs
             ]
 
         problem_name = str(problem.name) if problem.name is not None else ""
         hierarchy = None
         if isinstance(problem, model.htn.HierarchicalProblem):
             hierarchy = self.build_hierarchy(problem)
-
+        epsilon = None
+        if problem.epsilon is not None:
+            epsilon = proto.Real(
+                numerator=problem.epsilon.numerator,
+                denominator=problem.epsilon.denominator,
+            )
         return proto.Problem(
             domain_name=problem_name + "_domain",
             problem_name=problem_name,
             types=[self.convert(t) for t in problem.user_types],
             fluents=[self.convert(f, problem) for f in problem.fluents],
             objects=[self.convert(o) for o in problem.all_objects],
             actions=[self.convert(a) for a in problem.actions],
@@ -550,14 +570,20 @@
                 for (x, v) in problem.initial_values.items()
             ],
             timed_effects=[self.convert(e) for e in problem.timed_effects],
             goals=goals,
             features=[map_feature(feature) for feature in problem.kind.features],
             metrics=[self.convert(m) for m in problem.quality_metrics],
             hierarchy=hierarchy,
+            trajectory_constraints=[
+                self.convert(tc) for tc in problem.trajectory_constraints
+            ],
+            discrete_time=problem.discrete_time,
+            self_overlapping=problem.self_overlapping,
+            epsilon=epsilon,
         )
 
     @handles(model.metrics.MinimizeActionCosts)
     def _convert_minimize_action_costs(
         self, metric: model.metrics.MinimizeActionCosts
     ) -> proto.Metric:
         action_costs = {}
@@ -694,15 +720,16 @@
         ids: Dict[ActionInstance, str] = None,
     ) -> proto.Plan:
         action_instances = []
 
         for a in plan.timed_actions:
             id = ids.get(a[1]) if ids else None
             start_time = self.convert(a[0])
-            end_time = self.convert(a[0] + a[2])
+            duration = 0 if a[2] is None else a[2]
+            end_time = self.convert(a[0] + duration)
             instance = self._convert_action_instance(
                 a[1], start_time=start_time, end_time=end_time, id=id
             )
             action_instances.append(instance)
 
         return proto.Plan(actions=action_instances)
 
@@ -875,9 +902,11 @@
     def _convert_validation_result_status(
         self, status: unified_planning.engines.ValidationResultStatus
     ) -> proto.ValidationResult.ValidationResultStatus:
         if status == unified_planning.engines.ValidationResultStatus.VALID:
             return proto.ValidationResult.ValidationResultStatus.Value("VALID")
         elif status == unified_planning.engines.ValidationResultStatus.INVALID:
             return proto.ValidationResult.ValidationResultStatus.Value("INVALID")
+        elif status == unified_planning.engines.ValidationResultStatus.UNKNOWN:
+            return proto.ValidationResult.ValidationResultStatus.Value("UNKNOWN")
         else:
             raise UPException(f"Unknown result status: {status}")
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/interop/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/interop/from_tarski.py` & `unified_planning-0.6.0.94.dev1/unified_planning/interop/from_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/interop/to_tarski.py` & `unified_planning-0.6.0.94.dev1/unified_planning/interop/to_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/io/anml_grammar.py` & `unified_planning-0.6.0.94.dev1/unified_planning/io/anml_grammar.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/io/anml_reader.py` & `unified_planning-0.6.0.94.dev1/unified_planning/io/anml_reader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 
     #. statements containing the duration of an action are **not** mixed with other statements ( ``duration == 3 and at(l_from);`` ).
     #. the action duration can be set with:
 
         * ``duration == expression;``
         * ``duration := expression;``
         * ``duration CT expression and duration CT expression``, where ``CT`` are Compare Tokens, so ``>``, ``>=``, ``<`` and ``<=``.
-        All the other ways to define the duration of an Action are not supported.
 
+        All the other ways to define the duration of an Action are not supported.
     #. Statements containing both conditions and effects are **not** supported ( ``(at(l_from) == true) := false);`` or ``(at(l_from) == true) and (at(l_from) := false);`` ).
     #. Quantifier body does not support intervals, they can only be defined outside.
     #. Conditional effects are not supported inside an expression block.
     """
 
     def __init__(self, env: Optional[Environment] = None):
         self._env = get_environment(env)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/io/anml_writer.py` & `unified_planning-0.6.0.94.dev1/unified_planning/io/anml_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,17 @@
         for g in self.problem.goals:
             out.write(f"[ end ] {converter.convert(g)};\n")
 
         for i, gl in self.problem.timed_goals.items():
             for g in gl:
                 out.write(f"{self._convert_anml_interval(i)} {converter.convert(g)};\n")
 
+        for si in self.problem.state_invariants:
+            out.write(f"[ all ] {converter.convert(si)};\n")
+
     def print_problem(self):
         """Prints to std output the `ANML` problem."""
         self._write_problem(sys.stdout)
 
     def get_problem(self) -> str:
         """Returns the `ANML` problem."""
         out = StringIO()
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/io/ma_pddl_writer.py` & `unified_planning-0.6.0.94.dev1/unified_planning/io/ma_pddl_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/io/pddl_reader.py` & `unified_planning-0.6.0.94.dev1/unified_planning/io/pddl_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
             + set_results_name(
                 Group(ZeroOrMore(action_def | dur_action_def)), "actions"
             )
             + Suppress(")")
         )
 
         objects = set_results_name(
-            OneOrMore(Group(Group(OneOrMore(name)) + Optional(Suppress("-") + name))),
+            ZeroOrMore(Group(Group(OneOrMore(name)) + Optional(Suppress("-") + name))),
             "objects",
         )
 
         htn_def = Group(
             Suppress("(")
             + ":htn"
             - Optional(":parameters" - Suppress("(") + parameters + Suppress(")"))
@@ -306,15 +306,15 @@
                 + ":goal"
                 + set_results_name(nested_expr(), "goal")
                 + Suppress(")")
             )
             + Optional(
                 Suppress("(")
                 + ":constraints"
-                + set_results_name(nested_expr(), "constraints")
+                + set_results_name(OneOrMore(nested_expr()), "constraints")
                 + Suppress(")")
             )
             + Optional(Suppress("(") + ":metric" + metric + Suppress(")"))
             + Suppress(")")
         )
 
         domain.ignore(";" + rest_of_line)
@@ -1531,21 +1531,32 @@
                             + f"Line: {init.line_start(problem_str)}, col: {init.col_start(problem_str)}",
                         )
                     arg = self._parse_exp(
                         problem, None, types_map, {}, init[1], problem_str
                     )
                     problem.add_unknown_initial_constraint(arg)
                 else:
-                    problem.set_initial_value(
-                        self._parse_exp(
-                            problem, None, types_map, {}, init, problem_str
-                        ),
-                        self._em.TRUE(),
+                    exp = self._parse_exp(
+                        problem, None, types_map, {}, init, problem_str
                     )
-
+                    if not exp.is_not():
+                        if not exp.is_fluent_exp():
+                            raise SyntaxError(
+                                f"In init expected predicate, found {exp}\n"
+                                + f"Line: {init.line_start(problem_str)}, col: {init.col_start(problem_str)}",
+                            )
+                        problem.set_initial_value(
+                            exp,
+                            self._em.TRUE(),
+                        )
+                    elif not exp.arg(0).is_fluent_exp():
+                        raise SyntaxError(
+                            f"In init expected (not predicate), found {exp}\n"
+                            + f"Line: {init.line_start(problem_str)}, col: {init.col_start(problem_str)}",
+                        )
             if "goal" in problem_res:
                 problem.add_goal(
                     self._parse_exp(
                         problem,
                         None,
                         types_map,
                         {},
@@ -1553,24 +1564,25 @@
                         problem_str,
                     )
                 )
             elif not isinstance(problem, htn.HierarchicalProblem):
                 raise SyntaxError("Missing goal section in problem file.")
 
             if "constraints" in problem_res:
-                problem.add_trajectory_constraint(
-                    self._parse_exp(
-                        problem,
-                        None,
-                        types_map,
-                        {},
-                        CustomParseResults(problem_res["constraints"][0]),
-                        problem_str,
+                for tc in problem_res["constraints"]:
+                    problem.add_trajectory_constraint(
+                        self._parse_exp(
+                            problem,
+                            None,
+                            types_map,
+                            {},
+                            CustomParseResults(tc),
+                            problem_str,
+                        )
                     )
-                )
 
             has_actions_cost = has_actions_cost and self._problem_has_actions_cost(
                 problem
             )
             optimization = problem_res.get("optimization", None)
             m = problem_res.get("metric", None)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/io/pddl_writer.py` & `unified_planning-0.6.0.94.dev1/unified_planning/io/pddl_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,18 @@
                 or self.problem_kind.has_fluents_in_actions_cost()
             ):
                 out.write(" :numeric-fluents")
             if self.problem_kind.has_conditional_effects():
                 out.write(" :conditional-effects")
             if self.problem_kind.has_existential_conditions():
                 out.write(" :existential-preconditions")
-            if self.problem_kind.has_trajectory_constraints():
+            if (
+                self.problem_kind.has_trajectory_constraints()
+                or self.problem_kind.has_state_invariants()
+            ):
                 out.write(" :constraints")
             if self.problem_kind.has_universal_conditions():
                 out.write(" :universal-preconditions")
             if (
                 self.problem_kind.has_continuous_time()
                 or self.problem_kind.has_discrete_time()
             ):
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/io/utils.py` & `unified_planning-0.6.0.94.dev1/unified_planning/io/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/abstract_problem.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/abstract_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/action.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/contingent_problem.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/contingent_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/delta_stn.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/delta_stn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/effect.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/effect.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 This module defines the `Effect` class.
 A basic `Effect` has a `fluent` and an `expression`.
 A `condition` can be added to make it a `conditional effect`.
 """
 
 
 import unified_planning as up
-from unified_planning.exceptions import UPConflictingEffectsException
+from unified_planning.exceptions import (
+    UPConflictingEffectsException,
+    UPProblemDefinitionError,
+)
 from enum import Enum, auto
-from typing import List, Callable, Dict, Optional, Set, Tuple, Union
+from typing import List, Callable, Dict, Optional, Set, Union
 
 
 class EffectKind(Enum):
     """
     The `Enum` representing the possible `Effects` in the `unified_planning`.
 
     The semantic is the following of an `effect` with fluent `F`, value `V` and condition `C`:
@@ -50,14 +53,21 @@
     def __init__(
         self,
         fluent: "up.model.fnode.FNode",
         value: "up.model.fnode.FNode",
         condition: "up.model.fnode.FNode",
         kind: EffectKind = EffectKind.ASSIGN,
     ):
+        fve = fluent.environment.free_vars_extractor
+        fluents_in_fluent = fve.get(fluent)
+        fluents_in_fluent.remove(fluent)
+        if fluents_in_fluent:
+            raise UPProblemDefinitionError(
+                f"The fluent: {fluent} contains other fluents in his arguments: {fluents_in_fluent}"
+            )
         self._fluent = fluent
         self._value = value
         self._condition = condition
         self._kind = kind
         assert (
             fluent.environment == value.environment
             and value.environment == condition.environment
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/expression.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/expression.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/fluent.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/fluent.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 """
 This module defines the Fluent class.
 A Fluent has a name, a type and a signature
 that defines the types of its parameters.
 """
 
 import unified_planning as up
+from unified_planning.model.types import domain_size, domain_item, _IntType
 from unified_planning.environment import get_environment, Environment
-from unified_planning.model.types import domain_size, domain_item
-from typing import List, OrderedDict, Optional, Union, Iterator
+from unified_planning.exceptions import UPTypeError
+from typing import List, OrderedDict, Optional, Union, Iterator, cast
 
 
 class Fluent:
     """Represents a fluent."""
 
     def __init__(
         self,
@@ -65,14 +66,26 @@
             else:
                 raise NotImplementedError
         else:
             for param_name, param_type in kwargs.items():
                 self._signature.append(
                     up.model.parameter.Parameter(param_name, param_type, self._env)
                 )
+        for param in self._signature:
+            pt = param.type
+            if pt.is_real_type() or (
+                pt.is_int_type()
+                and (
+                    cast(_IntType, pt).lower_bound is None
+                    or cast(_IntType, pt).upper_bound is None
+                )
+            ):
+                raise UPTypeError(
+                    f"Parameter {param} of fluent {name} has type {pt}; fluents parameters must have finite domains."
+                )
 
     def __repr__(self) -> str:
         sign = ""
         if self.arity > 0:
             sign_items = [f"{p.name}={str(p.type)}" for p in self.signature]
             sign = f'[{", ".join(sign_items)}]'
         return f"{str(self.type)} {self.name}{sign}"
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/fnode.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/fnode.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/hierarchical_problem.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/hierarchical_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/method.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/method.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/ordering.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/ordering.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/task.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/task.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/task_network.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/htn/task_network.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/metrics.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/actions_set.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/actions_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/agents_set.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/agents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/fluents_set.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/fluents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/initial_state.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/initial_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         it's :func:`arity <unified_planning.model.Fluent.arity>` is `> 0`, the `fluent` parameter must be
         an `FNode` and the method :func:`~unified_planning.model.FNode.is_fluent_exp` must return `True`.
 
         :param fluent: The grounded `Fluent` of which the initial value must be set.
         :param value: The `value` assigned in the initial state to the given `fluent`.
         """
         fluent_exp, value_exp = self._env.expression_manager.auto_promote(fluent, value)
+        assert fluent_exp.is_fluent_exp(), "fluent field must be a fluent"
         if not fluent_exp.type.is_compatible(value_exp.type):
             raise UPTypeError("Initial value assignment has not compatible types!")
         self._initial_value[fluent_exp] = value_exp
 
     def initial_value(
         self, fluent: Union["up.model.fnode.FNode", "up.model.fluent.Fluent"]
     ) -> "up.model.fnode.FNode":
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/metrics.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/objects_set.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/objects_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         >>> o2 = problem.add_object("o2", cup)  # alternative syntax to create a new object and add it to the problem.
         """
         if isinstance(obj_or_name, up.model.object.Object):
             assert typename is None
             obj = obj_or_name
             assert (
                 obj.environment == self._env
-            ), "Object does not have the same environemt fo the problem"
+            ), "Object does not have the same environment fo the problem"
         else:
             assert typename is not None, "Missing type of the object"
             obj = up.model.object.Object(obj_or_name, typename, self._env)
         if self._has_name_method(obj.name):
             msg = f"Name {obj.name} already defined! Different elements of a problem can have the same name if the environment flag error_used_named is disabled."
             if self._env.error_used_name or any(
                 obj.name == o.name for o in self._objects
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/time_model.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/time_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,17 +29,19 @@
     request.
     """
 
     def __init__(
         self,
         epsilon_default: Optional[Fraction],
         discrete_time: bool,
+        self_overlapping: bool,
     ):
         self._epsilon = epsilon_default
         self._discrete_time = discrete_time
+        self._self_overlapping = self_overlapping
 
     @property
     def epsilon(self) -> Optional[Fraction]:
         """
         This parameter has meaning only in temporal problems: it defines the minimum
         amount of time that can elapse between 2 temporal events. A temporal event can
         be, for example, the start of an action, the end of an action, an intermediate
@@ -69,10 +71,23 @@
         """Returns True if the problem time is discrete, False if it is continuous."""
         return self._discrete_time
 
     @discrete_time.setter
     def discrete_time(self, new_value: bool):
         self._discrete_time = new_value
 
+    @property
+    def self_overlapping(self) -> bool:
+        """
+        The ``self_overlapping`` flag determines if 2 (or more) different instances of the same
+        action grounded with the same parameters can be running at the same time.
+        """
+        return self._self_overlapping
+
+    @self_overlapping.setter
+    def self_overlapping(self, new_value: bool):
+        self._self_overlapping = new_value
+
     def _clone_to(self, other: "TimeModelMixin"):
         other.epsilon = self._epsilon
         other.discrete_time = self._discrete_time
+        other.self_overlapping = self._self_overlapping
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/timed_conds_effs.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/timed_conds_effs.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/user_types_set.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/mixins/user_types_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/agent.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/ma_environment.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/ma_environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/ma_problem.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/multi_agent/ma_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/object.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/object.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/operators.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/operators.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/parameter.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/parameter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/problem.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     ObjectsSetMixin,
     UserTypesSetMixin,
     InitialStateMixin,
     MetricsMixin,
 )
 from unified_planning.model.expression import ConstantExpression
 from unified_planning.model.operators import OperatorKind
+from unified_planning.model.types import _IntType
 from unified_planning.exceptions import (
     UPProblemDefinitionError,
     UPTypeError,
-    UPConflictingEffectsException,
 )
 from fractions import Fraction
 from typing import Optional, List, Dict, Set, Tuple, Union, cast
 
 
 class Problem(  # type: ignore[misc]
     AbstractProblem,
@@ -60,15 +60,17 @@
         name: Optional[str] = None,
         environment: Optional["up.environment.Environment"] = None,
         *,
         initial_defaults: Dict["up.model.types.Type", "ConstantExpression"] = {},
     ):
         AbstractProblem.__init__(self, name, environment)
         UserTypesSetMixin.__init__(self, self.environment, self.has_name)
-        TimeModelMixin.__init__(self, epsilon_default=None, discrete_time=False)
+        TimeModelMixin.__init__(
+            self, epsilon_default=None, discrete_time=False, self_overlapping=False
+        )
         FluentsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name, initial_defaults
         )
         ActionsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name
         )
         ObjectsSetMixin.__init__(
@@ -91,27 +93,26 @@
         ] = {}
         self._fluents_inc_dec: Dict[
             "up.model.timing.Timing", Set["up.model.fnode.FNode"]
         ] = {}
 
     def __repr__(self) -> str:
         s = []
+        custom_str = lambda x: f"  {str(x)}\n"
         if self.name is not None:
             s.append(f"problem name = {str(self.name)}\n\n")
         if self._epsilon is not None:
             s.append(f"epsilon separation = {self._epsilon}\n\n")
         if len(self.user_types) > 0:
             s.append(f"types = {str(list(self.user_types))}\n\n")
         s.append("fluents = [\n")
-        for f in self.fluents:
-            s.append(f"  {str(f)}\n")
+        s.extend(map(custom_str, self.fluents))
         s.append("]\n\n")
         s.append("actions = [\n")
-        for a in self.actions:
-            s.append(f"  {str(a)}\n")
+        s.extend(map(custom_str, self.actions))
         s.append("]\n\n")
         if len(self.user_types) > 0:
             s.append("objects = [\n")
             for ty in self.user_types:
                 s.append(f"  {str(ty)}: {str(list(self.objects(ty)))}\n")
             s.append("]\n\n")
         s.append("initial fluents default = [\n")
@@ -135,26 +136,23 @@
             s.append("timed goals = [\n")
             for i, gl in self.timed_goals.items():
                 s.append(f"  {str(i)} :\n")
                 for g in gl:
                     s.append(f"    {str(g)}\n")
             s.append("]\n\n")
         s.append("goals = [\n")
-        for g in self.goals:
-            s.append(f"  {str(g)}\n")
+        s.extend(map(custom_str, self.goals))
         s.append("]\n\n")
         if self.trajectory_constraints:
             s.append("trajectory constraints = [\n")
-            for c in self.trajectory_constraints:
-                s.append(f"  {str(c)}\n")
+            s.extend(map(custom_str, self.trajectory_constraints))
             s.append("]\n\n")
         if len(self.quality_metrics) > 0:
             s.append("quality metrics = [\n")
-            for qm in self.quality_metrics:
-                s.append(f"  {str(qm)}\n")
+            s.extend(map(custom_str, self.quality_metrics))
             s.append("]\n\n")
         return "".join(s)
 
     def __eq__(self, oth: object) -> bool:
         if not (isinstance(oth, Problem)) or self._env != oth._env:
             return False
         if self.kind != oth.kind or self._name != oth._name:
@@ -604,14 +602,39 @@
         self._trajectory_constraints.append(constraint.simplify())
 
     def clear_trajectory_constraints(self):
         """Removes the trajectory_constraints."""
         self._trajectory_constraints = []
 
     @property
+    def state_invariants(self) -> List["up.model.fnode.FNode"]:
+        """Returns the List of ``state_invariants`` in the problem."""
+        em = self._env.expression_manager
+        state_invariants = []
+        for tc in self._trajectory_constraints:
+            if tc.is_always():
+                state_invariants.append(tc.arg(0))
+            elif tc.is_and():
+                for a in tc.args:
+                    if a.is_always():
+                        state_invariants.append(a.arg(0))
+            elif tc.is_forall() and tc.arg(0).is_always():
+                state_invariants.append(em.Forall(tc.arg(0).arg(0), *tc.variables()))
+        return state_invariants
+
+    def add_state_invariant(self, invariant: "up.model.expression.BoolExpression"):
+        """
+        Adds the given ``invariant`` to the problem's state invariants.
+        State invariants are added as ``Always`` trajectory constraints.
+
+        :param invariant: The invariant expression to add to this problem as a state invariant.
+        """
+        self.add_trajectory_constraint(self._env.expression_manager.Always(invariant))
+
+    @property
     def kind(self) -> "up.model.problem_kind.ProblemKind":
         """
         Calculates and returns the `problem kind` of this `planning problem`.
         If the `Problem` is modified, this method must be called again in order to be reliable.
 
         IMPORTANT NOTE: this property does a lot of computation, so it should be called as
         seldom as possible.
@@ -653,16 +676,19 @@
                     static_fluents,
                     simplifier,
                     linear_checker,
                 )
         if len(self._timed_goals) > 0:
             self._kind.set_time("TIMED_GOALS")
             self._kind.set_time("CONTINUOUS_TIME")
-        if len(self._trajectory_constraints) > 0:
-            self._kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
+        for tc in self._trajectory_constraints:
+            if tc.is_always():
+                self._kind.set_constraints_kind("STATE_INVARIANTS")
+            else:
+                self._kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         for goal_list in self._timed_goals.values():
             for goal in goal_list:
                 self._update_problem_kind_condition(goal, linear_checker)
         for goal in self._goals:
             self._update_problem_kind_condition(goal, linear_checker)
         if (
             not self._kind.has_continuous_numbers()
@@ -671,14 +697,18 @@
             self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
         else:
             if not self._kind.has_simple_numeric_planning():
                 self._kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         if self._kind.has_continuous_time() and self.discrete_time:
             self._kind.set_time("DISCRETE_TIME")
             self._kind.unset_time("CONTINUOUS_TIME")
+        if self._self_overlapping and (
+            self._kind.has_continuous_time() or self._kind.has_discrete_time()
+        ):
+            self._kind.set_time("SELF_OVERLAPPING")
         return self._kind
 
     def _update_problem_kind_effect(
         self,
         e: "up.model.effect.Effect",
         fluents_to_only_increase: Set["up.model.fluent.Fluent"],
         fluents_to_only_decrease: Set["up.model.fluent.Fluent"],
@@ -796,29 +826,46 @@
                 or numeric_type.upper_bound is not None
             ):
                 self._kind.set_numbers("BOUNDED_TYPES")
             if fluent not in unused_fluents:
                 self._kind.set_fluents_type("NUMERIC_FLUENTS")
         elif type.is_user_type():
             self._kind.set_fluents_type("OBJECT_FLUENTS")
-        for p in fluent.signature:
-            # TODO understant if here we need a check that the fluent is not unused
-            self._update_problem_kind_type(p.type)
+        for param in fluent.signature:
+            pt = param.type
+            self._update_problem_kind_type(pt)
+            if pt.is_bool_type():
+                self._kind.set_parameters("BOOL_FLUENT_PARAMETERS")
+            elif pt.is_int_type():
+                self._kind.set_parameters("BOUNDED_INT_FLUENT_PARAMETERS")
 
     def _update_problem_kind_action(
         self,
         action: "up.model.action.Action",
         fluents_to_only_increase: Set["up.model.fluent.Fluent"],
         fluents_to_only_decrease: Set["up.model.fluent.Fluent"],
         static_fluents: Set["up.model.fluent.Fluent"],
         simplifier: "up.model.walkers.simplifier.Simplifier",
         linear_checker: "up.model.walkers.linear_checker.LinearChecker",
     ):
-        for p in action.parameters:
-            self._update_problem_kind_type(p.type)
+        for param in action.parameters:
+            pt = param.type
+            self._update_problem_kind_type(pt)
+            if pt.is_bool_type():
+                self._kind.set_parameters("BOOL_ACTION_PARAMETERS")
+            elif pt.is_real_type():
+                self._kind.set_parameters("REAL_ACTION_PARAMETERS")
+            elif pt.is_int_type():
+                if (
+                    cast(_IntType, pt).lower_bound is None
+                    or cast(_IntType, pt).upper_bound is None
+                ):
+                    self._kind.set_parameters("UNBOUNDED_INT_ACTION_PARAMETERS")
+                else:
+                    self._kind.set_parameters("BOUNDED_INT_ACTION_PARAMETERS")
         if isinstance(action, up.model.action.SensingAction):
             self._kind.set_problem_class("CONTINGENT")
         if isinstance(action, up.model.tamp.InstantaneousMotionAction):
             if len(action.motion_constraints) > 0:
                 self._kind.set_problem_class("TAMP")
         if isinstance(action, up.model.action.InstantaneousAction):
             for c in action.preconditions:
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/problem_kind.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/problem_kind.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         "CONTINUOUS_TIME",
         "DISCRETE_TIME",
         "INTERMEDIATE_CONDITIONS_AND_EFFECTS",
         "EXTERNAL_CONDITIONS_AND_EFFECTS",
         "TIMED_EFFECTS",
         "TIMED_GOALS",
         "DURATION_INEQUALITIES",
+        "SELF_OVERLAPPING",
     ],
     "EXPRESSION_DURATION": ["STATIC_FLUENTS_IN_DURATIONS", "FLUENTS_IN_DURATIONS"],
     "NUMBERS": ["CONTINUOUS_NUMBERS", "DISCRETE_NUMBERS", "BOUNDED_TYPES"],
     "CONDITIONS_KIND": [
         "NEGATIVE_CONDITIONS",
         "DISJUNCTIVE_CONDITIONS",
         "EQUALITIES",
@@ -53,26 +54,34 @@
         "DECREASE_EFFECTS",
         "STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS",
         "STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS",
         "FLUENTS_IN_BOOLEAN_ASSIGNMENTS",
         "FLUENTS_IN_NUMERIC_ASSIGNMENTS",
     ],
     "TYPING": ["FLAT_TYPING", "HIERARCHICAL_TYPING"],
+    "PARAMETERS": [
+        "BOOL_FLUENT_PARAMETERS",
+        "BOUNDED_INT_FLUENT_PARAMETERS",
+        "BOOL_ACTION_PARAMETERS",
+        "BOUNDED_INT_ACTION_PARAMETERS",
+        "UNBOUNDED_INT_ACTION_PARAMETERS",
+        "REAL_ACTION_PARAMETERS",
+    ],
     "FLUENTS_TYPE": ["NUMERIC_FLUENTS", "OBJECT_FLUENTS"],
     "QUALITY_METRICS": [
         "ACTIONS_COST",
         "FINAL_VALUE",
         "MAKESPAN",
         "PLAN_LENGTH",
         "OVERSUBSCRIPTION",
         "TEMPORAL_OVERSUBSCRIPTION",
     ],
     "ACTIONS_COST_KIND": ["STATIC_FLUENTS_IN_ACTIONS_COST", "FLUENTS_IN_ACTIONS_COST"],
     "SIMULATED_ENTITIES": ["SIMULATED_EFFECTS"],
-    "CONSTRAINTS_KIND": ["TRAJECTORY_CONSTRAINTS"],
+    "CONSTRAINTS_KIND": ["TRAJECTORY_CONSTRAINTS", "STATE_INVARIANTS"],
     "HIERARCHICAL": [
         "METHOD_PRECONDITIONS",
         "TASK_NETWORK_CONSTRAINTS",
         "INITIAL_TASK_NETWORK_VARIABLES",
         "TASK_ORDER_TOTAL",
         "TASK_ORDER_PARTIAL",
         "TASK_ORDER_TEMPORAL",
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/activity.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/activity.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/chronicle.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/chronicle.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/scheduling_problem.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/scheduling/scheduling_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,27 +41,32 @@
     - it provides some shortcuts to deal with typical scheduling constructs (activities, resources, ...)
     """
 
     @property
     def kind(self) -> "up.model.problem_kind.ProblemKind":
         self._kind = up.model.problem_kind.ProblemKind()
         self._kind.set_problem_class("SCHEDULING")
-        # TODO: complete with ore precise kinds
+        # TODO: complete with more precise kinds
         return self._kind
 
     def __init__(
         self,
         name: Optional[str] = None,
         environment: Optional["up.environment.Environment"] = None,
         *,
         initial_defaults: Dict["up.model.types.Type", "ConstantExpression"] = {},
     ):
         AbstractProblem.__init__(self, name, environment)
         UserTypesSetMixin.__init__(self, self.environment, self.has_name)
-        TimeModelMixin.__init__(self, epsilon_default=Fraction(1), discrete_time=True)
+        TimeModelMixin.__init__(
+            self,
+            epsilon_default=Fraction(1),
+            discrete_time=True,
+            self_overlapping=False,
+        )
         FluentsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name, initial_defaults
         )
         ObjectsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name
         )
         InitialStateMixin.__init__(self, self, self, self.environment)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/state.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/action.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/objects.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/objects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/path.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/path.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/types.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/tamp/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/timing.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/timing.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/type_manager.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/type_manager.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/types.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
         return len(list(objects_set.objects(typename)))
     elif typename.is_int_type():
         typename = cast(_IntType, typename)
         lb = typename.lower_bound
         ub = typename.upper_bound
         if lb is None or ub is None:
             raise UPProblemDefinitionError("Parameter not groundable!")
-        return ub - lb
+        return ub - lb + 1
     else:
         raise UPProblemDefinitionError("Parameter not groundable!")
 
 
 def domain_item(
     objects_set: "unified_planning.model.mixins.ObjectsSetMixin",
     typename: "unified_planning.model.types.Type",
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/variable.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/variable.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/any.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/any.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/dag.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/dag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/dnf.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/fluents_substituter.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/fluents_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/free_vars.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/operators_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 
 import unified_planning.model.walkers as walkers
 from unified_planning.model.fnode import FNode
 from unified_planning.model.operators import OperatorKind
 from typing import List, Set
 
 
-class FreeVarsExtractor(walkers.dag.DagWalker):
-    """This expression walker returns all the `fluent` expression in the given expression."""
+class OperatorsExtractor(walkers.dag.DagWalker):
+    """This expression walker returns all the operators of a given expression."""
 
     def __init__(self):
         walkers.dag.DagWalker.__init__(self)
 
-    def get(self, expression: FNode) -> Set[FNode]:
+    def get(self, expression: FNode) -> Set[OperatorKind]:
         """
-        Returns all the `fluent expressions` in the given expression.
+        Returns all the operators of the given expression.
 
-        :param expression: The expression containing the `fluent expressions` to be returned.
-        :return: The set of `fluent expressions` appearing in the given expression.
+        :param expression: The target expression.
+        :return: The set containing all the operators appearing in the given expression.
         """
         return self.walk(expression)
 
     @walkers.handles(OperatorKind)
-    def walk_all_types(self, expression: FNode, args: List[Set[FNode]]) -> Set[FNode]:
-        res = set(x for y in args for x in y)
-        if expression.is_fluent_exp():
-            res = res | {expression}
-        return res
+    def walk_all_types(
+        self, expression: FNode, args: List[Set[OperatorKind]]
+    ) -> Set[OperatorKind]:
+        return set(x for y in args for x in y) | {expression.node_type}
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/generic.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 # NodeType to Function Name
 def nt_to_fun(o: OperatorKind) -> str:
     """Returns the name of the walk function for the given nodetype."""
     return "walk_%s" % (str(o).replace("OperatorKind.", "")).lower()
 
 
 class handles(object):
-    """Decorator for walker functions.
+    """
+    Decorator for walker functions.
     Use it by specifying the nodetypes that need to be handled by the
-    given function. It is possible to use groupd (e.g., OperatorKind.RELATIONS)
+    given function. It is possible to use grouped (e.g., OperatorKind.RELATIONS)
     directly. ::
-    `@handles(OperatorKind.NODE, ...)
-    def walk_special(...):
-        ...`
+
+        `@handles(OperatorKind.NODE, ...)
+        def walk_special(...):
+            ...`
 
     """
 
     def __init__(self, *nodetypes):
         if len(nodetypes) == 1 and isinstance(nodetypes[0], Iterable):
             nodetypes = nodetypes[0]  # type: ignore
         self.nodetypes = list(nodetypes)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/identitydag.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/identitydag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/linear_checker.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/linear_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/names_extractor.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/names_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/quantifier_simplifier.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/quantifier_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/simplifier.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/state_evaluator.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/state_evaluator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/substituter.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/type_checker.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/type_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/usertype_fluents_walker.py` & `unified_planning-0.6.0.94.dev1/unified_planning/model/walkers/usertype_fluents_walker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/plans/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/plans/contingent_plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/plans/contingent_plan.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import unified_planning as up
 import unified_planning.plans as plans
 from unified_planning.exceptions import UPUsageError
-from typing import Callable, Dict, Optional, List, Tuple
+from typing import Callable, Dict, Iterator, Optional, List, Set, Tuple, Deque
+from collections import deque
 
 
 class ContingentPlanNode:
     """This class represent a node in the tree representing a contingent plan."""
 
     def __init__(self, action_instance: "plans.plan.ActionInstance"):
         self._action_instance = action_instance
@@ -150,14 +151,55 @@
             return self.root_node == oth.root_node
         else:
             return False
 
     def __hash__(self) -> int:
         return hash(self.root_node)
 
+    def __str__(self) -> str:
+        if self._root_node is None:
+            return "ContingentPlan:\n  Actions:\n  Constraints:"
+        em = self.environment.expression_manager
+        nodes = list(visit_tree(self._root_node))
+        # give an ID, starting from 0, to every Node in the Plan
+        swap_couple = lambda x: (x[1], x[0])
+        id: Dict[ContingentPlanNode, int] = dict(
+            map(swap_couple, enumerate(visit_tree(self._root_node)))
+        )
+        convert_action_id = (
+            lambda action_id: f"    {action_id[1]}) {action_id[0].action_instance}"
+        )
+        ret = ["ContingentPlan:", "  Actions:"]
+        ret.extend(map(convert_action_id, id.items()))
+        ret.append("  Constraints:")
+
+        def handle_fluent(key_value):
+            fluent, value = key_value
+            ft = fluent.type
+            if ft.is_bool_type() and value.is_true():
+                return fluent
+            elif ft.is_bool_type() and value.is_false():
+                return em.Not(fluent)
+            else:
+                return em.Equals(fluent, value)
+
+        def convert_node(node):
+            node_id = id[node]
+            node_res: List[str] = []
+            for fluents, child in node.children:
+                if fluents:
+                    fluents_exp = em.And(map(handle_fluent, fluents.items()))
+                    node_res.append(f"    {node_id} -> {id[child]} if {fluents_exp}")
+                else:
+                    node_res.append(f"    {node_id} -> {id[child]}")
+            return "\n".join(node_res)
+
+        ret.extend(map(convert_node, nodes))
+        return "\n".join(ret)
+
     def __contains__(self, item: object) -> bool:
         if self.root_node is None:
             return False
         return item in self.root_node
 
     @property
     def root_node(self) -> Optional["ContingentPlanNode"]:
@@ -191,7 +233,26 @@
         :return: The plan equivalent to self but represented in the kind of
             `plan_kind`.
         """
         if plan_kind == self._kind:
             return self
         else:
             raise UPUsageError(f"{type(self)} can't be converted to {plan_kind}.")
+
+
+def visit_tree(root_node: ContingentPlanNode) -> Iterator[ContingentPlanNode]:
+    """
+    Method to visit all the Tree nodes once.
+
+    :param root_node: The starting node of the tree.
+    :return: The Iterator over all the Nodes in the tree.
+    """
+    stack: Deque[ContingentPlanNode] = deque()
+    stack.append(root_node)
+    already_visited: Set[ContingentPlanNode] = set()
+    while stack:
+        current_element: ContingentPlanNode = stack.popleft()
+        if current_element not in already_visited:
+            already_visited.add(current_element)
+            get_second_element = lambda x: x[1]
+            stack.extend(map(get_second_element, current_element.children))
+            yield current_element
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/plans/hierarchical_plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/plans/hierarchical_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,20 @@
             and self.decomposition.is_semantically_equivalent(other.decomposition)
         )
 
     def __hash__(self):
         return hash(self._flat_plan) + hash(self._decomposition)
 
     def __repr__(self):
-        return str(self.action_plan)
+        return (
+            f"# Action Plan\n{self.action_plan}\n# Decomposition\n{self.decomposition}"
+        )
+
+    def __str__(self) -> str:
+        return "Hiearchical " + str(self.action_plan)
 
     @property
     def decomposition(self) -> Decomposition:
         """The decomposition of the initial task network."""
         return self._decomposition
 
     @property
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/plans/partial_order_plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/plans/partial_order_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,15 +83,45 @@
                             "The environment given to the plan is not the same of the actions in the plan."
                         )
             self._graph = nx.convert.from_dict_of_lists(
                 adjacency_list, create_using=nx.DiGraph
             )
 
     def __repr__(self) -> str:
-        return str(self._graph)
+        return f"PartialOrderPlan({repr(self.get_adjacency_list)})"
+
+    def __str__(self) -> str:
+        ret = ["PartialOrderPlan:", "  actions:"]
+
+        # give an ID, starting from 0, to every ActionInstance in the Plan
+        swap_couple = lambda x: (x[1], x[0])
+        id: Dict[ActionInstance, int] = dict(
+            map(swap_couple, enumerate(nx.topological_sort(self._graph)))
+        )
+        convert_action_id = lambda action_id: f"    {action_id[1]}) {action_id[0]}"
+        ret.extend(map(convert_action_id, id.items()))
+
+        ret.append("  constraints:")
+        adj_list = self.get_adjacency_list
+
+        def convert_action_adjlist(action_adjlist):
+            action = action_adjlist[0]
+            adj_list = action_adjlist[1]
+            get_id_as_str = lambda ai: str(id[ai])
+            adj_list_str = " ,".join(map(get_id_as_str, adj_list))
+            return f"    {id[action]} < {adj_list_str}"
+
+        ret.extend(
+            map(
+                convert_action_adjlist,
+                ((act, adj) for act, adj in adj_list.items() if adj),
+            )
+        )
+
+        return "\n".join(ret)
 
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, PartialOrderPlan):
             return nx.is_isomorphic(
                 self._graph,
                 oth._graph,
                 node_match=_semantically_equivalent_action_instances,
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/plans/plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/plans/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 
 
 import unified_planning as up
 from unified_planning.environment import Environment, get_environment
 from unified_planning.model import AbstractProblem
 from abc import ABC, abstractmethod
-from typing import Callable, Optional, Tuple, Dict
+from typing import Callable, Optional, Sequence, Tuple, Dict
 from enum import Enum, auto
 
 
 """This module defines the general `Plan` interface and the `ActionInstance` class."""
 
 
 class ActionInstance:
@@ -32,24 +32,25 @@
     NOTE: two action instances of the same action with the same parameters are
     considered different as it is possible to have the same action twice in a `Plan`.
     """
 
     def __init__(
         self,
         action: "up.model.Action",
-        params: Tuple["up.model.FNode", ...] = tuple(),
+        params: Sequence["up.model.Expression"] = tuple(),
         agent: Optional["up.model.multi_agent.Agent"] = None,
         motion_paths: Optional[
             Dict["up.model.tamp.MotionConstraint", "up.model.tamp.Path"]
         ] = None,
     ):
-        assert len(action.parameters) == len(params)
+        auto_promote = action.environment.expression_manager.auto_promote
         self._agent = agent
         self._action = action
-        self._params = tuple(params)
+        self._params = tuple(auto_promote(params))
+        assert len(action.parameters) == len(self._params)
         self._motion_paths = motion_paths
 
     def __repr__(self) -> str:
         s = []
         if len(self._params) > 0:
             s.append("(")
             first = True
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/plans/sequential_plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/plans/sequential_plan.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,22 @@
         ):  # check that given environment and the environment in the actions is the same
             if ai.action.environment != self._environment:
                 raise UPUsageError(
                     "The environment given to the plan is not the same of the actions in the plan."
                 )
         self._actions = actions
 
+    def __str__(self) -> str:
+        ret = ["SequentialPlan:"]
+        convert_ai = lambda ai: f"    {ai}"
+        ret.extend(map(convert_ai, self._actions))
+        return "\n".join(ret)
+
     def __repr__(self) -> str:
-        return str(self._actions)
+        return f"SequentialPlan({self._actions})"
 
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, SequentialPlan) and len(self._actions) == len(oth._actions):
             for ai, oth_ai in zip(self._actions, oth._actions):
                 if not ai.is_semantically_equivalent(oth_ai):
                     return False
             return True
@@ -89,15 +95,15 @@
             ["plans.plan.ActionInstance"], Optional["plans.plan.ActionInstance"]
         ],
     ) -> "up.plans.plan.Plan":
         """
         Returns a new `SequentialPlan` where every `ActionInstance` of the current `Plan` is replaced using the given function.
 
         :param replace_function: The function that applied to an `ActionInstance A` returns the `ActionInstance B`; `B`
-        replaces `A` in the resulting `SequentialPlan`.
+            replaces `A` in the resulting `SequentialPlan`.
         :return: The `SequentialPlan` where every `ActionInstance` is replaced using the given `replace_function`.
         """
         new_ai = []
         for ai in self._actions:
             replaced_ai = replace_function(ai)
             if replaced_ai is not None:
                 new_ai.append(replaced_ai)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/plans/stn_plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/plans/stn_plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     Dict,
     Iterator,
     List,
     Optional,
     Set,
     Tuple,
     Union,
+    cast,
 )
 
 
 @dataclass(unsafe_hash=True, frozen=True)
 class STNPlanNode:
     """
     This class represents a node of the `STNPlan`.
@@ -99,14 +100,15 @@
 
     :param d: The dictionary to flatten.
     """
     for k, v in d.items():
         if not v:
             yield (k, None, None, k)
         for tup in v:
+            assert len(tup) == 3, str(tup)
             yield (k, *tup)
 
 
 class STNPlan(plans.plan.Plan):
     """
     Represents a `STNPlan`. A Simple Temporal Network plan is a generalization of
     a `TimeTriggeredPlan`, where the only constraints are among the start and the
@@ -225,14 +227,48 @@
             lb = None if lower_bound is None else Fraction(float(lower_bound))
             ub = None if upper_bound is None else Fraction(float(upper_bound))
             self._stn.insert_interval(a_node, b_node, left_bound=lb, right_bound=ub)
 
     def __repr__(self) -> str:
         return str(self._stn)
 
+    def __str__(self) -> str:
+        # give an ID, starting from 0, to every STNPlanNode in the Plan
+        swap_couple = lambda x: (x[1], x[0])
+        id: Dict[STNPlanNode, int] = dict(
+            map(swap_couple, enumerate(self._stn.distances.keys()))
+        )
+        convert_action_id = lambda action_id: f"    {action_id[1]}) {action_id[0]}"
+        ret = ["STNPlan:", "  Actions:"]
+        ret.extend(map(convert_action_id, id.items()))
+        ret.append("  Constraints:")
+
+        def convert_constraint(constraint):
+            left_element, lower_bound, upper_bound, right_element = constraint
+            if lower_bound is None:
+                str_lower_bound = "-inf"
+            elif lower_bound.denominator == 1:
+                str_lower_bound = str(lower_bound.numerator)
+            else:
+                str_lower_bound = str(float(lower_bound))
+            if upper_bound is None:
+                str_upper_bound = "+inf"
+            elif upper_bound.denominator == 1:
+                str_upper_bound = str(upper_bound.numerator)
+            else:
+                str_upper_bound = str(float(upper_bound))
+            return f"    {id[left_element]} --[{str_lower_bound}, {str_upper_bound}]--> {id[right_element]}"
+
+        constraints = cast(
+            Dict[STNPlanNode, List[Tuple[Optional[Real], Optional[Real], STNPlanNode]]],
+            self.get_constraints(),
+        )
+        ret.extend(map(convert_constraint, flatten_dict_structure(constraints)))
+        return "\n".join(ret)
+
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, STNPlan):
             self_contraints = self.get_constraints()
             oth_constraints = oth.get_constraints()
             if len(self_contraints) != len(oth_constraints):
                 return False
             for k, self_cl in self_contraints.items():
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/plans/time_triggered_plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/plans/time_triggered_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,27 @@
             if ai.action.environment != self._environment:
                 raise UPUsageError(
                     "The environment given to the plan is not the same of the actions in the plan."
                 )
         self._actions = actions
 
     def __repr__(self) -> str:
-        return str(self._actions)
+        return f"TimeTriggeredPlan({self._actions})"
+
+    def __str__(self) -> str:
+        def convert_ai(start_ai_dur):
+            start, ai, dur = start_ai_dur
+            if dur is None:
+                return f"    {float(start)}: {ai}"
+            else:
+                return f"    {float(start)}: {ai}: {float(dur)}"
+
+        ret = ["TimeTriggeredPlan:"]
+        ret.extend(map(convert_ai, sorted(self._actions)))
+        return "\n".join(ret)
 
     def __eq__(self, oth: object) -> bool:
         if isinstance(oth, TimeTriggeredPlan) and len(self._actions) == len(
             oth._actions
         ):
             for (s, ai, d), (oth_s, oth_ai, oth_d) in zip(self._actions, oth._actions):
                 if (
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/shortcuts.py` & `unified_planning-0.6.0.94.dev1/unified_planning/shortcuts.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 from unified_planning.model import *
 from unified_planning.model.tamp import *
 from unified_planning.engines import (
     Engine,
     CompilationKind,
     OptimalityGuarantee,
     OperationMode,
+    AnytimeGuarantee,
 )
 from unified_planning.plans import PlanKind
-from typing import IO, Any, Iterable, Union, Dict, Optional, Sequence
+from typing import IO, Any, Iterable, Union, Dict, Optional, Sequence, List
 from fractions import Fraction
 
 
 def And(*args: Union[BoolExpression, Iterable[BoolExpression]]) -> FNode:
     """
     | Returns a conjunction of terms.
     | This function has polymorphic n-arguments:
@@ -738,13 +739,80 @@
         name=name,
         params=params,
         problem_kind=problem_kind,
         optimality_guarantee=optimality_guarantee,
     )
 
 
-def print_engines_info(stream: IO[str] = sys.stdout, full_credits: bool = False):
-    get_environment().factory.print_engines_info(stream, full_credits)
+def get_all_applicable_engines(
+    problem_kind: ProblemKind,
+    operation_mode: OperationMode = OperationMode.ONESHOT_PLANNER,
+    *,
+    optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
+    anytime_guarantee: Optional[Union["AnytimeGuarantee", str]] = None,
+    plan_kind: Optional[Union["PlanKind", str]] = None,
+    compilation_kind: Optional[Union["CompilationKind", str]] = None,
+) -> List[str]:
+    """
+    | Returns all the engine names installed that are able to handle all the given
+        requirements.
+
+    | Since the semantic of the parameters given to this function depends on the chosen ``OperationMode``,
+        an user must have clear their meaning in the Operation Mode context.
+
+    :param problem_kind: An engine is returned only if it supports this ``problem_kind``.
+    :param operation_mode: An engine is returned only if it implements this ``operation_mode``; defaults to ``ONESHOT_PLANNER``.
+    :param optimality_guarantee: An engine is returned only if it satisfies this ``optimality_guarantee``. This parameter
+        can be specified only if the ``operation_mode`` is ``ONESHOT_PLANNER``, ``REPLANNER``, ``PLAN_REPAIRER``
+        or ``PORTFOLIO_SELECTOR``.
+    :param anytime_guarantee: An engine is returned only if it satisfies this ``anytime_guarantee``. This parameter
+        can be specified only if the ``operation_mode`` is ``ANYTIME_PLANNER``.
+    :param plan_kind: An engine is returned only if it is able to handle this ``plan_kind``. This parameter
+        can be specified only if the ``operation_mode`` is ``PLAN_VALIDATOR`` or ``PLAN_REPAIRER``.
+    :param compilation_kind: An engine is returned only if it is able to handle this ``compilation_kind``. This
+        parameter can be specified only if the ``operation_mode`` is ``COMPILER``.
+    :return: The list of engines names that satisfy all the given requirements.
+    """
+    return get_environment().factory.get_all_applicable_engines(
+        problem_kind,
+        operation_mode,
+        optimality_guarantee=optimality_guarantee,
+        anytime_guarantee=anytime_guarantee,
+        plan_kind=plan_kind,
+        compilation_kind=compilation_kind,
+    )
+
+
+def print_engines_info(
+    stream: IO[str] = sys.stdout,
+    *,
+    operation_mode: Optional[Union[OperationMode, str]] = None,
+    show_supported_kind: bool = True,
+    show_credits: bool = False,
+    full_credits: bool = True,
+):
+    """
+    Writes the info of all the installed engines in the given stream; the
+    default stream is the stdout.
+
+    :param stream: The ``IO[str]`` where all the engine's info are written;
+        defaults to sys.stdout.
+    :param operation_mode: If specified, writes info about the engines that support
+        that OperationMode.
+    :param show_supported_kind: If ``True`` writes the supported_kind of the engines.
+        defaults to ``True``.
+    :param show_credits: If ``True`` writes the credits of the engines.
+        defaults to ``False``.
+    :param full_credits: If ``True`` writes a longer version of the credits; ignored
+        if ``show_credits`` is ``False``; defaults to ``True``.
+    """
+    get_environment().factory.print_engines_info(
+        stream,
+        operation_mode=operation_mode,
+        show_supported_kind=show_supported_kind,
+        show_credits=show_credits,
+        full_credits=full_credits,
+    )
 
 
 def set_credits_stream(stream: Optional[IO[str]]):
     get_environment().credits_stream = stream
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/connected_locations.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/connected_locations.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/constants.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/constants.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/constants_no_variable_duration.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/constants_no_variable_duration.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/forall.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/forall.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/hydrone.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/hydrone.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match_int_id.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match_int_id.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match_test_parser.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/match_test_parser.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/simple_mais.anml` & `unified_planning-0.6.0.94.dev1/unified_planning/test/anml/simple_mais.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/__init__.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/hierarchical.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/hierarchical.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/minimals.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/minimals.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/multi_agent.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/realistic.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/realistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -882,14 +882,21 @@
                 Fraction(10, 1),
             ),
         ]
     )
     robot_static_fluents_duration = Example(problem=problem, plan=t_plan)
     problems["robot_with_static_fluents_duration"] = robot_static_fluents_duration
 
+    # Robot with timed_goals (extension of the previous problem with timed goals)
+    problem = problem.clone()
+    name = "robot_with_static_fluents_duration_timed_goals"
+    problem.name = name
+    problem.add_timed_goal(GlobalStartTiming() + 50, is_at(l5, r1))
+    problems[name] = Example(problem=problem, plan=t_plan)
+
     # travel
     problem = Problem("travel")
 
     Location = UserType("Location")
 
     is_at = Fluent("is_at", BoolType(), position=Location)
     is_connected = Fluent("is_connected", BoolType(), l_from=Location, l_to=Location)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/tamp.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/testing_variants.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/examples/testing_variants.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,87 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from itertools import product
 import unified_planning
 from unified_planning.shortcuts import *
 from collections import namedtuple
 
 Example = namedtuple("Example", ["problem", "plan"])
 
 
 def get_example_problems():
     problems = {}
 
+    # basic_bool_fluent_param
+    x = Fluent("x", int_param=BoolType())
+    a = InstantaneousAction("a")
+    a.add_precondition(Not(x(True)))
+    a.add_effect(x(True), True)
+    problem = Problem("basic_bool_fluent_param")
+    problem.add_fluent(x, default_initial_value=False)
+    problem.add_action(a)
+    problem.set_initial_value(x(False), True)
+    problem.add_goal(And(x(True), x(False)))
+    plan = up.plans.SequentialPlan([up.plans.ActionInstance(a)])
+    basic_bool_fluent_param = Example(problem=problem, plan=plan)
+    problems["basic_bool_fluent_param"] = basic_bool_fluent_param
+
+    # basic_int_fluent_param
+    int_3_6 = IntType(3, 6)
+    x = Fluent("x", int_param=int_3_6)
+    a = InstantaneousAction("a")
+    a.add_precondition(Not(x(3)))
+    a.add_effect(x(3), True)
+    problem = Problem("basic_int_fluent_param")
+    problem.add_fluent(x, default_initial_value=False)
+    problem.add_action(a)
+    problem.set_initial_value(x(4), True)
+    problem.add_goal(And(x(3), x(4), Not(x(5))))
+    plan = up.plans.SequentialPlan([up.plans.ActionInstance(a)])
+    basic_int_fluent_param = Example(problem=problem, plan=plan)
+    problems["basic_int_fluent_param"] = basic_int_fluent_param
+
+    # basic_bounded_int_action_param
+    int_3_6 = IntType(3, 6)
+    x = Fluent("x", int_param=int_3_6)
+    a = InstantaneousAction("a", int_param=int_3_6)
+    a.add_precondition(Not(x(a.int_param)))
+    a.add_effect(x(a.int_param), True)
+    problem = Problem("basic_bounded_int_action_param")
+    problem.add_fluent(x, default_initial_value=False)
+    problem.add_action(a)
+    problem.add_goal(And(x(3), x(4), Not(x(5))))
+    plan = up.plans.SequentialPlan(
+        [up.plans.ActionInstance(a, (Int(3),)), up.plans.ActionInstance(a, (Int(4),))]
+    )
+    basic_bounded_int_action_param = Example(problem=problem, plan=plan)
+    problems["basic_bounded_int_action_param"] = basic_bounded_int_action_param
+
+    # basic_unbounded_int_action_param
+    int_3_6 = IntType(3, 6)
+    int_3 = IntType(3)
+    x = Fluent("x", int_param=int_3_6)
+    a = InstantaneousAction("a", int_param=int_3)
+    a.add_precondition(Not(x(a.int_param)))
+    a.add_effect(x(a.int_param), True)
+    problem = Problem("basic_unbounded_int_action_param")
+    problem.add_fluent(x, default_initial_value=False)
+    problem.add_action(a)
+    problem.add_goal(And(x(3), x(4), Not(x(5))))
+    plan = up.plans.SequentialPlan(
+        [up.plans.ActionInstance(a, (Int(3),)), up.plans.ActionInstance(a, (Int(4),))]
+    )
+    basic_unbounded_int_action_param = Example(problem=problem, plan=plan)
+    problems["basic_unbounded_int_action_param"] = basic_unbounded_int_action_param
+
     # robot_real_constants
     # this version of the problem robot has reals instead of integers as constants
     Location = UserType("Location")
     robot_at = Fluent("robot_at", BoolType(), position=Location)
     battery_charge = Fluent("battery_charge", RealType(0, 100))
     move = InstantaneousAction("move", l_from=Location, l_to=Location)
     l_from = move.parameter("l_from")
@@ -203,14 +266,101 @@
         ]
     )
     robot_locations_connected_without_battery = Example(problem=problem, plan=plan)
     problems[
         "robot_locations_connected_without_battery"
     ] = robot_locations_connected_without_battery
 
+    # robot_loader_weak_bridge
+    # version of robot loader with weak bridges that can't be crossed with
+    # the cargo loaded. Uses global_constraints.
+    Location = UserType("Location")
+    locations = [Object(f"l{i}", Location) for i in range(1, 4)]
+    l1, l2, l3 = locations
+    robot_is_at = Fluent("robot_is_at", BoolType(), position=Location)
+    robot_was_at = Fluent("robot_was_at", BoolType(), past_position=Location)
+    cargo_at = Fluent("cargo_at", BoolType(), position=Location)
+    cargo_mounted = Fluent("cargo_mounted")
+    weak_bridge = Fluent("weak_bridge", BoolType(), l_from=Location, l_to=Location)
+
+    move = InstantaneousAction("move", l_from=Location, l_to=Location)
+    l_from = move.parameter("l_from")
+    l_to = move.parameter("l_to")
+    move.add_precondition(Not(Equals(l_from, l_to)))
+    move.add_precondition(robot_is_at(l_from))
+    move.add_precondition(Not(robot_is_at(l_to)))
+    move.add_effect(robot_is_at(l_from), False)
+    move.add_effect(robot_is_at(l_to), True)
+    move.add_effect(robot_was_at(l_from), True)
+    for l_obj in locations:  # note that this works for the add-after-delete semantic
+        move.add_effect(robot_was_at(l_obj), False)
+
+    load = InstantaneousAction("load", loc=Location)
+    loc = load.parameter("loc")
+    load.add_precondition(cargo_at(loc))
+    load.add_precondition(robot_is_at(loc))
+    load.add_precondition(Not(cargo_mounted))
+    load.add_effect(cargo_at(loc), False)
+    load.add_effect(cargo_mounted, True)
+    load.add_effect(robot_was_at(loc), True)
+    for l_obj in locations:
+        load.add_effect(robot_was_at(l_obj), False)
+
+    unload = InstantaneousAction("unload", loc=Location)
+    loc = unload.parameter("loc")
+    unload.add_precondition(Not(cargo_at(loc)))
+    unload.add_precondition(robot_is_at(loc))
+    unload.add_precondition(cargo_mounted)
+    unload.add_effect(cargo_at(loc), True)
+    unload.add_effect(cargo_mounted, False)
+    unload.add_effect(robot_was_at(loc), True)
+    for l_obj in locations:
+        unload.add_effect(robot_was_at(l_obj), False)
+
+    problem = Problem("robot_loader_weak_bridge")
+    problem.add_fluent(robot_is_at, default_initial_value=False)
+    problem.add_fluent(robot_was_at, default_initial_value=False)
+    problem.add_fluent(cargo_at, default_initial_value=False)
+    problem.add_fluent(cargo_mounted, default_initial_value=False)
+    problem.add_fluent(weak_bridge, default_initial_value=False)
+    problem.add_action(move)
+    problem.add_action(load)
+    problem.add_action(unload)
+    problem.add_objects(locations)
+    problem.set_initial_value(robot_is_at(l1), True)
+    problem.set_initial_value(robot_was_at(l1), True)
+    problem.set_initial_value(cargo_at(l3), True)
+    problem.set_initial_value(weak_bridge(l3, l1), True)
+    problem.set_initial_value(weak_bridge(l1, l3), True)
+    problem.add_goal(cargo_at(l1))
+    # for all the possible couples of locations, it must never be True that:
+    # The robot is loaded when crossing a weak bridge.
+    for l_from_v, l_to_v in product(locations, repeat=2):
+        problem.add_state_invariant(
+            Not(
+                And(
+                    weak_bridge(l_from_v, l_to_v),
+                    robot_was_at(l_from_v),
+                    robot_is_at(l_to_v),
+                    cargo_mounted,
+                )
+            )
+        )
+    plan = up.plans.SequentialPlan(
+        [
+            up.plans.ActionInstance(move, (ObjectExp(l1), ObjectExp(l3))),
+            up.plans.ActionInstance(load, (ObjectExp(l3),)),
+            up.plans.ActionInstance(move, (ObjectExp(l3), ObjectExp(l2))),
+            up.plans.ActionInstance(move, (ObjectExp(l2), ObjectExp(l1))),
+            up.plans.ActionInstance(unload, (ObjectExp(l1),)),
+        ]
+    )
+    robot_loader_weak_bridge = Example(problem=problem, plan=plan)
+    problems["robot_loader_weak_bridge"] = robot_loader_weak_bridge
+
     # hierarchical blocks world exists
     Entity = UserType("Entity", None)  # None can be avoided
     Location = UserType("Location", Entity)
     Unmovable = UserType("Unmovable", Location)
     TableSpace = UserType("TableSpace", Unmovable)
     Movable = UserType("Movable", Location)
     Block = UserType("Block", Movable)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/problem.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/citycar/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/problem2.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/counters/problem2.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/problem.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/depot/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/enhsp.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/enhsp.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import unified_planning as up
-import unified_planning.engines
-from unified_planning.model.problem_kind import ProblemKind
-from unified_planning.engines import PlanGenerationResult, PlanGenerationResultStatus
+from unified_planning.model import ProblemKind
+from unified_planning.engines import (
+    PlanGenerationResult,
+    PlanGenerationResultStatus,
+    PDDLAnytimePlanner,
+)
+from unified_planning.engines.pddl_anytime_planner import Writer
 from unified_planning.environment import get_environment
-from typing import List, Optional, Union, IO, Iterator
+from unified_planning.io import PDDLWriter
+from typing import List, Optional
 
 
 FILE_PATH = os.path.dirname(os.path.abspath(__file__))
 
 
-class ENHSP(up.engines.PDDLPlanner, up.engines.mixins.AnytimePlannerMixin):
+class ENHSP(PDDLAnytimePlanner):
     def __init__(self):
-        up.engines.PDDLPlanner.__init__(self, False, True)
-        self._options = ["-planner", "opt-hrmax"]
+        PDDLAnytimePlanner.__init__(self, False, True)
 
     @property
     def name(self) -> str:
         return "ENHSP"
 
     def _get_cmd(
         self, domanin_filename: str, problem_filename: str, plan_filename: str
@@ -44,15 +48,39 @@
             ),
             "-o",
             domanin_filename,
             "-f",
             problem_filename,
             "-sp",
             plan_filename,
-        ] + self._options
+            "-planner",
+            "opt-hrmax",
+        ]
+
+    def _get_anytime_cmd(
+        self, domanin_filename: str, problem_filename: str, plan_filename: str
+    ) -> List[str]:
+        return [
+            "java",
+            "-jar",
+            os.path.join(
+                FILE_PATH, "..", "..", "..", ".planners", "enhsp-20", "enhsp.jar"
+            ),
+            "-o",
+            domanin_filename,
+            "-f",
+            problem_filename,
+            "-sp",
+            plan_filename,
+            "-h",
+            "hadd",
+            "-s",
+            "gbfs",
+            "-anytime",
+        ]
 
     def _result_status(
         self,
         problem: "up.model.Problem",
         plan: Optional["up.plans.Plan"],
         retval: int,
         log_messages: Optional[List["up.engines.LogMessage"]] = None,
@@ -60,89 +88,22 @@
         if retval != 0:
             return up.engines.results.PlanGenerationResultStatus.INTERNAL_ERROR
         elif plan is None:
             return up.engines.results.PlanGenerationResultStatus.UNSOLVABLE_PROVEN
         else:
             return up.engines.results.PlanGenerationResultStatus.SOLVED_OPTIMALLY
 
-    def _get_solutions(
-        self,
-        problem: "up.model.AbstractProblem",
-        timeout: Optional[float] = None,
-        output_stream: Optional[IO[str]] = None,
-    ) -> Iterator["up.engines.results.PlanGenerationResult"]:
-        import threading
-        import queue
-
-        opts = self._options
-
-        self._options = [
-            "-h",
-            "hadd",
-            "-s",
-            "gbfs",
-            "-anytime",
-        ]
-
-        if timeout is not None:
-            self._options.extend(["-timeout", str(timeout)])
+    def _starting_plan_str(self) -> str:
+        return "Found Plan:"
 
-        q: queue.Queue = queue.Queue()
+    def _ending_plan_str(self) -> str:
+        return "Plan-Length:"
 
-        class Writer(up.AnyBaseClass):
-            def __init__(self, os, q, engine):
-                self._os = os
-                self._q = q
-                self._engine = engine
-                self._plan = []
-                self._storing = False
-
-            def write(self, txt: str):
-                if self._os is not None:
-                    self._os.write(txt)
-                for l in txt.splitlines():
-                    if "Found Plan:" in l:
-                        self._storing = True
-                    elif "Plan-Length:" in l:
-                        plan_str = "\n".join(self._plan)
-                        plan = self._engine._plan_from_str(
-                            problem, plan_str, self._engine._writer.get_item_named
-                        )
-                        res = PlanGenerationResult(
-                            PlanGenerationResultStatus.INTERMEDIATE,
-                            plan=plan,
-                            engine_name=self._engine.name,
-                        )
-                        self._q.put(res)
-                        self._plan = []
-                        self._storing = False
-                    elif self._storing and l:
-                        self._plan.append(l.split(":")[1])
-
-        def run():
-            writer: IO[str] = Writer(output_stream, q, self)
-            res = self._solve(problem, output_stream=writer)
-            q.put(res)
-
-        try:
-            t = threading.Thread(target=run, daemon=True)
-            t.start()
-            status = PlanGenerationResultStatus.INTERMEDIATE
-            while status == PlanGenerationResultStatus.INTERMEDIATE:
-                res = q.get()
-                status = res.status
-                yield res
-        finally:
-            if self._process is not None:
-                try:
-                    self._process.kill()
-                except OSError:
-                    pass  # This can happen if the process is already terminated
-            t.join()
-            self._options = opts
+    def _parse_plan_line(self, plan_line: str) -> str:
+        return plan_line.split(":")[1]
 
     @staticmethod
     def satisfies(optimality_guarantee: up.engines.OptimalityGuarantee) -> bool:
         return True
 
     @staticmethod
     def ensures(anytime_guarantee: up.engines.AnytimeGuarantee) -> bool:
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/domain.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/problem.hddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/htn-transport/problem.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/matchcellar/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/matchcellar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/miconic/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/miconic/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/safe_road/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/safe_road/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/sailing/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/sailing/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl` & `unified_planning-0.6.0.94.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/examples.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/examples.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/jobshop.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/scheduling/jobshop.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_anml_reader.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_anml_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_anml_writer.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_anytime.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_anytime.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_bounded_types_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_compilers_pipeline.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_compilers_quality_metrics.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_compilers_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_conditional_effects_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_contingent_pddl.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_contingent_pddl.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_credits.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_credits.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             "  * Engine name: ",
             "  * Developers:  ",
             "  * Description: ",
             "  * Contacts:    ",
             "  * Website:     ",
             "  * License:     ",
         ]
-        get_environment().factory.print_engines_info(credits, True)
+        get_environment().factory.print_engines_info(credits, show_credits=True)
         credits_printed = credits.getvalue()
         # test that every keyword occur the same number of time in the printed result
         number_of_credits_printed = credits_printed.count(credits_keywords[0])
         if number_of_credits_printed > 0:  # If at least one credit was printed
             for keyword in credits_keywords:
                 self.assertIn(keyword, credits_printed)
                 self.assertEqual(
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_disjunctive_conditions_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_dnf.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_expression_analysis.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_expression_analysis.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_factory.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,25 +12,50 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import inspect
 import tempfile
 import unified_planning
+from unified_planning.test.examples import get_example_problems
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase, skipIfEngineNotAvailable
 
 
 class TestFactory(TestCase):
+    def setUp(self):
+        TestCase.setUp(self)
+        self.problems = get_example_problems()
+
     @skipIfEngineNotAvailable("pyperplan")
     @skipIfEngineNotAvailable("tamer")
     def test_config_file(self):
         self.assertTrue("pyperplan" in get_environment().factory.preference_list)
         with tempfile.TemporaryDirectory() as tempdir:
             config_filename = os.path.join(tempdir, "up.ini")
             with open(config_filename, "w") as config:
                 config.write("[global]\n")
                 config.write("engine_preference_list: tamer\n")
             environment = unified_planning.environment.Environment()
             environment.factory.configure_from_file(config_filename)
             self.assertTrue("pyperplan" not in environment.factory.preference_list)
             self.assertEqual(environment.factory.preference_list, ["tamer"])
+
+    @skipIfEngineNotAvailable("pyperplan")
+    @skipIfEngineNotAvailable("tamer")
+    @skipIfEngineNotAvailable("opt-pddl-planner")
+    def test_get_all_applicable_engines(self):
+        problem = self.problems["basic"].problem
+        factory = problem.environment.factory
+        names = factory.get_all_applicable_engines(problem.kind)
+        expected_names = ["tamer", "opt-pddl-planner"]
+        for name in expected_names:
+            self.assertIn(name, names)
+
+        problem = self.problems["basic_without_negative_preconditions"].problem
+        names = factory.get_all_applicable_engines(problem.kind)
+        expected_names = ["tamer", "opt-pddl-planner", "pyperplan"]
+        for name in expected_names:
+            self.assertIn(name, names)
+
+        global_env_names = get_all_applicable_engines(problem.kind)
+        self.assertEqual(global_env_names, names)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_grounder.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_htn.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_htn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_infix_notation.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_infix_notation.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         b_3 = Parameter("b_3", BoolType(), environment)
         self._test_helper_function(i_1, r_1, i_2, r_2, b_1, b_2, b_3)
 
     def test_infix_on_objects(self):
         ut = UserType("ut")
         o_1 = Object("o_1", ut)
         o_2 = Object("o_2", ut)
-        f_i = Fluent("f_i", ut, id=IntType())
+        f_i = Fluent("f_i", ut, id=IntType(1, 5))
         f_o = Fluent("f_o", ut)
         expressions: List[Tuple[FNode, FNode]] = [
             (Equals(o_1, o_2), o_1.Equals(o_2)),
             (Equals(o_1, f_i(1)), o_1.Equals(f_i(1))),
             (Equals(o_1, f_o), o_1.Equals(f_o)),
         ]
         for exp, tested_exp in expressions:
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_model.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     def setUp(self):
         TestCase.setUp(self)
         self.problems = get_example_problems()
 
     def test_expression(self):
         test_type = UserType("test_type")
         identity = Fluent("identity", test_type, obj=test_type)
-        id = Fluent("id", test_type, obj_id=IntType())
+        id = Fluent("id", test_type, obj_id=IntType(0, 10))
         self.assertEqual(id(1).type, test_type)
         env_2 = up.environment.Environment()
         test_type_2 = env_2.type_manager.UserType("test_type")
-        it_2 = env_2.type_manager.IntType()
+        it_2 = env_2.type_manager.IntType(0, 10)
         id_2 = Fluent("id", test_type_2, obj_id=it_2, environment=env_2)
         obj_2 = Object("obj", test_type_2, env_2)
         self.assertEqual(id_2(1).type, test_type_2)
         self.assertNotEqual(id_2(1).type, test_type)
         with self.assertRaises(AssertionError) as e:
             Equals(id_2(1), obj_2)
         self.assertEqual(
@@ -386,7 +386,12 @@
                     Int(10),
                     TRUE(),
                     unified_planning.model.EffectKind.INCREASE,
                 )
             ),
             str(problem),
         )
+
+    def test_parameters(self):
+        int_5 = IntType(5)
+        with self.assertRaises(UPTypeError):
+            Fluent("x", p1=int_5)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_multi_agent.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_negative_conditions_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_partial_order_plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_pddl_io.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_pddl_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,14 +471,21 @@
         for example in self.problems.values():
             problem = example.problem
             kind = problem.kind
             if (
                 kind.has_intermediate_conditions_and_effects()
                 or kind.has_object_fluents()
                 or kind.has_oversubscription()
+                or kind.has_timed_goals()
+                or kind.has_bool_fluent_parameters()
+                or kind.has_bounded_int_fluent_parameters()
+                or kind.has_bool_action_parameters()
+                or kind.has_bounded_int_action_parameters()
+                or kind.has_unbounded_int_action_parameters()
+                or kind.has_real_action_parameters()
             ):
                 continue
             with tempfile.TemporaryDirectory() as tempdir:
                 domain_filename = os.path.join(tempdir, "domain.pddl")
                 problem_filename = os.path.join(tempdir, "problem.pddl")
 
                 w = PDDLWriter(problem)
@@ -521,14 +528,23 @@
                             self.assertEqual(len(a.effects), len(parsed_a.effects))
                     elif isinstance(a, DurativeAction):
                         assert isinstance(parsed_a, DurativeAction)
                         self.assertEqual(str(a.duration), str(parsed_a.duration))
                         for t, e in a.effects.items():
                             self.assertEqual(len(e), len(parsed_a.effects[t]))
 
+                self.assertEqual(
+                    len(problem.trajectory_constraints),
+                    len(parsed_problem.trajectory_constraints),
+                )
+                self.assertEqual(
+                    set(map(str, problem.trajectory_constraints)),
+                    set(map(str, parsed_problem.trajectory_constraints)),
+                )
+
     def test_basic_with_object_constant(self):
         problem = self.problems["basic_with_object_constant"].problem
 
         w = PDDLWriter(problem)
 
         pddl_domain = w.get_domain()
         pddl_problem = w.get_problem()
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_pddl_planner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_planner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,32 @@
                 self.assertEqual(len(plan.actions), 1)
                 self.assertEqual(plan.actions[0].action, a)
                 self.assertEqual(len(plan.actions[0].actual_parameters), 0)
                 self.assertEqual(len(w), 1)
                 self.assertEqual("Tamer does not support timeout.", str(w[-1].message))
 
     @skipIfEngineNotAvailable("tamer")
+    def test_basic_parameters(self):
+        problem_names = [
+            "basic_bool_fluent_param",
+            "basic_int_fluent_param",
+            "basic_bounded_int_action_param",
+        ]
+        problem = self.problems["basic_bool_fluent_param"].problem
+        for problem_name in problem_names:
+            problem = self.problems[problem_name].problem
+        with OneshotPlanner(name="tamer") as planner:
+            self.assertNotEqual(planner, None)
+            plan = planner.solve(problem).plan
+            self.assertIsNotNone(plan)
+            with PlanValidator(name="sequential_plan_validator") as validator:
+                val_res = validator.validate(problem, plan)
+                self.assertTrue(val_res)
+
+    @skipIfEngineNotAvailable("tamer")
     def test_basic_parallel(self):
         problem = self.problems["basic"].problem
         a = problem.action("a")
 
         with OneshotPlanner(
             names=["tamer", "tamer"],
             params=[{"heuristic": "hadd"}, {"heuristic": "hmax"}],
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_problem.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,14 +521,17 @@
 
         names_of_SNP_problems = [
             "counter_to_50",
             "robot_decrease",
             "robot_locations_connected",
             "robot_locations_visited",
             "robot_fluent_of_user_type_with_int_id",
+            "basic_int_fluent_param",
+            "basic_bounded_int_action_param",
+            "basic_unbounded_int_action_param",
         ]
         for problem, _ in self.problems.values():
             if problem.name in names_of_SNP_problems:
                 self.assertTrue(problem.kind.has_simple_numeric_planning())
             else:
                 self.assertFalse(problem.kind.has_simple_numeric_planning())
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_protobuf_io.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_protobuf_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,23 +398,38 @@
 
         self.pb_writer = ProtobufWriter()
         self.pb_reader = ProtobufReader()
 
     def test_all_problems(self):
         for name, example in self.problems.items():
             problem = example.problem
+            kind = problem.kind
             problem_pb = self.pb_writer.convert(problem)
             problem_up = self.pb_reader.convert(problem_pb)
 
             self.assertEqual(problem, problem_up)
             self.assertEqual(
                 hash(problem),
                 hash(problem_up),
                 f"[hash] Error on problem {name}: \n\n{problem}\n=====\n{problem_up}",
             )
+            if kind.has_continuous_time():
+                problem = problem.clone()
+                problem.epsilon = "2"
+                problem.self_overlapping = True
+                problem.discrete_time = True
+                problem_pb = self.pb_writer.convert(problem)
+                problem_up = self.pb_reader.convert(problem_pb)
+
+                self.assertEqual(problem, problem_up)
+                self.assertEqual(
+                    hash(problem),
+                    hash(problem_up),
+                    f"[hash] Error on problem {name}: \n\n{problem}\n=====\n{problem_up}",
+                )
 
     def test_all_plans(self):
         for name, example in self.problems.items():
             problem = example.problem
             plan = example.plan
             plan_pb = self.pb_writer.convert(plan)
             plan_up = self.pb_reader.convert(plan_pb, problem)
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_pyperplan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_pyperplan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_quantifier_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_quantifier_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_replanner.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_scheduling.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_sequential_simulator.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_sequential_simulator.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from typing import cast
+import warnings
 import unified_planning as up
 import pytest
 from itertools import product
 from unified_planning.shortcuts import *
 from unified_planning.engines import UPSequentialSimulator, SequentialSimulatorMixin
 from unified_planning.model import State
 from unified_planning.plans import ActionInstance
@@ -188,15 +190,15 @@
         problem.add_fluent(condition2, default_initial_value=True)
         problem.add_fluent(condition3, default_initial_value=True)
         problem.add_fluent(fluent, default_initial_value=0)
 
         with SequentialSimulator(problem=problem) as simulator:
             init = simulator.get_initial_state()
 
-            self.assertTrue(simulator.is_applicable(init, test_int))
+            self.assertFalse(simulator.is_applicable(init, test_int))
             self.assertIsNone(simulator.apply(init, test_int))
 
             new_state = simulator.apply(init, unset_cond_2)
             self.assertIsNone(simulator.apply(new_state, test_int))
 
             new_state = simulator.apply(new_state, unset_cond_3)
             test_state = simulator.apply(new_state, test_int)
@@ -218,7 +220,46 @@
             init = simulator.get_initial_state()
 
             self.assertTrue(simulator.is_applicable(init, act))
 
             goal_state = simulator.apply_unsafe(init, act)
 
             self.assertTrue(simulator.is_goal(goal_state))
+
+    def test_parameters_type(self):
+        # Test that the simulator correctly handles fluents with bool parameters
+        problem, plan = self.problems["basic_bool_fluent_param"]
+        simulator = UPSequentialSimulator(problem)
+        state: Optional[State] = simulator.get_initial_state()
+        for ai in plan.actions:
+            state = simulator.apply(cast(State, state), ai)
+            self.assertIsNotNone(state)
+        self.assertTrue(simulator.is_goal(cast(State, state)))
+
+        # Test that the simulator correctly handles fluents with integer parameters
+        problem, plan = self.problems["basic_int_fluent_param"]
+        simulator = UPSequentialSimulator(problem)
+        state = simulator.get_initial_state()
+        for ai in plan.actions:
+            state = simulator.apply(cast(State, state), ai)
+            self.assertIsNotNone(state)
+        self.assertTrue(simulator.is_goal(cast(State, state)))
+
+        # Test that the simulator correctly handles actions with bounded integer parameters
+        problem, plan = self.problems["basic_bounded_int_action_param"]
+        simulator = UPSequentialSimulator(problem)
+        state = simulator.get_initial_state()
+        self.assertEqual(4, len(tuple(simulator.get_applicable_actions(state))))
+        for ai in plan.actions:
+            state = simulator.apply(cast(State, state), ai)
+            self.assertIsNotNone(state)
+        self.assertTrue(simulator.is_goal(cast(State, state)))
+
+        # Test that the simulator correctly handles actions with bounded integer parameters
+        problem, plan = self.problems["basic_unbounded_int_action_param"]
+        with warnings.catch_warnings(record=True) as _:
+            simulator = UPSequentialSimulator(problem, error_on_failed_checks=False)
+        state = simulator.get_initial_state()
+        for ai in plan.actions:
+            state = simulator.apply(cast(State, state), ai)
+            self.assertIsNotNone(state)
+        self.assertTrue(simulator.is_goal(cast(State, state)))
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_simplifier.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_simulated_effects.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_simulated_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_stn_plan.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_substituter.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_tamp.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_tarski_converter.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_tarski_converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_tarski_grounder.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_temporal.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_temporal.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_trajectory_constraint.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_trajectory_constraint.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_trajectory_constraints_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_usertype_fluents_remover.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_usertype_fluents_remover.py`

 * *Files 21% similar despite different names*

```diff
@@ -126,21 +126,21 @@
         ]
         a = InstantaneousAction("a")
         for condition in conds:
             a.add_precondition(condition)
         a.add_effect(f1, g1)
 
         b = InstantaneousAction("b")
-        b.add_effect(f1_r(f1), g1)
+        b.add_effect(f1_r(obj_1), g1)
 
         c = InstantaneousAction("c")
         c.add_effect(f1, g1, b1(g1))
 
         d = InstantaneousAction("d")
-        d.add_effect(f1_b_ut1(b1(g1), g1), g1)
+        d.add_effect(f1_b_ut1(True, obj_1), g1)
 
         problem.add_fluents([f1, g1, f1_r, b1, b1_1, f1_b_ut1, int1])
         problem.add_objects([obj_1, obj_2])
         problem.add_actions([a, b, c, d])
 
         init: Dict[FNode, Union[Object, int, bool]] = {
             f1(): obj_1,
@@ -198,55 +198,35 @@
             Effect(
                 new_f1(obj_2),
                 FALSE(),
                 Not(new_g1(obj_2)),
             ),
         }
 
-        # b effect -> f1_r(f1):= g1
+        # b effect -> f1_r(obj_1):= g1
         expected_effects[b.name] = {
             Effect(
                 new_f1_r(obj_1, obj_1),
                 TRUE(),
-                And(new_f1(obj_1), new_g1(obj_1)),
+                new_g1(obj_1),
             ),
             Effect(
                 new_f1_r(obj_1, obj_1),
                 FALSE(),
-                And(new_f1(obj_1), Not(new_g1(obj_1))),
-            ),
-            Effect(
-                new_f1_r(obj_2, obj_1),
-                TRUE(),
-                And(new_f1(obj_2), new_g1(obj_1)),
-            ),
-            Effect(
-                new_f1_r(obj_2, obj_1),
-                FALSE(),
-                And(new_f1(obj_2), Not(new_g1(obj_1))),
+                Not(new_g1(obj_1)),
             ),
             Effect(
                 new_f1_r(obj_1, obj_2),
                 TRUE(),
-                And(new_f1(obj_1), new_g1(obj_2)),
+                new_g1(obj_2),
             ),
             Effect(
                 new_f1_r(obj_1, obj_2),
                 FALSE(),
-                And(new_f1(obj_1), Not(new_g1(obj_2))),
-            ),
-            Effect(
-                new_f1_r(obj_2, obj_2),
-                TRUE(),
-                And(new_f1(obj_2), new_g1(obj_2)),
-            ),
-            Effect(
-                new_f1_r(obj_2, obj_2),
-                FALSE(),
-                And(new_f1(obj_2), Not(new_g1(obj_2))),
+                Not(new_g1(obj_2)),
             ),
         }
 
         # c effect -> if  b1(g1) then f1 := g1
         expected_effects[c.name] = {
             Effect(
                 new_f1(obj_1),
@@ -270,57 +250,35 @@
                 FALSE(),
                 And(
                     Exists(And(b1(g1_var), new_g1(g1_var)), g1_var), Not(new_g1(obj_2))
                 ),
             ),
         }
 
-        # d effect -> f1_b_ut1(b1(g1), g1) := g1
+        # d effect -> f1_b_ut1(True, obj_1) := g1
         expected_effects[d.name] = {
             Effect(
-                new_f1_b_ut1(
-                    Exists(And(b1(g1_var), new_g1(g1_var)), g1_var), obj_1, obj_1
-                ),
+                new_f1_b_ut1(True, obj_1, obj_1),
                 TRUE(),
                 new_g1(obj_1),
             ),
             Effect(
-                new_f1_b_ut1(
-                    Exists(And(b1(g1_var), new_g1(g1_var)), g1_var), obj_2, obj_1
-                ),
-                TRUE(),
-                And(new_g1(obj_2), new_g1(obj_1)),
-            ),
-            Effect(
-                new_f1_b_ut1(
-                    Exists(And(b1(g1_var), new_g1(g1_var)), g1_var), obj_2, obj_1
-                ),
+                new_f1_b_ut1(True, obj_1, obj_1),
                 FALSE(),
-                And(new_g1(obj_2), Not(new_g1(obj_1))),
+                Not(new_g1(obj_1)),
             ),
             Effect(
-                new_f1_b_ut1(
-                    Exists(And(b1(g1_var), new_g1(g1_var)), g1_var), obj_2, obj_2
-                ),
+                new_f1_b_ut1(True, obj_1, obj_2),
                 TRUE(),
                 new_g1(obj_2),
             ),
             Effect(
-                new_f1_b_ut1(
-                    Exists(And(b1(g1_var), new_g1(g1_var)), g1_var), obj_1, obj_2
-                ),
-                TRUE(),
-                And(new_g1(obj_1), new_g1(obj_2)),
-            ),
-            Effect(
-                new_f1_b_ut1(
-                    Exists(And(b1(g1_var), new_g1(g1_var)), g1_var), obj_1, obj_2
-                ),
+                new_f1_b_ut1(True, obj_1, obj_2),
                 FALSE(),
-                And(new_g1(obj_1), Not(new_g1(obj_2))),
+                Not(new_g1(obj_2)),
             ),
         }
         simplifier = QuantifierSimplifier(problem.environment, problem)
         compiled_simplifier = QuantifierSimplifier(
             compiled_problem.environment, compiled_problem
         )
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/test/test_validator.py` & `unified_planning-0.6.0.94.dev1/unified_planning/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning/utils.py` & `unified_planning-0.6.0.94.dev1/unified_planning/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning.egg-info/PKG-INFO` & `unified_planning-0.6.0.94.dev1/unified_planning.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified-planning
-Version: 0.6.0.9.dev1
+Version: 0.6.0.94.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: UNKNOWN
 Keywords: planning logic STRIPS RDDL
@@ -25,8 +25,9 @@
 Provides-Extra: pyperplan
 Provides-Extra: tamer
 Provides-Extra: enhsp
 Provides-Extra: fast-downward
 Provides-Extra: lpg
 Provides-Extra: fmap
 Provides-Extra: aries
+Provides-Extra: symk
 Provides-Extra: engines
```

### Comparing `unified_planning-0.6.0.9.dev1/unified_planning.egg-info/SOURCES.txt` & `unified_planning-0.6.0.94.dev1/unified_planning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 unified_planning/engines/__init__.py
 unified_planning/engines/credits.py
 unified_planning/engines/engine.py
 unified_planning/engines/factory.py
 unified_planning/engines/meta_engine.py
 unified_planning/engines/oversubscription_planner.py
 unified_planning/engines/parallel.py
+unified_planning/engines/pddl_anytime_planner.py
 unified_planning/engines/pddl_planner.py
 unified_planning/engines/plan_validator.py
 unified_planning/engines/replanner.py
 unified_planning/engines/results.py
 unified_planning/engines/sequential_simulator.py
 unified_planning/engines/compilers/__init__.py
 unified_planning/engines/compilers/bounded_types_remover.py
 unified_planning/engines/compilers/compilers_pipeline.py
 unified_planning/engines/compilers/conditional_effects_remover.py
 unified_planning/engines/compilers/disjunctive_conditions_remover.py
 unified_planning/engines/compilers/grounder.py
 unified_planning/engines/compilers/negative_conditions_remover.py
 unified_planning/engines/compilers/quantifiers_remover.py
+unified_planning/engines/compilers/state_invariants_remover.py
 unified_planning/engines/compilers/tarski_grounder.py
 unified_planning/engines/compilers/trajectory_constraints_remover.py
 unified_planning/engines/compilers/usertype_fluents_remover.py
 unified_planning/engines/compilers/utils.py
 unified_planning/engines/mixins/__init__.py
 unified_planning/engines/mixins/anytime_planner.py
 unified_planning/engines/mixins/compiler.py
@@ -58,15 +60,14 @@
 unified_planning/io/__init__.py
 unified_planning/io/anml_grammar.py
 unified_planning/io/anml_reader.py
 unified_planning/io/anml_writer.py
 unified_planning/io/ma_pddl_writer.py
 unified_planning/io/pddl_reader.py
 unified_planning/io/pddl_writer.py
-unified_planning/io/python_writer.py
 unified_planning/io/utils.py
 unified_planning/model/__init__.py
 unified_planning/model/abstract_problem.py
 unified_planning/model/action.py
 unified_planning/model/contingent_problem.py
 unified_planning/model/delta_stn.py
 unified_planning/model/effect.py
@@ -163,21 +164,21 @@
 unified_planning/test/test_pddl_io.py
 unified_planning/test/test_pddl_planner.py
 unified_planning/test/test_plan_validator.py
 unified_planning/test/test_planner.py
 unified_planning/test/test_problem.py
 unified_planning/test/test_protobuf_io.py
 unified_planning/test/test_pyperplan.py
-unified_planning/test/test_python_writer.py
 unified_planning/test/test_quantifier_remover.py
 unified_planning/test/test_replanner.py
 unified_planning/test/test_scheduling.py
 unified_planning/test/test_sequential_simulator.py
 unified_planning/test/test_simplifier.py
 unified_planning/test/test_simulated_effects.py
+unified_planning/test/test_state_invariants.py
 unified_planning/test/test_stn_plan.py
 unified_planning/test/test_substituter.py
 unified_planning/test/test_tamp.py
 unified_planning/test/test_tarski_converter.py
 unified_planning/test/test_tarski_grounder.py
 unified_planning/test/test_temporal.py
 unified_planning/test/test_trajectory_constraint.py
```

