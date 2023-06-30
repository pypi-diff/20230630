# Comparing `tmp/ibm-generative-ai-0.1.17.tar.gz` & `tmp/ibm-generative-ai-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-generative-ai-0.1.17.tar", last modified: Fri Jun 23 15:21:40 2023, max compression
+gzip compressed data, was "ibm-generative-ai-0.1.18.tar", last modified: Fri Jun 30 17:57:54 2023, max compression
```

## Comparing `ibm-generative-ai-0.1.17.tar` & `ibm-generative-ai-0.1.18.tar`

### file list

```diff
@@ -1,236 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.214784 ibm-generative-ai-0.1.17/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.170784 ibm-generative-ai-0.1.17/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.170784 ibm-generative-ai-0.1.17/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/ISSUE_TEMPLATE/01_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/ISSUE_TEMPLATE/02_feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/ISSUE_TEMPLATE/03_documentation_update.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.170784 ibm-generative-ai-0.1.17/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/workflows/integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/ACTIVE_PROJECT_TEAM.md
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/EXTENSIONS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-23 15:21:40.214784 ibm-generative-ai-0.1.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/SUPPORT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.170784 ibm-generative-ai-0.1.17/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/.nojekyll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.170784 ibm-generative-ai-0.1.17/documentation/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/assets/pull_request_from_fork_to_base.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.170784 ibm-generative-ai-0.1.17/documentation/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.174784 ibm-generative-ai-0.1.17/documentation/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.174784 ibm-generative-ai-0.1.17/documentation/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.174784 ibm-generative-ai-0.1.17/documentation/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.174784 ibm-generative-ai-0.1.17/documentation/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/_templates/custom_landing_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.178784 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.178784 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/async.examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/async.examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/extensions.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/prompts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/prompts.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.credentials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.prompt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.schemas.history_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.schemas.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.schemas.responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.schemas.token_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.services.request_handler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.services.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.services.service_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/local_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.166784 ibm-generative-ai-0.1.17/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.182784 ibm-generative-ai-0.1.17/examples/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/dev/async-flaky-responses-ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/dev/generate-all-models.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/dev/history-async.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/dev/load_token_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/dev/logging_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.186784 ibm-generative-ai-0.1.17/examples/user/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/alice_bob_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/alice_bob_talk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.190784 ibm-generative-ai-0.1.17/examples/user/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/assets/country-capital.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/assets/penguins2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/assets/seed_tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/assets/seed_tasks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/async_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/async_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/async_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/async_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/complete_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/country-capital-qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/explain_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/generate_with_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/gpt_chat_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/grid_search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/grid_search_params_greeating.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/jsonprompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/jsonprompt_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/langchain_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.190784 ibm-generative-ai-0.1.17/examples/user/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/localserver/localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/localserver/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/logprob_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/many_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/model_as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompt-raw-string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompt_csv_random_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompt_from_all_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompt_from_all_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompt_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompt_reuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.190784 ibm-generative-ai-0.1.17/examples/user/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompts/Country-Capital-Factual-QA
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.190784 ibm-generative-ai-0.1.17/examples/user/prompts_adult_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/saving_prompts_as_hf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/self-reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/self_instruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.190784 ibm-generative-ai-0.1.17/examples/user/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/templates/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/templates/instruction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/templates/qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/templates/self-reflection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/templates/synth-animal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/tokenize-sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/examples/user/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:21:40.214784 ibm-generative-ai-0.1.17/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.166784 ibm-generative-ai-0.1.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.194784 ibm-generative-ai-0.1.17/src/genai/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 15:21:39.000000 ibm-generative-ai-0.1.17/src/genai/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.194784 ibm-generative-ai-0.1.17/src/genai/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/exceptions/genai_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.166784 ibm-generative-ai-0.1.17/src/genai/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.194784 ibm-generative-ai-0.1.17/src/genai/extensions/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/huggingface/save_huggingface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.194784 ibm-generative-ai-0.1.17/src/genai/extensions/langchain/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/langchain/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/langchain/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.194784 ibm-generative-ai-0.1.17/src/genai/extensions/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/localserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/localserver/custom_model_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/localserver/local_api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/localserver/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.194784 ibm-generative-ai-0.1.17/src/genai/extensions/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/extensions/pandas/prompt_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22054 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/prompt_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.202784 ibm-generative-ai-0.1.17/src/genai/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/schemas/descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/schemas/generate_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/schemas/history_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/schemas/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/schemas/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/schemas/token_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.202784 ibm-generative-ai-0.1.17/src/genai/services/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/services/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/services/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/services/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/services/service_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.202784 ibm-generative-ai-0.1.17/src/genai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/utils/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/src/genai/utils/search_space_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.202784 ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-23 15:21:40.000000 ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-23 15:21:40.000000 ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:21:40.000000 ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-23 15:21:40.000000 ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 15:21:40.000000 ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.206784 ibm-generative-ai-0.1.17/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.210784 ibm-generative-ai-0.1.17/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/age-gender.csv
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/capital-qa-content.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/capital-qa-multivar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/capital-qa-sub-noheader.csv
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/capital-qa-sub.csv
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/capital-qa-sub.json
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/capital-qa-sub.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/csv_file.csv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/csv_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/invalid-content-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/invalid-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/prompt_contents.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/response_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/story.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/assets/story_sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.210784 ibm-generative-ai-0.1.17/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/extensions/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/extensions/test_localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/extensions/test_save_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/extensions/test_sub_from_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:21:40.210784 ibm-generative-ai-0.1.17/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/integration/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/integration/test_terms_of_use.py
--rw-r--r--   0 runner    (1001) docker     (123)    17750 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_generate_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_model_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_prompt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_service_interface_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_service_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 15:21:03.000000 ibm-generative-ai-0.1.17/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.112575 ibm-generative-ai-0.1.18/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/ISSUE_TEMPLATE/01_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/ISSUE_TEMPLATE/02_feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/ISSUE_TEMPLATE/03_documentation_update.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/workflows/integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/ACTIVE_PROJECT_TEAM.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/EXTENSIONS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-06-30 17:57:54.112575 ibm-generative-ai-0.1.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/SUPPORT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/documentation/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/assets/pull_request_from_fork_to_base.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/documentation/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/documentation/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/documentation/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/documentation/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.092575 ibm-generative-ai-0.1.18/documentation/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/_templates/custom_landing_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.096575 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.096575 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/async.examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/async.examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/extensions.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/prompts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/prompts.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.prompt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.schemas.history_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.schemas.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.schemas.responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.schemas.token_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.services.request_handler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.services.service_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/local_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.088575 ibm-generative-ai-0.1.18/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.096575 ibm-generative-ai-0.1.18/examples/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/dev/async-flaky-request-handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/dev/async-flaky-responses-ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/dev/generate-all-models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/dev/history-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/dev/load_token_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/dev/logging_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.100575 ibm-generative-ai-0.1.18/examples/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/alice_bob_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/alice_bob_talk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.100575 ibm-generative-ai-0.1.18/examples/user/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/assets/country-capital.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/assets/penguins2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/assets/seed_tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/assets/seed_tasks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/async_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/async_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/async_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/async_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/complete_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/country-capital-qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/explain_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/generate_with_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/gpt_chat_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/grid_search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/grid_search_params_greeating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/jsonprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/jsonprompt_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/langchain_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.100575 ibm-generative-ai-0.1.18/examples/user/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/localserver/localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/localserver/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/logprob_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/many_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/model_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt-raw-string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_csv_random_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_from_all_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_from_all_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.100575 ibm-generative-ai-0.1.18/examples/user/prompt_templating/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_templating/watsonx-prompt-output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompt_templating/watsonx-prompt-templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.100575 ibm-generative-ai-0.1.18/examples/user/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompts/Country-Capital-Factual-QA
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.100575 ibm-generative-ai-0.1.18/examples/user/prompts_adult_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/saving_prompts_as_hf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/self-reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/self_instruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/examples/user/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/templates/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/templates/instruction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/templates/qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/templates/self-reflection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/templates/synth-animal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/tokenize-sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/examples/user/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:57:54.112575 ibm-generative-ai-0.1.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.088575 ibm-generative-ai-0.1.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/src/genai/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-30 17:57:53.000000 ibm-generative-ai-0.1.18/src/genai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/src/genai/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/exceptions/genai_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.088575 ibm-generative-ai-0.1.18/src/genai/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/src/genai/extensions/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/huggingface/save_huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/src/genai/extensions/langchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/langchain/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/langchain/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/src/genai/extensions/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/localserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/localserver/custom_model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/localserver/local_api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/localserver/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/src/genai/extensions/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/extensions/pandas/prompt_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/prompt_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/src/genai/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/routers/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.104575 ibm-generative-ai-0.1.18/src/genai/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/schemas/descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/schemas/generate_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/schemas/history_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/schemas/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/schemas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/schemas/token_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.108575 ibm-generative-ai-0.1.18/src/genai/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/services/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/services/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/services/prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/services/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/services/service_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.108575 ibm-generative-ai-0.1.18/src/genai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/utils/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/utils/search_space_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/src/genai/utils/watsonx_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.108575 ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-06-30 17:57:54.000000 ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-06-30 17:57:54.000000 ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:57:54.000000 ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 17:57:54.000000 ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 17:57:54.000000 ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.108575 ibm-generative-ai-0.1.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.112575 ibm-generative-ai-0.1.18/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/age-gender.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/capital-qa-content.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/capital-qa-multivar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/capital-qa-sub-noheader.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/capital-qa-sub.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/capital-qa-sub.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/capital-qa-sub.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/csv_file.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/csv_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/invalid-content-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/invalid-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/prompt_contents.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/response_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/story.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/assets/story_sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.112575 ibm-generative-ai-0.1.18/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/extensions/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/extensions/test_localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/extensions/test_save_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/extensions/test_sub_from_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:57:54.112575 ibm-generative-ai-0.1.18/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/integration/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/integration/test_terms_of_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_generate_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_model_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_prompt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_prompt_pattern_watsonx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_service_interface_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-30 17:57:26.000000 ibm-generative-ai-0.1.18/tests/test_version.py
```

### Comparing `ibm-generative-ai-0.1.17/.github/ISSUE_TEMPLATE/01_bug_report.md` & `ibm-generative-ai-0.1.18/.github/ISSUE_TEMPLATE/01_bug_report.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.github/ISSUE_TEMPLATE/02_feature_request.md` & `ibm-generative-ai-0.1.18/.github/ISSUE_TEMPLATE/02_feature_request.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.github/ISSUE_TEMPLATE/03_documentation_update.md` & `ibm-generative-ai-0.1.18/.github/ISSUE_TEMPLATE/03_documentation_update.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.github/PULL_REQUEST_TEMPLATE.md` & `ibm-generative-ai-0.1.18/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.github/workflows/documentation.yml` & `ibm-generative-ai-0.1.18/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.github/workflows/integration-test.yml` & `ibm-generative-ai-0.1.18/.github/workflows/integration-test.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.github/workflows/main.yml` & `ibm-generative-ai-0.1.18/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.github/workflows/python-publish.yml` & `ibm-generative-ai-0.1.18/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.gitignore` & `ibm-generative-ai-0.1.18/.gitignore`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/.pre-commit-config.yaml` & `ibm-generative-ai-0.1.18/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/CODE_OF_CONDUCT.md` & `ibm-generative-ai-0.1.18/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/DEVELOPMENT.md` & `ibm-generative-ai-0.1.18/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/EXTENSIONS.md` & `ibm-generative-ai-0.1.18/EXTENSIONS.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/LICENSE` & `ibm-generative-ai-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/PKG-INFO` & `ibm-generative-ai-0.1.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 0.1.17
+Version: 0.1.18
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: langchain
 Provides-Extra: huggingface
@@ -14,15 +14,15 @@
 License-File: LICENSE
 
 # IBM Generative AI Python SDK
 
 
 This is the Python SDK for IBM Foundation Models Studio to bring IBM Generative AI into Python programs and to also extend it with useful operations and types.
 
-:books:	API Documentation: [Link](https://ibm.github.io/ibm-generative-ai/)
+:books:	**API Documentation: [Link](https://ibm.github.io/ibm-generative-ai/)**
 
 *This is an early access library and requires invitation to use the technical preview of [watsonx.ai](https://watsonx.ai/). You can join the waitlist by visiting. https://www.ibm.com/products/watsonx-ai.*
 
 *Looking for the JavaScript/TypeScript version? Check out https://github.com/IBM/ibm-generative-ai-node-sdk.*
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/IBM/ibm-generative-ai/blob/main/LICENSE)
 ![PyPI](https://img.shields.io/pypi/v/ibm-generative-ai)
@@ -112,30 +112,31 @@
 
 ```
 
 
 ## <a name='Examples'></a>Examples
 
 There are a number of examples you can try in the [`examples/user`](examples/user) directory.
-Login to [workbench.res.ibm.com](https://workbench.res.ibm.com/) and get your GenAI API key. Then, create a `.env` file and assign the `GENAI_KEY` value as:
+Login to [workbench.res.ibm.com](https://workbench.res.ibm.com/) and get your GenAI API key. Then, create a `.env` file and assign the `GENAI_KEY` value as below example. [More information](#gen-ai-endpoint)
 
 
 ```ini
 GENAI_KEY=YOUR_GENAI_API_KEY
+# GENAI_API=GENAI_API_ENDPOINT << for a different endpoint
 ```
 
 ### <a name='AsyncExample'></a>Async Example
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -153,15 +154,15 @@
     top_k=50,
     top_p=1,
 )
 
 # creds object
 creds = Credentials(api_key, api_endpoint)
 # model object
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting = "Hello! How are you?"
 lots_of_greetings = [greeting] * 1000
 num_of_greetings = len(lots_of_greetings)
 num_said_greetings = 0
 greeting1 = "Hello! How are you?"
 
@@ -181,15 +182,15 @@
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -207,15 +208,15 @@
     top_k=50,
     top_p=1,
 )
 
 # creds object
 creds = Credentials(api_key, api_endpoint)
 # model object
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting1 = "Hello! How are you?"
 greeting2 = "I am fine and you?"
 
 # Call generate function
 responses = model.generate_as_completed([greeting1, greeting2] * 4)
 for response in responses:
@@ -303,29 +304,29 @@
 ```
 Currently the langchain extension allows IBM Generative AI models to be wrapped as Langchain LLMs and translation between genai PromptPatterns and LangChain PromptTemplates. Below are sample snippets
 ```python
 import os
 from dotenv import load_dotenv
 import genai.extensions.langchain
 from genai.extensions.langchain import LangChainInterface
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 from genai import Credentials, Model, PromptPattern
 
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
 creds = Credentials(api_key, api_endpoint)
 params = GenerateParams(decoding_method="greedy")
 
 # As LangChain Model
-langchain_model = LangChainInterface(model=ModelType.FLAN_UL2, params=params, credentials=creds)
+langchain_model = LangChainInterface(model="google/flan-ul2", params=params, credentials=creds)
 print(langchain_model("Answer this question: What is life?"))
 
 # As GenAI Model
-genai_model = Model(model=ModelType.FLAN_UL2, params=params, credentials=creds)
+genai_model = Model(model="google/flan-ul2", params=params, credentials=creds)
 print(genai_model.generate(["Answer this question: What is life?"])[0].generated_text)
 
 # GenAI prompt pattern to langchain PromptTemplate and vice versa
 seed_pattern = PromptPattern.from_str("Answer this question: {{question}}")
 template = seed_pattern.langchain.as_template()
 pattern = PromptPattern.langchain.from_template(template)
```

### Comparing `ibm-generative-ai-0.1.17/README.md` & `ibm-generative-ai-0.1.18/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # IBM Generative AI Python SDK
 
 
 This is the Python SDK for IBM Foundation Models Studio to bring IBM Generative AI into Python programs and to also extend it with useful operations and types.
 
-:books:	API Documentation: [Link](https://ibm.github.io/ibm-generative-ai/)
+:books:	**API Documentation: [Link](https://ibm.github.io/ibm-generative-ai/)**
 
 *This is an early access library and requires invitation to use the technical preview of [watsonx.ai](https://watsonx.ai/). You can join the waitlist by visiting. https://www.ibm.com/products/watsonx-ai.*
 
 *Looking for the JavaScript/TypeScript version? Check out https://github.com/IBM/ibm-generative-ai-node-sdk.*
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/IBM/ibm-generative-ai/blob/main/LICENSE)
 ![PyPI](https://img.shields.io/pypi/v/ibm-generative-ai)
@@ -97,30 +97,31 @@
 
 ```
 
 
 ## <a name='Examples'></a>Examples
 
 There are a number of examples you can try in the [`examples/user`](examples/user) directory.
-Login to [workbench.res.ibm.com](https://workbench.res.ibm.com/) and get your GenAI API key. Then, create a `.env` file and assign the `GENAI_KEY` value as:
+Login to [workbench.res.ibm.com](https://workbench.res.ibm.com/) and get your GenAI API key. Then, create a `.env` file and assign the `GENAI_KEY` value as below example. [More information](#gen-ai-endpoint)
 
 
 ```ini
 GENAI_KEY=YOUR_GENAI_API_KEY
+# GENAI_API=GENAI_API_ENDPOINT << for a different endpoint
 ```
 
 ### <a name='AsyncExample'></a>Async Example
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -138,15 +139,15 @@
     top_k=50,
     top_p=1,
 )
 
 # creds object
 creds = Credentials(api_key, api_endpoint)
 # model object
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting = "Hello! How are you?"
 lots_of_greetings = [greeting] * 1000
 num_of_greetings = len(lots_of_greetings)
 num_said_greetings = 0
 greeting1 = "Hello! How are you?"
 
@@ -166,15 +167,15 @@
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -192,15 +193,15 @@
     top_k=50,
     top_p=1,
 )
 
 # creds object
 creds = Credentials(api_key, api_endpoint)
 # model object
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting1 = "Hello! How are you?"
 greeting2 = "I am fine and you?"
 
 # Call generate function
 responses = model.generate_as_completed([greeting1, greeting2] * 4)
 for response in responses:
@@ -288,29 +289,29 @@
 ```
 Currently the langchain extension allows IBM Generative AI models to be wrapped as Langchain LLMs and translation between genai PromptPatterns and LangChain PromptTemplates. Below are sample snippets
 ```python
 import os
 from dotenv import load_dotenv
 import genai.extensions.langchain
 from genai.extensions.langchain import LangChainInterface
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 from genai import Credentials, Model, PromptPattern
 
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
 creds = Credentials(api_key, api_endpoint)
 params = GenerateParams(decoding_method="greedy")
 
 # As LangChain Model
-langchain_model = LangChainInterface(model=ModelType.FLAN_UL2, params=params, credentials=creds)
+langchain_model = LangChainInterface(model="google/flan-ul2", params=params, credentials=creds)
 print(langchain_model("Answer this question: What is life?"))
 
 # As GenAI Model
-genai_model = Model(model=ModelType.FLAN_UL2, params=params, credentials=creds)
+genai_model = Model(model="google/flan-ul2", params=params, credentials=creds)
 print(genai_model.generate(["Answer this question: What is life?"])[0].generated_text)
 
 # GenAI prompt pattern to langchain PromptTemplate and vice versa
 seed_pattern = PromptPattern.from_str("Answer this question: {{question}}")
 template = seed_pattern.langchain.as_template()
 pattern = PromptPattern.langchain.from_template(template)
```

### Comparing `ibm-generative-ai-0.1.17/SUPPORT.md` & `ibm-generative-ai-0.1.18/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/assets/pull_request_from_fork_to_base.png` & `ibm-generative-ai-0.1.18/documentation/assets/pull_request_from_fork_to_base.png`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/Makefile` & `ibm-generative-ai-0.1.18/documentation/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/make.bat` & `ibm-generative-ai-0.1.18/documentation/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/_templates/custom_landing_page.html` & `ibm-generative-ai-0.1.18/documentation/docs/source/_templates/custom_landing_page.html`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/conf.py` & `ibm-generative-ai-0.1.18/documentation/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/index.rst` & `ibm-generative-ai-0.1.18/documentation/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/async.examples.user.rst` & `ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/async.examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/examples.user.rst` & `ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/extensions.user.rst` & `ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/extensions.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/examples/prompts.user.rst` & `ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/examples/prompts.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst` & `ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/genai.prompt.quickstart.rst` & `ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/genai.prompt.quickstart.rst`

 * *Files 5% similar despite different names*

```diff
@@ -22,48 +22,24 @@
 many prompts as possible** using the data.
 
 A crucial step is to provide the mapping between the template's variables and the csv's column names.
 
 
 Assuming local :ref:`synth-animal.yaml<File : synth-animal.yaml>` and :ref:`penguins.csv<File : penguins.csv>` and files.
 
-..  code-block:: python
+.. literalinclude:: ../../../../examples/user/prompt_from_all_csv.py
+    :language: python
+    :lines: 42-44, 46-66
     :caption: Multiple Prompt Patterns using complete file
-
-    from genai.prompt_pattern import PromptPattern
-
-    _path_to_template_file = "my_templates/synth-animal.yaml"
-    _path_to_csv_file = "my_data/penguins.csv"
-
-    prompt = PromptPattern.from_file(_path_to_template_file)
-    print("\nGiven template:\n", prompt)
-
-    prompt.sub("animal", "penguins")
-    mapping = {
-        "species": ["species1", "species2", "species3"],
-        "island": ["location1", "location2", "location3"],
-        "flipper_length_mm": ["length1", "length2", "length3"],
-        "year": ["dob1", "dob2", "dob3"],
-    }
-
-    list_of_prompts = prompt.sub_all_from_csv(
-        csv_path=_path_to_csv_file,
-        col_to_var=mapping,
-    )
-
-    print("-----------------------")
-    print("generated prompt")
-    print(list_of_prompts)
-    print(len(list_of_prompts))
-    print("-----------------------")
-
-    responses = bloomz.generate_as_completed(list_of_prompts)
-    for response in responses:
-        # do something with response.generated_text
-
+    :prepend: from genai.prompt_pattern import PromptPattern
+              _path_to_template_file = "my_templates/synth-animal.yaml"
+              _path_to_csv_file = "my_data/penguins.csv"
+              # Create prompt pattern from the file
+              prompt = PromptPattern.from_file(_path_to_template_file)
+    :append:      # do something with response.generated_text
 
 ..  code-block:: console
     :caption: Output
 
     Given template:
     Please generate synthetic data about {{animal}}.
     1,{{species1}},{{location1}},{{length1}},{{dob1}}
@@ -130,15 +106,15 @@
     print("-----------------------")
     print("generated prompt")
     print(list_of_prompts)
     print(len(list_of_prompts))
     print("-----------------------")
 
 
-    responses = bloomz.generate_as_completed(list_of_prompts)
+    responses = flan_ul2.generate_as_completed(list_of_prompts)
     for response in responses:
         # do something with response.generated_text
 
 
 .. code-block:: console
     :caption: Output
 
@@ -221,15 +197,15 @@
 
     print("-----------------------")
     print("generated prompt")
     print(list_of_prompts)
     print(len(list_of_prompts))
     print("-----------------------")
 
-    responses = bloomz.generate_as_completed(list_of_prompts)
+    responses = flan_ul2.generate_as_completed(list_of_prompts)
     for response in responses:
         # do something with response.generated_text
 
 
 ..  code-block:: console
     :caption: Output
```

### Comparing `ibm-generative-ai-0.1.17/documentation/docs/source/rst_source/local_server.rst` & `ibm-generative-ai-0.1.18/documentation/docs/source/rst_source/local_server.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/dev/async-flaky-responses-ordered.py` & `ibm-generative-ai-0.1.18/examples/dev/async-flaky-responses-ordered.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from genai.schemas import GenerateParams, ModelType, TokenParams
 from genai.services.async_generator import AsyncResponseGenerator
 
 num_requests = 0
 
 
 class FlakyAsyncResponseGenerator(AsyncResponseGenerator):
-    async def _get_response_json(self, model, inputs, params):
+    async def _get_response_json(self, model, inputs, params, options):
         try:
             global num_requests
             num_requests += 1
             if num_requests % 2 == 0:
                 await asyncio.sleep(random.randint(0, 5))
-                response_raw = await self.service_fn_(model, inputs, params)
+                response_raw = await self.service_fn_(model, inputs, params, options)
             else:
                 await asyncio.sleep(random.randint(0, 5))
                 response_raw = None  # bad response
             response = response_raw.json()
         except Exception as _:  # noqa
             response = None
         return response
@@ -31,30 +31,38 @@
 
 class FlakyModel(Model):
     def generate_async(
         self,
         prompts,
         ordered: bool = False,
         callback=None,
+        options=None,
     ):
         try:
             with FlakyAsyncResponseGenerator(
-                self.model, prompts, self.params, self.service, ordered=ordered, callback=callback
+                self.model, prompts, self.params, self.service, ordered=ordered, callback=callback, options=options
             ) as asynchelper:
                 for response in asynchelper.generate_response():
                     yield response
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
 
-    def tokenize_async(self, prompts, ordered=False, callback=None):
+    def tokenize_async(self, prompts, ordered=False, callback=None, options=None):
         try:
             with FlakyAsyncResponseGenerator(
-                self.model, prompts, self.params, self.service, fn="tokenize", ordered=ordered, callback=callback
+                self.model,
+                prompts,
+                self.params,
+                self.service,
+                fn="tokenize",
+                ordered=ordered,
+                callback=callback,
+                options=options,
             ) as asynchelper:
                 for response in asynchelper.generate_response():
                     yield response
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
```

### Comparing `ibm-generative-ai-0.1.17/examples/dev/generate-all-models.py` & `ibm-generative-ai-0.1.18/examples/dev/generate-all-models.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/dev/history-async.py` & `ibm-generative-ai-0.1.18/examples/dev/history-async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/dev/logging_example.py` & `ibm-generative-ai-0.1.18/examples/dev/logging_example.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/alice_bob_qa.py` & `ibm-generative-ai-0.1.18/examples/user/alice_bob_qa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -29,22 +29,22 @@
 )
 
 alice_params = GenerateParams(
     decoding_method="sample",
     max_new_tokens=45,
     min_new_tokens=1,
     stream=False,
-    temperature=0,
+    temperature=0.05,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-bob_model = Model(ModelType.FLAN_UL2, params=bob_params, credentials=creds)
-alice_model = Model(ModelType.FLAN_T5, params=alice_params, credentials=creds)
+bob_model = Model("google/flan-ul2", params=bob_params, credentials=creds)
+alice_model = Model("google/flan-t5-xxl", params=alice_params, credentials=creds)
 
 alice_q = "What is 1 + 1?"
 print(f"[Alice][Q] {alice_q}")
 
 for x in range(max_cycles):
     bob_response = bob_model.generate([alice_q])
     bob_a = bob_response[0].generated_text
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/alice_bob_talk.py` & `ibm-generative-ai-0.1.18/examples/user/alice_bob_talk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -29,22 +29,22 @@
 )
 
 alice_params = GenerateParams(
     decoding_method="sample",
     max_new_tokens=45,
     min_new_tokens=1,
     stream=False,
-    temperature=0,
+    temperature=0.05,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-bob_model = Model(ModelType.FLAN_UL2, params=bob_params, credentials=creds)
-alice_model = Model(ModelType.FLAN_T5, params=alice_params, credentials=creds)
+bob_model = Model("google/flan-ul2", params=bob_params, credentials=creds)
+alice_model = Model("google/flan-t5-xxl", params=alice_params, credentials=creds)
 
 sentence = "Hello! How are you?"
 print(f"[Alice] --> {sentence}")
 
 for x in range(max_cycles):
     bob_response = bob_model.generate([sentence])
     # from first batch get first result generated text
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/assets/penguins.csv` & `ibm-generative-ai-0.1.18/examples/user/assets/penguins.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/assets/penguins2.csv` & `ibm-generative-ai-0.1.18/examples/user/assets/penguins2.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/assets/seed_tasks.json` & `ibm-generative-ai-0.1.18/examples/user/assets/seed_tasks.json`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/assets/seed_tasks.jsonl` & `ibm-generative-ai-0.1.18/examples/user/assets/seed_tasks.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/async_callback.py` & `ibm-generative-ai-0.1.18/examples/user/async_callback.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -22,15 +22,15 @@
     stream=False,
     temperature=0.7,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting = "Hello! How are you?"
 lots_of_greetings = [greeting] * 1000
 
 # some global state for our call back
 num_of_greetings = len(lots_of_greetings)
 num_said_greetings = 0
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/async_greetings.py` & `ibm-generative-ai-0.1.18/examples/user/many_greetings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
 
-print("\n------------- Example (Async Greetings)-------------\n")
+print("\n------------- Example (Greetings)-------------\n")
 
 params = GenerateParams(
     decoding_method="sample",
     max_new_tokens=10,
     min_new_tokens=1,
     stream=False,
     temperature=0.7,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
-greeting = "Hello! How are you?"
-lots_of_greetings = [greeting] * 500
-num_of_greetings = len(lots_of_greetings)
-num_said_greetings = 0
 greeting1 = "Hello! How are you?"
+greeting2 = "I am fine and you?"
 
-# yields batch of results that are produced asynchronously and in parallel
-for result in model.generate_async(lots_of_greetings):
-    num_said_greetings += 1
-    print(f"[Progress {str(float(num_said_greetings/num_of_greetings)*100)}%]")
-    print(f"\t {result.generated_text}")
+# Call generate function
+responses = model.generate_as_completed([greeting1, greeting2] * 4)
+for response in responses:
+    print(f"Generated text: {response.generated_text}")
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/async_ordered.py` & `ibm-generative-ai-0.1.18/examples/user/async_ordered.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType, TokenParams
+from genai.schemas import GenerateParams, TokenParams
 
 logging.getLogger("genai").setLevel(logging.INFO)
 
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
@@ -20,15 +20,15 @@
 
 
 # Instantiate parameters for text generation
 generate_params = GenerateParams(decoding_method="sample", max_new_tokens=500, min_new_tokens=10)
 tokenize_params = TokenParams(return_tokens=True)
 
 
-flan_ul2 = Model(ModelType.FLAN_UL2_20B, params=generate_params, credentials=creds)
+flan_ul2 = Model("google/flan-ul2", params=generate_params, credentials=creds)
 prompts = ["Explain life in one sentence:", "Write a python function to permute an array."] * 5
 print("======== Async Generate (responses need not be in order) ======== ")
 counter = 0
 for response in flan_ul2.generate_async(prompts):
     counter += 1
     if response is not None:
         print(counter, response.input_text, " --> ", response.generated_text)
@@ -50,15 +50,15 @@
             response.generated_text,
         )
     else:
         print(counter, ":", None)
 
 
 # Instantiate a model proxy object to send your requests
-flan_ul2 = Model(ModelType.FLAN_UL2_20B, params=tokenize_params, credentials=creds)
+flan_ul2 = Model("google/flan-ul2", params=tokenize_params, credentials=creds)
 prompts = ["Explain life in one sentence:", "Write a python function to permute an array." * 5] * 5
 print("======== Async Tokenize (responses need not be in order) ======== ")
 counter = 0
 for response in flan_ul2.tokenize_async(prompts):
     counter += 1
     if response is not None:
         print(counter, ":", response.input_text, " --> ", response.tokens)
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/async_tokenize.py` & `ibm-generative-ai-0.1.18/examples/user/async_tokenize.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import ModelType, TokenParams
+from genai.schemas import TokenParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
 
 print("\n------------- Example (Async Greetings)-------------\n")
 
 params = TokenParams(return_tokens=True)
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting = "Hello! How are you?"
 lots_of_greetings = [greeting] * 100
 num_of_greetings = len(lots_of_greetings)
 num_said_greetings = 0
 greeting1 = "Hello! How are you?"
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/complete_my_code.py` & `ibm-generative-ai-0.1.18/examples/user/complete_my_code.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -23,15 +23,15 @@
     stream=False,
     temperature=0.7,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-code_explainer = Model(ModelType.CODEGEN_MONO_16B, params=params, credentials=creds)
+code_explainer = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 # pass in an actual python function to explain
 def add_numbers(number_one, number_two):
     return number_one
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/country-capital-qa.py` & `ibm-generative-ai-0.1.18/examples/user/country-capital-qa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pathlib
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType, ReturnOptions
+from genai.schemas import GenerateParams, ReturnOptions
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -24,15 +24,15 @@
     temperature=0.7,
     top_k=50,
     top_p=1,
     return_options=ReturnOptions(input_text=False, input_tokens=True),
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 prompt_path = pathlib.Path(__file__, "..", "prompts", "Country-Capital-Factual-QA").resolve()
 print(prompt_path)
 # load a prompt from file
 with open(prompt_path, "r") as f:
     prompt = f.read()
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/explain_my_code.py` & `ibm-generative-ai-0.1.18/examples/user/explain_my_code.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -23,15 +23,15 @@
     stream=False,
     temperature=0.7,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-code_explainer = Model(ModelType.CODEGEN_MONO_16B, params=params, credentials=creds)
+code_explainer = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 # pass in an actual python function to explain
 def add_numbers(number_one, number_two):
     return number_one + number_two
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/generate_with_input_text.py` & `ibm-generative-ai-0.1.18/examples/user/generate_with_input_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
 creds = Credentials(api_key, api_endpoint)  # credentials object to access GENAI
 
 # Instantiate parameters for text generation
 params = GenerateParams(decoding_method="sample", max_new_tokens=10)
 
 # Instantiate a model proxy object to send your requests
-flan_ul2 = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+flan_ul2 = Model("google/flan-ul2", params=params, credentials=creds)
 
 prompts = ["Hello! How are you?", "How's the weather?"]
 for response in flan_ul2.generate_async(prompts):
     print(f"Prompt: {response.input_text}\nResponse: {response.generated_text}")
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/gpt_chat_bash.py` & `ibm-generative-ai-0.1.18/examples/user/gpt_chat_bash.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -22,15 +22,15 @@
     stream=False,
     temperature=0.7,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-chat = Model(ModelType.FLAN_UL2_20B, params=params, credentials=creds)
+chat = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 prompt = "Write a bash script to split string on comma display as list"
 print(f"Prompt {prompt}")
 responses = chat.generate([prompt])
 for response in responses:
     print(f"Generated text:\n {response.generated_text}")
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/grid_search_params.py` & `ibm-generative-ai-0.1.18/examples/user/grid_search_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import ModelType
 from genai.utils.search_space_params import grid_search_generate_params
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint> (optional) DEFAULT_API = "https://workbench-api.res.ibm.com/v1"
 load_dotenv()
 API_KEY = os.getenv("GENAI_KEY", None)
@@ -31,15 +30,15 @@
 pt = PromptPattern.from_str("The capital of {{country}} is {{capital}}. The capital of Taiwan is")
 pt.sub("capital", "Madrid").sub("country", "Spain")
 
 # generate all combinations of parameters, returns a list of GenerateParams
 generate_params_list = grid_search_generate_params(my_space_params)
 
 for params in generate_params_list:
-    model = Model(ModelType.FLAN_T5, params=params, credentials=creds)
+    model = Model("google/flan-t5-xxl", params=params, credentials=creds)
     responses = model.generate_async([str(pt)])
 
     print(f"Used params: \n{params} \n")
     print(pt)
     for response in responses:
         print(f"Generated text: {response.generated_text}")
     print("------------------------------------")
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/grid_search_params_greeating.py` & `ibm-generative-ai-0.1.18/examples/user/grid_search_params_greeating.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import ModelType
 from genai.utils.search_space_params import grid_search_generate_params
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint> (optional) DEFAULT_API = "https://workbench-api.res.ibm.com/v1"
 load_dotenv()
 API_KEY = os.getenv("GENAI_KEY", None)
@@ -32,15 +31,15 @@
 greeting1 = "Hello! How are you?"
 greeting2 = "I am fine and you?"
 
 # generate all combinations of parameters, returns a list of GenerateParams
 generate_params_list = grid_search_generate_params(my_space_params)
 
 for params in generate_params_list:
-    model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+    model = Model("google/flan-ul2", params=params, credentials=creds)
     responses = model.generate_as_completed([greeting1, greeting2] * 4)
 
     print(f"Used params: \n{params} \n")
 
     print(greeting1)
     print(greeting2)
     for response in responses:
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/history.py` & `ibm-generative-ai-0.1.18/examples/user/history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/jsonprompt.py` & `ibm-generative-ai-0.1.18/examples/user/jsonprompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -26,15 +26,15 @@
     temperature=0.7,
     top_k=50,
     top_p=1,
     random_seed=2,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 pt = PromptPattern.from_file(str(PATH) + os.sep + "templates" + os.sep + "instruction.yaml")
 print("\nGiven template:\n", pt)
 
 json_path = str(PATH) + os.sep + "assets" + os.sep + "seed_tasks.jsonl"
 mapping = {
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/jsonprompt_multi.py` & `ibm-generative-ai-0.1.18/examples/user/jsonprompt_multi.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -26,15 +26,15 @@
     temperature=0.7,
     top_k=50,
     top_p=1,
     random_seed=2,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 # load prompt pattern from file
 pt = PromptPattern.from_file(str(PATH) + os.sep + "templates" + os.sep + "instruction.yaml")
 print("\nGiven template:\n", pt)
 
 json_path = str(PATH) + os.sep + "assets" + os.sep + "seed_tasks.jsonl"
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/langchain_qa.py` & `ibm-generative-ai-0.1.18/examples/user/langchain_qa.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     from langchain import PromptTemplate
     from langchain.chains import LLMChain, SimpleSequentialChain
 except ImportError:
     raise ImportError("Could not import langchain: Please install ibm-generative-ai[langchain] extension.")
 
 from genai.credentials import Credentials
 from genai.extensions.langchain import LangChainInterface
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
 
@@ -32,13 +32,13 @@
 pt2 = PromptTemplate(
     input_variables=["question"],
     template="Answer the following question: {question}",
 )
 
 
 creds = Credentials(api_key, api_endpoint)
-flan = LangChainInterface(model=ModelType.FLAN_UL2, credentials=creds, params=params)
-model = LangChainInterface(model=ModelType.FLAN_UL2, credentials=creds)
+flan = LangChainInterface(model="google/flan-ul2", credentials=creds, params=params)
+model = LangChainInterface(model="google/flan-ul2", credentials=creds)
 prompt_to_flan = LLMChain(llm=flan, prompt=pt1)
 flan_to_model = LLMChain(llm=model, prompt=pt2)
 qa = SimpleSequentialChain(chains=[prompt_to_flan, flan_to_model], verbose=True)
 qa.run("life")
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/localserver/localserver.py` & `ibm-generative-ai-0.1.18/examples/user/localserver/localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/logprob_returns.py` & `ibm-generative-ai-0.1.18/examples/user/logprob_returns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType, ReturnOptions
+from genai.schemas import GenerateParams, ReturnOptions
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -23,15 +23,15 @@
     temperature=0.7,
     top_k=50,
     top_p=1,
     return_options=ReturnOptions(generated_tokens=True, token_logprobs=True, input_text=True),
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting1 = "Hello! How are you?"
 greeting2 = "I am fine and you?"
 
 # Call generate function
 responses = model.generate_as_completed([greeting1, greeting2] * 4)
 for response in responses:
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/many_greetings.py` & `ibm-generative-ai-0.1.18/examples/user/prompt_reuse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import os
+import pathlib
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.prompt_pattern import PromptPattern
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
+PATH = pathlib.Path(__file__).parent.resolve()
 
 print("\n------------- Example (Greetings)-------------\n")
 
 params = GenerateParams(
     decoding_method="sample",
     max_new_tokens=10,
     min_new_tokens=1,
     stream=False,
     temperature=0.7,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
-greeting1 = "Hello! How are you?"
-greeting2 = "I am fine and you?"
-
-# Call generate function
-responses = model.generate_as_completed([greeting1, greeting2] * 4)
+# can live locally or at an url endpoint
+pt = PromptPattern.from_file(str(PATH) + os.sep + "templates" + os.sep + "capital-qa.yaml")
+pt.sub("country", "Spain")
+print(pt)
+responses = model.generate_as_completed([str(pt)])
 for response in responses:
     print(f"Generated text: {response.generated_text}")
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/model_as_string.py` & `ibm-generative-ai-0.1.18/examples/user/model_as_string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/prompt-raw-string.py` & `ibm-generative-ai-0.1.18/examples/user/prompt-raw-string.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -23,15 +23,15 @@
     stream=False,
     temperature=0.7,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 # can live locally or at an url endpoint
 pt = PromptPattern.from_str("The capital of {{country}} is {{capital}}. The capital of Taiwan is")
 pt.sub("capital", "Madrid").sub("country", "Spain")
 
 print(pt)
 responses = model.generate_async([str(pt)])
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/prompt_csv_random_rows.py` & `ibm-generative-ai-0.1.18/examples/user/prompt_csv_random_rows.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 #
 # In this demo, the following dataset was used:
 #
 # Gorman KB, Williams TD, Fraser WR (2014) "Ecological Sexual Dimorphism and Environmental Variability within a Community of Antarctic Penguins (Genus Pygoscelis)." PLoS ONE 9(3): e90081. doi:10.1371/journal.pone.0090081 # noqa
 
 # make sure you have a .env file under genai root with
@@ -27,15 +27,15 @@
     decoding_method="greedy",
     max_new_tokens=15,
     min_new_tokens=1,
     stream=False,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 pt = PromptPattern.from_file(str(PATH) + os.sep + "templates" + os.sep + "synth-animal.yaml")
 print("\nGiven template:\n", pt)
 
 pt.sub("animal", "penguins")
 cvs_path = str(PATH) + os.sep + "assets" + os.sep + "penguins.csv"
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/prompt_from_all_csv.py` & `ibm-generative-ai-0.1.18/examples/user/prompt_from_all_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 #
 # In this demo, the following dataset was used:
 #
 # Gorman KB, Williams TD, Fraser WR (2014) "Ecological Sexual Dimorphism and Environmental Variability within a Community of Antarctic Penguins (Genus Pygoscelis)." PLoS ONE 9(3): e90081. doi:10.1371/journal.pone.0090081  # noqa
 
 # make sure you have a .env file under genai root with
@@ -27,30 +27,30 @@
     decoding_method="greedy",
     max_new_tokens=15,
     min_new_tokens=1,
     stream=False,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 
-pt = PromptPattern.from_file(str(PATH) + os.sep + "templates" + os.sep + "synth-animal.yaml")
-print("\nGiven template:\n", pt)
+prompt = PromptPattern.from_file(str(PATH) + os.sep + "templates" + os.sep + "synth-animal.yaml")
+print("\nGiven template:\n", prompt)
 
-pt.sub("animal", "penguins")
+prompt.sub("animal", "penguins")
 csv_path = str(PATH) + os.sep + "assets" + os.sep + "penguins.csv"
 mapping = {
     "species": ["species1", "species2", "species3"],
     "island": ["location1", "location2", "location3"],
     "flipper_length_mm": ["length1", "length2", "length3"],
     "year": ["dob1", "dob2", "dob3"],
 }
 
-list_of_prompts = pt.sub_all_from_csv(
+list_of_prompts = prompt.sub_all_from_csv(
     csv_path=csv_path,
     col_to_var=mapping,
 )
 
 print("-----------------------")
 print("generated prompt")
 print(list_of_prompts)
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/prompt_from_all_dataframe.py` & `ibm-generative-ai-0.1.18/examples/user/prompt_from_all_dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from dotenv import load_dotenv
 
 import genai.extensions.pandas  # noqa: F401
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 #
 # In this demo, the following dataset was used:
 #
 # Gorman KB, Williams TD, Fraser WR (2014) "Ecological Sexual Dimorphism and Environmental Variability within a Community of Antarctic Penguins (Genus Pygoscelis)." PLoS ONE 9(3): e90081. doi:10.1371/journal.pone.0090081 # noqa
 
 
@@ -34,15 +34,15 @@
     decoding_method="greedy",
     max_new_tokens=15,
     min_new_tokens=1,
     stream=False,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 pt = PromptPattern.from_file(str(PATH) + os.sep + "templates" + os.sep + "synth-animal.yaml")
 print("\nGiven template:\n", pt)
 
 csv_path = str(PATH) + os.sep + "assets" + os.sep + "penguins2.csv"
 df = pd.read_csv(csv_path, index_col=0)
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/prompt_from_dataframe.py` & `ibm-generative-ai-0.1.18/examples/user/prompt_from_dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from dotenv import load_dotenv
 
 import genai.extensions.pandas  # noqa: F401
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 #
 # In this demo, the following dataset was used:
 #
 # Gorman KB, Williams TD, Fraser WR (2014) "Ecological Sexual Dimorphism and Environmental Variability within a Community of Antarctic Penguins (Genus Pygoscelis)." PLoS ONE 9(3): e90081. doi:10.1371/journal.pone.0090081 # noqa
 
 # make sure you have a .env file under genai root with
@@ -33,15 +33,15 @@
     decoding_method="greedy",
     max_new_tokens=15,
     min_new_tokens=1,
     stream=False,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 
 csv_path = str(PATH) + os.sep + "assets" + os.sep + "penguins.csv"
 df = pd.read_csv(csv_path, index_col=0)
 
 pt = PromptPattern.from_str("{{species}}: {{island}}, {{flipper_length_mm}}, {{year}}\n")
 list_of_prompts = pt.pandas.sub_from_dataframe(dataframe=df, start_index=15, n=2, strategy="sample")
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py` & `ibm-generative-ai-0.1.18/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py` & `ibm-generative-ai-0.1.18/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/saving_prompts_as_hf_dataset.py` & `ibm-generative-ai-0.1.18/examples/user/saving_prompts_as_hf_dataset.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/self-reflection.py` & `ibm-generative-ai-0.1.18/examples/user/self-reflection.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
 from genai.prompt_pattern import PromptPattern
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -22,15 +22,15 @@
     decoding_method="greedy",
     max_new_tokens=20,
     min_new_tokens=1,
     stream=False,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 # (1) Prompt
 prompt = "Is McDonald's or Burger King better?"
 
 print("INPUT>> " + prompt + "\n")
 responses = model.generate([prompt])
 gen_response = responses[0].generated_text.strip()
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/self_instruct.py` & `ibm-generative-ai-0.1.18/examples/user/self_instruct.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/examples/user/streaming.py` & `ibm-generative-ai-0.1.18/examples/user/streaming.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType, ReturnOptions
+from genai.schemas import GenerateParams, ReturnOptions
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -18,15 +18,15 @@
 
 # Instantiate parameters for text generation
 params = GenerateParams(
     decoding_method="sample", max_new_tokens=500, min_new_tokens=10, return_options=ReturnOptions(generated_tokens=True)
 )
 
 # Instantiate a model proxy object to send your requests
-flan_ul2 = Model(ModelType.FLAN_UL2_20B, params=params, credentials=creds)
+flan_ul2 = Model("google/flan-ul2", params=params, credentials=creds)
 
 prompts = [" Explain life in one sentence"]
 count = 0
 
 for response in flan_ul2.generate_stream(prompts):
     print(response.input_token_count) if count == 0 else print(response.generated_text)
     count = count + 1
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/tokenize-sync.py` & `ibm-generative-ai-0.1.18/examples/user/tokenize-sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import ModelType, TokenParams
+from genai.schemas import TokenParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
 
 print("\n------------- Example (Tokenize)-------------\n")
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=TokenParams, credentials=creds)
+model = Model("google/flan-ul2", params=TokenParams, credentials=creds)
 
 sentence = "Hello! How are you?"
 
 tokenized_response = model.tokenize([sentence], return_tokens=True)
 print(f"Tokenized response: {tokenized_response}")
```

### Comparing `ibm-generative-ai-0.1.17/examples/user/tokens.py` & `ibm-generative-ai-0.1.18/examples/user/tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -22,15 +22,15 @@
     stream=False,
     temperature=0.7,
     top_k=50,
     top_p=1,
 )
 
 creds = Credentials(api_key, api_endpoint)
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting1 = "Hello! How are you?"
 greeting2 = "I am fine and you?"
 
 # just get the token counts
 responses = model.tokenize_as_completed([greeting1, greeting2])
 for response in responses:
```

### Comparing `ibm-generative-ai-0.1.17/pyproject.toml` & `ibm-generative-ai-0.1.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/credentials.py` & `ibm-generative-ai-0.1.18/src/genai/credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/exceptions/genai_exception.py` & `ibm-generative-ai-0.1.18/src/genai/exceptions/genai_exception.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/extensions/huggingface/save_huggingface.py` & `ibm-generative-ai-0.1.18/src/genai/extensions/huggingface/save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/extensions/langchain/llm.py` & `ibm-generative-ai-0.1.18/src/genai/extensions/langchain/llm.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/extensions/langchain/prompt.py` & `ibm-generative-ai-0.1.18/src/genai/extensions/langchain/prompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/extensions/localserver/custom_model_interface.py` & `ibm-generative-ai-0.1.18/src/genai/extensions/localserver/custom_model_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/extensions/localserver/local_api_server.py` & `ibm-generative-ai-0.1.18/src/genai/extensions/localserver/local_api_server.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/extensions/pandas/prompt_sub.py` & `ibm-generative-ai-0.1.18/src/genai/extensions/pandas/prompt_sub.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/metadata.py` & `ibm-generative-ai-0.1.18/src/genai/metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/model.py` & `ibm-generative-ai-0.1.18/src/genai/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, Callable, Union
 
 from tqdm import tqdm
 
 from genai.credentials import Credentials
 from genai.exceptions import GenAiException
 from genai.metadata import Metadata
+from genai.options import Options
 from genai.prompt_pattern import PromptPattern
 from genai.schemas import GenerateParams, ModelType, TokenParams
 from genai.schemas.responses import (
     GenerateResponse,
     GenerateResult,
     GenerateStreamResponse,
     TokenizeResponse,
@@ -36,24 +37,26 @@
             credentials (Credentials): The API Credentials
         """
         logger.debug(f"Model Created:  Model: {model}, endpoint: {credentials.api_endpoint}")
         self.model = model
         self.params = params
         self.service = ServiceInterface(service_url=credentials.api_endpoint, api_key=credentials.api_key)
 
-    def generate_stream(self, prompts: Union[list[str], list[PromptPattern]]) -> Generator[GenerateStreamResponse]:
+    def generate_stream(
+        self, prompts: Union[list[str], list[PromptPattern]], options: Options = None
+    ) -> Generator[GenerateStreamResponse]:
         if len(prompts) > 0 and isinstance(prompts[0], PromptPattern):
             prompts = PromptPattern.list_str(prompts)
 
         try:
             for i in range(0, len(prompts), Metadata.DEFAULT_MAX_PROMPTS):
                 batch = prompts[i : min(i + Metadata.DEFAULT_MAX_PROMPTS, len(prompts))]
 
                 self.params.stream = True
-                response_gen = self.service.generate(self.model, batch, self.params, streaming=True)
+                response_gen = self.service.generate(self.model, batch, self.params, options=options, streaming=True)
 
                 for chunk in response_gen:
                     if "status_code" in chunk:
                         error = ast.literal_eval(chunk)
                         raise GenAiException(error)
 
                     # we assume the returned string from the service is of shape "data: {...}"
@@ -66,37 +69,41 @@
                         logger.error("Could not parse {} as literal_eval".format(response))
 
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
 
-    def generate_as_completed(self, prompts: Union[list[str], list[PromptPattern]]) -> Generator[GenerateResponse]:
+    def generate_as_completed(
+        self, prompts: Union[list[str], list[PromptPattern]], options: Options = None
+    ) -> Generator[GenerateResponse]:
         """The generate endpoint is the centerpiece of the GENAI alpha.
         It provides a simplified and flexible, yet powerful interface to the supported
         models as a service. Given a text prompt as inputs, and required parameters
         the selected model (model_id) will generate a completion text as generated_text.
 
         Args:
             prompts (list[str]): The list of one or more prompt strings.
+            options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Yields:
             Generator[GenerateResult]: A generator of results
         """
         if len(prompts) > 0 and isinstance(prompts[0], PromptPattern):
             prompts = PromptPattern.list_str(prompts)
 
         logger.debug(f"Calling Generate. Prompts: {prompts}, params: {self.params}")
 
         try:
             for i in range(0, len(prompts), Metadata.DEFAULT_MAX_PROMPTS):
                 response_gen = self.service.generate(
-                    self.model,
-                    prompts[i : min(i + Metadata.DEFAULT_MAX_PROMPTS, len(prompts))],
-                    self.params,
+                    model=self.model,
+                    inputs=prompts[i : min(i + Metadata.DEFAULT_MAX_PROMPTS, len(prompts))],
+                    params=self.params,
+                    options=options,
                 )
                 if response_gen.status_code == 200:
                     response_gen = response_gen.json()
                     for y, result in enumerate(response_gen["results"]):
                         result["input_text"] = prompts[i + y]
                     responses = GenerateResponse(**response_gen)
                     for result in responses.results:
@@ -104,61 +111,66 @@
                 else:
                     raise GenAiException(response_gen)
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
 
-    def generate(self, prompts: Union[list[str], list[PromptPattern]]) -> list[GenerateResponse]:
+    def generate(
+        self, prompts: Union[list[str], list[PromptPattern]], options: Options = None
+    ) -> list[GenerateResponse]:
         """The generate endpoint is the centerpiece of the GENAI alpha.
         It provides a simplified and flexible, yet powerful interface to the supported
         models as a service. Given a text prompt as inputs, and required parameters
         the selected model (model_id) will generate a completion text as generated_text.
 
         Args:
             prompts (list[str]): The list of one or more prompt strings.
+            options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Returns:
             list[GenerateResult]: A list of results
         """
-        return list(self.generate_as_completed(prompts))
+        return list(self.generate_as_completed(prompts, options))
 
     def generate_async(
         self,
         prompts: Union[list[str], list[PromptPattern]],
         ordered: bool = False,
         callback: Callable[[GenerateResult], Any] = None,
         hide_progressbar: bool = False,
+        options: Options = None,
     ) -> Generator[Union[GenerateResult, None]]:
         """The generate endpoint is the centerpiece of the GENAI alpha.
         It provides a simplified and flexible, yet powerful interface to the supported
         models as a service. Given a text prompt as inputs, and required parameters
         the selected model (model_id) will generate a completion text as generated_text.
         This python method generates responses utilizing async capabilities and returns
         responses as they arrive.
 
         Args:
             prompts (list[str]): The list of one or more prompt strings.
             ordered (bool): Whether the responses should be returned in-order.
             callback (Callable[[GenerateResult], Any]): Optional callback
                 to be called after generating result for a prompt.
-            hide_progressbar: boolean flag to hide or show a progress bar.
+            hide_progressbar (bool, optional): boolean flag to hide or show a progress bar.
                 By defaul bar will be always shown.
+            options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Returns:
             Generator[Union[GenerateResult, None]]: A list of results
         """
         if len(prompts) > 0 and isinstance(prompts[0], PromptPattern):
             prompts = PromptPattern.list_str(prompts)
 
         logger.debug(f"Calling Generate Async. Prompts: {prompts}, params: {self.params}")
 
         try:
             with AsyncResponseGenerator(
-                self.model, prompts, self.params, self.service, ordered=ordered, callback=callback
+                self.model, prompts, self.params, self.service, ordered=ordered, callback=callback, options=options
             ) as asynchelper:
                 for response in tqdm(
                     asynchelper.generate_response(),
                     total=len(prompts),
                     desc="Progress",
                     unit=" inputs",
                     disable=hide_progressbar,
@@ -166,15 +178,15 @@
                     yield response
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
 
     def tokenize_as_completed(
-        self, prompts: Union[list[str], list[PromptPattern]], return_tokens: bool = False
+        self, prompts: Union[list[str], list[PromptPattern]], return_tokens: bool = False, options: Options = None
     ) -> Generator[TokenizeResult]:
         """The tokenize endpoint allows you to check the conversion of provided prompts to tokens
         for a given model. It splits text into words or subwords, which then are converted to ids
         through a look-up table (vocabulary). Tokenization allows the model to have a reasonable
         vocabulary size.
 
         Args:
@@ -186,17 +198,18 @@
         if len(prompts) > 0 and isinstance(prompts[0], PromptPattern):
             prompts = PromptPattern.list_str(prompts)
 
         try:
             params = TokenParams(return_tokens=return_tokens)
             for i in range(0, len(prompts), Metadata.DEFAULT_MAX_PROMPTS):
                 tokenize_response = self.service.tokenize(
-                    self.model,
-                    prompts[i : min(i + Metadata.DEFAULT_MAX_PROMPTS, len(prompts))],
-                    params,
+                    model=self.model,
+                    inputs=prompts[i : min(i + Metadata.DEFAULT_MAX_PROMPTS, len(prompts))],
+                    params=params,
+                    options=options,
                 )
 
                 if tokenize_response.status_code == 200:
                     response_json = tokenize_response.json()
                     for y, result in enumerate(response_json["results"]):
                         result["input_text"] = prompts[i + y]
                     responses = TokenizeResponse(**response_json)
@@ -207,58 +220,69 @@
                     raise GenAiException(tokenize_response)
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
 
     def tokenize(
-        self, prompts: Union[list[str], list[PromptPattern]], return_tokens: bool = False
+        self, prompts: Union[list[str], list[PromptPattern]], return_tokens: bool = False, options: Options = None
     ) -> list[TokenizeResult]:
         """The tokenize endpoint allows you to check the conversion of provided prompts to tokens
         for a given model. It splits text into words or subwords, which then are converted to ids
         through a look-up table (vocabulary). Tokenization allows the model to have a reasonable
         vocabulary size.
 
         Args:
             prompts (list[str]): The list of one or more prompt strings.
             return_tokens (bool, optional): Return tokens with the response. Defaults to False.
 
         Returns:
             list[TokenizeResult]: The Tokenized input
         """
-        return list(self.tokenize_as_completed(prompts, return_tokens))
+        return list(self.tokenize_as_completed(prompts, return_tokens, options=options))
 
     def tokenize_async(
         self,
         prompts: Union[list[str], list[PromptPattern]],
         ordered: bool = False,
         callback: Callable[[TokenizeResult], Any] = None,
+        return_tokens: bool = False,
+        options: Options = None,
     ) -> Generator[Union[TokenizeResult, None]]:
         """The tokenize endpoint allows you to check the conversion of provided prompts to tokens
         for a given model. It splits text into words or subwords, which then are converted to ids
         through a look-up table (vocabulary). Tokenization allows the model to have a reasonable
         vocabulary size. This python method utilizes async capabilities and returns
         responses as they arrive.
 
         Args:
             prompts (list[str]): The list of one or more prompt strings.
             ordered (bool): Whether the responses should be returned in-order.
             callback (Callable[[TokenizeResult], Any]): Callback to call for each result.
+            return_tokens (bool, optional): Return tokens with the response. Defaults to False.
 
         Returns:
             Generator[Union[TokenizeResult, None]]: The Tokenized input
         """
         if len(prompts) > 0 and isinstance(prompts[0], PromptPattern):
             prompts = PromptPattern.list_str(prompts)
 
         logger.debug(f"Calling Tokenize Async. Prompts: {prompts}, params: {self.params}")
 
         try:
+            params = TokenParams(return_tokens=return_tokens)
             with AsyncResponseGenerator(
-                self.model, prompts, self.params, self.service, fn="tokenize", ordered=ordered, callback=callback
+                self.model,
+                prompts,
+                params,
+                self.service,
+                fn="tokenize",
+                ordered=ordered,
+                callback=callback,
+                options=options,
             ) as asynchelper:
                 for response in asynchelper.generate_response():
                     yield response
         except GenAiException as me:
             raise me
         except Exception as ex:
             raise GenAiException(ex)
```

### Comparing `ibm-generative-ai-0.1.17/src/genai/prompt_pattern.py` & `ibm-generative-ai-0.1.18/src/genai/prompt_pattern.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 import re
 from typing import Literal, Union
 
 import requests
 from yaml import CLoader as Loader
 from yaml import load
 
+from genai import Credentials
 from genai.exceptions import GenAiException
+from genai.schemas.responses import WatsonxTemplate
+from genai.services import PromptTemplateManager
 from genai.utils.json_utils import json_extract, json_get_all_keys, json_load
 
 
 class PromptPattern:
     _accessors = set()
 
     def _create(self, *args, **kwargs):
         self.url: str = None
         self.literal: bool = False
         self.dump = None
         self.yaml = None
         self.token: str = None
 
+        self.watsonx: WatsonxTemplate = None
+        self.credentials: Credentials = None
+
         for key, value in kwargs.items():
             setattr(self, key, value)
 
         self.raw_content = self._fetch_prompt()
 
     @classmethod
     def from_url(cls, url: str, token=""):
@@ -71,14 +77,40 @@
         Returns:
             PromptPattern: Returns the created PromptPattern instance.
         """
         pt = PromptPattern()
         pt._create(url=prompt, literal=True)
         return pt
 
+    @classmethod
+    def from_watsonx(cls, credentials: Credentials, name: str = None, template: dict = None, id: str = None):
+        # Cases :
+        # fetching an existing template : name OR id
+        # updating an existing template : template + (name OR id)
+        # creating a new template       : template + name
+
+        if not template:
+            wx = PromptTemplateManager.load_template(credentials=credentials, id=id, name=name)
+            pt = PromptPattern()
+            pt._create(url=wx.value, watsonx=wx, credentials=credentials, literal=True)
+            return pt
+
+        try:
+            saved_template = PromptTemplateManager.load_template(credentials=credentials, id=id, name=name)
+            id = saved_template.id
+            name = name if name else saved_template.name
+            wx = PromptTemplateManager.update_template(credentials=credentials, id=id, name=name, template=template)
+        except Exception:
+            # Template with name doesn't exist. Save template
+            wx = PromptTemplateManager.save_template(template=template, name=name, credentials=credentials)
+
+        pt = PromptPattern()
+        pt._create(url=wx.value, watsonx=wx, credentials=credentials, literal=True)
+        return pt
+
     def _fetch_prompt(self):
         """
         Gets the raw content as a string at the path indicated by the url.
         The url can point to any http endpoint or a local path
 
         Returns:
             str: Contents of file located at url as a str
@@ -548,20 +580,38 @@
             complete_pt = self._sub_from_tabular_data(data, columns, col_to_var, start_index, n, strategy)
 
         # if n == 1, return a single PromptPattern
         self._return_single_prompt_from_completed_list(complete_pt, n)
 
         return complete_pt
 
+    def render(self, inputs, data):
+        if not self.watsonx:
+            raise GenAiException("Method only available for watsonx prompt templates.")
+
+        _data = {}
+        _data["value"] = self.watsonx.value
+        _data["data"] = data
+
+        return PromptTemplateManager.render_watsonx_prompts(credentials=self.credentials, inputs=inputs, data=_data)
+
+    def delete(self) -> str:
+        if not self.watsonx:
+            raise GenAiException("Method only available for watsonx prompt templates.")
+        return PromptTemplateManager.delete_template(credentials=self.credentials, id=self.watsonx.id)
+
     def __str__(self):
         return self.dump
 
     def __repr__(self):
         return self.dump
 
+    def __contains__(self, val):
+        return self.__dict__.__contains__(val)
+
     @staticmethod
     def list_str(list_of_prompts: list["PromptPattern"]) -> list[str]:
         return [str(x) for x in list_of_prompts]
 
     @staticmethod
     def validate_start_index(strategy, start_index, data):
         if strategy == "sequential" and start_index >= len(data):
```

### Comparing `ibm-generative-ai-0.1.17/src/genai/schemas/__init__.py` & `ibm-generative-ai-0.1.18/src/genai/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/schemas/descriptions.py` & `ibm-generative-ai-0.1.18/src/genai/schemas/descriptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,25 +20,21 @@
     # Params.Generate
     DECODING_METHOD = (
         "Decoding method used for generation. Options are greedy or sample. Defaults to sample if not specified."
     )
     LENGTH_PENALTY = "It can be used to exponentially increase the likelihood of the text generation terminating once a specified number of tokens have been generated."
     MAX_NEW_TOKEN = "The maximum number of new tokens to be generated. The range is 1 to 1024, defaults to 20."
     MIN_NEW_TOKEN = "If stop sequences are given, they are ignored until minimum tokens are generated."
-    RANDOM_SEED = (
-        "Manually passed seed to initialize the randomization for experimental repeatability. The range is 1 to 9999."
-    )
+    RANDOM_SEED = "Manually passed seed to initialize the randomization for experimental repeatability. The range is 1 to 9999. Valid only with decoding_method=sample."
     STOP_SQUENCES = "Stop sequences are one or more strings which will cause the text generation to stop if/when they are produced as part of the output. Stop sequences encountered prior to the minimum number of tokens being generated will be ignored."
     STREAM = "Enables to stream partial progress as server-sent events. Defaults to false."
-    TEMPERATURE = "The value used to module the next token probabilities. The range is 0.00 to 2.00, a value set to 0.00 would make it deterministic."
+    TEMPERATURE = "The value used to module the next token probabilities. The range is 0.05 to 2.00, a value set to 0.05 would make it deterministic. Valid only with decoding_method=sample."
     TIME_LIMIT = "Time limit in milliseconds - if not completed within this time, generation will stop. The text generated so far will be returned along with the TIME_LIMIT stop reason."
-    TOP_K = (
-        "The number of highest probability vocabulary tokens to keep for top-k-filtering. The range is any value >= 1."
-    )
-    TOP_P = "If set to value < 1, only the most probable tokens with probabilities that add up to top_p or higher are kept for generation. The range is 0.00 to 1.00."
+    TOP_K = "The number of highest probability vocabulary tokens to keep for top-k-filtering. The range is any value >= 1. Valid only with decoding_method=sample."
+    TOP_P = "If set to value < 1, only the most probable tokens with probabilities that add up to top_p or higher are kept for generation. The range is 0.00 to 1.00. Valid only with decoding_method=sample."
     REPETITION_PENALTY = "The parameter for repetition penalty. 1.0 means no penalty."
     TRUNCATE_INPUT_TOKENS = "Truncate to this many input tokens. Can be used to avoid requests failing due to input being longer than configured limits. Zero means don't truncate."
 
     # Params.Token
     RETURN_TOKEN = "Return tokens with the response. Defaults to false."
 
     # Params.History
```

### Comparing `ibm-generative-ai-0.1.17/src/genai/schemas/generate_params.py` & `ibm-generative-ai-0.1.18/src/genai/schemas/generate_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/schemas/history_params.py` & `ibm-generative-ai-0.1.18/src/genai/schemas/history_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/schemas/models.py` & `ibm-generative-ai-0.1.18/src/genai/schemas/models.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/schemas/responses.py` & `ibm-generative-ai-0.1.18/src/genai/schemas/responses.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,7 +139,24 @@
 
 
 class ErrorResponse(GenAiResponseModel):
     status_code: int
     error: str
     message: str
     extensions: Optional[ErrorExtensions]
+
+
+class WatsonxTemplate(GenAiResponseModel):
+    id: str
+    name: str
+    value: str
+    created_at: datetime
+    data: Optional[dict]
+
+
+class WatsonxTemplatesResponse(GenAiResponseModel):
+    results: list[WatsonxTemplate]
+    totalCount: int
+
+
+class WatsonxRenderedPrompts(GenAiResponseModel):
+    results: list[str]
```

### Comparing `ibm-generative-ai-0.1.17/src/genai/services/async_generator.py` & `ibm-generative-ai-0.1.18/src/genai/services/async_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import asyncio
 import heapq
 import logging
 from concurrent.futures import ThreadPoolExecutor
 from queue import Queue
 
 from genai.exceptions import GenAiException
+from genai.options import Options
 from genai.schemas.responses import GenerateResponse, TokenizeResponse
 from genai.services.connection_manager import ConnectionManager
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["AsyncResponseGenerator"]
 
 
 class AsyncResponseGenerator:
-    def __init__(self, model_id, prompts, params, service, fn="generate", ordered=False, callback=None):
+    def __init__(
+        self, model_id, prompts, params, service, fn="generate", ordered=False, callback=None, options: Options = None
+    ):
         """Instantiates the ConcurrentWrapper Interface.
 
         Args:
             model_id (ModelType): The type of model to use
             prompts (list): List of prompts
             params (GenerateParams): Parameters to use during generate requests
             service (ServiceInterface): The service interface
@@ -28,14 +31,15 @@
         self.model_id = model_id
         self.prompts = prompts
         self.params = params
         self.service = service
         self.callback = callback
         self.fn = fn
         self.ordered = ordered
+        self.options = options
 
     def __enter__(self):
         self.accumulator = []
         self._initialize_fn_specific_params()
         self.queue_ = Queue()
         self.loop_ = asyncio.new_event_loop()
         return self
@@ -60,22 +64,24 @@
 
     def _initialize_fn_specific_params(self):
         if self.fn == "generate":
             self.batch_size_ = 1
             self.num_batches_ = len(self.prompts)
             self.message_type_ = GenerateResponse
             self.service_fn_ = self.service.async_generate
+            self.max_active_tasks_ = ConnectionManager.MAX_CONCURRENT_GENERATE
             ConnectionManager.make_generate_client()
             self.client_close_fn_ = ConnectionManager.delete_generate_client
         elif self.fn == "tokenize":
             self.batch_size_ = 5
             a, b = divmod(len(self.prompts), self.batch_size_)
             self.num_batches_ = a + (b > 0)
             self.message_type_ = TokenizeResponse
             self.service_fn_ = self.service.async_tokenize
+            self.max_active_tasks_ = ConnectionManager.MAX_REQ_PER_SECOND_TOKENIZE
             ConnectionManager.make_tokenize_client()
             self.client_close_fn_ = ConnectionManager.delete_tokenize_client
 
     def _generate_batch(self):
         for i in range(0, len(self.prompts), self.batch_size_):
             yield self.prompts[i : min(i + self.batch_size_, len(self.prompts))]
 
@@ -83,54 +89,57 @@
         if response is None:
             for _ in range(batch_size):
                 yield None
         else:
             for result in response.results:
                 yield result
 
-    async def _get_response_json(self, model, inputs, params):
+    async def _get_response_json(self, model, inputs, params, options):
         try:
-            response_raw = await self.service_fn_(model, inputs, params)
+            response_raw = await self.service_fn_(model, inputs, params, options)
             response = response_raw.json()
         except Exception as ex:
             logger.error("Error in _get_response_json {}: {}".format(type(ex), str(ex)))
             response = None
         return response
 
     async def _task(self, inputs, batch_num):
-        response = None
-        try:
-            response = await self._get_response_json(self.model_id, inputs, self.params)
-            logger.debug("Received response = {}".format(response))
-            for i in range(len(response["results"])):
-                response["results"][i]["input_text"] = inputs[i]
-            response = self.message_type_(**response)
-            logger.debug("Cast to Response = {}".format(response))
-        except Exception as e:
-            logger.error(
-                "Exception raised async_generate and casting : {}, response = {}, inputs = {}".format(
-                    str(e), response, inputs
+        async with self.semaphore_:
+            response = None
+            try:
+                response = await self._get_response_json(self.model_id, inputs, self.params, self.options)
+                logger.debug("Received response = {}".format(response))
+                for i in range(len(response["results"])):
+                    response["results"][i]["input_text"] = inputs[i]
+                response = self.message_type_(**response)
+                logger.debug("Cast to Response = {}".format(response))
+            except Exception as e:
+                logger.error(
+                    "Exception raised async_generate and casting : {}, response = {}, inputs = {}".format(
+                        str(e), response, inputs
+                    )
+                )
+                self.queue_.put_nowait((batch_num, len(inputs), None))
+                return
+            try:
+                self.queue_.put_nowait((batch_num, len(inputs), response))
+                if self.callback is not None:
+                    for result in response.results:
+                        self.callback(result)
+            except Exception as e:
+                logger.error(
+                    "Exception raised in callback : {}, response = {}, inputs = {}".format(str(e), response, inputs)
                 )
-            )
-            self.queue_.put_nowait((batch_num, len(inputs), None))
-            return
-        try:
-            self.queue_.put_nowait((batch_num, len(inputs), response))
-            if self.callback is not None:
-                for result in response.results:
-                    self.callback(result)
-        except Exception as e:
-            logger.error(
-                "Exception raised in callback : {}, response = {}, inputs = {}".format(str(e), response, inputs)
-            )
 
     async def _schedule_requests(self):
         tasks = []
         batch_num = 0
+        self.semaphore_ = asyncio.Semaphore(self.max_active_tasks_)
         for batch in self._generate_batch():
+            logger.debug("Creating task for batch_num {}".format(batch_num))
             task = asyncio.create_task(self._task(batch, batch_num))
             tasks.append(task)
             batch_num += 1
         await asyncio.gather(*tasks)
 
     def _request_launcher(self):
         asyncio.set_event_loop(self.loop_)
```

### Comparing `ibm-generative-ai-0.1.17/src/genai/services/connection_manager.py` & `ibm-generative-ai-0.1.18/src/genai/services/connection_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/services/request_handler.py` & `ibm-generative-ai-0.1.18/src/genai/services/request_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import asyncio
 import logging
 
 import httpx
 from httpx import Response
 
 from genai._version import version
+from genai.options import Options
 from genai.services.connection_manager import ConnectionManager
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["RequestHandler"]
 
 
@@ -15,77 +17,80 @@
     @staticmethod
     def _metadata(
         method: str,
         key: str,
         model_id: str = None,
         inputs: list = None,
         parameters: dict = None,
+        options: Options = None,
     ) -> tuple[dict, dict]:
         """General function to build header and/or json_data for /post and /get requests.
 
         Args:
             method (str): Request type. Currently accepts GET or POST
             key (str): API key for authorization.
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
+            options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Returns:
             tuple[dict,dict]: Headers, json_data for request
         """
 
         headers = {
             "Authorization": f"Bearer {key}",
             "x-request-origin": f"python-sdk/{version}",
         }
         json_data = {}
 
-        if method == "POST":
+        if method == "POST" or method == "PUT":
             headers["Content-Type"] = "application/json"
 
             if model_id is not None:
                 json_data["model_id"] = model_id
 
             if inputs is not None:
                 json_data["inputs"] = inputs
 
             if parameters is not None:
                 json_data["parameters"] = parameters
 
+            if options is not None:
+                for key in options.keys():
+                    json_data[key] = options[key]
+
         if method == "PATCH":
             headers["Content-Type"] = "application/json"
 
         return headers, json_data
 
     @staticmethod
     async def async_post(
         endpoint: str,
         key: str,
         model_id: str = None,
         inputs: list = None,
         parameters: dict = None,
+        options: Options = None,
     ):
         """Low level API for async /post request to REST API.
 
         Args:
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
         headers, json_data = RequestHandler._metadata(
-            method="POST",
-            key=key,
-            model_id=model_id,
-            inputs=inputs,
-            parameters=parameters,
+            method="POST", key=key, model_id=model_id, inputs=inputs, parameters=parameters, options=options
         )
         response = None
         async with httpx.AsyncClient(timeout=ConnectionManager.TIMEOUT) as client:
             response = await client.post(endpoint, headers=headers, json=json_data)
         return response
 
     @staticmethod
@@ -111,72 +116,74 @@
     @staticmethod
     async def async_generate(
         endpoint: str,
         key: str,
         model_id: str = None,
         inputs: list = None,
         parameters: dict = None,
+        options: Options = None,
     ):
         """Low level API for async /generate request to REST API.
 
         Args:
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
         headers, json_data = RequestHandler._metadata(
-            method="POST",
-            key=key,
-            model_id=model_id,
-            inputs=inputs,
-            parameters=parameters,
+            method="POST", key=key, model_id=model_id, inputs=inputs, parameters=parameters, options=options
         )
-        response = await ConnectionManager.async_generate_client.post(endpoint, headers=headers, json=json_data)
+        response = None
+        for attempt in range(0, ConnectionManager.MAX_RETRIES_GENERATE):
+            response = await ConnectionManager.async_generate_client.post(endpoint, headers=headers, json=json_data)
+            if response.status_code in [httpx.codes.SERVICE_UNAVAILABLE, httpx.codes.TOO_MANY_REQUESTS]:
+                await asyncio.sleep(2 ** (attempt + 1))
+            else:
+                break
         return response
 
     @staticmethod
     async def async_tokenize(
         endpoint: str,
         key: str,
         model_id: str = None,
         inputs: list = None,
         parameters: dict = None,
+        options: Options = None,
     ):
         """Low level API for async /tokenize request to REST API.
 
         Args:
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
         """
         headers, json_data = RequestHandler._metadata(
-            method="POST",
-            key=key,
-            model_id=model_id,
-            inputs=inputs,
-            parameters=parameters,
+            method="POST", key=key, model_id=model_id, inputs=inputs, parameters=parameters, options=options
         )
         response = None
-        for _ in range(0, ConnectionManager.MAX_RETRIES_TOKENIZE):
+        for attempt in range(0, ConnectionManager.MAX_RETRIES_TOKENIZE):
             # NOTE: We don't retry-fail with httpx since that'd not
             # not respect the ratelimiting below (5 requests per second).
             # Instead, we do the ratelimiting here with the help of limiter.
             async with ConnectionManager.async_tokenize_limiter:
                 response = await ConnectionManager.async_tokenize_client.post(endpoint, headers=headers, json=json_data)
-                if response.status_code == httpx.codes.OK:
+                if response.status_code in [httpx.codes.SERVICE_UNAVAILABLE, httpx.codes.TOO_MANY_REQUESTS]:
+                    await asyncio.sleep(2 ** (attempt + 1))
+                else:
                     break
         return response
 
     @staticmethod
     async def async_get(endpoint: str, key: str, parameters: dict = None):
         """Low level API for async /get request to REST API.
 
@@ -198,35 +205,33 @@
     def post(
         endpoint: str,
         key: str,
         model_id: str = None,
         inputs: list = None,
         parameters: dict = None,
         streaming: bool = False,
+        options: Options = None,
     ):
         """Low level API for /post request to REST API.
 
         Args:
             endpoint (str): Remote endpoint to be queried.
             key (str): API key for authorization.
             model_id (str, optional): The id of the language model to be queried. Defaults to None.
             inputs (list, optional): List of inputs to be queried. Defaults to None.
             parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
+            options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Returns:
             httpx.Response: Response from the REST API.
             or
             Generator of streamed response payloads from the REST API.
         """
         headers, json_data = RequestHandler._metadata(
-            method="POST",
-            key=key,
-            model_id=model_id,
-            inputs=inputs,
-            parameters=parameters,
+            method="POST", key=key, model_id=model_id, inputs=inputs, parameters=parameters, options=options
         )
 
         if streaming:
             return RequestHandler.post_stream(endpoint=endpoint, headers=headers, json_data=json_data)
         else:
             with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
                 response = s.post(url=endpoint, headers=headers, json=json_data)
@@ -271,7 +276,41 @@
         Returns:
             httpx.Response: Response from the REST API.
         """
         headers, _ = RequestHandler._metadata(method="GET", key=key)
         with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
             response = s.get(url=endpoint, headers=headers, params=parameters)
             return response
+
+    @staticmethod
+    def put(endpoint: str, key: str, options: Options = None) -> Response:
+        """Low level API for /get request to REST API.
+
+        Args:
+            endpoint (str): Remote endpoint to be queried.
+            key (str): API key for authorization.
+            options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
+
+        Returns:
+            requests.models.Response: Response from the REST API.
+        """
+        headers, json_data = RequestHandler._metadata(method="PUT", key=key, options=options)
+        with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
+            response = s.put(url=endpoint, headers=headers, json=json_data)
+            return response
+
+    @staticmethod
+    def delete(endpoint: str, key: str, parameters: dict = None) -> Response:
+        """Low level API for /get request to REST API.
+
+        Args:
+            endpoint (str): Remote endpoint to be queried.
+            key (str): API key for authorization.
+            parameters (dict, optional): Key-value pairs for model parameters. Defaults to None.
+
+        Returns:
+            requests.models.Response: Response from the REST API.
+        """
+        headers, _ = RequestHandler._metadata(method="DELETE", key=key)
+        with httpx.Client(timeout=ConnectionManager.TIMEOUT) as s:
+            response = s.delete(url=endpoint, headers=headers, params=parameters)
+            return response
```

### Comparing `ibm-generative-ai-0.1.17/src/genai/services/service_interface.py` & `ibm-generative-ai-0.1.18/src/genai/services/service_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from httpx import Response
 
 from genai.exceptions import GenAiException
+from genai.options import Options
+from genai.routers import PromptTemplateRouter
 from genai.schemas import GenerateParams, HistoryParams, TokenParams
 from genai.services import RequestHandler
 
 
 class ServiceInterface:
     GENERATE = "/generate"
     TOKENIZE = "/tokenize"
@@ -17,61 +19,63 @@
         Args:
             service_url (str): Base URL for querying.
             api_key (str): User API key for authorization.
             use_async (bool): Use async version of methods
         """
         self.service_url = service_url.rstrip("/")
         self.key = api_key
+        self._prompt_templating = PromptTemplateRouter(service_url=service_url, api_key=api_key)
 
     def generate(
-        self,
-        model: str,
-        inputs: list,
-        params: GenerateParams = None,
-        streaming: bool = False,
+        self, model: str, inputs: list, params: GenerateParams = None, streaming: bool = False, options: Options = None
     ):
         """Generate a completion text for the given model, inputs, and params.
 
         Args:
             model (str): Model id.
             inputs (list): List of inputs.
             params (GenerateParams, optional): Parameters for generation. Defaults to None.
+            streaming (bool, optional): Streaming response flag. Defaults to False.
+            options (Options, optional): Additional parameters to pass in the query payload. Defaults to None.
 
         Returns:
             Any: json from querying for text completion.
         """
         try:
             params = ServiceInterface._sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.GENERATE
             return RequestHandler.post(
                 endpoint,
                 key=self.key,
                 model_id=model,
                 inputs=inputs,
                 parameters=params,
                 streaming=streaming,
+                options=options,
             )
         except Exception as e:
             raise GenAiException(e)
 
-    def tokenize(self, model: str, inputs: list, params: TokenParams = None):
+    def tokenize(self, model: str, inputs: list, params: TokenParams = None, options: Options = None):
         """Do the conversion of provided inputs to tokens for a given model.
 
         Args:
             model (str): Model id.
             inputs (list): List of inputs.
             params (TokenParams, optional): Parameters for generation. Defaults to None.
 
         Returns:
             Any: json from querying for tokenization.
         """
         try:
             params = ServiceInterface._sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.TOKENIZE
-            return RequestHandler.post(endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params)
+            return RequestHandler.post(
+                endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params, options=options
+            )
         except Exception as e:
             raise GenAiException(e)
 
     def history(self, params: HistoryParams = None):
         """Retrieve past generation requests and responses returned by the given models.
 
         Args:
@@ -107,51 +111,51 @@
             return RequestHandler.patch(endpoint, key=self.key, json_data=tou_payload)
         except Exception as e:
             raise GenAiException(e)
 
     # * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
     #   ASYNC
     # * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
-    async def async_generate(self, model, inputs, params: GenerateParams = None):
+    async def async_generate(self, model, inputs, params: GenerateParams = None, options: Options = None):
         """Generate a completion text for the given model, inputs, and params.
 
         Args:
             model (str): Model id.
             inputs (list): List of inputs.
             params (GenerateParams, optional): Parameters for generation. Defaults to None.
 
         Returns:
             Any: json from querying for text completion.
         """
         try:
             params = ServiceInterface._sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.GENERATE
             return await RequestHandler.async_generate(
-                endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params
+                endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params, options=options
             )
         except Exception as e:
             # without VPN this will fail
             raise GenAiException(e)
 
-    async def async_tokenize(self, model, inputs, params: TokenParams = None):
+    async def async_tokenize(self, model, inputs, params: TokenParams = None, options: Options = None):
         """Do the conversion of provided inputs to tokens for a given model.
 
         Args:
             model (str): Model id.
             inputs (list): List of inputs.
             params (TokenParams, optional): Parameters for generation. Defaults to None.
 
         Returns:
             Any: json from querying for tokenization.
         """
         try:
             params = ServiceInterface._sanitize_params(params)
             endpoint = self.service_url + ServiceInterface.TOKENIZE
             return await RequestHandler.async_tokenize(
-                endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params
+                endpoint, key=self.key, model_id=model, inputs=inputs, parameters=params, options=options
             )
         except Exception as e:
             raise GenAiException(e)
 
     async def async_history(self, params: HistoryParams = None):
         """Retrieve past generation requests and responses returned by the given models.
```

### Comparing `ibm-generative-ai-0.1.17/src/genai/utils/extensions.py` & `ibm-generative-ai-0.1.18/src/genai/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/utils/json_utils.py` & `ibm-generative-ai-0.1.18/src/genai/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/genai/utils/search_space_params.py` & `ibm-generative-ai-0.1.18/src/genai/utils/search_space_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/PKG-INFO` & `ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 0.1.17
+Version: 0.1.18
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: langchain
 Provides-Extra: huggingface
@@ -14,15 +14,15 @@
 License-File: LICENSE
 
 # IBM Generative AI Python SDK
 
 
 This is the Python SDK for IBM Foundation Models Studio to bring IBM Generative AI into Python programs and to also extend it with useful operations and types.
 
-:books:	API Documentation: [Link](https://ibm.github.io/ibm-generative-ai/)
+:books:	**API Documentation: [Link](https://ibm.github.io/ibm-generative-ai/)**
 
 *This is an early access library and requires invitation to use the technical preview of [watsonx.ai](https://watsonx.ai/). You can join the waitlist by visiting. https://www.ibm.com/products/watsonx-ai.*
 
 *Looking for the JavaScript/TypeScript version? Check out https://github.com/IBM/ibm-generative-ai-node-sdk.*
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/IBM/ibm-generative-ai/blob/main/LICENSE)
 ![PyPI](https://img.shields.io/pypi/v/ibm-generative-ai)
@@ -112,30 +112,31 @@
 
 ```
 
 
 ## <a name='Examples'></a>Examples
 
 There are a number of examples you can try in the [`examples/user`](examples/user) directory.
-Login to [workbench.res.ibm.com](https://workbench.res.ibm.com/) and get your GenAI API key. Then, create a `.env` file and assign the `GENAI_KEY` value as:
+Login to [workbench.res.ibm.com](https://workbench.res.ibm.com/) and get your GenAI API key. Then, create a `.env` file and assign the `GENAI_KEY` value as below example. [More information](#gen-ai-endpoint)
 
 
 ```ini
 GENAI_KEY=YOUR_GENAI_API_KEY
+# GENAI_API=GENAI_API_ENDPOINT << for a different endpoint
 ```
 
 ### <a name='AsyncExample'></a>Async Example
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -153,15 +154,15 @@
     top_k=50,
     top_p=1,
 )
 
 # creds object
 creds = Credentials(api_key, api_endpoint)
 # model object
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting = "Hello! How are you?"
 lots_of_greetings = [greeting] * 1000
 num_of_greetings = len(lots_of_greetings)
 num_said_greetings = 0
 greeting1 = "Hello! How are you?"
 
@@ -181,15 +182,15 @@
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
 from genai.model import Credentials, Model
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
@@ -207,15 +208,15 @@
     top_k=50,
     top_p=1,
 )
 
 # creds object
 creds = Credentials(api_key, api_endpoint)
 # model object
-model = Model(ModelType.FLAN_UL2, params=params, credentials=creds)
+model = Model("google/flan-ul2", params=params, credentials=creds)
 
 greeting1 = "Hello! How are you?"
 greeting2 = "I am fine and you?"
 
 # Call generate function
 responses = model.generate_as_completed([greeting1, greeting2] * 4)
 for response in responses:
@@ -303,29 +304,29 @@
 ```
 Currently the langchain extension allows IBM Generative AI models to be wrapped as Langchain LLMs and translation between genai PromptPatterns and LangChain PromptTemplates. Below are sample snippets
 ```python
 import os
 from dotenv import load_dotenv
 import genai.extensions.langchain
 from genai.extensions.langchain import LangChainInterface
-from genai.schemas import GenerateParams, ModelType
+from genai.schemas import GenerateParams
 from genai import Credentials, Model, PromptPattern
 
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
 api_endpoint = os.getenv("GENAI_API", None)
 creds = Credentials(api_key, api_endpoint)
 params = GenerateParams(decoding_method="greedy")
 
 # As LangChain Model
-langchain_model = LangChainInterface(model=ModelType.FLAN_UL2, params=params, credentials=creds)
+langchain_model = LangChainInterface(model="google/flan-ul2", params=params, credentials=creds)
 print(langchain_model("Answer this question: What is life?"))
 
 # As GenAI Model
-genai_model = Model(model=ModelType.FLAN_UL2, params=params, credentials=creds)
+genai_model = Model(model="google/flan-ul2", params=params, credentials=creds)
 print(genai_model.generate(["Answer this question: What is life?"])[0].generated_text)
 
 # GenAI prompt pattern to langchain PromptTemplate and vice versa
 seed_pattern = PromptPattern.from_str("Answer this question: {{question}}")
 template = seed_pattern.langchain.as_template()
 pattern = PromptPattern.langchain.from_template(template)
```

### Comparing `ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/SOURCES.txt` & `ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 documentation/docs/source/rst_source/examples/async.examples.user.rst
 documentation/docs/source/rst_source/examples/examples.rst
 documentation/docs/source/rst_source/examples/examples.user.rst
 documentation/docs/source/rst_source/examples/extensions.rst
 documentation/docs/source/rst_source/examples/extensions.user.rst
 documentation/docs/source/rst_source/examples/prompts.rst
 documentation/docs/source/rst_source/examples/prompts.user.rst
+examples/dev/async-flaky-request-handler.py
 examples/dev/async-flaky-responses-ordered.py
 examples/dev/generate-all-models.py
 examples/dev/history-async.py
 examples/dev/load_token_env.py
 examples/dev/logging_example.py
 examples/user/alice_bob_qa.py
 examples/user/alice_bob_talk.py
@@ -99,57 +100,66 @@
 examples/user/assets/country-capital.csv
 examples/user/assets/penguins.csv
 examples/user/assets/penguins2.csv
 examples/user/assets/seed_tasks.json
 examples/user/assets/seed_tasks.jsonl
 examples/user/localserver/localserver.py
 examples/user/localserver/requirements.txt
+examples/user/prompt_templating/watsonx-prompt-output.py
+examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
+examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
+examples/user/prompt_templating/watsonx-prompt-templating.py
 examples/user/prompts/Country-Capital-Factual-QA
 examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
 examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
 examples/user/templates/capital-qa.yaml
 examples/user/templates/instruction.yaml
 examples/user/templates/qa.yaml
 examples/user/templates/self-reflection.yaml
 examples/user/templates/synth-animal.yaml
 src/genai/__init__.py
 src/genai/_version.py
 src/genai/credentials.py
 src/genai/metadata.py
 src/genai/model.py
+src/genai/options.py
 src/genai/prompt_pattern.py
 src/genai/exceptions/__init__.py
 src/genai/exceptions/genai_exception.py
 src/genai/extensions/huggingface/__init__.py
 src/genai/extensions/huggingface/save_huggingface.py
 src/genai/extensions/langchain/__init__.py
 src/genai/extensions/langchain/llm.py
 src/genai/extensions/langchain/prompt.py
 src/genai/extensions/localserver/__init__.py
 src/genai/extensions/localserver/custom_model_interface.py
 src/genai/extensions/localserver/local_api_server.py
 src/genai/extensions/localserver/schemas.py
 src/genai/extensions/pandas/__init__.py
 src/genai/extensions/pandas/prompt_sub.py
+src/genai/routers/__init__.py
+src/genai/routers/prompt_template.py
 src/genai/schemas/__init__.py
 src/genai/schemas/descriptions.py
 src/genai/schemas/generate_params.py
 src/genai/schemas/history_params.py
 src/genai/schemas/models.py
 src/genai/schemas/responses.py
 src/genai/schemas/token_params.py
 src/genai/services/__init__.py
 src/genai/services/async_generator.py
 src/genai/services/connection_manager.py
+src/genai/services/prompt_template_manager.py
 src/genai/services/request_handler.py
 src/genai/services/service_interface.py
 src/genai/utils/__init__.py
 src/genai/utils/extensions.py
 src/genai/utils/json_utils.py
 src/genai/utils/search_space_params.py
+src/genai/utils/watsonx_helpers.py
 src/ibm_generative_ai.egg-info/PKG-INFO
 src/ibm_generative_ai.egg-info/SOURCES.txt
 src/ibm_generative_ai.egg-info/dependency_links.txt
 src/ibm_generative_ai.egg-info/requires.txt
 src/ibm_generative_ai.egg-info/top_level.txt
 tests/__init__.py
 tests/test_concurrent.py
@@ -158,14 +168,16 @@
 tests/test_history.py
 tests/test_json_utils.py
 tests/test_logging.py
 tests/test_metadata.py
 tests/test_model.py
 tests/test_model_async.py
 tests/test_prompt_pattern.py
+tests/test_prompt_pattern_watsonx.py
+tests/test_prompt_template_manager.py
 tests/test_request_handler.py
 tests/test_schema_validation.py
 tests/test_service_interface.py
 tests/test_service_interface_async.py
 tests/test_service_utils.py
 tests/test_token.py
 tests/test_version.py
```

### Comparing `ibm-generative-ai-0.1.17/src/ibm_generative_ai.egg-info/requires.txt` & `ibm-generative-ai-0.1.18/src/ibm_generative_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/assets/response_helper.py` & `ibm-generative-ai-0.1.18/tests/assets/response_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -144,7 +144,19 @@
             if "inputs" not in kwargs:
                 return SimpleResponse.error(
                     400,
                     "Bad Request",
                     " must have required property 'inputs'",
                     {"code": "INVALID_INPUT", "state": [{"instancePath": "", "params": {"missingProperty": "inputs"}}]},
                 )
+
+    @staticmethod
+    def prompt_template(template, name):
+        response = {
+            "results": {
+                "id": "5XU9Zv6mrG6KIACN",
+                "name": name,
+                "value": template,
+                "created_at": "2023-05-08T11:51:18.000Z",
+            }
+        }
+        return response
```

### Comparing `ibm-generative-ai-0.1.17/tests/extensions/test_langchain.py` & `ibm-generative-ai-0.1.18/tests/extensions/test_langchain.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/extensions/test_localserver.py` & `ibm-generative-ai-0.1.18/tests/extensions/test_localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/extensions/test_save_huggingface.py` & `ibm-generative-ai-0.1.18/tests/extensions/test_save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/extensions/test_sub_from_pandas.py` & `ibm-generative-ai-0.1.18/tests/extensions/test_sub_from_pandas.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/integration/conftest.py` & `ibm-generative-ai-0.1.18/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/integration/test_examples.py` & `ibm-generative-ai-0.1.18/tests/integration/test_examples.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_concurrent.py` & `ibm-generative-ai-0.1.18/tests/test_concurrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import logging
 import queue
 import random
+import time
 from unittest.mock import AsyncMock
 
+import httpx
 import pytest
 
 from genai.schemas import GenerateParams, ReturnOptions, TokenParams
 from genai.schemas.responses import GenerateResponse, TokenizeResponse
 from genai.services import AsyncResponseGenerator, RequestHandler, ServiceInterface
 from genai.services.connection_manager import ConnectionManager
 from tests.assets.response_helper import SimpleResponse
@@ -123,22 +125,52 @@
     @pytest.mark.asyncio
     async def test_concurrent_tokenize_dropped_request(self, httpx_mock, tokenize_params):
         # Return a 429 for a tokenize request from RequestHandler
         httpx_mock.add_response(method="POST", status_code=429, json={})
         num_prompts = 17
         counter = 0
         with AsyncResponseGenerator(
-            self.model, self.inputs * num_prompts, tokenize_params, self.service
+            self.model, self.inputs * num_prompts, tokenize_params, self.service, fn="tokenize"
         ) as asynchelper:
             for result in asynchelper.generate_response():
                 assert result is None
                 counter += 1
             assert counter == num_prompts
 
     @pytest.mark.asyncio
+    async def test_concurrent_generate_retry(self, httpx_mock, generate_params):
+        saved = ConnectionManager.MAX_RETRIES_GENERATE
+        ConnectionManager.MAX_RETRIES_GENERATE = 2
+        for code in [httpx.codes.SERVICE_UNAVAILABLE, httpx.codes.TOO_MANY_REQUESTS]:
+            httpx_mock.add_response(method="POST", status_code=code, json={})
+            with AsyncResponseGenerator(self.model, self.inputs, generate_params, self.service) as asynchelper:
+                time_start = time.time()
+                for result in asynchelper.generate_response():
+                    assert result is None
+                time_end = time.time()
+                assert time_end - time_start > 5
+        ConnectionManager.MAX_RETRIES_GENERATE = saved
+
+    @pytest.mark.asyncio
+    async def test_concurrent_tokenize_retry(self, httpx_mock, tokenize_params):
+        saved = ConnectionManager.MAX_RETRIES_TOKENIZE
+        ConnectionManager.MAX_RETRIES_TOKENIZE = 2
+        for code in [httpx.codes.SERVICE_UNAVAILABLE, httpx.codes.TOO_MANY_REQUESTS]:
+            httpx_mock.add_response(method="POST", status_code=code, json={})
+            with AsyncResponseGenerator(
+                self.model, self.inputs, tokenize_params, self.service, fn="tokenize"
+            ) as asynchelper:
+                time_start = time.time()
+                for result in asynchelper.generate_response():
+                    assert result is None
+                time_end = time.time()
+                assert time_end - time_start > 5
+        ConnectionManager.MAX_RETRIES_TOKENIZE = saved
+
+    @pytest.mark.asyncio
     async def test_concurrent_generate_dropped_request(self, httpx_mock, generate_params):
         failed_id = 4
         single_response = SimpleResponse.generate(model=self.model, inputs=self.inputs, params=generate_params)
         headers, json_data = RequestHandler._metadata(
             "POST",
             key="TEST_KEY",
             model_id=self.model,
```

### Comparing `ibm-generative-ai-0.1.17/tests/test_generate_schema.py` & `ibm-generative-ai-0.1.18/tests/test_generate_schema.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_generate_service.py` & `ibm-generative-ai-0.1.18/tests/test_generate_service.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_history.py` & `ibm-generative-ai-0.1.18/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_json_utils.py` & `ibm-generative-ai-0.1.18/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_logging.py` & `ibm-generative-ai-0.1.18/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_metadata.py` & `ibm-generative-ai-0.1.18/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_model.py` & `ibm-generative-ai-0.1.18/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_model_async.py` & `ibm-generative-ai-0.1.18/tests/test_model_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_prompt_pattern.py` & `ibm-generative-ai-0.1.18/tests/test_prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_request_handler.py` & `ibm-generative-ai-0.1.18/tests/test_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_schema_validation.py` & `ibm-generative-ai-0.1.18/tests/test_schema_validation.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_service_interface.py` & `ibm-generative-ai-0.1.18/tests/test_service_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_service_interface_async.py` & `ibm-generative-ai-0.1.18/tests/test_service_interface_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_service_utils.py` & `ibm-generative-ai-0.1.18/tests/test_service_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.1.17/tests/test_token.py` & `ibm-generative-ai-0.1.18/tests/test_token.py`

 * *Files identical despite different names*

