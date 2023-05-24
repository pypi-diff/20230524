# Comparing `tmp/Shimmy-1.0.0.tar.gz` & `tmp/Shimmy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimmy-1.0.0.tar", last modified: Tue May  2 14:30:37 2023, max compression
+gzip compressed data, was "Shimmy-1.0.1.tar", last modified: Wed May 24 18:26:22 2023, max compression
```

## Comparing `Shimmy-1.0.0.tar` & `Shimmy-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.885100 Shimmy-1.0.0/
--rw-r--r--   0 marktowers   (501) staff       (20)     1650 2023-05-02 14:30:37.883837 Shimmy-1.0.0/PKG-INFO
--rw-r--r--   0 marktowers   (501) staff       (20)     6012 2023-05-02 14:30:15.000000 Shimmy-1.0.0/README.md
-drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.861810 Shimmy-1.0.0/Shimmy.egg-info/
--rw-r--r--   0 marktowers   (501) staff       (20)     1650 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/PKG-INFO
--rw-r--r--   0 marktowers   (501) staff       (20)      903 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/SOURCES.txt
--rw-r--r--   0 marktowers   (501) staff       (20)        1 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/dependency_links.txt
--rw-r--r--   0 marktowers   (501) staff       (20)       72 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/entry_points.txt
--rw-r--r--   0 marktowers   (501) staff       (20)      614 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/requires.txt
--rw-r--r--   0 marktowers   (501) staff       (20)        7 2023-05-02 14:30:37.000000 Shimmy-1.0.0/Shimmy.egg-info/top_level.txt
--rw-r--r--   0 marktowers   (501) staff       (20)      535 2023-02-01 20:35:48.000000 Shimmy-1.0.0/pyproject.toml
--rw-r--r--   0 marktowers   (501) staff       (20)       38 2023-05-02 14:30:37.885245 Shimmy-1.0.0/setup.cfg
--rw-r--r--   0 marktowers   (501) staff       (20)     2894 2023-05-02 14:30:15.000000 Shimmy-1.0.0/setup.py
-drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.871284 Shimmy-1.0.0/shimmy/
--rw-r--r--   0 marktowers   (501) staff       (20)     2763 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/__init__.py
--rw-r--r--   0 marktowers   (501) staff       (20)    16080 2023-02-16 23:15:58.000000 Shimmy-1.0.0/shimmy/atari_env.py
--rw-r--r--   0 marktowers   (501) staff       (20)     3452 2023-04-07 10:51:23.000000 Shimmy-1.0.0/shimmy/bsuite_compatibility.py
--rw-r--r--   0 marktowers   (501) staff       (20)     9609 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/dm_control_compatibility.py
--rw-r--r--   0 marktowers   (501) staff       (20)     9952 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/dm_control_multiagent_compatibility.py
--rw-r--r--   0 marktowers   (501) staff       (20)     6942 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/dm_lab_compatibility.py
--rw-r--r--   0 marktowers   (501) staff       (20)     8553 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/meltingpot_compatibility.py
--rw-r--r--   0 marktowers   (501) staff       (20)    11282 2023-04-07 10:51:23.000000 Shimmy-1.0.0/shimmy/openai_gym_compatibility.py
--rw-r--r--   0 marktowers   (501) staff       (20)    14925 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/openspiel_compatibility.py
--rw-r--r--   0 marktowers   (501) staff       (20)    10209 2023-04-06 21:59:58.000000 Shimmy-1.0.0/shimmy/registration.py
-drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.876132 Shimmy-1.0.0/shimmy/utils/
--rw-r--r--   0 marktowers   (501) staff       (20)       36 2023-02-01 20:35:48.000000 Shimmy-1.0.0/shimmy/utils/__init__.py
--rw-r--r--   0 marktowers   (501) staff       (20)     1764 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/utils/dm_control_multiagent.py
--rw-r--r--   0 marktowers   (501) staff       (20)     3054 2023-04-06 21:59:58.000000 Shimmy-1.0.0/shimmy/utils/dm_env.py
--rw-r--r--   0 marktowers   (501) staff       (20)     4735 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/utils/dm_lab.py
--rw-r--r--   0 marktowers   (501) staff       (20)     5752 2023-02-27 19:48:27.000000 Shimmy-1.0.0/shimmy/utils/envs_configs.py
--rw-r--r--   0 marktowers   (501) staff       (20)     2183 2023-05-02 14:30:15.000000 Shimmy-1.0.0/shimmy/utils/meltingpot.py
-drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-05-02 14:30:37.881784 Shimmy-1.0.0/tests/
--rw-r--r--   0 marktowers   (501) staff       (20)     3729 2023-04-07 10:51:23.000000 Shimmy-1.0.0/tests/test_atari.py
--rw-r--r--   0 marktowers   (501) staff       (20)     8175 2023-04-07 10:51:23.000000 Shimmy-1.0.0/tests/test_bsuite.py
--rw-r--r--   0 marktowers   (501) staff       (20)    11017 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_dm_control.py
--rw-r--r--   0 marktowers   (501) staff       (20)     6288 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_dm_control_multi_agent.py
--rw-r--r--   0 marktowers   (501) staff       (20)     3502 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_dm_lab.py
--rw-r--r--   0 marktowers   (501) staff       (20)     3824 2023-02-17 11:19:14.000000 Shimmy-1.0.0/tests/test_gym.py
--rw-r--r--   0 marktowers   (501) staff       (20)     5241 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_meltingpot.py
--rw-r--r--   0 marktowers   (501) staff       (20)     7075 2023-05-02 14:30:15.000000 Shimmy-1.0.0/tests/test_openspiel.py
--rw-r--r--   0 marktowers   (501) staff       (20)      440 2023-03-27 22:11:25.000000 Shimmy-1.0.0/tests/test_pickling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.394135 Shimmy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-24 18:26:22.394135 Shimmy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-24 18:26:19.000000 Shimmy-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.390135 Shimmy-1.0.1/Shimmy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 18:26:22.000000 Shimmy-1.0.1/Shimmy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-24 18:26:19.000000 Shimmy-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:26:22.394135 Shimmy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-24 18:26:19.000000 Shimmy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.390135 Shimmy-1.0.1/shimmy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/atari_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/bsuite_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/dm_control_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/dm_control_multiagent_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/dm_lab_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/meltingpot_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/openai_gym_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/openspiel_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.390135 Shimmy-1.0.1/shimmy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/dm_control_multiagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/dm_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/envs_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-24 18:26:19.000000 Shimmy-1.0.1/shimmy/utils/meltingpot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:26:22.394135 Shimmy-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_atari.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_bsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_dm_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_dm_control_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_meltingpot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-24 18:26:19.000000 Shimmy-1.0.1/tests/test_openspiel.py
```

### Comparing `Shimmy-1.0.0/PKG-INFO` & `Shimmy-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimmy
-Version: 1.0.0
+Version: 1.0.1
 Summary: An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.
 Home-page: https://github.com/Farama-Foundation/Shimmy
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Shimmy-1.0.0/README.md` & `Shimmy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/Shimmy.egg-info/PKG-INFO` & `Shimmy-1.0.1/Shimmy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimmy
-Version: 1.0.0
+Version: 1.0.1
 Summary: An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.
 Home-page: https://github.com/Farama-Foundation/Shimmy
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Shimmy-1.0.0/Shimmy.egg-info/SOURCES.txt` & `Shimmy-1.0.1/Shimmy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,9 +26,8 @@
 tests/test_atari.py
 tests/test_bsuite.py
 tests/test_dm_control.py
 tests/test_dm_control_multi_agent.py
 tests/test_dm_lab.py
 tests/test_gym.py
 tests/test_meltingpot.py
-tests/test_openspiel.py
-tests/test_pickling.py
+tests/test_openspiel.py
```

### Comparing `Shimmy-1.0.0/pyproject.toml` & `Shimmy-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/setup.py` & `Shimmy-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,31 +29,33 @@
     raise RuntimeError("bad version data in __init__.py")
 
 
 version = get_version()
 header_count, long_description = get_description()
 
 extras = {
-    "gym-v21": ["gym>=0.21.0", "pyglet==1.5.11"],
+    "gym-v21": ["gym>=0.21.0,<0.26", "pyglet==1.5.11"],
     "gym-v26": ["gym>=0.26.2"],
     "atari": ["ale-py~=0.8.1"],
     # "imageio" should be "gymnasium[mujoco]>=0.26" but there are install conflicts
     "dm-control": ["dm-control>=1.0.10", "imageio", "h5py>=3.7.0"],
     "dm-control-multi-agent": [
         "dm-control>=1.0.10",
         "imageio",
         "h5py>=3.7.0",
-        "pettingzoo>=1.22.3",
+        "pettingzoo>=1.23",
     ],
     "dm-lab": ["dm-env>=1.6"],
-    "openspiel": ["open_spiel>=1.2", "pettingzoo>=1.22.3"],
-    "meltingpot": ["pettingzoo>=1.22.3"],
+    "openspiel": ["open_spiel>=1.2", "pettingzoo>=1.23"],
+    "meltingpot": ["pettingzoo>=1.23"],
     "bsuite": ["bsuite>=0.3.5"],
 }
-extras["all"] = list({lib for libs in extras.values() for lib in libs})
+extras["all"] = [
+    lib for key, libs in extras.items() if key != "gym-v21" for lib in libs
+]
 extras["testing"] = [
     "pytest==7.1.3",
     "pillow>=9.3.0",
     "autorom[accept-rom-license]~=0.6.0",
 ]
 
 setup(
```

### Comparing `Shimmy-1.0.0/shimmy/__init__.py` & `Shimmy-1.0.1/shimmy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     "DmLabCompatibilityV0",
     "GymV21CompatibilityV0",
     "GymV26CompatibilityV0",
     "MeltingPotCompatibilityV0",
 ]
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 try:
     import sys
 
     from farama_notifications import notifications
```

### Comparing `Shimmy-1.0.0/shimmy/atari_env.py` & `Shimmy-1.0.1/shimmy/atari_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/shimmy/bsuite_compatibility.py` & `Shimmy-1.0.1/shimmy/bsuite_compatibility.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,37 +31,36 @@
     def __init__(
         self,
         env: Environment,
         render_mode: str | None = None,
     ):
         """Initialises the environment with a render mode along with render information."""
         EzPickle.__init__(self, env, render_mode)
-        self._env = env
+        self._env: Any = env
 
         self.observation_space = dm_spec2gym_space(env.observation_spec())
         self.action_space = dm_spec2gym_space(env.action_spec())
 
         assert render_mode is None, "No render modes available in BSuite."
 
     def reset(
         self, *, seed: int | None = None, options: dict[str, Any] | None = None
     ) -> tuple[ObsType, dict[str, Any]]:
         """Resets the bsuite environment."""
         super().reset(seed=seed)
         if seed is not None:
             self.np_random = np.random.RandomState(seed=seed)
-            self._env._rng = self.np_random  # pyright: ignore[reportGeneralTypeIssues]
+            self._env._rng = self.np_random
             if hasattr(self._env, "raw_env"):
                 self._env.raw_env._rng = self.np_random
 
         timestep = self._env.reset()
-
         obs, reward, terminated, truncated, info = dm_env_step2gym_step(timestep)
 
-        return obs, info  # pyright: ignore[reportGeneralTypeIssues]
+        return obs, info
 
     def step(self, action: int) -> tuple[ObsType, float, bool, bool, dict[str, Any]]:
         """Steps through the bsuite environment."""
         timestep = self._env.step(action)
 
         obs, reward, terminated, truncated, info = dm_env_step2gym_step(timestep)
```

### Comparing `Shimmy-1.0.0/shimmy/dm_control_compatibility.py` & `Shimmy-1.0.1/shimmy/dm_control_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 import math
 from enum import Enum
 from typing import Any, Callable, Optional
 
 import dm_env
 import gymnasium
-import mujoco
 import numpy as np
 from dm_control import composer
 from dm_control.mujoco.engine import Physics as MujocoEnginePhysics
 from dm_control.rl import control
 from gymnasium.core import ObsType
 from gymnasium.envs.mujoco.mujoco_rendering import MujocoRenderer
 from gymnasium.utils import EzPickle
+from mujoco._structs import MjvScene
 
 from shimmy.utils.dm_env import dm_env_step2gym_step, dm_spec2gym_space
 
 
 class EnvType(Enum):
     """The environment type."""
 
@@ -58,15 +58,15 @@
     def __init__(
         self,
         env: composer.Environment | control.Environment | dm_env.Environment,
         render_mode: str | None = None,
         render_height: int = 84,
         render_width: int = 84,
         camera_id: int | str = 0,
-        render_scene_callback: (Callable[[MujocoEnginePhysics, mujoco.MjvScene], None])
+        render_scene_callback: (Callable[[MujocoEnginePhysics, MjvScene], None])
         | None = None,
         render_kwargs: dict[str, Any] | None = None,
     ):
         """Initialises the environment with a render mode along with render information.
 
         Note: this wrapper supports multi-camera rendering via the `render_mode` argument (render_mode = "multi_camera")
 
@@ -85,15 +85,15 @@
                 the scene has been created and before it is rendered. Can be used to add more geoms to the scene.
             render_kwargs (Optional[dict[str, Any]]): Additional keyword arguments for rendering. Note: kwargs are not used
                 for human rendering, which uses simpler Gymnasium MuJoCo rendering.
         """
         EzPickle.__init__(
             self, env, render_mode, render_height, render_width, camera_id
         )
-        self._env = env
+        self._env: Any = env
         self.env_type = self._find_env_type(env)
         self.metadata["render_fps"] = self._env.control_timestep()
 
         self.observation_space = dm_spec2gym_space(env.observation_spec())
         self.action_space = dm_spec2gym_space(env.action_spec())
 
         assert render_mode is None or render_mode in self.metadata["render_modes"]
@@ -117,15 +117,14 @@
     ) -> tuple[ObsType, dict[str, Any]]:
         """Resets the dm-control environment."""
         super().reset(seed=seed)
         if seed is not None:
             self.np_random = np.random.RandomState(seed=seed)
 
         timestep = self._env.reset()
-
         obs, reward, terminated, truncated, info = dm_env_step2gym_step(timestep)
 
         return obs, info
 
     def step(
         self, action: np.ndarray
     ) -> tuple[ObsType, float, bool, bool, dict[str, Any]]:
@@ -224,14 +223,18 @@
             return EnvType.COMPOSER
         elif isinstance(env, control.Environment):
             return EnvType.RL_CONTROL
         else:
             assert isinstance(env, dm_env.Environment)
 
             if hasattr(env, "_env"):
-                return self._find_env_type(env._env)
+                return self._find_env_type(
+                    env._env  # pyright: ignore[reportGeneralTypeIssues]
+                )
             elif hasattr(env, "env"):
-                return self._find_env_type(env.env)
+                return self._find_env_type(
+                    env.env  # pyright: ignore[reportGeneralTypeIssues]
+                )
             else:
                 raise AttributeError(
                     f"Can't know the dm-control environment type, actual type: {type(env)}"
                 )
```

### Comparing `Shimmy-1.0.0/shimmy/dm_control_multiagent_compatibility.py` & `Shimmy-1.0.1/shimmy/dm_control_multiagent_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         self.agent_name_id_mapping = dict(zip(self.possible_agents, range(num_players)))
 
         # the official spaces
         self.obs_spaces = dict(zip(self.possible_agents, all_obs_spaces))
         self.act_spaces = dict(zip(self.possible_agents, all_act_spaces))
 
         if self.render_mode == "human":
+            assert self._env.physics is not None
             self.viewer = MujocoRenderer(
                 self._env.physics.model.ptr, self._env.physics.data.ptr
             )
 
     @functools.lru_cache(maxsize=None)
     def observation_space(self, agent: AgentID) -> gymnasium.spaces.Space:
         """observation_space.
@@ -203,42 +204,43 @@
             return
 
     def close(self):
         """close.
 
         Closes the environment.
         """
+        assert self._env.physics is not None
         self._env.physics.free()
         self._env.close()
 
         if hasattr(self, "viewer"):
             self.viewer.close()
 
     def reset(
         self, seed: int | None = None, options: dict[AgentID, Any] | None = None
-    ) -> ObsDict:
+    ) -> tuple[ObsDict, dict[str, Any]]:
         """reset.
 
         Resets the dm-control environment.
 
         Args:
             seed: the seed to reset the environment with
-            options: the options to reset the environment with
+            options: the options to reset the environment with (unused)
 
         Returns:
             observations
         """
         self.agents = self.possible_agents[:]
         self.num_moves = 0
 
+        self._env._random_state = np.random.RandomState(seed)
         timestep = self._env.reset()
+        observations, _, _, _, info = _unravel_ma_timestep(timestep, self.agents)
 
-        observations, _, _, _, _ = _unravel_ma_timestep(timestep, self.agents)
-
-        return observations
+        return observations, info
 
     def step(
         self, actions: ActionDict
     ) -> tuple[
         ObsDict,
         dict[AgentID, float],
         dict[AgentID, bool],
@@ -256,16 +258,15 @@
             (observations, rewards, terminations, truncations, infos)
         """
         # assert that the actions _must_ have actions for all agents
         assert len(actions) == len(
             self.agents
         ), f"Must have actions for all {len(self.agents)} agents, currently only found {len(actions)}."
 
-        actions = actions.values()
-        timestep = self._env.step(actions)
+        timestep = self._env.step(actions.values())
 
         obs, rewards, terminations, truncations, infos = _unravel_ma_timestep(
             timestep, self.agents
         )
 
         if self.render_mode == "human":
             self.viewer.render(self.render_mode)
```

### Comparing `Shimmy-1.0.0/shimmy/dm_lab_compatibility.py` & `Shimmy-1.0.1/shimmy/dm_lab_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/shimmy/meltingpot_compatibility.py` & `Shimmy-1.0.1/shimmy/meltingpot_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 https://github.com/deepmind/meltingpot/blob/main/examples/pettingzoo/utils.py
 and modified to modern PettingZoo API
 """
 # pyright: reportOptionalSubscript=false
 from __future__ import annotations
 
 import functools
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
+import dm_env
 import gymnasium
 import numpy as np
 import pygame
 from gymnasium.utils.ezpickle import EzPickle
 from pettingzoo.utils.env import ActionDict, AgentID, ObsDict, ParallelEnv
 
 import shimmy.utils.meltingpot as utils
@@ -153,33 +154,36 @@
         """
         return self._env.observation()
 
     def reset(
         self,
         seed: int | None = None,
         options: dict | None = None,
-    ) -> ObsDict:
+    ) -> tuple[ObsDict, dict[str, Any]]:
         """reset.
 
         Resets the environment.
 
         Args:
             seed: the seed to reset the environment with (not used, due to nondeterministic underlying environment)
             options: the options to reset the environment with
 
         Returns:
             observations
         """
-        timestep = self._env.reset()
+        timestep: dm_env.TimeStep = self._env.reset()
         self.agents = self.possible_agents[:]
         self.num_cycles = 0
 
         observations = utils.timestep_to_observations(timestep)
 
-        return observations
+        return observations, {
+            "step-type": timestep.step_type,
+            "discount": timestep.discount,
+        }
 
     def step(
         self, actions: ActionDict
     ) -> tuple[
         ObsDict, dict[str, float], dict[str, bool], dict[str, bool], dict[str, dict]
     ]:
         """step.
@@ -188,16 +192,15 @@
 
         Args:
             actions: actions to step through the environment with
 
         Returns:
             (observations, rewards, terminations, truncations, infos)
         """
-        actions = [actions[agent] for agent in self.agents]
-        timestep = self._env.step(actions)
+        timestep = self._env.step([actions[agent] for agent in self.agents])
         rewards = {
             agent: timestep.reward[index] for index, agent in enumerate(self.agents)
         }
         self.num_cycles += 1
         termination = timestep.last()
         terminations = {agent: termination for agent in self.agents}
         truncation = self.num_cycles >= self.max_cycles
```

### Comparing `Shimmy-1.0.0/shimmy/openai_gym_compatibility.py` & `Shimmy-1.0.1/shimmy/openai_gym_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/shimmy/openspiel_compatibility.py` & `Shimmy-1.0.1/shimmy/openspiel_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Wrapper to convert an OpenSpiel environment into a pettingzoo compatible environment."""
 from __future__ import annotations
 
 import functools
+import string
 from typing import Any, Dict, Optional
 
 import numpy as np
 import pettingzoo as pz
 import pyspiel
 from gymnasium import spaces
 from gymnasium.utils import EzPickle, seeding
@@ -65,14 +66,15 @@
             zip(range(self._env.num_players()), self.possible_agents)
         )
         self.agent_name_id_mapping = dict(
             zip(self.possible_agents, range(self._env.num_players()))
         )
 
         self.game_type = self._env.get_type()
+        self.game_name = self.game_type.short_name
 
         self.render_mode = render_mode
 
     @functools.lru_cache(maxsize=None)
     def observation_space(self, agent: AgentID):
         """observation_space.
 
@@ -101,15 +103,17 @@
                 shape=self._env.information_state_tensor_shape(),
                 dtype=np.float64,
             )
         elif (
             self.game_type.provides_information_state_string
             or self.game_type.provides_observation_string
         ):
-            return spaces.Text(max_length=2**16)
+            return spaces.Text(
+                min_length=0, max_length=2**16, charset=string.printable
+            )
         else:
             raise NotImplementedError(
                 f"No information/observation tensor/string implemented for {self._env}."
             )
 
     @functools.lru_cache(maxsize=None)
     def action_space(self, agent: AgentID):
@@ -138,15 +142,15 @@
         if not hasattr(self, "game_state"):
             raise UserWarning(
                 "You must reset the environment using reset() before calling render()."
             )
 
         print(self.game_state)
 
-    def observe(self, agent: AgentID) -> ObsType:
+    def observe(self, agent: AgentID) -> Any:
         """observe.
 
         Args:
             agent (AgentID): agent
 
         Returns:
             observation
@@ -164,24 +168,29 @@
     ):
         """reset.
 
         Args:
             seed (Optional[int]): seed
             options (Optional[Dict]): options
         """
-        # initialize the seed
-        self.np_random, seed = seeding.np_random(seed)
+        # initialize np random the seed
+        self.np_random, self.np_seed = seeding.np_random(seed)
+
+        # seed argument is only valid for three games
+        if self.game_name in ["deep_sea", "hanabi", "mfg_garnet"] and seed is not None:
+            self.game_name = self.game_type.short_name
+            self._env = pyspiel.load_game(self.game_name, {"seed": seed})
 
         # all agents
         self.agents = self.possible_agents[:]
         self.agent_ids = [self.agent_name_id_mapping[a] for a in self.agents]
 
         # boilerplate stuff
-        self._cumulative_rewards = {a: 0 for a in self.agents}
-        self.rewards = {a: 0 for a in self.agents}
+        self._cumulative_rewards = {a: 0.0 for a in self.agents}
+        self.rewards = {a: 0.0 for a in self.agents}
         self.terminations = {a: False for a in self.agents}
         self.truncations = {a: False for a in self.agents}
         self.infos = {a: {} for a in self.agents}
 
         # get a new game state, game_length = number of game nodes
         self.game_length = 1
         self.game_state = self._env.new_initial_state()
@@ -229,27 +238,28 @@
             action (int): action
         """
         # if the game state is a simultaneous node, we need to collect all actions first
         if self.game_state.is_simultaneous_node():
             # store the agent's action
             self.simultaneous_actions[self.agent_selection] = action
 
-            # set the agents reward to 0 since it's seen it
-            self._cumulative_rewards[self.agent_selection] = 0
-
             if all(a in self.simultaneous_actions for a in self.agents):
                 # if we already have all the actions, just step regularly
                 self.game_state.apply_actions(list(self.simultaneous_actions.values()))
                 self.game_length += 1
 
                 # clear the simultaneous actions holder
                 self.simultaneous_actions = dict()
         else:
             # if not simultaneous, step the state generically
-            self.game_state.apply_action(action)
+            try:
+                self.game_state.apply_action(action)
+            except pyspiel.SpielError:
+                print()
+                self.game_state.apply_action(action)
             self.game_length += 1
 
     def _choose_next_agent(self):
         # handle possibility that we don't have anymore agents
         if not self.agents:
             return
 
@@ -313,32 +323,29 @@
         elif self.game_type.provides_information_state_string:
             self.observations = {
                 self.agents[a]: self.game_state.information_state_string(a)
                 for a in self.agent_ids
             }
         else:
             raise NotImplementedError(
-                f"No information/observation tensor/string implemented for {self.game}."
+                f"No information/observation tensor/string implemented for {self._env}."
             )
 
     def _update_action_masks(self):
         """Updates all the action masks inside the infos dictionary."""
         for agent_id, agent_name in zip(self.agent_ids, self.agents):
             action_mask = np.zeros(self.action_space(agent_name).n, dtype=np.int8)
             action_mask[self.game_state.legal_actions(agent_id)] = 1
 
             self.infos[agent_name] = {"action_mask": action_mask}
 
     def _update_rewards(self):
         """Updates all the _cumulative_rewards of the environment."""
-        # update cumulative rewards
-        rewards = self.game_state.rewards()
-        self._cumulative_rewards = {
-            self.agent_id_name_mapping[id]: rewards[id] for id in self.agent_ids
-        }
+        # retrieve rewards
+        self.rewards = {a: r for a, r in zip(self.agents, self.game_state.rewards())}
 
     def _update_termination_truncation(self):
         """Updates all terminations and truncations of the environment."""
         # check for terminal
         self.terminations = {a: self.terminations[a] for a in self.agents}
         if self.game_state.current_player() <= -4:
             self.terminations = {a: True for a in self.agents}
@@ -382,18 +389,25 @@
         """Steps.
 
         Steps the agent with an action.
 
         Args:
             action (int): action
         """
+        # reset the cumulative rewards for the current agent
+        self._cumulative_rewards[self.agent_selection] = 0.0
+
         # handle the possibility of an end step
         if not self._end_routine():
             # step the environment
             self._execute_action_node(action)
             self._execute_chance_node()
             self._update_action_masks()
             self._update_observations()
             self._update_rewards()
             self._update_termination_truncation()
 
+        # pick the next agent
         self._choose_next_agent()
+
+        # accumulate the rewards
+        self._accumulate_rewards()
```

### Comparing `Shimmy-1.0.0/shimmy/registration.py` & `Shimmy-1.0.1/shimmy/registration.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/shimmy/utils/dm_control_multiagent.py` & `Shimmy-1.0.1/shimmy/utils/dm_control_multiagent.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,19 @@
         terminate_on_goal (Optional[bool]): flag to terminate the environment on goal
         walker_type (Optional[dm_soccer.WalkerType]): specify walker type (BOXHEAD, ANT, or HUMANOID)
 
     Returns:
         env (dm_control.composer.Environment): dm control soccer environment
     """
     env = dm_soccer.load(
-        team_size if team_size is not None else 2,
-        time_limit if time_limit is not None else 10.0,
-        disable_walker_contacts if disable_walker_contacts is not None else False,
-        enable_field_box if enable_field_box is not None else True,
-        terminate_on_goal if terminate_on_goal is not None else False,
-        walker_type if walker_type is not None else dm_soccer.WalkerType.BOXHEAD,
+        team_size=team_size if team_size is not None else 2,
+        time_limit=time_limit if time_limit is not None else 10.0,
+        disable_walker_contacts=disable_walker_contacts
+        if disable_walker_contacts is not None
+        else False,
+        enable_field_box=enable_field_box if enable_field_box is not None else True,
+        terminate_on_goal=terminate_on_goal if terminate_on_goal is not None else False,
+        walker_type=walker_type
+        if walker_type is not None
+        else dm_soccer.WalkerType.BOXHEAD,
     )
     return env
```

### Comparing `Shimmy-1.0.0/shimmy/utils/dm_env.py` & `Shimmy-1.0.1/shimmy/utils/dm_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,29 +17,39 @@
         return spaces.Dict(
             {key: dm_spec2gym_space(value) for key, value in copy.copy(spec).items()}
         )
     # not possible to use isinstance due to inheritance
     elif type(spec) is BoundedArray:
         low = np.broadcast_to(spec.minimum, spec.shape)
         high = np.broadcast_to(spec.maximum, spec.shape)
-        return spaces.Box(low=low, high=high, shape=spec.shape, dtype=spec.dtype)
+        return spaces.Box(
+            low=low,
+            high=high,
+            shape=spec.shape,
+            dtype=spec.dtype,  # pyright: ignore[reportGeneralTypeIssues]
+        )
     elif type(spec) is Array:
         if np.issubdtype(spec.dtype, np.integer):
             low = np.iinfo(spec.dtype).min
             high = np.iinfo(spec.dtype).max
         elif np.issubdtype(spec.dtype, np.inexact):
             low = float("-inf")
             high = float("inf")
         elif spec.dtype == "bool":
             low = int(0)
             high = int(1)
         else:
             raise TypeError(f"Unknown dtype {spec.dtype} for spec {spec}.")
 
-        return spaces.Box(low=low, high=high, shape=spec.shape, dtype=spec.dtype)
+        return spaces.Box(
+            low=low,
+            high=high,
+            shape=spec.shape,
+            dtype=spec.dtype,  # pyright: ignore[reportGeneralTypeIssues]
+        )
     elif type(spec) is DiscreteArray:
         return spaces.Discrete(spec.num_values)
     else:
         raise NotImplementedError(
             f"Cannot convert dm_spec to gymnasium space, unknown spec: {spec}, please report."
         )
```

### Comparing `Shimmy-1.0.0/shimmy/utils/dm_lab.py` & `Shimmy-1.0.1/shimmy/utils/dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/shimmy/utils/envs_configs.py` & `Shimmy-1.0.1/shimmy/utils/envs_configs.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/shimmy/utils/meltingpot.py` & `Shimmy-1.0.1/shimmy/utils/meltingpot.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/tests/test_atari.py` & `Shimmy-1.0.1/tests/test_atari.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/tests/test_bsuite.py` & `Shimmy-1.0.1/tests/test_bsuite.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/tests/test_dm_control.py` & `Shimmy-1.0.1/tests/test_dm_control.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/tests/test_dm_control_multi_agent.py` & `Shimmy-1.0.1/tests/test_dm_control_multi_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,25 +115,27 @@
 
     env1.reset(seed=42)
     env2.reset(seed=42)
 
     for agent in env1.possible_agents:
         env1.action_space(agent).seed(42)
         env2.action_space(agent).seed(42)
+        env1.observation_space(agent).seed(42)
+        env2.observation_space(agent).seed(42)
 
     while env1.agents:
         actions1 = {agent: env1.action_space(agent).sample() for agent in env1.agents}
         actions2 = {agent: env2.action_space(agent).sample() for agent in env2.agents}
 
         assert data_equivalence(actions1, actions2), "Incorrect action seeding"
 
         obs1, rewards1, terminations1, truncations1, infos1 = env1.step(actions1)
         obs2, rewards2, terminations2, truncations2, infos2 = env2.step(actions2)
 
-        assert data_equivalence(obs1, obs2)
+        assert data_equivalence(obs1, obs2), "Incorrect observations"
         assert data_equivalence(rewards1, rewards2), "Incorrect values for rewards"
         assert data_equivalence(terminations1, terminations2), "Incorrect terminations."
         assert data_equivalence(truncations1, truncations2), "Incorrect truncations"
         assert data_equivalence(infos1, infos2), "Incorrect infos"
     env1.close()
     env2.close()
```

### Comparing `Shimmy-1.0.0/tests/test_dm_lab.py` & `Shimmy-1.0.1/tests/test_dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/tests/test_gym.py` & `Shimmy-1.0.1/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/tests/test_meltingpot.py` & `Shimmy-1.0.1/tests/test_meltingpot.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.0.0/tests/test_openspiel.py` & `Shimmy-1.0.1/tests/test_openspiel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """Tests the functionality of the OpenSpielCompatibility wrapper on OpenSpiel envs."""
+# pyright: reportGeneralTypeIssues=false
 import pickle
 
-import numpy as np
 import pyspiel
 import pytest
 from gymnasium.utils.env_checker import data_equivalence
+from pettingzoo.test import api_test
 
 from shimmy.openspiel_compatibility import OpenSpielCompatibilityV0
 
-# todo add api_test however chess causes a OOM error
-# from pettingzoo.test import api_test
-
-
 _PASSING_GAMES = [
     "2048",
     "amazons",
-    "backgammon",
     "bargaining",
     "battleship",
     "blackjack",
     "blotto",
     "breakthrough",
     "bridge",
     "bridge_uncontested_bidding",
@@ -82,28 +78,32 @@
     "phantom_ttt",
     "phantom_ttt_ir",
     "pig",
     "quoridor",
     "rbc",
     "sheriff",
     "skat",
-    "solitaire",
     "stones_and_gems",
     "tarok",
     "tic_tac_toe",
     "tiny_bridge_2p",
     "tiny_bridge_4p",
     "tiny_hanabi",
     "trade_comm",
     "ultimate_tic_tac_toe",
     "universal_poker",
     "y",
     "mfg_dynamic_routing",
 ]
 
+_SOMETIMES_FAILING_GAMES = [
+    "backgammon",
+    "solitaire",
+]
+
 _FAILING_GAMES = [
     "efg_game",
     "misere",
     "normal_form_extensive_game",
     "repeated_game",
     "restricted_nash_response",
     "start_at",
@@ -117,15 +117,16 @@
 def test_passing_games(game_name):
     """Tests the conversion of all OpenSpiel environments using the OpenSpielCompatibility wrapper."""
     for _ in range(5):
         env = pyspiel.load_game(game_name)
         env = OpenSpielCompatibilityV0(env=env, render_mode=None)
 
         # api test the env (disabled because some environments fail the test)
-        # api_test(env)
+        # TODO: fix this (fails play_test, not sure what the cause is)
+        api_test(env)
 
         env.reset()
         for agent in env.agent_iter():
             observation, reward, termination, truncation, info = env.last()
             action = env.action_space(agent).sample(mask=info["action_mask"])
             env.step(action)
 
@@ -139,15 +140,15 @@
 
 @pytest.mark.parametrize("game_name", _PASSING_GAMES)
 def test_loading_env(game_name):
     """Tests the loading of all OpenSpiel environments using the OpenSpielCompatibility wrapper."""
     env = OpenSpielCompatibilityV0(game_name=game_name, render_mode=None)
 
     # api test the env
-    # api_test(env)
+    api_test(env)
 
     # run through the environment
     env.reset()
     for agent in env.agent_iter():
         observation, reward, termination, truncation, info = env.last()
         action = env.action_space(agent).sample(mask=info["action_mask"])
         env.step(action)
```

