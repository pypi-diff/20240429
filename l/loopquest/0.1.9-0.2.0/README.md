# Comparing `tmp/loopquest-0.1.9.tar.gz` & `tmp/loopquest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopquest-0.1.9.tar", last modified: Mon Oct  2 21:00:29 2023, max compression
+gzip compressed data, was "loopquest-0.2.0.tar", last modified: Mon Apr 29 07:03:08 2024, max compression
```

## Comparing `loopquest-0.1.9.tar` & `loopquest-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 jinyu     (1000) jinyu     (1000)        0 2023-10-02 21:00:29.908970 loopquest-0.1.9/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)    11357 2023-08-14 22:24:33.000000 loopquest-0.1.9/LICENSE
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     4075 2023-10-02 21:00:29.908970 loopquest-0.1.9/PKG-INFO
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     3671 2023-09-27 05:57:39.000000 loopquest-0.1.9/README.md
-drwxr-xr-x   0 jinyu     (1000) jinyu     (1000)        0 2023-10-02 21:00:29.908970 loopquest-0.1.9/loopquest/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)       64 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/__init__.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     3257 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/api.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     4638 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/crud.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     1640 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/datasets.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6286 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/gym_wrappers.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     3009 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/private_api.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     4548 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/schema.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)      376 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/ui.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     3619 2023-09-27 05:57:39.000000 loopquest-0.1.9/loopquest/utils.py
-drwxr-xr-x   0 jinyu     (1000) jinyu     (1000)        0 2023-10-02 21:00:29.908970 loopquest-0.1.9/loopquest.egg-info/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     4075 2023-10-02 21:00:29.000000 loopquest-0.1.9/loopquest.egg-info/PKG-INFO
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)      447 2023-10-02 21:00:29.000000 loopquest-0.1.9/loopquest.egg-info/SOURCES.txt
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)        1 2023-10-02 21:00:29.000000 loopquest-0.1.9/loopquest.egg-info/dependency_links.txt
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     1129 2023-10-02 21:00:29.000000 loopquest-0.1.9/loopquest.egg-info/requires.txt
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)       10 2023-10-02 21:00:29.000000 loopquest-0.1.9/loopquest.egg-info/top_level.txt
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)       38 2023-10-02 21:00:29.908970 loopquest-0.1.9/setup.cfg
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)      946 2023-10-02 19:10:20.000000 loopquest-0.1.9/setup.py
-drwxr-xr-x   0 jinyu     (1000) jinyu     (1000)        0 2023-10-02 21:00:29.908970 loopquest-0.1.9/tests/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     1451 2023-09-27 05:57:39.000000 loopquest-0.1.9/tests/test_datasets.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     4677 2023-09-27 05:57:39.000000 loopquest-0.1.9/tests/test_performance.py
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)      832 2023-09-27 05:57:39.000000 loopquest-0.1.9/tests/test_wrappers.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-04-29 07:03:08.142345 loopquest-0.2.0/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.0/LICENSE
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     5944 2024-04-29 07:03:08.142345 loopquest-0.2.0/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     3360 2024-04-19 04:42:45.000000 loopquest-0.2.0/README.md
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-04-29 07:03:08.142345 loopquest-0.2.0/loopquest/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.0/loopquest/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1439 2024-04-24 05:33:47.000000 loopquest-0.2.0/loopquest/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9075 2024-04-28 15:10:40.000000 loopquest-0.2.0/loopquest/crud.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.0/loopquest/datasets.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5145 2024-04-29 04:54:43.000000 loopquest-0.2.0/loopquest/eval.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1994 2024-04-24 04:19:39.000000 loopquest-0.2.0/loopquest/private_api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5685 2024-04-28 05:00:52.000000 loopquest-0.2.0/loopquest/schema.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.0/loopquest/typing.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.0/loopquest/ui.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4216 2024-04-19 04:43:26.000000 loopquest-0.2.0/loopquest/utils.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-04-29 07:03:08.142345 loopquest-0.2.0/loopquest.egg-info/
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     5944 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      459 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1175 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/requires.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-04-29 07:03:08.000000 loopquest-0.2.0/loopquest.egg-info/top_level.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-04-29 07:03:08.142345 loopquest-0.2.0/setup.cfg
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      946 2024-04-29 07:01:19.000000 loopquest-0.2.0/setup.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-04-29 07:03:08.142345 loopquest-0.2.0/tests/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1397 2024-04-19 04:43:26.000000 loopquest-0.2.0/tests/test_datasets.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4677 2024-04-19 04:42:45.000000 loopquest-0.2.0/tests/test_performance.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      832 2024-04-19 04:42:45.000000 loopquest-0.2.0/tests/test_wrappers.py
```

### Comparing `loopquest-0.1.9/LICENSE` & `loopquest-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loopquest-0.1.9/PKG-INFO` & `loopquest-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,13 @@
-Metadata-Version: 2.1
-Name: loopquest
-Version: 0.1.9
-Summary: A Production Tool for Embodied AI.
-Home-page: https://github.com/LoopMind-AI/loopquest
-Author: LoopMind
-Author-email: contactus@loopmind.ai
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # :scroll:Loopquest
 
-[![Downloads](https://static.pepy.tech/badge/loopquest)](https://pepy.tech/project/loopquest)
-[![Downloads](https://static.pepy.tech/badge/loopquest/month)](https://pepy.tech/project/loopquest)
-[![Downloads](https://static.pepy.tech/badge/loopquest/week)](https://pepy.tech/project/loopquest)
-
 A Production Tool for Embodied AI.
-![loopquest frontend](screenshots/loopquest-screenshot.png)
+![loopquest demo](screenshots/open_loopquest_demo.gif)
 
-- :video_camera:[Tutorial Video - Updated 9/4/2023](https://capture.dropbox.com/UXKQxGkwel6VRZJQ), [Dataset Demo](https://capture.dropbox.com/AOF5rGxHWyRb9T58)
+- :video_camera:[Quickstart Demo](https://capture.dropbox.com/embed/CpS8Y4g21ClHlief), [Dataset Demo](https://capture.dropbox.com/AOF5rGxHWyRb9T58)
 - :house:[Discord](https://discord.gg/FTnFYeSy9r)
 
 # Major features
 
 - Imitation Learning / Offline Reinforcement Learning Oriented MLOps. Log all the observation, action, reward, rendered images into database with only ONE extra line of code.
 
 ```python
```

### Comparing `loopquest-0.1.9/loopquest/datasets.py` & `loopquest-0.2.0/loopquest/datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from datasets import Dataset
 from .crud import get_steps_by_experiment, get_image_by_url
 from .api import get_backend_url
+from .env.space_utils import recover_from_space_val
 from PIL import Image
 
 
 def dataset_gen(experiment_ids: list[str]):
     for experiment_id in experiment_ids:
         # TODO: this can be further optimized by fetching a batch of steps at a
         # time. Maybe this is already considered by huggingface datasets?
         steps = get_steps_by_experiment(get_backend_url(), experiment_id)
         for step in steps:
-            yield step
+            step_dict = step.model_dump()
+            step_dict["observation"] = recover_from_space_val(step.observation)
+            if step.action is not None:
+                step_dict["action"] = recover_from_space_val(step.action)
+            yield step_dict
 
 
 def to_pilow(examples):
     image_urls_across_examples = examples["image_urls"]
     images = [
         [get_image_by_url(url) for url in image_urls]
         for image_urls in image_urls_across_examples
```

### Comparing `loopquest-0.1.9/loopquest/private_api.py` & `loopquest-0.2.0/loopquest/private_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,31 @@
 import time
 import requests
 import os
-from .utils import update_or_append_env_var
-
-LOCAL_FRONTEND_URL = "http://localhost:5667"
-LOCAL_BACKEND_URL = "http://localhost:8000"
-CLOUD_FRONTEND_URL = "https://open.loopquest.ai"
-CLOUD_BACKEND_URL = "https://open.loopquest.ai/api"
-# For local development
-# CLOUD_FRONTEND_URL = "http://localhost:3000"
-# CLOUD_BACKEND_URL = "http://localhost:3000/api"
-TOKEN_ENV_VAR_NAME = "LOOPQUEST_USER_TOKEN"
+from .utils import update_or_append_env_var, is_docker_installed
 
+# CLOUD_FRONTEND_URL = "http://localhost:5667"
+# CLOUD_BACKEND_URL = "http://localhost:5667/api"
 
-def is_local_instance_initialized():
-    try:
-        backend_response = requests.get(LOCAL_BACKEND_URL)
-        frontend_response = requests.get(LOCAL_FRONTEND_URL)
-        return (
-            backend_response.status_code == 200 and frontend_response.status_code == 200
-        )
-    except:
-        return False
+# For Dev
+CLOUD_FRONTEND_URL = "http://localhost:5667"
+CLOUD_BACKEND_URL = "http://localhost:5667/api"
+TOKEN_ENV_VAR_NAME = "LOOPQUEST_USER_TOKEN"
 
 
 def is_cloud_instance_initialized():
     from .crud import get_cloud_user_id
 
     try:
         get_cloud_user_id(CLOUD_BACKEND_URL)
         return True
     except Exception as e:
         return False
 
 
-def wait_for_local_instance_init():
-    start_time = time.time()
-    timeout = 60  # seconds
-    try:
-        while True:
-            if is_local_instance_initialized():
-                break
-
-            elapsed_time = time.time() - start_time
-            if elapsed_time > timeout:
-                raise Exception(
-                    f"Timeout ({timeout} sec) exceeded while waiting for local instance to initialize."
-                )
-    except KeyboardInterrupt as e:
-        print(
-            "KeyboardInterrupt received. Stop waiting for the local instance to initialize."
-        )
-        return
-
-
 def verify_token(token):
     try:
         response = requests.get(
             f"{CLOUD_BACKEND_URL}/user_id", headers={"Authorization": f"Bearer {token}"}
         )
         response.raise_for_status()
         return True
```

### Comparing `loopquest-0.1.9/loopquest/schema.py` & `loopquest-0.2.0/loopquest/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,42 @@
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Any, Dict
 import datetime
-from pydantic import BaseModel
+from pydantic import BaseModel, Json
 import enum
 
 
 Scalar = Union[float, int, str]
 
 
-class ScalarInfo(BaseModel):
+class VarNode(BaseModel):
+    # This path is used by the api for the value retrieval.
+    path: Optional[str] = None
+    # This path represents the path from the root to this node in the VarNode
+    # tree.
+    tree_path: Optional[str] = None
     name: Optional[str] = None
     description: Optional[str] = None
+    spec: Optional[str] = None
+    children: Optional[List["VarNode"]] = []
 
 
-class VectorSpec(BaseModel):
-    # Name is optional, and it is mostly useful for composite spaces
-    # (https://gymnasium.farama.org/api/spaces/#composite-spaces).
-    # If the vector is not composite, the name is unnecessary.
-    name: Optional[str] = None
-    space: str
-    # All the observations or actions are flattened into a 1D array.
-    size: int
-    var_info: Optional[List[ScalarInfo]] = None
+class NumpyLike(BaseModel):
+    shape: List[int] = []
+    value: List[int | float] = []
+    type: str = None
+
+
+class SpaceVal(BaseModel):
+    spec: str = None
+    # Discrete (int), Text (str), Box/MultiBinary/MultiDiscrete (NumpyLike) values are saved here.
+    value: Optional[int | float | str | NumpyLike] = None
+    # Only Sequence values are saved here.
+    seq: Optional[List["SpaceVal"]] = None
+    # Dict, Tuple (keyed by index string) and Graph values are saved here.
+    dic: Optional[Dict[str, "SpaceVal"]] = None
 
 
 class EnvironmentCreate(BaseModel):
     # This could be gym id, [namespace/](env-name)[-v(version)].
     id: str
     name: Optional[str] = ""
     # Created by this user.
@@ -33,21 +45,18 @@
     gym_id: Optional[str] = None
     description: Optional[str] = None
     # JSON string of gym env spec
     # https://gymnasium.farama.org/api/registry/#gymnasium.envs.registration.EnvSpec
     env_spec: Optional[str] = None
     # Multiple VectorSpecs are used to represent composite spaces, e.g. Dict,
     # Tuple, Sequence etc.
-    action_spec: Optional[List[VectorSpec]] = None
-    observation_spec: Optional[List[VectorSpec]] = None
-    reward_upper_limit: Optional[float] = None
-    reward_lower_limit: Optional[float] = None
+    action_metadata: Optional[VarNode] = None
+    observation_metadata: Optional[VarNode] = None
     git_repo: Optional[str] = None
-    is_legacy_gym: Optional[bool] = False
-    is_native_gym: Optional[bool] = True
+    support_remote_eval: Optional[bool] = False
 
 
 class Environment(EnvironmentCreate):
     creation_time: datetime.datetime
     update_time: Optional[datetime.datetime] = None
 
 
@@ -61,28 +70,48 @@
     text: str
     image: Optional[List[str]] = None  # image urls
     video: Optional[List[str]] = None  # video urls
     # This should be the consistent with observation_spec.
     observable_state: Optional[List[Scalar]] = None
 
 
+class ProjectCreate(BaseModel):
+    name: str
+    user_id: str
+    description: Optional[str] = None
+    experiment_ids: Optional[List[str]] = []
+    experiment_names: Optional[List[str]] = []
+    environment_ids: Optional[List[str]] = []
+
+
+class Project(ProjectCreate):
+    id: str
+    creation_time: datetime.datetime
+    update_time: Optional[datetime.datetime] = None
+
+
+class ProjectUpdate(ProjectCreate):
+    name: Optional[str] = None
+    user_id: Optional[str] = None
+
+
 # This client schema needs to be synced with the server schema.
 class ExperimentCreate(BaseModel):
-    # TODO: support multipe envs.
-    environment_id: str
+    environment_ids: Optional[List[str]] = []
+    project_id: Optional[str] = None
     user_id: str
-    agent_id: Optional[str] = None
+    policy_repo_id: Optional[str] = None
+    policy_filename: Optional[str] = None
+    algorithm_name: Optional[str] = None
     num_episodes: Optional[int] = None
     num_steps: Optional[int] = None
     name: Optional[str] = None
-
     random_seed: Optional[int] = None
-    environment_configs: Optional[str] = None  # JSON string of experiment configs
-    agent_configs: Optional[str] = None  # JSON string of agent config
-    goal: Optional[Goal] = None
+    configs: Optional[Dict[str, Any]] = None
+    is_public: Optional[bool] = False
 
 
 class ExperimentStatus(str, enum.Enum):
     PENDING = "pending"
     RUNNING = "running"
     FINISHED = "finished"
     FAILED = "failed"
@@ -94,48 +123,64 @@
     creation_time: datetime.datetime
     update_time: Optional[datetime.datetime] = None
     error_message: Optional[str] = None
 
 
 class ExperimentUpdate(ExperimentCreate):
     status: Optional[ExperimentStatus] = ExperimentStatus.PENDING
-    environment_id: Optional[str] = None
+    environment_ids: Optional[List[str]] = None
     agent_id: Optional[str] = None
+    project_id: Optional[str] = None
     user_id: Optional[str] = None
     num_steps: Optional[int] = None
     error_message: Optional[str] = None
 
 
 class StepCreate(BaseModel):
     experiment_id: str
+    environment_id: str
     episode: int
     # In simulation, all the observations and actions are aligned in time.
     step: int
     # NOTE: observation and action are flattened into 1D arrays.
-    observation: List[Scalar] = None
-    action: Optional[List[Scalar]] = None
+    observation: Optional[SpaceVal] = None
+    action: Optional[SpaceVal] = None
     reward: Optional[float] = 0.0
-    # NOTE: even though this is redundant and suboptimal for space, it makes
-    # the MDP transition complete and much more convenient for training.
-    prev_observation: Optional[List[Scalar]] = None
     # This is potentially useful to train a policy conditioned on sub goals.
     sub_goal: Optional[Goal] = None
     image_urls: Optional[List[str]] = []
     termnated: Optional[bool] = False
     truncated: Optional[bool] = False
     # This is deprecated by Gymnasium, but we still keep it for backward
     # compatibility.
     done: Optional[bool] = False
-    info: Optional[str] = None  # JSON string of step info
+    info: Optional[Dict[str, Any]] = None  # JSON string of step info
 
 
 class Step(StepCreate):
     id: str
     creation_time: datetime.datetime
     update_time: Optional[datetime.datetime] = None
 
 
 class StepUpdate(StepCreate):
     experiment_id: Optional[str] = None
+    environment_id: Optional[str] = None
     episode: Optional[int] = None
     # In simulation, all the observations and actions are aligned in time.
     step: Optional[int] = None
+
+
+class EvalRequest(BaseModel):
+    huggingface_repo_id: str
+    huggingface_filename: str
+    algorithm_name: str
+    env_ids: list[str]
+    num_episodes: int = 10
+    num_steps_per_episode: int = 1000
+    project_name: str = None
+    project_description: str = None
+    experiment_name: str = None
+    experiment_description: str = ""
+    experiment_configs: dict[str, Any] = None
+    use_thread_pool: bool = True
+    max_workers: int = 10
```

### Comparing `loopquest-0.1.9/loopquest/utils.py` & `loopquest-0.2.0/loopquest/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import os
 
 
 def cast_to_list(
     x,
 ) -> list[float | int | str]:
     if isinstance(x, np.ndarray):
+        if x.size == 1:
+            return [x.item()]
         return x.tolist()
     elif isinstance(x, np.generic):
         return [x.item()]
     elif isinstance(x, (float, int, str)):
         return [x]
     else:
         # TODO: handle other types, and better error handling
@@ -26,20 +28,20 @@
 
 
 def flatten_and_cast_to_list(space, x):
     flattened_x = flatten(space, x)
     return cast_to_list(flattened_x)
 
 
-def jsonize_dict(d):
+def safe_jsonize(d):
     try:
-        json_str = json.dumps(d)
+        json.dumps(d)
     except:
-        json_str = "{'error': 'The dictionary is not JSON serializable.'}"
-    return json_str
+        d = {"error": "The dictionary is not JSON serializable."}
+    return d
 
 
 def pickle_to_str(x):
     return base64.b64encode(pickle.dumps(x)).decode()
 
 
 def unpickle_from_str(x):
@@ -55,14 +57,46 @@
 
 
 def replace_special_chars_with_dash(s):
     # Replace all non-alphanumeric characters with a dash
     return re.sub(r"[^a-zA-Z0-9]", "-", s)
 
 
+def generate_project_name():
+    adjectives = [
+        "Future",
+        "NextGen",
+        "Innovative",
+        "Revolutionary",
+        "Dynamic",
+        "Epic",
+        "Creative",
+        "Ultimate",
+        "Smart",
+        "NewAge",
+    ]
+    nouns = [
+        "Explorer",
+        "Creator",
+        "Vision",
+        "Quest",
+        "Journey",
+        "Horizon",
+        "Pioneer",
+        "Odyssey",
+        "Voyage",
+        "Destination",
+    ]
+
+    adjective = random.choice(adjectives)
+    noun = random.choice(nouns)
+
+    return f"{adjective}-{noun}"
+
+
 def generate_experiment_name():
     adjectives = [
         "fuzzy",
         "giant",
         "tiny",
         "swift",
         "clever",
```

### Comparing `loopquest-0.1.9/setup.py` & `loopquest-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 reqs = parse_requirements("requirements.txt")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loopquest",
-    version="0.1.9",
+    version="0.2.0",
     description="A Production Tool for Embodied AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="LoopMind",
     author_email="contactus@loopmind.ai",
     url="https://github.com/LoopMind-AI/loopquest",
     packages=["loopquest"],
```

### Comparing `loopquest-0.1.9/tests/test_datasets.py` & `loopquest-0.2.0/tests/test_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from loopquest.datasets import load_dataset, load_datasets
-import gymnasium
 import loopquest
 from unittest.mock import patch
 
 
 def run_sim():
     name = "MountainCarContinuous-v0"
     with patch("builtins.input", return_value="2"):
-        env = loopquest.make_env(
-            gymnasium.make(name, render_mode="rgb_array"),
-        )
+        env = loopquest.make_env(name, render_mode="rgb_array")
     obs, info = env.reset()
     for i in range(10):
         action = env.action_space.sample()
         obs, reward, terminated, truncated, info = env.step(action)
         rgb_array = env.render()
         if terminated or truncated:
             break
@@ -50,8 +47,8 @@
     ds = load_datasets(exp_ids, preload_images=True)
     for step in ds:
         assert "images" in step
 
 
 if __name__ == "__main__":
     test_load_dataset()
-    test_load_datasets()
+    # test_load_datasets()
```

### Comparing `loopquest-0.1.9/tests/test_performance.py` & `loopquest-0.2.0/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.1.9/tests/test_wrappers.py` & `loopquest-0.2.0/tests/test_wrappers.py`

 * *Files identical despite different names*

