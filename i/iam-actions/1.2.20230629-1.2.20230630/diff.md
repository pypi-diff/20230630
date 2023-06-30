# Comparing `tmp/iam_actions-1.2.20230629.tar.gz` & `tmp/iam_actions-1.2.20230630.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230629.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230630.tar", max compression
```

## Comparing `iam_actions-1.2.20230629.tar` & `iam_actions-1.2.20230630.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/README.md
--rw-r--r--   0        0        0      228 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/__init__.py
--rw-r--r--   0        0        0  4357291 2023-06-29 02:50:49.062111 iam_actions-1.2.20230629/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-29 02:49:07.677692 iam_actions-1.2.20230629/iam_actions/generate/services.py
--rw-r--r--   0        0        0   560422 2023-06-29 02:50:49.062111 iam_actions-1.2.20230629/iam_actions/policies.json
--rw-r--r--   0        0        0   197134 2023-06-29 02:50:49.062111 iam_actions-1.2.20230629/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   543554 2023-06-29 02:50:49.062111 iam_actions-1.2.20230629/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-29 02:50:49.818115 iam_actions-1.2.20230629/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230629/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230629/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/README.md
+-rw-r--r--   0        0        0      228 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4360093 2023-06-30 02:47:51.000463 iam_actions-1.2.20230630/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-30 02:45:58.675131 iam_actions-1.2.20230630/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   560805 2023-06-30 02:47:51.000463 iam_actions-1.2.20230630/iam_actions/policies.json
+-rw-r--r--   0        0        0   197240 2023-06-30 02:47:51.000463 iam_actions-1.2.20230630/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   543926 2023-06-30 02:47:51.000463 iam_actions-1.2.20230630/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-30 02:47:51.880422 iam_actions-1.2.20230630/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230630/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230630/PKG-INFO
```

### Comparing `iam_actions-1.2.20230629/LICENSE` & `iam_actions-1.2.20230630/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230629/README.md` & `iam_actions-1.2.20230630/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230629/iam_actions/actions.json` & `iam_actions-1.2.20230630/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997851464059598%*

 * *Differences: {"'appstream'": "{'CreateAppBlockBuilderStreamingURL': OrderedDict([('access_level', "*

 * *                "'Undocumented'), ('action', 'CreateAppBlockBuilderStreamingURL'), "*

 * *                "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *                "False), ('resources', [])]), 'StartAppBlockBuilder': "*

 * *                "OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                "'StartAppBlockBuilder'), ('condition_keys', []), ('description', 'Not Document […]*

```diff
@@ -6359,14 +6359,22 @@
             "orphan": false,
             "resources": [
                 "vpcingressconnection"
             ]
         }
     },
     "appstream": {
+        "AssociateAppBlockBuilderAppBlock": {
+            "access_level": "Undocumented",
+            "action": "AssociateAppBlockBuilderAppBlock",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "AssociateApplicationFleet": {
             "access_level": "Write",
             "action": "AssociateApplicationFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to associate the specified application with the fleet",
@@ -6443,14 +6451,30 @@
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an app block. App blocks store details about the virtual hard disk that contains the files for the application in an S3 bucket. It also stores the setup script with details about how to mount the virtual hard disk. App blocks are only supported for Elastic fleets",
             "orphan": false,
             "resources": []
         },
+        "CreateAppBlockBuilder": {
+            "access_level": "Undocumented",
+            "action": "CreateAppBlockBuilder",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateAppBlockBuilderStreamingURL": {
+            "access_level": "Undocumented",
+            "action": "CreateAppBlockBuilderStreamingURL",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateApplication": {
             "access_level": "Write",
             "action": "CreateApplication",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
@@ -6583,14 +6607,22 @@
             ],
             "description": "Grants permission to delete the specified app block",
             "orphan": false,
             "resources": [
                 "app-block"
             ]
         },
+        "DeleteAppBlockBuilder": {
+            "access_level": "Undocumented",
+            "action": "DeleteAppBlockBuilder",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteApplication": {
             "access_level": "Write",
             "action": "DeleteApplication",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to delete the specified application",
@@ -6689,14 +6721,30 @@
             "access_level": "Write",
             "action": "DeleteUser",
             "condition_keys": [],
             "description": "Grants permission to delete a user from the user pool",
             "orphan": false,
             "resources": []
         },
+        "DescribeAppBlockBuilderAppBlockAssociations": {
+            "access_level": "Undocumented",
+            "action": "DescribeAppBlockBuilderAppBlockAssociations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeAppBlockBuilders": {
+            "access_level": "Undocumented",
+            "action": "DescribeAppBlockBuilders",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeAppBlocks": {
             "access_level": "Read",
             "action": "DescribeAppBlocks",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list that describes one or more specified app blocks, if the app block arns are provided. Otherwise, all app blocks in the account are described",
             "orphan": false,
             "resources": [
@@ -6833,14 +6881,22 @@
             "access_level": "Write",
             "action": "DisableUser",
             "condition_keys": [],
             "description": "Grants permission to disable the specified user in the user pool. This action does not delete the user",
             "orphan": false,
             "resources": []
         },
+        "DisassociateAppBlockBuilderAppBlock": {
+            "access_level": "Undocumented",
+            "action": "DisassociateAppBlockBuilderAppBlock",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DisassociateApplicationFleet": {
             "access_level": "Write",
             "action": "DisassociateApplicationFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to disassociate the specified application from the specified fleet",
@@ -6923,14 +6979,22 @@
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of all tags for the specified AppStream 2.0 resource. The following resources can be tagged: Image builders, images, fleets, and stacks",
             "orphan": false,
             "resources": []
         },
+        "StartAppBlockBuilder": {
+            "access_level": "Undocumented",
+            "action": "StartAppBlockBuilder",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartFleet": {
             "access_level": "Write",
             "action": "StartFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to start the specified fleet",
@@ -6947,14 +7011,22 @@
             ],
             "description": "Grants permission to start the specified image builder",
             "orphan": false,
             "resources": [
                 "image-builder"
             ]
         },
+        "StopAppBlockBuilder": {
+            "access_level": "Undocumented",
+            "action": "StopAppBlockBuilder",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StopFleet": {
             "access_level": "Write",
             "action": "StopFleet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to stop the specified fleet",
@@ -7019,14 +7091,22 @@
                 "application",
                 "fleet",
                 "image",
                 "image-builder",
                 "stack"
             ]
         },
+        "UpdateAppBlockBuilder": {
+            "access_level": "Undocumented",
+            "action": "UpdateAppBlockBuilder",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateApplication": {
             "access_level": "Write",
             "action": "UpdateApplication",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to update the specified fields for the specified application",
@@ -57749,14 +57829,22 @@
             "access_level": "List",
             "action": "ListStudios",
             "condition_keys": [],
             "description": "Grants permission to list summary information about EMR Studios",
             "orphan": false,
             "resources": []
         },
+        "ListSupportedInstanceTypes": {
+            "access_level": "Undocumented",
+            "action": "ListSupportedInstanceTypes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListWorkspaceAccessIdentities": {
             "access_level": "List",
             "action": "ListWorkspaceAccessIdentities",
             "condition_keys": [],
             "description": "Grants permission to list identities that are granted access to a workspace",
             "orphan": false,
             "resources": [
@@ -82464,38 +82552,42 @@
             "description": "Grants permission to delete an existing attachment",
             "orphan": false,
             "resources": [
                 "attachment"
             ]
         },
         "DisableIndividualPublicProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisableIndividualPublicProfile",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to disable individual public profile page",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "expert"
+            ]
         },
         "DownloadAttachment": {
             "access_level": "Read",
             "action": "DownloadAttachment",
             "condition_keys": [],
             "description": "Grants permission to download existing attachment",
             "orphan": false,
             "resources": [
                 "attachment"
             ]
         },
         "EnableIndividualPublicProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "EnableIndividualPublicProfile",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to enable individual public profile page",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "expert"
+            ]
         },
         "EndCall": {
             "access_level": "Write",
             "action": "EndCall",
             "condition_keys": [],
             "description": "Grants permission to end a voice/video call",
             "orphan": false,
@@ -82550,20 +82642,22 @@
             "description": "Grants permission to request a websocket token for the conversation notifications",
             "orphan": false,
             "resources": [
                 "token"
             ]
         },
         "GetCompanyChatMessages": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetCompanyChatMessages",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to read chat messages in a company conversation",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "conversation"
+            ]
         },
         "GetCompanyProfile": {
             "access_level": "Read",
             "action": "GetCompanyProfile",
             "condition_keys": [],
             "description": "Grants permission to read a company profile",
             "orphan": false,
@@ -82666,20 +82760,22 @@
             "action": "InitiateCall",
             "condition_keys": [],
             "description": "Grants permission to start a voice/video call",
             "orphan": false,
             "resources": []
         },
         "LinkAwsCertification": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "LinkAwsCertification",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to link an AWS certification to individual profile",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "expert"
+            ]
         },
         "ListAttachments": {
             "access_level": "List",
             "action": "ListAttachments",
             "condition_keys": [],
             "description": "Grants permission to list existing attachments",
             "orphan": false,
@@ -82694,20 +82790,22 @@
             "description": "Grants permission to list existing conversations",
             "orphan": false,
             "resources": [
                 "conversation"
             ]
         },
         "ListExpertAccessLogs": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListExpertAccessLogs",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list access logs of expert activity",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "permission"
+            ]
         },
         "ListListings": {
             "access_level": "Read",
             "action": "ListListings",
             "condition_keys": [],
             "description": "Grants permission to list listings",
             "orphan": false,
@@ -82813,20 +82911,22 @@
             "description": "Grants permission to unarchive a conversation",
             "orphan": false,
             "resources": [
                 "conversation"
             ]
         },
         "UnlinkAwsCertification": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UnlinkAwsCertification",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to unlink an AWS certification from individual profile",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "expert"
+            ]
         },
         "UpdateCompanyProfile": {
             "access_level": "Write",
             "action": "UpdateCompanyProfile",
             "condition_keys": [],
             "description": "Grants permission to update a company profile",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230629/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230630/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230629/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230630/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230629/iam_actions/generate/generate.py` & `iam_actions-1.2.20230630/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230629/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230630/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230629/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230630/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230629/iam_actions/generate/services.py` & `iam_actions-1.2.20230630/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230629/iam_actions/policies.json` & `iam_actions-1.2.20230630/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999984201869806%*

 * *Differences: {"'serviceMap'": "{'Amazon Elastic MapReduce': {'Actions': {insert: [(51, "*

 * *                 "'ListSupportedInstanceTypes')]}}, 'Amazon AppStream 2.0': {'Actions': {insert: "*

 * *                 "[(0, 'AssociateAppBlockBuilderAppBlock'), (8, 'CreateAppBlockBuilder'), (9, "*

 * *                 "'CreateAppBlockBuilderStreamingURL'), (22, 'DeleteAppBlockBuilder'), (33, "*

 * *                 "'DescribeAppBlockBuilderAppBlockAssociations'), (34, "*

 * *                 "'DescribeAppBlockBuilders'), (50, 'DisassociateAppBlockB […]*

```diff
@@ -10073,43 +10073,49 @@
                 "aws:TagKeys"
             ]
         },
         "Amazon AppStream 2.0": {
             "ARNFormat": "arn:aws:appstream:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:appstream:.+",
             "Actions": [
+                "AssociateAppBlockBuilderAppBlock",
                 "AssociateApplicationFleet",
                 "AssociateApplicationToEntitlement",
                 "AssociateFleet",
                 "BatchAssociateUserStack",
                 "BatchDisassociateUserStack",
                 "CopyImage",
                 "CreateAppBlock",
+                "CreateAppBlockBuilder",
+                "CreateAppBlockBuilderStreamingURL",
                 "CreateApplication",
                 "CreateDirectoryConfig",
                 "CreateEntitlement",
                 "CreateFleet",
                 "CreateImageBuilder",
                 "CreateImageBuilderStreamingURL",
                 "CreateStack",
                 "CreateStreamingURL",
                 "CreateUpdatedImage",
                 "CreateUsageReportSubscription",
                 "CreateUser",
                 "DeleteAppBlock",
+                "DeleteAppBlockBuilder",
                 "DeleteApplication",
                 "DeleteDirectoryConfig",
                 "DeleteEntitlement",
                 "DeleteFleet",
                 "DeleteImage",
                 "DeleteImageBuilder",
                 "DeleteImagePermissions",
                 "DeleteStack",
                 "DeleteUsageReportSubscription",
                 "DeleteUser",
+                "DescribeAppBlockBuilderAppBlockAssociations",
+                "DescribeAppBlockBuilders",
                 "DescribeAppBlocks",
                 "DescribeApplicationFleetAssociations",
                 "DescribeApplications",
                 "DescribeDirectoryConfigs",
                 "DescribeEntitlements",
                 "DescribeFleets",
                 "DescribeImageBuilders",
@@ -10117,30 +10123,34 @@
                 "DescribeImages",
                 "DescribeSessions",
                 "DescribeStacks",
                 "DescribeUsageReportSubscriptions",
                 "DescribeUserStackAssociations",
                 "DescribeUsers",
                 "DisableUser",
+                "DisassociateAppBlockBuilderAppBlock",
                 "DisassociateApplicationFleet",
                 "DisassociateApplicationFromEntitlement",
                 "DisassociateFleet",
                 "EnableUser",
                 "ExpireSession",
                 "ListAssociatedFleets",
                 "ListAssociatedStacks",
                 "ListEntitledApplications",
                 "ListTagsForResource",
+                "StartAppBlockBuilder",
                 "StartFleet",
                 "StartImageBuilder",
+                "StopAppBlockBuilder",
                 "StopFleet",
                 "StopImageBuilder",
                 "Stream",
                 "TagResource",
                 "UntagResource",
+                "UpdateAppBlockBuilder",
                 "UpdateApplication",
                 "UpdateDirectoryConfig",
                 "UpdateEntitlement",
                 "UpdateFleet",
                 "UpdateImagePermissions",
                 "UpdateStack"
             ],
@@ -13756,14 +13766,15 @@
                 "ListNotebookExecutions",
                 "ListReleaseLabels",
                 "ListRepositories",
                 "ListSecurityConfigurations",
                 "ListSteps",
                 "ListStudioSessionMappings",
                 "ListStudios",
+                "ListSupportedInstanceTypes",
                 "ListWorkspaceAccessIdentities",
                 "ModifyCluster",
                 "ModifyInstanceFleet",
                 "ModifyInstanceGroups",
                 "OpenEditorInConsole",
                 "PutAutoScalingPolicy",
                 "PutAutoTerminationPolicy",
```

### Comparing `iam_actions-1.2.20230629/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230630/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999016135379772%*

 * *Differences: {"'iq'": "{'permission': OrderedDict([('arn_pattern', 'arn:*:iq-permission:*::permission/*'), "*

 * *         "('condition_keys', None)])}"}*

```diff
@@ -3618,14 +3618,18 @@
             "arn_pattern": "arn:*:iq:*::paymentRequest/*/*/*",
             "condition_keys": null
         },
         "paymentSchedule": {
             "arn_pattern": "arn:*:iq:*::paymentSchedule/*/*/*",
             "condition_keys": null
         },
+        "permission": {
+            "arn_pattern": "arn:*:iq-permission:*::permission/*",
+            "condition_keys": null
+        },
         "proposal": {
             "arn_pattern": "arn:*:iq:*::proposal/*/*",
             "condition_keys": null
         },
         "request": {
             "arn_pattern": "arn:*:iq:*::request/*",
             "condition_keys": null
```

### Comparing `iam_actions-1.2.20230629/iam_actions/services.json` & `iam_actions-1.2.20230630/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999834620124691%*

 * *Differences: {"'appstream'": "{'Actions': {insert: [(0, 'AssociateAppBlockBuilderAppBlock'), (8, "*

 * *                "'CreateAppBlockBuilder'), (9, 'CreateAppBlockBuilderStreamingURL'), (22, "*

 * *                "'DeleteAppBlockBuilder'), (33, 'DescribeAppBlockBuilderAppBlockAssociations'), "*

 * *                "(34, 'DescribeAppBlockBuilders'), (50, 'DisassociateAppBlockBuilderAppBlock'), "*

 * *                "(60, 'StartAppBlockBuilder'), (63, 'StopAppBlockBuilder'), (69, "*

 * *                "'UpdateAppBlockBuilder')]}}",*

 * * "'elast […]*

```diff
@@ -1071,43 +1071,49 @@
         "ARNFormats": [
             "arn:aws:appstream:${Region}:${Account}:${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
             "^arn:aws:appstream:.+"
         ],
         "Actions": [
+            "AssociateAppBlockBuilderAppBlock",
             "AssociateApplicationFleet",
             "AssociateApplicationToEntitlement",
             "AssociateFleet",
             "BatchAssociateUserStack",
             "BatchDisassociateUserStack",
             "CopyImage",
             "CreateAppBlock",
+            "CreateAppBlockBuilder",
+            "CreateAppBlockBuilderStreamingURL",
             "CreateApplication",
             "CreateDirectoryConfig",
             "CreateEntitlement",
             "CreateFleet",
             "CreateImageBuilder",
             "CreateImageBuilderStreamingURL",
             "CreateStack",
             "CreateStreamingURL",
             "CreateUpdatedImage",
             "CreateUsageReportSubscription",
             "CreateUser",
             "DeleteAppBlock",
+            "DeleteAppBlockBuilder",
             "DeleteApplication",
             "DeleteDirectoryConfig",
             "DeleteEntitlement",
             "DeleteFleet",
             "DeleteImage",
             "DeleteImageBuilder",
             "DeleteImagePermissions",
             "DeleteStack",
             "DeleteUsageReportSubscription",
             "DeleteUser",
+            "DescribeAppBlockBuilderAppBlockAssociations",
+            "DescribeAppBlockBuilders",
             "DescribeAppBlocks",
             "DescribeApplicationFleetAssociations",
             "DescribeApplications",
             "DescribeDirectoryConfigs",
             "DescribeEntitlements",
             "DescribeFleets",
             "DescribeImageBuilders",
@@ -1115,30 +1121,34 @@
             "DescribeImages",
             "DescribeSessions",
             "DescribeStacks",
             "DescribeUsageReportSubscriptions",
             "DescribeUserStackAssociations",
             "DescribeUsers",
             "DisableUser",
+            "DisassociateAppBlockBuilderAppBlock",
             "DisassociateApplicationFleet",
             "DisassociateApplicationFromEntitlement",
             "DisassociateFleet",
             "EnableUser",
             "ExpireSession",
             "ListAssociatedFleets",
             "ListAssociatedStacks",
             "ListEntitledApplications",
             "ListTagsForResource",
+            "StartAppBlockBuilder",
             "StartFleet",
             "StartImageBuilder",
+            "StopAppBlockBuilder",
             "StopFleet",
             "StopImageBuilder",
             "Stream",
             "TagResource",
             "UntagResource",
+            "UpdateAppBlockBuilder",
             "UpdateApplication",
             "UpdateDirectoryConfig",
             "UpdateEntitlement",
             "UpdateFleet",
             "UpdateImagePermissions",
             "UpdateStack"
         ],
@@ -7797,14 +7807,15 @@
             "ListNotebookExecutions",
             "ListReleaseLabels",
             "ListRepositories",
             "ListSecurityConfigurations",
             "ListSteps",
             "ListStudioSessionMappings",
             "ListStudios",
+            "ListSupportedInstanceTypes",
             "ListWorkspaceAccessIdentities",
             "ModifyCluster",
             "ModifyInstanceFleet",
             "ModifyInstanceGroups",
             "OpenEditorInConsole",
             "PutAutoScalingPolicy",
             "PutAutoTerminationPolicy",
```

### Comparing `iam_actions-1.2.20230629/pyproject.toml` & `iam_actions-1.2.20230630/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230629"
+version = "1.2.20230630"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230629/setup.py` & `iam_actions-1.2.20230630/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230629',
+    'version': '1.2.20230630',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230629/PKG-INFO` & `iam_actions-1.2.20230630/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230629
+Version: 1.2.20230630
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

