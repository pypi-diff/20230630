# Comparing `tmp/huntflow_webhook_models-0.0.5.tar.gz` & `tmp/huntflow_webhook_models-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_webhook_models-0.0.5.tar", last modified: Wed Jun  7 07:34:31 2023, max compression
+gzip compressed data, was "huntflow_webhook_models-0.0.6.tar", last modified: Fri Jun 30 07:10:06 2023, max compression
```

## Comparing `huntflow_webhook_models-0.0.5.tar` & `huntflow_webhook_models-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/LICENSE
--rw-r--r--   0        0        0       69 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/README.md
--rw-r--r--   0        0        0      122 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/__init__.py
--rw-r--r--   0        0        0      666 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/applicant.py
--rw-r--r--   0        0        0     1331 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/base.py
--rw-r--r--   0        0        0        0 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/__init__.py
--rw-r--r--   0        0        0     6585 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/applicant.py
--rw-r--r--   0        0        0     5459 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/calendar_event.py
--rw-r--r--   0        0        0      669 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/hf_base.py
--rw-r--r--   0        0        0     2950 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/survey_questionary.py
--rw-r--r--   0        0        0     3252 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/vacancy.py
--rw-r--r--   0        0        0     1638 2023-06-07 07:34:17.424665 huntflow_webhook_models-0.0.5/huntflow_webhook_models/consts.py
--rw-r--r--   0        0        0     1403 2023-06-07 07:34:31.064895 huntflow_webhook_models-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 huntflow_webhook_models-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/LICENSE
+-rw-r--r--   0        0        0       69 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/README.md
+-rw-r--r--   0        0        0      276 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/__init__.py
+-rw-r--r--   0        0        0      666 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/applicant.py
+-rw-r--r--   0        0        0     1341 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/base.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/__init__.py
+-rw-r--r--   0        0        0     6596 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/applicant.py
+-rw-r--r--   0        0        0     5459 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/calendar_event.py
+-rw-r--r--   0        0        0      669 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/hf_base.py
+-rw-r--r--   0        0        0     2950 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/survey_questionary.py
+-rw-r--r--   0        0        0     3710 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/vacancy.py
+-rw-r--r--   0        0        0     1208 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/vacancy_request.py
+-rw-r--r--   0        0        0     1884 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/consts.py
+-rw-r--r--   0        0        0      558 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/vacancy.py
+-rw-r--r--   0        0        0      645 2023-06-30 07:09:46.502714 huntflow_webhook_models-0.0.6/huntflow_webhook_models/vacancy_request.py
+-rw-r--r--   0        0        0     1403 2023-06-30 07:10:06.582597 huntflow_webhook_models-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 huntflow_webhook_models-0.0.6/PKG-INFO
```

### Comparing `huntflow_webhook_models-0.0.5/LICENSE` & `huntflow_webhook_models-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.5/huntflow_webhook_models/applicant.py` & `huntflow_webhook_models-0.0.6/huntflow_webhook_models/applicant.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.5/huntflow_webhook_models/base.py` & `huntflow_webhook_models-0.0.6/huntflow_webhook_models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     email: str = Field(..., description="Account owner email", example="test@example.com")
     name: str = Field(..., description="Account owner name", example="John")
     meta: Optional[Dict] = Field(None, description="Additional data", example={"data": "data"})
 
 
 class WebhookMetaInfoBase(BaseModel):
     account: Account
-    author: Author
+    author: Optional[Author]
     event_type: WebhookEventType = Field(
         ...,
         description="Webhook event type",
         example=WebhookEventType.APPLICANT,
     )
     version: str = Field(..., description="Webhook version", example="2.0")
     retry: int = Field(..., description="Webhook retry count", example=1)
```

### Comparing `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/applicant.py` & `huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/applicant.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         description="Additional applicant fields",
         example={"favorite_language": "python"},
     )
 
 
 class Respondent(BaseModel):
     account_id: int = Field(..., description="Account ID", example=1)
-    custom_id: int = Field(..., description="Custom ID", example=1)
+    custom_id: Optional[int] = Field(None, description="Custom ID", example=1)
     name: Optional[str] = Field(None, description="Respondent name", example="John")
     email: str = Field(..., description="Respondent email", example="test@example.com")
 
 
 class Survey(BaseModel):
     id: int = Field(..., description="Survey ID", example=1)
     name: str = Field(..., description="Survey name", example="test")
```

### Comparing `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/calendar_event.py` & `huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/calendar_event.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/hf_base.py` & `huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/hf_base.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/survey_questionary.py` & `huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/survey_questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_webhook_models-0.0.5/huntflow_webhook_models/common_models/vacancy.py` & `huntflow_webhook_models-0.0.6/huntflow_webhook_models/common_models/vacancy.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pydantic import BaseModel, Field
 
 from huntflow_webhook_models.consts import VacancyState
 
 
 class FillQuota(BaseModel):
     id: int = Field(..., description="Fill quota ID", example=1)
-    applicants_to_hire: int = Field(..., description="Amoun of applicant to hire", example=1)
+    applicants_to_hire: int = Field(..., description="Amount of applicant to hire", example=1)
     closed: Optional[datetime] = Field(
         None,
         description="Date time the fill quota was closed",
         example=datetime(1970, 1, 1, 1, 1, 1),
     )
     created: datetime = Field(
         ...,
@@ -63,24 +63,39 @@
         ...,
         description="Date the vacancy was created",
         example=datetime(1970, 1, 1, 1, 1, 1),
     )
     deadline: Optional[date] = Field(..., description="Vacancy deadline", example=date(1970, 1, 1))
     fill_quotas: List[FillQuota] = Field([], description="Vacancy fill quota")
     frame_id: int = Field(..., description="Vacancy frame ID", example=1)
-    hidden: bool = Field(..., description="Hidden vacnacy flag", example=True)
-    money: Optional[str] = Field(None, description="Salary for vacacny", example="100000")
+    hidden: bool = Field(..., description="Hidden vacancy flag", example=True)
+    money: Optional[str] = Field(None, description="Salary for vacancy", example="100000")
     multiple: bool = Field(..., description="Multiple vacancy flag", example=False)
-    parent: Optional[int] = Field(None, description="Vacnacy parent ID", example=1)
+    parent: Optional[int] = Field(None, description="Vacancy parent ID", example=1)
     position: str = Field(..., description="Vacancy position", example="Python developer")
     priority: int = Field(..., description="Vacancy priority", example=1)
     requirements: Optional[str] = Field(
         None,
         description="vacancy requirements(HTML)",
         example="<p>Work responsibly</p>",
     )
-    state: VacancyState = Field(..., description="Vacnacy state", example=VacancyState.OPEN)
+    state: VacancyState = Field(..., description="Vacancy state", example=VacancyState.OPEN)
     values: Dict = Field(
         {},
         description="Additional vacancy fields",
         example={"experience": "without"},
     )
+
+
+class VacancyLog(BaseModel):
+    id: int = Field(..., description="Vacancy log ID", example=1)
+    state: VacancyState = Field(
+        ...,
+        description="Vacancy log state",
+        example=VacancyState.OPEN,
+    )
+    created: datetime = Field(
+        ...,
+        description="Date time the vacancy log created",
+        example=datetime(1970, 1, 1, 1, 1, 1),
+    )
+    # TODO: Solve close reason field problem (field exists with another name)
```

### Comparing `huntflow_webhook_models-0.0.5/huntflow_webhook_models/consts.py` & `huntflow_webhook_models-0.0.6/huntflow_webhook_models/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     VACANCY_REQUEST = "VACANCY-REQUEST"
     RESPONSE = "RESPONSE"
     OFFER = "OFFER"
     RECRUITMENT_EVALUATION = "RECRUITMENT-EVALUATION"
     SURVEY_QUESTIONARY = "SURVEY-QUESTIONARY"
 
 
+class CommonWebhookActionType(str, Enum):
+    ADD = "ADD"
+
+
 class ApplicantWebhookActionType(str, Enum):
     ADD = "ADD"
     EDIT = "EDIT"
     DELETE = "DELETE"
 
 
 class ApplicantLogType(str, Enum):
@@ -49,14 +53,24 @@
     OPEN = "OPEN"
     CLOSED = "CLOSED"
     HOLD = "HOLD"
     REOPEN = "REOPEN"
     VACANCY_REQUEST_ATTACH = "VACANCY_REQUEST_ATTACH"
     RESUME = "RESUME"
     CREATED = "CREATED"
+    EDIT = "EDIT"
+    LEAVE = "LEAVE"
+    JOIN = "JOIN"
+
+
+class VacancyRequestLogAction(str, Enum):
+    CREATE = "CREATE"
+    EDIT = "EDIT"
+    REMOVE = "REMOVE"
+    MIGRATE = "MIGRATE"
 
 
 class CalendarEventStatus(str, Enum):
     accepted = "accepted"
     declined = "declined"
     confirmed = "confirmed"
     tentative = "tentative"
```

### Comparing `huntflow_webhook_models-0.0.5/pyproject.toml` & `huntflow_webhook_models-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "huntflow-webhook-models"
-version = "0.0.5"
+version = "0.0.6"
 description = "Huntflow webhooks requests data models"
 authors = [
     { name = "Developers huntflow", email = "developer@huntflow.ru" },
 ]
 dependencies = [
     "pydantic>=1.7.2",
     "openapi-schema-pydantic>=1.2.4",
```

### Comparing `huntflow_webhook_models-0.0.5/PKG-INFO` & `huntflow_webhook_models-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huntflow-webhook-models
-Version: 0.0.5
+Version: 0.0.6
 Summary: Huntflow webhooks requests data models
 Author-Email: Developers huntflow <developer@huntflow.ru>
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

