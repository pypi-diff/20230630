# Comparing `tmp/kaiju_tasks-2.1.1-py3-none-any.whl.zip` & `tmp/kaiju_tasks-2.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 18200 bytes, number of entries: 15
--rw-r--r--  2.0 unx      131 b- defN 23-Jun-29 13:02 kaiju_tasks/__init__.py
--rw-r--r--  2.0 unx    36802 b- defN 23-Jun-29 13:02 kaiju_tasks/services.py
--rw-r--r--  2.0 unx     4360 b- defN 23-Jun-29 13:02 kaiju_tasks/types.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-29 13:02 kaiju_tasks/tasks_gui/__init__.py
--rw-r--r--  2.0 unx     2011 b- defN 23-Jun-29 13:02 kaiju_tasks/tasks_gui/models.py
--rw-r--r--  2.0 unx     4272 b- defN 23-Jun-29 13:02 kaiju_tasks/tasks_gui/service.py
--rw-r--r--  2.0 unx      350 b- defN 23-Jun-29 13:02 kaiju_tasks/tasks_gui/validators.py
--rw-r--r--  2.0 unx       42 b- defN 23-Jun-29 13:02 kaiju_tasks/tests/__init__.py
--rw-r--r--  2.0 unx     2014 b- defN 23-Jun-29 13:02 kaiju_tasks/tests/fixtures.py
--rw-r--r--  2.0 unx    12224 b- defN 23-Jun-29 13:02 kaiju_tasks/tests/test_tasks.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-29 13:02 kaiju_tasks-2.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3056 b- defN 23-Jun-29 13:02 kaiju_tasks-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 13:02 kaiju_tasks-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-29 13:02 kaiju_tasks-2.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-29 13:02 kaiju_tasks-2.1.1.dist-info/RECORD
-15 files, 67271 bytes uncompressed, 16108 bytes compressed:  76.1%
+Zip file size: 18305 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-30 16:29 kaiju_tasks/__init__.py
+-rw-r--r--  2.0 unx    37518 b- defN 23-Jun-30 16:29 kaiju_tasks/services.py
+-rw-r--r--  2.0 unx     4360 b- defN 23-Jun-30 16:29 kaiju_tasks/types.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-30 16:29 kaiju_tasks/tasks_gui/__init__.py
+-rw-r--r--  2.0 unx     2011 b- defN 23-Jun-30 16:29 kaiju_tasks/tasks_gui/models.py
+-rw-r--r--  2.0 unx     4272 b- defN 23-Jun-30 16:29 kaiju_tasks/tasks_gui/service.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Jun-30 16:29 kaiju_tasks/tasks_gui/validators.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-30 16:29 kaiju_tasks/tests/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 23-Jun-30 16:29 kaiju_tasks/tests/fixtures.py
+-rw-r--r--  2.0 unx    12224 b- defN 23-Jun-30 16:29 kaiju_tasks/tests/test_tasks.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3056 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/RECORD
+15 files, 68031 bytes uncompressed, 16213 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: kaiju_tasks/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_tasks/tests/test_tasks.py
 Comment: 
 
-Filename: kaiju_tasks-2.1.1.dist-info/LICENSE
+Filename: kaiju_tasks-2.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_tasks-2.1.1.dist-info/METADATA
+Filename: kaiju_tasks-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_tasks-2.1.1.dist-info/WHEEL
+Filename: kaiju_tasks-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_tasks-2.1.1.dist-info/top_level.txt
+Filename: kaiju_tasks-2.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_tasks-2.1.1.dist-info/RECORD
+Filename: kaiju_tasks-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_tasks/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .types import *
 from .services import *
 
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_tasks/services.py

```diff
@@ -12,14 +12,15 @@
 from kaiju_tools.app import ContextableService, Scheduler, service_class_registry
 from kaiju_tools.exceptions import ValidationError, InternalError
 from kaiju_tools.interfaces import PublicInterface
 from kaiju_tools.functions import get_short_uid, retry
 from kaiju_tools.streams import StreamRPCClient, Topic
 from kaiju_tools.templates import Template
 from kaiju_tools.rpc import JSONRPCServer, JSONRPCHeaders, RPCError
+from kaiju_tools.types import Scope
 from kaiju_db import SQLService, DatabaseService
 from kaiju_redis import RedisTransportService
 
 from kaiju_tasks.types import TaskStatus, RestartPolicy, Limit, Task, ExecutorTask, Notification
 
 __all__ = ['TaskService', 'NotificationService', 'TaskManager', 'TaskExecutor']
 
@@ -79,23 +80,23 @@
     )  # TODO: is_not for alchemy 1.4
     sa.Index(
         f'idx__{table.name}__status__idle',
         table.c.next_run.desc(),
         postgresql_where=sa.and_(table.c.enabled.is_(True), table.c.status == TaskStatus.IDLE.value),
     )
 
-    task_command = j.Object(
+    _task_command = j.Object(
         {'id': j.Integer(), 'method': j.String(), 'params': j.Object()}, additionalProperties=False, required=['method']
     )
 
-    validator = j.Object(
+    _task_validator = j.Object(
         {
             'id': j.String(minLength=1),
             'app': j.String(),
-            'commands': j.Array(task_command, minItems=1, maxItems=Limit.MAX_STAGES.value),
+            'commands': j.Array(_task_command, minItems=1, maxItems=Limit.MAX_STAGES.value),
             'kws': j.Object(),
             'cron': j.String(),
             'max_exec_timeout': j.Integer(minimum=Limit.MIN_T.value, maximum=Limit.MAX_T.value),
             'max_retries': j.Integer(minimum=0, maximum=Limit.MAX_RETRIES.value),
             'restart_policy': j.Enumerated(enum=[RestartPolicy.CURRENT.value, RestartPolicy.FIRST.value]),
             'next_task': j.String(minLength=1),
             'notify': j.Boolean(),
@@ -117,15 +118,15 @@
         return {
             '*': self.PermissionKeys.GLOBAL_USER_PERMISSION,
             'delete_old_tasks': self.PermissionKeys.GLOBAL_SYSTEM_PERMISSION,
         }
 
     @property
     def validators(self) -> dict:
-        return {'create': self.validator}
+        return {'create': j.Object({'data': self._task_validator}, additionalProperties=True, required=['data'])}
 
     async def delete_old_tasks(self, interval_days: int = 7) -> None:
         """Delete old tasks and notifications, cron tasks are excluded."""
         sql = self.table.delete().where(
             sa.and_(self.table.c.cron.is_(None), self.table.c.created < datetime.now() - timedelta(days=interval_days))
         )
         await self._wrap_delete(None, sql)
@@ -388,15 +389,15 @@
             .values({'status': TaskStatus.SUSPENDED.value, 'executor_id': None})
         )
         await self._db.execute(sql)
         await self._redis.hdel(self.executor_map_key, [str(executor_id)])
 
     async def execute_stage(self, task_id: str, executor_id: UUID, stage: int) -> None:
         """Tell the manager what a task stage is being executed."""
-        self.logger.info('Stage is executed', task_id=task_id, stage=stage, executor_id=executor_id)
+        self.logger.info('Stage executed', task_id=task_id, stage=stage, executor_id=executor_id)
         sql = (
             self.table.update()
             .where(sa.and_(self.table.c.id == task_id, self.table.c.status == TaskStatus.QUEUED.value))
             .values(
                 {
                     'status': TaskStatus.EXECUTED.value,
                     # 'stage': stage,
@@ -412,96 +413,108 @@
     ) -> None:
         """Write stage result to the task table.
 
         This method will also change task status depending on which stage has been executed. The task my become
         'FINISHED' or 'FAILED'.
         """
         sql = self.table.update().where(
-            sa.and_(
-                self.table.c.id == task_id,
-                self.table.c.executor_id == executor_id,
-                self.table.c.stage == stage,
-                self.table.c.status.in_([TaskStatus.EXECUTED.value, TaskStatus.QUEUED.value]),
+            sa.or_(
+                sa.and_(
+                    self.table.c.id == task_id,
+                    self.table.c.executor_id == executor_id,
+                    self.table.c.stage == stage,
+                    self.table.c.status.in_([TaskStatus.EXECUTED.value]),
+                ),
+                sa.and_(
+                    self.table.c.id == task_id,
+                    self.table.c.executor_id.is_(None),
+                    self.table.c.stage == stage,
+                    self.table.c.status.in_([TaskStatus.QUEUED.value]),
+                ),
             )
         )
         columns = [self.table.c.job_id, self.table.c.result, self.table.c.notify, self.table.c.user_id]
         if error:
-            self.logger.info('Stage failed', stage=stage, task_id=id, executor_id=executor_id, error=error)
             sql = sql.values(
                 {
                     'status': TaskStatus.FAILED.value,
                     'error': result,
                     'exit_code': self.ExitCode.EXECUTION_ERROR.value,
                     'executor_id': None,
                     'next_run': None,
                 }
             ).returning(*columns)
             task = await self._db.execute(sql)
             task = task.first()
-            if task and task.notify:
-                task = task._asdict()  # noqa
-                notification = Notification(
-                    message='task.result',
-                    user_id=task['user_id'],
-                    task_id=task_id,
-                    job_id=task['job_id'],
-                    status=TaskStatus.FAILED.value,
-                    result=task['result'],
-                    exit_code=self.ExitCode.EXECUTION_ERROR.value,
-                    error=result,
-                )
-                await self._notifications.create(notification, columns=[])
+            if task:
+                self.logger.error('Stage failed', stage=stage, task_id=task_id, executor_id=executor_id, error=result)
+                if task.notify:
+                    task = task._asdict()  # noqa
+                    notification = Notification(
+                        message='task.result',
+                        user_id=task['user_id'],
+                        task_id=task_id,
+                        job_id=task['job_id'],
+                        status=TaskStatus.FAILED.value,
+                        result=task['result'],
+                        exit_code=self.ExitCode.EXECUTION_ERROR.value,
+                        error=result,
+                    )
+                    await self._notifications.create(notification, columns=[])
         elif stage == stages - 1:
-            self.logger.info('Task finished', stage=stage, task_id=task_id, executor_id=executor_id)
             columns.append(self.table.c.next_task)
             sql = sql.values(
                 {
                     'status': TaskStatus.FINISHED.value,
                     'result': self.table.c.result + [result],
                     'exit_code': self.ExitCode.SUCCESS.value,
                     'executor_id': None,
                     'next_run': None,
                 }
             ).returning(*columns)
             task = await self._db.execute(sql)
             task = task.first()
-            if task and task.next_task:
-                self.logger.info('Starting next task', task_id=task_id, next_task=task.next_task)
-                sql = (
-                    self.table.update()
-                    .where(
-                        sa.and_(
-                            self.table.c.id == task.next_task,
-                            self.table.c.status.in_(
-                                [TaskStatus.IDLE.value, TaskStatus.FAILED.value, TaskStatus.FINISHED.value]
-                            ),
-                            self.table.c.enabled.is_(True),
+            if task:
+                self.logger.info('Task finished', stage=stage, task_id=task_id, executor_id=executor_id)
+                if task.next_task:
+                    self.logger.info('Starting next task', task_id=task_id, next_task=task.next_task)
+                    sql = (
+                        self.table.update()
+                        .where(
+                            sa.and_(
+                                self.table.c.id == task.next_task,
+                                self.table.c.status.in_(
+                                    [TaskStatus.IDLE.value, TaskStatus.FAILED.value, TaskStatus.FINISHED.value]
+                                ),
+                                self.table.c.enabled.is_(True),
+                            )
                         )
+                        .values({'status': TaskStatus.IDLE.value, 'next_run': int(time())})
                     )
-                    .values({'status': TaskStatus.IDLE.value, 'next_run': int(time())})
-                )
-                await self._db.execute(sql)
-            if task and task.notify:
-                task = task._asdict()  # noqa
-                notification = Notification(
-                    message='task.result',
-                    user_id=task['user_id'],
-                    task_id=task_id,
-                    job_id=task['job_id'],
-                    status=TaskStatus.FINISHED.value,
-                    result=task['result'],
-                    exit_code=self.ExitCode.SUCCESS.value,
-                )
-                await self._notifications.create(notification, columns=[])
+                    await self._db.execute(sql)
+                if task.notify:
+                    task = task._asdict()  # noqa
+                    notification = Notification(
+                        message='task.result',
+                        user_id=task['user_id'],
+                        task_id=task_id,
+                        job_id=task['job_id'],
+                        status=TaskStatus.FINISHED.value,
+                        result=task['result'],
+                        exit_code=self.ExitCode.SUCCESS.value,
+                    )
+                    await self._notifications.create(notification, columns=[])
         else:
-            self.logger.info('Stage finished', stage=stage, task_id=task_id, executor_id=executor_id)
             sql = sql.values(
                 {'status': TaskStatus.EXECUTED.value, 'result': self.table.c.result + [result], 'stage': stage + 1}
             )
-            await self._db.execute(sql)
+            task = await self._db.execute(sql)
+            task = task.first()
+            if task:
+                self.logger.info('Stage finished', stage=stage, task_id=task_id, executor_id=executor_id)
 
     async def _queue_tasks(self):
         """Iterate."""
         await self._expell_dead_executors()
         await self._abort_timed_out_tasks()
         await self._restart_cron_tasks()
         await self._queue_suspended_and_idle()
@@ -550,14 +563,16 @@
                 )
             )
             .values(
                 {
                     'status': TaskStatus.QUEUED.value,
                     'queued_at': int(time()),
                     'exec_deadline': int(time()) + self.table.c.max_exec_timeout,
+                    'exit_code': None,
+                    'error': None,
                 }
             )
             .returning(
                 self.table.c.id,
                 self.table.c.commands,
                 self.table.c.kws,
                 self.table.c.stage,
@@ -661,16 +676,16 @@
             .values(
                 {
                     'status': TaskStatus.IDLE.value,
                     'result': [],
                     'stage': 0,
                     'executor_id': None,
                     'retries': 0,
-                    'exit_code': None,
-                    'error': None,
+                    # 'exit_code': None,
+                    # 'error': None,
                 }
             )
             .returning(self.table.c.id, self.table.c.cron)
         )
         async with self._db.begin() as conn:
             cron_tasks = await conn.execute(sql)
             cron_tasks = [r._asdict() for r in cron_tasks.all()]  # noqa
@@ -787,60 +802,61 @@
             JSONRPCHeaders.CORRELATION_ID_HEADER: data['job_id'],
         }
         for n, cmd in enumerate(data['commands']):
             if self._closing:
                 break
             stage = data['stage'] + n
             await self._alert_on_stage_execution(data, stage)
+            self.logger.info(
+                'Stage executed', task_id=data['id'], stage=stage, method=cmd['method'], deadline=data['exec_deadline']
+            )
             try:
                 cmd = Template(cmd).fill(template_data)
-                _, result = await self._rpc.call(body=cmd, headers=headers)
+                _, result = await self._rpc.call(body=cmd, headers=headers, scope=Scope.SYSTEM)
             except Exception as exc:
-                self.logger.error('Stage error', exc_info=exc, task_id=data['id'], stage=stage)
-                result = RPCError(id=None, error=InternalError(base_exc=exc, message='Template evaluation error'))
-                await self._write_stage_result(data, stage, error=True, result=result)
-                break
+                error = result = RPCError(
+                    id=None, error=InternalError(base_exc=exc, message='Template evaluation error')
+                )
             else:
-                self.logger.info('Stage finished', task_id=data['id'], stage=stage)
                 error, result = self._parse_result(result)
-                await self._write_stage_result(data, stage, error, result)
-                if error:
-                    break
+
+            if error:
+                self.logger.error(
+                    'Stage failed', task_id=data['id'], stage=stage, method=cmd['method'], error=error.error
+                )
+                await self._write_stage_result(data, stage, error=True, result=result)
+                return
+            else:
+                self.logger.info('Stage finished', task_id=data['id'], stage=stage, method=cmd['method'])
                 template_data[str(stage)] = result
+                await self._write_stage_result(data, stage, error=False, result=result)
 
     @staticmethod
     def _get_template_data(data: ExecutorTask) -> dict:
         env = {str(stage): data['result'][stage] for stage in range(data['stage'])}
         env['kws'] = data['kws']
         return env
 
     @staticmethod
     def _parse_result(result) -> tuple:
         """Get error flag and result from rpc server response."""
         if isinstance(result, list):
             _result = []
             for r in result:
                 if isinstance(r, RPCError):
-                    result.append(r.repr())
+                    result.append(r)
                 else:
                     result.append(r.result)
             return False, _result
         elif isinstance(result, RPCError):
-            result = result.repr()
-            return True, result
+            return result, result
         else:
             return False, result.result
 
     async def _alert_on_stage_execution(self, data: ExecutorTask, stage: int):
-        self.logger.info(
-            'Executing stage',
-            task_id=data['id'],
-            stage=stage,
-            deadline=data['exec_deadline'],
-        )
         await retry(
             self._stream.call,
             kws=dict(
                 headers={JSONRPCHeaders.CORRELATION_ID_HEADER: data['job_id']},
                 method=f'{self.manager_service_name}.execute_stage',
                 params={'task_id': data['id'], 'executor_id': self.app.id, 'stage': stage},
                 app=self._manager_app,
@@ -848,17 +864,14 @@
             ),
             retries=3,
             retry_timeout=1,
             logger=self.logger,
         )
 
     async def _write_stage_result(self, data: ExecutorTask, stage: int, error: bool, result):
-        self.logger.info(
-            'Writing stage result', task_id=data['id'], stage=stage, deadline=data['exec_deadline'], error=error
-        )
         await retry(
             self._stream.call,
             kws=dict(
                 headers={JSONRPCHeaders.CORRELATION_ID_HEADER: data['job_id']},
                 method=f'{self.manager_service_name}.write_stage',
                 params={
                     'task_id': data['id'],
```

## kaiju_tasks/tests/fixtures.py

```diff
@@ -2,15 +2,16 @@
 
 from kaiju_tasks.services import *
 
 __all__ = ['task_service', 'notification_service', 'mock_task_executor', 'task_manager']
 
 
 @pytest.fixture
-def task_service(app, database_service) -> TaskService:
+def task_service(app, rpc, database_service) -> TaskService:
+    rpc._use_annotation_parser = False
     service = TaskService(app=app, database_service=database_service)
     app.services.add_service(service)
     return service
 
 
 @pytest.fixture
 def notification_service(app, database_service, task_service) -> NotificationService:
```

## Comparing `kaiju_tasks-2.1.1.dist-info/LICENSE` & `kaiju_tasks-2.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_tasks-2.1.1.dist-info/METADATA` & `kaiju_tasks-2.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-tasks
-Version: 2.1.1
+Version: 2.1.2
 Summary: Service and user task management
 Home-page: https://gitlab.com/kaiju-python/kaiju-tasks
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `kaiju_tasks-2.1.1.dist-info/RECORD` & `kaiju_tasks-2.1.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-kaiju_tasks/__init__.py,sha256=UDvdpeRLEfRiyJDvmAQUEz-rPmNZ83ixesPG1TljA00,131
-kaiju_tasks/services.py,sha256=Sho52cJFL-kTNJYO-Wdr2q2U-AcT6e6o_fOpGzirT-s,36802
+kaiju_tasks/__init__.py,sha256=8DSTDuF26lO6QQluj4ZgjADvGIXDPHlNRgW9scwh6HE,131
+kaiju_tasks/services.py,sha256=dDqf5ydswVbQxaxB-SmIUl-r-2ineSabshAx14goJ_w,37518
 kaiju_tasks/types.py,sha256=tp6fm6GJv8B5B6YhhiiZIbf00ahIBHUqaZNEQJFXEuw,4360
 kaiju_tasks/tasks_gui/__init__.py,sha256=_gDfM5r8uxCvydv3NOUN21imwJW_NW9R16UXWExQAE8,38
 kaiju_tasks/tasks_gui/models.py,sha256=iXqYnYYh8TJ7jkVxyEmMeykfpmoNfEfEERW-1jwzjsk,2011
 kaiju_tasks/tasks_gui/service.py,sha256=_qCURg-h6I9OI5uZdTGYCzJglXPXomcqAt6D7ODLRmU,4272
 kaiju_tasks/tasks_gui/validators.py,sha256=QybfHwKMWJq9AcGlXO7F5fuEGLssjHN2jcAV0UI6FPc,350
 kaiju_tasks/tests/__init__.py,sha256=WlPruePOcaMi5ikqn6GheE1Z-zYcysb9M1dj6SteWGY,42
-kaiju_tasks/tests/fixtures.py,sha256=gN_EbsLRnw8W6JD0FFuFCzMpHrMkFTP8_AmIhz1crLY,2014
+kaiju_tasks/tests/fixtures.py,sha256=1WRWnb5aCklCpRo0iqp1rquZSB8qgKBULv5MhaO2rck,2058
 kaiju_tasks/tests/test_tasks.py,sha256=YvmLscWAwko7eQ2Jw4vXTrO7SkefFu_P8eOEMNT-lkk,12224
-kaiju_tasks-2.1.1.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_tasks-2.1.1.dist-info/METADATA,sha256=5yLKLunb0Pad7lm7FBomcl7-aJy1kgNMzpHaZyrHpT4,3056
-kaiju_tasks-2.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_tasks-2.1.1.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
-kaiju_tasks-2.1.1.dist-info/RECORD,,
+kaiju_tasks-2.1.2.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_tasks-2.1.2.dist-info/METADATA,sha256=V5-rqyn0UshFZEgXiCOxubapGze8tv5CKme92ncDRMU,3056
+kaiju_tasks-2.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_tasks-2.1.2.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
+kaiju_tasks-2.1.2.dist-info/RECORD,,
```

