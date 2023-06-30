# Comparing `tmp/glsm-0.1.0.tar.gz` & `tmp/glsm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glsm-0.1.0.tar", last modified: Tue Apr  4 17:12:44 2023, max compression
+gzip compressed data, was "glsm-0.1.1.tar", last modified: Fri Jun 30 03:36:26 2023, max compression
```

## Comparing `glsm-0.1.0.tar` & `glsm-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-04-04 17:12:44.414325 glsm-0.1.0/
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-03-30 08:02:39.000000 glsm-0.1.0/LICENSE
--rwxrwxrwx   0 valar     (1000) valar     (1000)    10601 2023-04-04 17:12:44.410325 glsm-0.1.0/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)     9934 2023-04-04 17:03:13.000000 glsm-0.1.0/README.md
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-04-04 17:12:44.266130 glsm-0.1.0/glsm/
--rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-03-30 19:17:50.000000 glsm-0.1.0/glsm/__init__.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)      560 2023-04-04 17:03:02.000000 glsm-0.1.0/glsm/features.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     2412 2023-04-01 12:50:23.000000 glsm-0.1.0/glsm/non_predictive.py
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-04-04 17:12:44.383327 glsm-0.1.0/glsm.egg-info/
--rwxrwxrwx   0 valar     (1000) valar     (1000)    10601 2023-04-04 17:12:43.000000 glsm-0.1.0/glsm.egg-info/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)      222 2023-04-04 17:12:44.000000 glsm-0.1.0/glsm.egg-info/SOURCES.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-04-04 17:12:43.000000 glsm-0.1.0/glsm.egg-info/dependency_links.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)        9 2023-04-04 17:12:43.000000 glsm-0.1.0/glsm.egg-info/requires.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)        5 2023-04-04 17:12:43.000000 glsm-0.1.0/glsm.egg-info/top_level.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-04-04 17:12:44.415326 glsm-0.1.0/setup.cfg
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1453 2023-04-04 17:07:04.000000 glsm-0.1.0/setup.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-30 03:36:26.984862 glsm-0.1.1/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1091 2023-04-09 23:14:04.000000 glsm-0.1.1/LICENSE
+-rwxrwxrwx   0 valar     (1000) valar     (1000)    15753 2023-06-30 03:36:26.981852 glsm-0.1.1/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)    15086 2023-06-30 03:23:43.000000 glsm-0.1.1/README.md
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-30 03:36:26.876275 glsm-0.1.1/glsm/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-03-30 19:17:50.000000 glsm-0.1.1/glsm/__init__.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-30 03:36:26.962233 glsm-0.1.1/glsm.egg-info/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)    15753 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      182 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      231 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/requires.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        5 2023-06-30 03:36:26.000000 glsm-0.1.1/glsm.egg-info/top_level.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-06-30 03:36:26.985864 glsm-0.1.1/setup.cfg
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1552 2023-06-30 03:36:00.000000 glsm-0.1.1/setup.py
```

### Comparing `glsm-0.1.0/LICENSE` & `glsm-0.1.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+FITNESS FOR A PARTICULAR PURPOSE AND NON INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `glsm-0.1.0/README.md` & `glsm-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,150 @@
+Metadata-Version: 2.1
+Name: glsm
+Version: 0.1.1
+Summary: A Python package that simplifies the process of building predictive and non-predictive lead scoring models.
+Author: Victor Valar
+Author-email: <valar@victorvalar.me>
+License: LICENSE.txt
+Keywords: python,lead score,modeling,lead generation,lead scoring,lead scoring model
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # Generic Lead Scoring Model
+
 ## About
+
 `glsm` is a user-friendly Python package that simplifies the process of building lead scoring models. It supports both predictive and non-predictive models, providing flexibility and ease of use.
 
 The goal of the lead score is to provide a qualification metric for comparison between leads. It is based on product interest and company interaction data.
 
 ### Predictive Model
+
 Soon!
+
 ### Non-predictive Model
 
-| Name | Description | Variable |
-|------------ |------------|------------|
-Weight| Feature weight   that represents the relative importance of each feature | $$w$$
-Points| Assigned points of each feature | $$p$$
-Normalized weight | Weights unit vector normalization | $${\hat{w}} = \frac{w_n}{\sqrt{\sum\limits^{n}_{i=0}w_i^2}}$$
-Lead score | A weighted sum of assigned points for each feature, where the feature weights are normalized to form a unit vector. | $$\lambda = \sum_{i=1}^n {\hat{w}_i^2}{p_i}$$
 
-***
+| Name | Description | Variable|
+|-------------------|-------------------|-------------------|
+| Weight| Feature weight that represents the relative importance of each feature | $$w$$ |
+| Points| Assigned points of each feature | $$p$$ |
+| Normalized weight | Weights unit vector normalization | $${\hat{w}} = \frac{w}{\sqrt{\sum\limits^{n}_{i=0}w_i^2}}$$ |
+| Lead score | A weighted sum of assigned points for each feature, where the feature weights are normalized to form a unit vector. | $$\lambda = \sum_{i=1}^n {\hat{w}_i^2}{p_i}$$ |
+
+---
 
 ## Index
+
 1. [About](#about)
-    1. [Predictive Model](#predictive-model)
-    2. [Non-predictive Model](#non-predictive-model)
+   1. [Predictive Model](#predictive)
+   2. [Non-predictive Model](#non-predictive)
 2. [Disclaimer](#disclaimer)
 3. [Installation](#installation)
-4. [Theory](#understanding-the-models)
-    1. [Predictive Model](#predictive-model-1)
-    2. [Non-predictive Model](#non-predictive-model-1)
-        1. [Weight (${w}$):](#weight-w)
-        2. [Normalized Weight (${\hat{w}}$):](#normalized-weight-hatw)
-            1. [Unit vector nomalization:](#unit-vector-nomalization)
-            2. [Feature vector magnitude:](#feature-vector-magnitude)
-            3. [Normalized weight vector:](#normalized-weight-vector)
-        3. [Points (${p}$):](#points-p)
-        4. [Lead Score ($\lambda$):](#lead-score-lambda)
-        5. [Features ($f_n$)](#features-f1f2f3--fn)
+4. [Theory](#theory)
+   1. [Predictive Model](#predictive-model)
+   2. [Non-predictive Model](#non-predictive-model)
+      1. [Weight:](#weight-w)
+      2. [Normalized Weight:](#normalized-weight-hatw)
+         1. [Unit vector normalization:](#unit-vector-normalization)
+         2. [Feature weights vector magnitude:](#feature-weights-vector-magnitude)
+         3. [Normalized weight vector:](#normalized-weight-vector)
+      3. [Qualification threshold](#qualification-threshold)
+      4. [Points:](#points-p)
+      5. [Lead Score:](#lead-score-lambda)
+      6. [Features](#features)
 5. [Usage](#usage)
-    1. [Predictive Model](#predictive-model-2)
-    2. [Non-predictive Model](#non-predictive-model-2)
-        1. [Importing the library](#importing-the-library)
-        2. [Instantiating the model and adding features](#instantiating-the-model-and-adding-features)
-        3. [Importing lead data](#importing-lead-data)
-            1. [From a dictionary](#from-a-dictionary)
-            2. [From a csv](#from-a-csv)
-        4. [Calculating the lead score](#calculating-the-lead-score)
-
+   1. [Predictive Model](#predictive-model-usage)
+   2. [Non-predictive Model](#non-predictive-model-usage)
+      1. [Importing the library](#importing-the-library)
+      2. [Instantiating the model and adding features](#instantiating-the-model-and-adding-features)
+      3. [Removing features](#removing-features)
+      4. [Calculating the lead score](#calculating-the-lead-score)
+         1. [From a dictionary](#from-a-dictionary)
+         2. [From a csv](#from-a-csv)
 
 ## Disclaimer
-This library is in active development. Suggestions and contributions are welcome.
+
+This library is in beta. Suggestions and contributions are welcome.
+
 ## Installation
+
 ### Requirements
+
 - pydantic
+- pandas
 
 Can be installed using pip:
+
 ```bash
 pip install glsm
 ```
-***
+
+---
+
 # Theory
+
 There are two ways for you to understand the proposed models:
 
 1. Through the [Google Sheets simulator](https://docs.google.com/spreadsheets/d/1ESEtcjno36ZLW5XMEoHqLKHjiZMkrZeIECcrcgFxHzA/edit?usp=sharing) (Non-predictive only)
 2. Reading the following sections
-## Predictive Model
+
+## Predictive
+
 Soon!
 
-***
-## Non-predictive Model
+---
+
+## Non-predictive
 
 This model and the following set of rules are a suggestion to get you started. You can use them as a starting point and adapt them to your business needs.
 The library is flexible enough to allow you to use your own assumptions and  rules.
 
-
 The non-predictive model has the following characteristics:
+
 1. It avoids the use of predictive algorithms, which can be data-intensive and require significant computational power and technical expertise to operate effectively.
 2. It uses relative feature weights, meaning that the inclusion of a new feature won't change the weights of the existing ones. This can simplify the implementation and interpretation of the model.
 3. It provides a score that ranges from 0 to 100 points, with 50 being the minimum threshold for lead qualification. The score reflects the current objectives and scenarios of the company, allowing for comparisons of lead performance over time.
 
-###  Weight (${w}$):
+### Weight (${w}$):
+
 Feature weight is a value that multiplies the points assigned to each feature. It is used to differentiate the importance of each feature.
 
 You can make it easier to understand by thinking of it as a multiplier. The higher the weight, the more important the feature is. You can use any range of values (due to the unit vector normalization), but it is easier to interpret if the weights are between 0 and 1.
 
 Suppose you choose to use values from 0 to 1. Your most important feature will have a weight of 1. Other features should have a weight less than 1.
 
-
 ### Normalized Weight (${\hat{w}}$):
+
 The model needs to be flexible and adaptable to accommodate changes in the business environment. Sometime after the model is built, the company may change its focus or process. In this case, features may need to be added or removed.
 
 The normalized weight is a unit vector that is used to scale data in a way that preserves the relative relationships between the features when new features are added.
 
 The basic idea is to transform the data such that the magnitude of the vector formed by the features is equal to 1. This ensures that each feature is scaled proportionally to the others, so the relative relationships between them is preserved when new features are added.
 
-You may be asking yourself, why not just recalculate the weights after adding or removing a feature?
-Well, this may work if you have the original data and just want to make a report out of it, but once you calculate the lead score and send the conversion events to plaftorms such as Google Analytics, Facebook Ads, etc, the scores registered in those platforms can't be changed. Later on you may want to create audiences based on the lead score, but you won't be able to do that if the scoring model has changed. The normalized weight vector solves this problem.
+You may be asking yourself why not just recalculate the weights after adding or removing a feature?
+Well, this may work if you have the original data and just want to make a report out of it, but once you calculate the lead score and send the conversion events to platforms such as Google Analytics, Facebook Ads, etc. The scores registered in those platforms can't be changed. Later on you may want to create audiences based on the lead score, but you won't be able to do that if the scoring model has changed. The normalized weight vector solves this problem.
 
 <!-- #TODO rewrite this section -->
 
-#### Unit vector nomalization:
+#### Unit vector normalization:
+
 $$
 \hat{w_n} = \frac{w_n}{|w|}
 $$
+
 #### Feature weights vector magnitude:
+
 $$
 |w| = \sqrt{\sum\limits^{n}_{i=0}w_i^2}
 $$
 
 #### Normalized weight vector:
 
 $$
@@ -113,124 +153,194 @@
 
 In this way the sum of the squares of the normalized weights is equal to 1:
 
 $$
 \sum\limits^{n}_{i=0}{\hat{w}_i^2} = 1
 $$
 
+### Qualification threshold:
+
+The qualification threshold is the value that determines whether a lead is qualified or not. It is calculated as the midpoint of the range of points assigned to each feature.
+
+$$
+\theta = \text{points range}_{max} - \frac{\text{points range}_{max} - \text{points range}_{min}}{2}
+$$
+
+If the lead score $\geq \theta$ then the lead is qualified.
+
+Note that you can always change the qualification threshold to suit your needs. Since the default points range is 0 to 100, the default threshold is 50.
 
 ### Points ($p$):
-Assigned points per feature.The score assigned to each option of a feature. 50 shloud  assigned to the option that represents your ICP.
 
+Points assigned to each option of each feature. The points are assigned based on the desirability of each option. The points are then multiplied by the normalized weight of the feature to obtain the weighted points that are then summed to obtain the lead score.
 
+> **NOTE:** The numbers below are only a suggestion. You can use any set of values. The important thing is to be consistent.
 
-These numbers are only a suggestion. You can use any range of values, but it is easier to interpret if the points are $0  \leq p \geq 100$ and 50 is the ICP.
+The proposed points assignment framework is as follows:
+
+1. Order the options from least desirable to most desirable.
+2. Determine the range of points for each feature: Define the minimum and maximum points for each feature. The minimum points should be assigned to the least desirable option, and the maximum points to the most desirable option. For instance, you could assign points on a scale of 0 to 100.
+3. Determine if the feature is numeric or categorical.
+
+   - **If defining from numeric variables:**
+     Specify the target ranges that best represents the ICP.
+     For example, in a feature called "Monthly users", the ICP range could be "50k to 100k"
+   - **If defining from categorical variables:**
+     Identify the options that best represent the ICP. For example, in a feature called "Industry", the ICP options could be "Retail" and "Telecom".
+4. Assign points to the ICP option: Assign the qualification threshold points (suppose 50 points in this case) to the ICP option(s).
+5. Divide the remaining points range into equal intervals: For options less desirable than the ICP option, divide the range from the minimum points to the qualification threshold points (0 to 50) into equal intervals. For options more desirable than the ICP option, divide the range from the qualification threshold points to the maximum points (50 to 100) into equal intervals.
+
+   Suppose a feature A has 4 options: A1, A2, A3, A4. The ICP option is A2:
+
+   - For options less desirable than A2 (A1): Divide the range 0 to 50 into equal intervals (0 to 50, one interval of 50 points).
+   - For options more desirable than A2 (A3 and A4): Divide the range 50 to 100 into equal intervals (50 to 100, two intervals of 25 points each).
+6. Assign points to the other options based on their position in the intervals: Assign points to each option based on the position of that option within the equal intervals.
+
+   - A1: 0 points (minimum)
+   - A2: 50 points (ICP option)
+   - A3: 75 points
+   - A4: 100 points (maximum)
+
+   If none of the options seem to be a good fit for assigning 0 points, you can introduce a new baseline option that represents the least desirable criteria. This baseline option will be assigned 0 points, and the other options will be assigned points accordingly.
+
+   The options for feature A would now be: A0, A1, A2, A3, and A4, with A0 being the new baseline option. The points assignment will now follow the same steps as before, but with A0 receiving 0 points:
+
+   - A0: 0 points (minimum)
+   - A1: 25 points
+   - A2: 50 points (ICP option)
+   - A3: 75 points
+   - A4: 100 points (maximum)
+
+Use your best judgement and domain knowledge or historical data that suggests a certain lead score is more indicative of a qualified lead to determine the target ranges and how many options to include before and after the ICP options.
+
+Note that more than one ICP option can be defined for each feature as seen below:
+
+
+| Industry       | Points | Calculation             |
+| -------------- | ------ | ----------------------- |
+| Other          | 0      | 50 - (50/5)*5           |
+| Agriculture    | 10     | 50 - (50/5)*4           |
+| Transportation | 20     | 50 - (50/5)*3           |
+| Healthcare     | 30     | 50 - (50/5)*2           |
+| Manufacturing  | 40     | 50 - (50/5)             |
+| Education      | 50     | qualification_threshold |
+| Finance        | 50     | qualification_threshold |
+| Technology     | 50     | qualification_threshold |
+| Retail         | 75     | 50 + 50/2               |
+| Telecom        | 100    | 50 + (50/2)*2           |
 
 ### Lead Score ($\lambda$):
-Lead score is the sum of squares the normalized weights of each feature multiplied by the points assined to each feature.
 
+Lead score is the sum of squares the normalized weights of each feature multiplied by the points assigned to each feature.
 
 $$
 \lambda = \sum_{i=1}^n {\hat{w}_i^2}{p_i} = ({\hat{w}_1^2}{p_1})+({\hat{w}_2^2}{p_2})+({\hat{w}_3^2}{p_3})...({\hat{w}_n^2}{p_n})
 $$
 
-### Features ($f_n$)
+The higher the lead score, the more desirable the lead is. The lead score is then compared to the qualification threshold to determine if the lead is qualified or not.
+
+Lead score can be used to rank and prioritize leads, and to create audiences based on the lead score on platforms such as Google Analytics, Facebook Ads, etc.
+
+### Features
+
 Features are a set of characteristics assigned to each lead. If you have difficulties finding out which features to add, start by adding relevant lead form or CRM fields as features.
 
-Each feature has points associated with it, which are assigned to each option of the feature. The points assigned to each option are relative to the minimum viable option for the lead to be considered qualified (50 points).
+Each feature has points associated with it, which are assigned to each option of the feature. The points assigned to each option are relative to the qualification threshold. The higher the points, the more desirable the option.
 
-You should first define the features and their options, then assign 50 points to the minimum viable option for the lead to be considered qualified. The remaining points should be distributed among the other options in a way that reflects the relative importance of each option.
+Each feature has a weight associated with it, which is used to differentiate the importance of each feature. The higher the weight, the more important the feature is.
 
-In this way if $\lambda \geq 50$ the lead is considered qualified.
+A feature have several options, each of which represent a range of values. For example, the feature "Monthly Website Users" has the following options:
 
-Remember that this is a suggestion, you can assign the points as you see fit and as your business requires. You may want to use negative points to penalize leads that do not meet certain criteria for example. It is generally easier to work with positive points, but it is up to you.
 
-#### Example:
-| Monthly Website Users | Points|
-|------------ | ------------|
-Up to 50k | 30
-50k - 100k | 50 (ICP)
-100k - 200k | 80
-More than 200k | 100
+| Monthly Website Users | Points   |
+| --------------------- | -------- |
+| Up to 50k             | 0        |
+| 50k - 100k            | 50 (ICP) |
+| 100k - 200k           | 75       |
+| More than 200k        | 100      |
 
-***
+You should first define the features and their options, then assign 50 points to the minimum viable option for the lead to be considered qualified. The remaining points should be distributed among the other options in a way that reflects the relative importance of each option.
 
+Remember that this is a suggestion, you can assign the points as you see fit and as your business requires. You may want to use negative points to penalize leads that do not meet certain criteria for example. It is generally easier to work with positive points, but it is up to you.
 
 # Usage
-## Predictive Model
+
+## Predictive Model usage
+
 Soon!
-## Non-predictive Model
+
+## Non-predictive Model usage
+
 In the examples folder you can find a Jupyter Notebook with a step-by-step guide on how to use the library.
 You may also want to check the [Google Sheets simulator](https://docs.google.com/spreadsheets/d/1ESEtcjno36ZLW5XMEoHqLKHjiZMkrZeIECcrcgFxHzA/edit?usp=sharing) (Non-predictive only)
+
 ### Importing the library
+
 ```python
-from glsm.non_predictive import NonPredictive
-from glsm.features import Feature
+from glsm.non_predictive.model import NonPredictive
+from glsm.non_predictive.features import Feature
 ```
+
 ### Instantiating the model and adding features
 ```python
 model = NonPredictive()
 
 feature_a = Feature(
     name="Monthly Users",
     weight=0.5,
-    points_map=[
-        ("Up to 50K",00),
-        ("50K - 100K",50),
-        ("100K - 200K",70),
-        ("More than 200K",100),
-    ]
+    options_df=pd.DataFrame([
+            {"label": "Up to 50k", "is_ICP": False},
+            {"label": "50k - 100k", "is_ICP": True},
+            {"label": "100k - 200k", "is_ICP": False},
+            {"label": "More than 200k", "is_ICP": False},
+        ])
 )
-
 feature_b = Feature(
     name="Industry",
     weight=0.25,
-    points_map=[
-        ("Technology",70),
-        ("Real State",20),
-        ("Retail",50),
-        ("Education",50),
-        ("Health",100),
-    ]
+    options_df=pd.DataFrame([
+            {"label": "Other", "is_ICP": False},
+            {"label": "Agriculture", "is_ICP": False},
+            {"label": "Transportation", "is_ICP": False},
+            {"label": "Healthcare", "is_ICP": False},
+            {"label": "Manufacturing", "is_ICP": False},
+            {"label": "Education", "is_ICP": True},
+            {"label": "Finance", "is_ICP": True},
+            {"label": "Technology", "is_ICP": True},
+            {"label": "Retail", "is_ICP": False},
+            {"label": "Telecom", "is_ICP": False},
+        ])
 )
-
 model.add_features([feature_a, feature_b])
 ```
 
-### Importing lead data
+### Removing features
+```python
+model.remove_features(['Industry'], ['Monthly Users'])
+```
+
+### Calculating the lead score
+
 #### From a dictionary
+
 ```python
-lead = { # lambda = 81.43
+lead = {
         "Monthly Users": "50K - 100K",
         "Industry": "Technology",
         "Mkt Investment": "$300K - $400K",
     }
-```
-#### From a csv
-```python
-import csv
-
-with open('leads.csv', 'r') as file:
-    if file.read(3) == b'\xef\xbb\xbf':
-        file.seek(3)
-    csv_reader = csv.reader(file)
-    headers = next(csv_reader)
-
-    # New csv file adding lambda values
-    with open('leads_with_lambda.csv', 'w', newline='') as new_file:
-        csv_writer = csv.writer(new_file)
-        csv_writer.writerow(headers + ['lambda'])
-
-        for row in csv_reader:
-            lead = dict(zip(headers, row))
-            lambda_value = model.compute_lambda(lead)
-            csv_writer.writerow(row + [lambda_value])
 
+lambda_value = model.compute_lambda(lead)
 ```
 
-### Calculating the lead score
+#### From a csv
+Check out the leads.csv file in the examples folder.
 ```python
-lambda_value = model.compute_lambda(lead)
+df = pd.read_csv('leads.csv')
+df['lambda'] = df.apply(
+    lambda row: model.compute_lambda(row.to_dict()),
+    axis=1
+)
 ```
```

### Comparing `glsm-0.1.0/setup.py` & `glsm-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 print(requirements_filename)
 readme_filename = os.path.join(here, 'README.md')
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 with open(requirements_filename) as f:
-    INSTALL_REQUIRES = ['pydantic',]
+    INSTALL_REQUIRES = f.read().splitlines()
 
-VERSION = '0.1.0'
-DESCRIPTION = 'A Python package that simplifies the process of building predictive and non-predictive lead scoring models.'
+# EXTRA_REQUIRES = ['pytest']
+VERSION = '0.1.1'
+DESCRIPTION = 'A Python package that simplifies the process of building predictive and non-predictive lead scoring ' \
+              'models.'
 LONG_DESCRIPTION = long_description
 PACKAGE_LICENSE = 'LICENSE.txt'
 
 # Setting up
 setup(
     name="glsm",
     version=VERSION,
@@ -26,17 +28,18 @@
     author="Victor Valar",
     author_email="<valar@victorvalar.me>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=INSTALL_REQUIRES,
+    # extras_require=EXTRA_REQUIRES,
     keywords=['python', 'lead score', 'modeling', 'lead generation', 'lead scoring', 'lead scoring model'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

