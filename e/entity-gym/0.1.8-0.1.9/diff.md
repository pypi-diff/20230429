# Comparing `tmp/entity_gym-0.1.8.tar.gz` & `tmp/entity_gym-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity_gym-0.1.8.tar", max compression
+gzip compressed data, was "entity_gym-0.1.9.tar", max compression
```

## Comparing `entity_gym-0.1.8.tar` & `entity_gym-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0     9693 2022-11-07 16:05:43.056602 entity_gym-0.1.8/LICENSE-APACHE
--rw-r--r--   0        0        0     1088 2022-11-07 16:05:43.056602 entity_gym-0.1.8/LICENSE-MIT
--rw-r--r--   0        0        0     1974 2022-11-07 16:05:43.056602 entity_gym-0.1.8/README.md
--rw-r--r--   0        0        0      126 2022-11-07 16:05:43.056602 entity_gym-0.1.8/entity_gym/__init__.py
--rw-r--r--   0        0        0     1019 2022-11-07 16:05:43.056602 entity_gym-0.1.8/entity_gym/dataclass_utils.py
--rw-r--r--   0        0        0     2557 2022-11-07 16:05:43.056602 entity_gym-0.1.8/entity_gym/env/__init__.py
--rw-r--r--   0        0        0     5967 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/env/action.py
--rw-r--r--   0        0        0     3787 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/env/add_metrics_wrapper.py
--rw-r--r--   0        0        0      206 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/env/common.py
--rw-r--r--   0        0        0     5331 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/env/env_list.py
--rw-r--r--   0        0        0    10611 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/env/environment.py
--rw-r--r--   0        0        0     7009 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/env/parallel_env_list.py
--rw-r--r--   0        0        0     7345 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/env/validator.py
--rw-r--r--   0        0        0    16710 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/env/vec_env.py
--rw-r--r--   0        0        0     1530 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/__init__.py
--rw-r--r--   0        0        0     2907 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/cherry_pick.py
--rw-r--r--   0        0        0     3243 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/count.py
--rw-r--r--   0        0        0     3384 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/floor_is_lava.py
--rw-r--r--   0        0        0     5314 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/minefield.py
--rw-r--r--   0        0        0     5663 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/minesweeper.py
--rw-r--r--   0        0        0     4501 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/move_to_origin.py
--rw-r--r--   0        0        0     1590 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/multi_armed_bandit.py
--rw-r--r--   0        0        0     7745 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/multi_snake.py
--rw-r--r--   0        0        0     2840 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/not_hotdog.py
--rw-r--r--   0        0        0     4004 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/pick_matching_balls.py
--rw-r--r--   0        0        0     3380 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/rock_paper_scissors.py
--rw-r--r--   0        0        0     2770 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/tutorial.py
--rw-r--r--   0        0        0     2281 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/examples/xor.py
--rw-r--r--   0        0        0      555 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/main.py
--rw-r--r--   0        0        0        0 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/py.typed
--rw-r--r--   0        0        0     1586 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/ragged_dict.py
--rw-r--r--   0        0        0    13185 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/runner.py
--rw-r--r--   0        0        0      124 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/serialization/__init__.py
--rw-r--r--   0        0        0     3041 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/serialization/msgpack_ragged.py
--rw-r--r--   0        0        0     7578 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/serialization/sample_loader.py
--rw-r--r--   0        0        0     6249 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/serialization/sample_recorder.py
--rw-r--r--   0        0        0     1921 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/simple_trace.py
--rw-r--r--   0        0        0    24369 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/tests/test_environment.py
--rw-r--r--   0        0        0     4051 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/tests/test_sample_recorder.py
--rw-r--r--   0        0        0      733 2022-11-07 16:05:43.060601 entity_gym-0.1.8/entity_gym/tests/test_validator.py
--rw-r--r--   0        0        0      785 2022-11-07 16:05:43.060601 entity_gym-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 entity_gym-0.1.8/setup.py
--rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 entity_gym-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     9693 2023-03-08 05:22:11.905764 entity_gym-0.1.9/LICENSE-APACHE
+-rw-r--r--   0        0        0     1088 2023-03-08 05:22:11.905764 entity_gym-0.1.9/LICENSE-MIT
+-rw-r--r--   0        0        0     1974 2023-03-08 05:22:11.905764 entity_gym-0.1.9/README.md
+-rw-r--r--   0        0        0      126 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/__init__.py
+-rw-r--r--   0        0        0     1019 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/dataclass_utils.py
+-rw-r--r--   0        0        0     2557 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/env/__init__.py
+-rw-r--r--   0        0        0     5967 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/env/action.py
+-rw-r--r--   0        0        0     3787 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/env/add_metrics_wrapper.py
+-rw-r--r--   0        0        0      206 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/env/common.py
+-rw-r--r--   0        0        0     5331 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/env/env_list.py
+-rw-r--r--   0        0        0    10611 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/env/environment.py
+-rw-r--r--   0        0        0     7009 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/env/parallel_env_list.py
+-rw-r--r--   0        0        0     7345 2023-03-08 05:22:11.905764 entity_gym-0.1.9/entity_gym/env/validator.py
+-rw-r--r--   0        0        0    16710 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/env/vec_env.py
+-rw-r--r--   0        0        0     1530 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/__init__.py
+-rw-r--r--   0        0        0     2907 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/cherry_pick.py
+-rw-r--r--   0        0        0     3243 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/count.py
+-rw-r--r--   0        0        0     3384 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/floor_is_lava.py
+-rw-r--r--   0        0        0     5314 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/minefield.py
+-rw-r--r--   0        0        0     5663 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/minesweeper.py
+-rw-r--r--   0        0        0     4501 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/move_to_origin.py
+-rw-r--r--   0        0        0     1590 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/multi_armed_bandit.py
+-rw-r--r--   0        0        0     7377 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/multi_snake.py
+-rw-r--r--   0        0        0     2840 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/not_hotdog.py
+-rw-r--r--   0        0        0     4004 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/pick_matching_balls.py
+-rw-r--r--   0        0        0     3380 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/rock_paper_scissors.py
+-rw-r--r--   0        0        0     2770 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/tutorial.py
+-rw-r--r--   0        0        0     2281 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/examples/xor.py
+-rw-r--r--   0        0        0      555 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/main.py
+-rw-r--r--   0        0        0        0 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/py.typed
+-rw-r--r--   0        0        0     1586 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/ragged_dict.py
+-rw-r--r--   0        0        0    14018 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/runner.py
+-rw-r--r--   0        0        0      124 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/serialization/__init__.py
+-rw-r--r--   0        0        0     3041 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/serialization/msgpack_ragged.py
+-rw-r--r--   0        0        0     7578 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/serialization/sample_loader.py
+-rw-r--r--   0        0        0     6249 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/serialization/sample_recorder.py
+-rw-r--r--   0        0        0     1921 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/simple_trace.py
+-rw-r--r--   0        0        0    24369 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/tests/test_environment.py
+-rw-r--r--   0        0        0     4051 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/tests/test_sample_recorder.py
+-rw-r--r--   0        0        0      733 2023-03-08 05:22:11.909764 entity_gym-0.1.9/entity_gym/tests/test_validator.py
+-rw-r--r--   0        0        0      785 2023-03-08 05:22:11.909764 entity_gym-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 entity_gym-0.1.9/PKG-INFO
```

### Comparing `entity_gym-0.1.8/LICENSE-APACHE` & `entity_gym-0.1.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/LICENSE-MIT` & `entity_gym-0.1.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/README.md` & `entity_gym-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/dataclass_utils.py` & `entity_gym-0.1.9/entity_gym/dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/env/__init__.py` & `entity_gym-0.1.9/entity_gym/env/__init__.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/env/action.py` & `entity_gym-0.1.9/entity_gym/env/action.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/env/add_metrics_wrapper.py` & `entity_gym-0.1.9/entity_gym/env/add_metrics_wrapper.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/env/env_list.py` & `entity_gym-0.1.9/entity_gym/env/env_list.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/env/environment.py` & `entity_gym-0.1.9/entity_gym/env/environment.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/env/parallel_env_list.py` & `entity_gym-0.1.9/entity_gym/env/parallel_env_list.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/env/validator.py` & `entity_gym-0.1.9/entity_gym/env/validator.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/env/vec_env.py` & `entity_gym-0.1.9/entity_gym/env/vec_env.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/__init__.py` & `entity_gym-0.1.9/entity_gym/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/cherry_pick.py` & `entity_gym-0.1.9/entity_gym/examples/cherry_pick.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/count.py` & `entity_gym-0.1.9/entity_gym/examples/count.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/floor_is_lava.py` & `entity_gym-0.1.9/entity_gym/examples/floor_is_lava.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/minefield.py` & `entity_gym-0.1.9/entity_gym/examples/minefield.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/minesweeper.py` & `entity_gym-0.1.9/entity_gym/examples/minesweeper.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/move_to_origin.py` & `entity_gym-0.1.9/entity_gym/examples/move_to_origin.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/multi_armed_bandit.py` & `entity_gym-0.1.9/entity_gym/examples/multi_armed_bandit.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/multi_snake.py` & `entity_gym-0.1.9/entity_gym/examples/multi_snake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import random
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Dict, List, Mapping, Tuple
 
-import numpy as np
-
 from entity_gym.env import (
     Action,
     ActionSpace,
     CategoricalAction,
     CategoricalActionMask,
     CategoricalActionSpace,
     Entity,
@@ -176,44 +174,35 @@
 
         def cycle_color(color: int) -> int:
             return (color - color_offset) % self.num_snakes
 
         return Observation(
             global_features=[self.step],
             features={
-                "SnakeHead": np.array(
-                    [
-                        [
-                            s.segments[-1][0],
-                            s.segments[-1][1],
-                            cycle_color(s.color),
-                        ]
-                        for s in self.snakes
-                    ],
-                    dtype=np.float32,
-                ),
-                "SnakeBody": np.array(
-                    [
-                        [sx, sy, cycle_color(snake.color)]
-                        for snake in self.snakes
-                        for sx, sy in snake.segments[:-1]
-                    ],
-                    dtype=np.float32,
-                ).reshape(-1, 3),
-                "Food": np.array(
-                    [
-                        [
-                            f.position[0],
-                            f.position[1],
-                            cycle_color(f.color),
-                        ]
-                        for f in self.food
-                    ],
-                    dtype=np.float32,
-                ),
+                "SnakeHead": [
+                    (
+                        s.segments[-1][0],
+                        s.segments[-1][1],
+                        cycle_color(s.color),
+                    )
+                    for s in self.snakes
+                ],
+                "SnakeBody": [
+                    (sx, sy, cycle_color(snake.color))
+                    for snake in self.snakes
+                    for sx, sy in snake.segments[:-1]
+                ],
+                "Food": [
+                    (
+                        f.position[0],
+                        f.position[1],
+                        cycle_color(f.color),
+                    )
+                    for f in self.food
+                ],
             },
             ids={
                 "SnakeHead": list(range(self.num_snakes)),
             },
             actions={
                 "move": CategoricalActionMask(
                     actor_types=["SnakeHead"],
```

### Comparing `entity_gym-0.1.8/entity_gym/examples/not_hotdog.py` & `entity_gym-0.1.9/entity_gym/examples/not_hotdog.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/pick_matching_balls.py` & `entity_gym-0.1.9/entity_gym/examples/pick_matching_balls.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/rock_paper_scissors.py` & `entity_gym-0.1.9/entity_gym/examples/rock_paper_scissors.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/tutorial.py` & `entity_gym-0.1.9/entity_gym/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/examples/xor.py` & `entity_gym-0.1.9/entity_gym/examples/xor.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/main.py` & `entity_gym-0.1.9/entity_gym/main.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/ragged_dict.py` & `entity_gym-0.1.9/entity_gym/ragged_dict.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/runner.py` & `entity_gym-0.1.9/entity_gym/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,25 +101,40 @@
                         )
 
                     click.echo(
                         f"Choose "
                         + click.style(f"{action_name}", fg="green")
                         + f" ({choices})"
                     )
-                    try:
-                        inp = input()
-                        if inp == "" and agent_action is not None:
-                            choice_id = agent_action[action_name].index  # type: ignore
-                        else:
-                            choice_id = int(inp)
-                        received_action = True
-                    except KeyboardInterrupt:
-                        print()
-                        print("Exiting")
-                        return
+                    while True:
+                        try:
+                            inp = input()
+                            if inp == "" and agent_action is not None:
+                                choice_id = agent_action[action_name].index  # type: ignore
+                            else:
+                                try:
+                                    choice_id = int(inp)
+                                except ValueError:
+                                    print(
+                                        f"Invalid choice '{inp}' (must be an integer)"
+                                    )
+                                    continue
+                                if choice_id < 0 or choice_id >= len(
+                                    action_def.index_to_label
+                                ):
+                                    print(
+                                        f"Invalid choice {inp} (must be in range [0, {len(action_def.index_to_label) - 1}])"
+                                    )
+                                    continue
+                            received_action = True
+                            break
+                        except KeyboardInterrupt:
+                            print()
+                            print("Exiting")
+                            return
                     action[action_name] = GlobalCategoricalAction(
                         index=choice_id,
                         label=action_def.index_to_label[choice_id],
                     )
                     continue
                 elif action_mask.actor_ids is not None:
                     actor_ids = action_mask.actor_ids
```

### Comparing `entity_gym-0.1.8/entity_gym/serialization/msgpack_ragged.py` & `entity_gym-0.1.9/entity_gym/serialization/msgpack_ragged.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/serialization/sample_loader.py` & `entity_gym-0.1.9/entity_gym/serialization/sample_loader.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/serialization/sample_recorder.py` & `entity_gym-0.1.9/entity_gym/serialization/sample_recorder.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/simple_trace.py` & `entity_gym-0.1.9/entity_gym/simple_trace.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/tests/test_environment.py` & `entity_gym-0.1.9/entity_gym/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/tests/test_sample_recorder.py` & `entity_gym-0.1.9/entity_gym/tests/test_sample_recorder.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/entity_gym/tests/test_validator.py` & `entity_gym-0.1.9/entity_gym/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `entity_gym-0.1.8/pyproject.toml` & `entity_gym-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entity-gym"
-version = "0.1.8"
+version = "0.1.9"
 description = "Entity Gym"
 authors = ["Clemens Winter <clemenswinter1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `entity_gym-0.1.8/PKG-INFO` & `entity_gym-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entity-gym
-Version: 0.1.8
+Version: 0.1.9
 Summary: Entity Gym
 License: MIT
 Author: Clemens Winter
 Author-email: clemenswinter1@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
```

