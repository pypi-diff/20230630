# Comparing `tmp/pygame_ecs-0.2.8.tar.gz` & `tmp/pygame_ecs-0.2.9.tar.gz`

## Comparing `pygame_ecs-0.2.8.tar` & `pygame_ecs-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/.gitattributes
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pygame_ecs/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pygame_ecs/entity.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pygame_ecs/exceptions.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pygame_ecs/components/base_component.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pygame_ecs/managers/component_manager.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pygame_ecs/managers/entity_manager.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pygame_ecs/managers/system_manager.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pygame_ecs/systems/base_system.py
--rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/test/circle.png
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/test/draw_test.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/test/particle_test_cpu.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/test/particle_test_gpu.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/test/speed_test.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/test/tester.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/LICENSE
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/README.md
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pygame_ecs-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/.gitattributes
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pygame_ecs/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pygame_ecs/entity.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pygame_ecs/exceptions.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pygame_ecs/components/base_component.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pygame_ecs/managers/component_manager.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pygame_ecs/managers/entity_manager.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pygame_ecs/managers/system_manager.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pygame_ecs/systems/base_system.py
+-rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/test/circle.png
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/test/draw_test.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/test/particle_test_cpu.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/test/particle_test_gpu.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/test/speed_test.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/test/tester.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/README.md
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 pygame_ecs-0.2.9/PKG-INFO
```

### Comparing `pygame_ecs-0.2.8/pygame_ecs/managers/component_manager.py` & `pygame_ecs-0.2.9/pygame_ecs/managers/component_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pygame_ecs.exceptions import EntityDoesNotHaveComponent
 
 
 ComponentInstanceType = typing.TypeVar("ComponentInstanceType", bound=BaseComponent)
 
 
 class ComponentManager:
+    __slots__ = ("components",)
     def __init__(self) -> None:
         self.components: dict[typing.Type[BaseComponent], dict[Entity, ComponentInstanceType]] = {}  # type: ignore
 
     def init_components(self):
         # get all subclasses using BaseComponent
         component_subclasses = BaseComponent.__subclasses__()
         for component_subclass in component_subclasses:
```

### Comparing `pygame_ecs-0.2.8/pygame_ecs/managers/entity_manager.py` & `pygame_ecs-0.2.9/pygame_ecs/managers/entity_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pygame_ecs.entity import Entity
 from pygame_ecs.managers.component_manager import ComponentManager
 from pygame_ecs.exceptions import EntityAlreadyInLimbo
 
 
 class EntityManager:
+    __slots__ = ("component_manager", "entities", "dead_entities", "_limbo", "count")
     def __init__(self, component_manager: ComponentManager) -> None:
         self.component_manager = component_manager
         self.entities: dict[Entity, None] = {}
         self.dead_entities: list[Entity] = []
         self._limbo: dict[Entity, None] = {}
         self.count: int = 0
```

### Comparing `pygame_ecs-0.2.8/pygame_ecs/managers/system_manager.py` & `pygame_ecs-0.2.9/pygame_ecs/managers/system_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pygame_ecs.managers.component_manager import ComponentManager
 from pygame_ecs.managers.entity_manager import EntityManager
 
 SystemType = typing.TypeVar("SystemType", bound=BaseSystem)
 
 
 class SystemManager:
+    __slots__ = ("entity_manager", "component_manager", "systems")
     def __init__(
         self, entity_manager: EntityManager, component_manager: ComponentManager
     ) -> None:
         self.entity_manager = entity_manager
         self.component_manager = component_manager
         self.systems: list[BaseSystem] = []
```

### Comparing `pygame_ecs-0.2.8/pygame_ecs/systems/base_system.py` & `pygame_ecs-0.2.9/pygame_ecs/systems/base_system.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.8/test/circle.png` & `pygame_ecs-0.2.9/test/circle.png`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.8/test/draw_test.py` & `pygame_ecs-0.2.9/test/draw_test.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.8/test/particle_test_cpu.py` & `pygame_ecs-0.2.9/test/particle_test_cpu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 import random
 import pygame
 import pygame_ecs
 
 
 class Position(pygame_ecs.BaseComponent):
+    __slots__ = ("x", "y")
     def __init__(self, x: int, y: int):
         super().__init__()
         self.x = x
         self.y = y
 
 
 class BallRenderer(pygame_ecs.BaseComponent):
+    __slots__ = ("radius", "color")
     def __init__(self, radius: int, color) -> None:
         super().__init__()
         self.radius = radius
         self.color = color
 
 
 class Velocity(pygame_ecs.BaseComponent):
+    __slots__ = ("vec",)
     def __init__(self, vec: pygame.math.Vector2) -> None:
         super().__init__()
         self.vec = vec
 
 
 class BallDrawSystem(pygame_ecs.BaseSystem):
+    __slots__ = ("screen",)
     def __init__(self, screen) -> None:
         super().__init__(required_component_types=[Position, BallRenderer])
         self.screen = screen
 
     def update_entity(self, entity, entity_components):
         pos: Position = entity_components[Position]  # type: ignore
         ball_renderer: BallRenderer = entity_components[BallRenderer]  # type: ignore
         pygame.draw.circle(self.screen, ball_renderer.color, (pos.x, pos.y), ball_renderer.radius)  # type: ignore
 
 
 class BallPhysics(pygame_ecs.BaseSystem):
+    __slots__ = ("dt", "screen")
     def __init__(self, screen) -> None:
         super().__init__(required_component_types=[Position, Velocity])
         self.dt = 0
         self.screen = screen
 
     def update_entity(self, entity, entity_components):
         pos: Position = entity_components[Position]  # type: ignore
```

### Comparing `pygame_ecs-0.2.8/test/particle_test_gpu.py` & `pygame_ecs-0.2.9/test/particle_test_gpu.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.8/test/speed_test.py` & `pygame_ecs-0.2.9/test/speed_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 # TODO: put entities as a list in entity_manager
 # Also make the component manager be kept as a reference in the system_manager
 # I can insert EntityManager reference into BaseSystem Subclasses using the same method I've used with components nvm i cant lol
 # actually add the systems into
 
 
 class Position(pygame_ecs.BaseComponent):
+    __slots__ = ("x", "y")
     def __init__(self, x: int, y: int):
         super().__init__()
         self.x = x
         self.y = y
 
 
 class Velocity(pygame_ecs.BaseComponent):
+    __slots__ = ("vec",)
     def __init__(self, vec: list[int | float]) -> None:
         super().__init__()
         self.vec = vec
 
 
 class BallPhysics(pygame_ecs.BaseSystem):
     def __init__(self) -> None:
@@ -91,11 +93,11 @@
     entity = entity_manager.add_entity()
     component_manager.add_component(entity, Position(center[0], center[1]))
     if arg == "perfect":
         component_manager.add_component(entity, Velocity(vel))
 
 REPEAT = 1_000
 
-res = timeit(lambda: system_manager.update_entities(), number=REPEAT)  # type: ignore
+result = timeit(lambda: system_manager.update_entities(), number=REPEAT)  # type: ignore
 print(
-    f"Took {res/REPEAT} roughly for each frame, using {len(entity_manager.entities)} entities, setting: {arg}"
+    f"Took a total of {result} and {result/REPEAT} roughly for each frame, using {len(entity_manager.entities)} entities, setting: {arg}"
 )
```

### Comparing `pygame_ecs-0.2.8/.gitignore` & `pygame_ecs-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.8/LICENSE` & `pygame_ecs-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.2.8/README.md` & `pygame_ecs-0.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```python
 entity = entity_manager.add_entity()
 ```
 
 You can delete an entity like this:
 ```python
-    entity_manager.kill_entity(entity)
+entity_manager.kill_entity(entity)
 ```
 
 Components are just classes that hold data
 
 ```python
 class Position(pygame_ecs.BaseComponent):
     def __init__(self, x: int, y: int):
```

### Comparing `pygame_ecs-0.2.8/pyproject.toml` & `pygame_ecs-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "pygame_ecs"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Notenlish", email="71970100+Notenlish@users.noreply.github.com" },
 ]
 description = "Pure Python, simple to use Entity Component System(ECS) for pygame"
 packages=["pygame_ecs", "pygame_ecs.components", "pygame_ecs.managers", "pygame_ecs.systems"]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pygame_ecs-0.2.8/PKG-INFO` & `pygame_ecs-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_ecs
-Version: 0.2.8
+Version: 0.2.9
 Summary: Pure Python, simple to use Entity Component System(ECS) for pygame
 Project-URL: Homepage, https://github.com/Notenlish/pygame_ecs
 Project-URL: Bug Tracker, https://github.com/Notenlish/pygame_ecs/issues
 Author-email: Notenlish <71970100+Notenlish@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ECS,component,ecs,entity,entity component system,pygame,pygame-ce,pygame_ecs,system
@@ -34,15 +34,15 @@
 
 ```python
 entity = entity_manager.add_entity()
 ```
 
 You can delete an entity like this:
 ```python
-    entity_manager.kill_entity(entity)
+entity_manager.kill_entity(entity)
 ```
 
 Components are just classes that hold data
 
 ```python
 class Position(pygame_ecs.BaseComponent):
     def __init__(self, x: int, y: int):
```

