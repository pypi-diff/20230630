# Comparing `tmp/swarms-0.0.1.tar.gz` & `tmp/swarms-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.0.1.tar", last modified: Thu Jun 29 19:58:30 2023, max compression
+gzip compressed data, was "swarms-0.0.3.tar", last modified: Fri Jun 30 13:27:30 2023, max compression
```

## Comparing `swarms-0.0.1.tar` & `swarms-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:58:30.128712 swarms-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 19:58:13.000000 swarms-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-29 19:58:30.128712 swarms-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-29 19:58:13.000000 swarms-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:58:30.128712 swarms-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-29 19:58:13.000000 swarms-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:58:30.128712 swarms-0.0.1/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-29 19:58:30.000000 swarms-0.0.1/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 19:58:30.000000 swarms-0.0.1/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:58:30.000000 swarms-0.0.1/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 19:58:30.000000 swarms-0.0.1/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:58:30.000000 swarms-0.0.1/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:30.460657 swarms-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 13:27:17.000000 swarms-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 13:27:30.460657 swarms-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-06-30 13:27:17.000000 swarms-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 13:27:30.460657 swarms-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-30 13:27:17.000000 swarms-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:30.460657 swarms-0.0.3/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 13:27:17.000000 swarms-0.0.3/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:30.460657 swarms-0.0.3/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:17.000000 swarms-0.0.3/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-30 13:27:17.000000 swarms-0.0.3/swarms/agents/swarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-06-30 13:27:17.000000 swarms-0.0.3/swarms/agents/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:27:30.460657 swarms-0.0.3/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 13:27:30.000000 swarms-0.0.3/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.0.1/LICENSE` & `swarms-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.0.1/PKG-INFO` & `swarms-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.1
+Version: 0.0.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.0.1/README.md` & `swarms-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Agora
 
 ![Agora banner](Agora-Banner-blend.png)
 
 [Swarms is brought to you by Agora, the open source AI research organization. Join Agora and Help create swarms and or recieve support to advance Humanity. ](https://discord.gg/qUtxnK2NMf)
 
 # Swarming Language Models (Swarms)
+
+![Swarming banner](swarms.png)
+
 [![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)
 
 [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)
 
 
@@ -34,44 +37,65 @@
 
 ## Usage
 There are 2 methods, one is very simple to test it out and then there is another to explore the agents and so on! Check out the [Documetation file ](/DOCUMENTATION.md) to understand the classes
 
 ### Method 1
 Simple example `python3 example.py`
 
-### Method 2
-The primary agent in this repository is the `AutoAgent` from `./swarms/agents/workers/auto_agent.py`.
 
-This `AutoAgent` is used to create the `MultiModalVisualAgent`, an autonomous agent that can process tasks in a multi-modal environment, like dealing with both text and visual data.
+### Method2
+
+I see, my apologies for the confusion. Here is an updated usage example that just utilizes the `BossNode` class:
 
-To use this agent, you need to import the agent and instantiate it. Here is a brief guide:
+One of the main components of swarms is the `BossNode` class. This class acts as a "boss" that assigns tasks to other components.
+
+Below is an example of how to use the `BossNode` class in Langchain:
 
 ```python
-from swarms.agents.auto_agent import MultiModalVisualAgent
+from swarms import BossNode
+#or swarms.agents.swarms import BossNode
+
+# Initialize BossNode
+boss_node = BossNode()
 
-# Initialize the agent
-multimodal_agent = MultiModalVisualAgent()
+# Create and execute a task
+task = boss_node.create_task("Write a summary of the latest news about artificial intelligence.")
+boss_node.execute_task(task)
 ```
 
-### Working with MultiModalVisualAgentTool
-The `MultiModalVisualAgentTool` class is a tool wrapper around the `MultiModalVisualAgent`. It simplifies working with the agent by encapsulating agent-related logic within its methods. Here's a brief guide on how to use it:
+This will create a task for the BossNode, which is to write a summary of the latest news about artificial intelligence. 
+
+## BossNode
+
+The `BossNode` class is a key component of Swarms. It represents a "boss" in the system that assigns tasks to other components.
+
+Here is an example of how you can use it:
 
 ```python
-from swarms.agents.auto_agent import MultiModalVisualAgent, MultiModalVisualAgentTool
+class BossNode:
+    def __init__(self, tools):
+        # initialization code goes here
 
-# Initialize the agent
-multimodal_agent = MultiModalVisualAgent()
+    def create_task(self, objective):
+        return {"objective": objective}
 
-# Initialize the tool with the agent
-multimodal_agent_tool = MultiModalVisualAgentTool(multimodal_agent)
+    def execute_task(self, task):
+        # task execution code goes here
+```
 
-# Now, you can use the agent tool to perform tasks. The run method is one of them.
-result = multimodal_agent_tool.run('Your text here')
+With the `BossNode` class, you can create tasks for your tools to perform. For example, you can create a task to write a summary of a specific topic:
+
+```python
+boss_node = BossNode()
+task = boss_node.create_task("Write a summary of the latest news about quantum computing.")
+boss_node.execute_task(task)
 ```
 
+This will create and execute a task to write a summary about the latest news on quantum computing. The result will be the summary of the news.
+
 ## Note
 - The `AutoAgent` makes use of several helper tools and context managers for tasks such as processing CSV files, browsing web pages, and querying web pages. For the best use of this agent, understanding these tools is crucial.
 
 - Additionally, the agent uses the ChatOpenAI, a language learning model (LLM), to perform its tasks. You need to provide an OpenAI API key to make use of it. 
 
 - Detailed knowledge of FAISS, a library for efficient similarity search and clustering of dense vectors, is also essential as it's used for memory storage and retrieval. 
 
@@ -126,8 +150,17 @@
 
 * Create unit tests
 
 * Create benchmrks
 
 * Create evaluations
 
-* Add new tool that uses WhiseperX to transcribe a youtube video
+* Add new tool that uses WhiseperX to transcribe a youtube video
+
+* Integrate hf agents as tools
+
+* [Integrate tools from here](https://integrations.langchain.com/)
+
+
+* Create extensive and useful examples 
+
+* And, recreate exampels and usage in readme.
```

### Comparing `swarms-0.0.1/setup.py` & `swarms-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.0.1',
+  version = '0.0.3',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.0.1/swarms.egg-info/PKG-INFO` & `swarms-0.0.3/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.0.1
+Version: 0.0.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

