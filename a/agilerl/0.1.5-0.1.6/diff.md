# Comparing `tmp/agilerl-0.1.5.tar.gz` & `tmp/agilerl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agilerl-0.1.5.tar", max compression
+gzip compressed data, was "agilerl-0.1.6.tar", max compression
```

## Comparing `agilerl-0.1.5.tar` & `agilerl-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.5/agilerl/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.5/agilerl/algorithms/__init__.py
--rw-r--r--   0        0        0    20456 2023-05-05 09:35:55.662695 agilerl-0.1.5/agilerl/algorithms/bc_lm.py
--rw-r--r--   0        0        0    17131 2023-05-05 09:35:55.670696 agilerl-0.1.5/agilerl/algorithms/ddpg.py
--rw-r--r--   0        0        0    12025 2023-05-05 09:35:55.670696 agilerl-0.1.5/agilerl/algorithms/dqn.py
--rw-r--r--   0        0        0    72764 2023-05-05 09:35:55.678696 agilerl-0.1.5/agilerl/algorithms/ilql.py
--rw-r--r--   0        0        0     5486 2023-05-05 09:35:55.678696 agilerl-0.1.5/agilerl/benchmarking.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.238404 agilerl-0.1.5/agilerl/components/__init__.py
--rw-r--r--   0        0        0     3874 2023-05-05 09:35:55.678696 agilerl-0.1.5/agilerl/components/replay_buffer.py
--rw-r--r--   0        0        0        0 2023-05-05 09:35:55.678696 agilerl-0.1.5/agilerl/data/__init__.py
--rw-r--r--   0        0        0     1688 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/data/language_environment.py
--rw-r--r--   0        0        0     8013 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/data/rl_data.py
--rw-r--r--   0        0        0     1303 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/data/tokenizer.py
--rw-r--r--   0        0        0     1175 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/data/torch_datasets.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.239407 agilerl-0.1.5/agilerl/hpo/__init__.py
--rw-r--r--   0        0        0    19911 2023-05-05 09:35:55.686685 agilerl-0.1.5/agilerl/hpo/mutation.py
--rw-r--r--   0        0        0     2153 2023-05-05 09:35:55.695030 agilerl-0.1.5/agilerl/hpo/tournament.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.241395 agilerl-0.1.5/agilerl/networks/__init__.py
--rw-r--r--   0        0        0    37557 2023-05-05 09:35:55.695030 agilerl-0.1.5/agilerl/networks/evolvable_bert.py
--rw-r--r--   0        0        0    25101 2023-05-05 09:35:55.695030 agilerl-0.1.5/agilerl/networks/evolvable_cnn.py
--rw-r--r--   0        0        0    37684 2023-05-05 09:35:55.695030 agilerl-0.1.5/agilerl/networks/evolvable_gpt.py
--rw-r--r--   0        0        0    14781 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/networks/evolvable_mlp.py
--rw-r--r--   0        0        0        0 2023-03-06 12:15:09.242405 agilerl-0.1.5/agilerl/training/__init__.py
--rw-r--r--   0        0        0     7408 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/training/train.py
--rw-r--r--   0        0        0     8771 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/training/train_bc_lm.py
--rw-r--r--   0        0        0     9326 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/training/train_ilql.py
--rw-r--r--   0        0        0        0 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/utils/__init__.py
--rw-r--r--   0        0        0     1628 2023-05-05 09:35:55.703476 agilerl-0.1.5/agilerl/utils/cache.py
--rw-r--r--   0        0        0     3952 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/ilql_utils.py
--rw-r--r--   0        0        0    10349 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/load_objects.py
--rw-r--r--   0        0        0     2444 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/log_utils.py
--rw-r--r--   0        0        0      120 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/mp_cache.py
--rw-r--r--   0        0        0     2205 2023-05-05 09:35:55.711952 agilerl-0.1.5/agilerl/utils/sampling_utils.py
--rw-r--r--   0        0        0     3307 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/utils/serve_queue.py
--rw-r--r--   0        0        0     1496 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/utils/torch_utils.py
--rw-r--r--   0        0        0     3389 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/utils/utils.py
--rw-r--r--   0        0        0        0 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/wordle/__init__.py
--rw-r--r--   0        0        0     7021 2023-05-05 09:35:55.719952 agilerl-0.1.5/agilerl/wordle/policy.py
--rw-r--r--   0        0        0     5900 2023-05-05 09:35:55.728286 agilerl-0.1.5/agilerl/wordle/wordle_dataset.py
--rw-r--r--   0        0        0     1119 2023-05-05 09:35:55.728286 agilerl-0.1.5/agilerl/wordle/wordle_env.py
--rw-r--r--   0        0        0     9110 2023-05-05 09:35:55.728286 agilerl-0.1.5/agilerl/wordle/wordle_evaluators.py
--rw-r--r--   0        0        0    11117 2023-05-05 09:35:55.728286 agilerl-0.1.5/agilerl/wordle/wordle_game.py
--rw-r--r--   0        0        0     2510 2023-05-05 09:35:55.736340 agilerl-0.1.5/agilerl/wordle/wordle_tokenizer.py
--rw-r--r--   0        0        0    11558 2023-03-06 12:15:09.243395 agilerl-0.1.5/LICENSE
--rw-r--r--   0        0        0      550 2023-05-05 09:36:45.006777 agilerl-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    18536 2023-05-05 09:35:55.662695 agilerl-0.1.5/README.md
--rw-r--r--   0        0        0    19107 1970-01-01 00:00:00.000000 agilerl-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.6/agilerl/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.235410 agilerl-0.1.6/agilerl/algorithms/__init__.py
+-rw-r--r--   0        0        0    20456 2023-05-05 09:35:55.662695 agilerl-0.1.6/agilerl/algorithms/bc_lm.py
+-rw-r--r--   0        0        0    12694 2023-05-23 16:32:48.664828 agilerl-0.1.6/agilerl/algorithms/cqn.py
+-rw-r--r--   0        0        0    17154 2023-05-17 09:02:17.797477 agilerl-0.1.6/agilerl/algorithms/ddpg.py
+-rw-r--r--   0        0        0    12392 2023-05-17 09:16:01.664740 agilerl-0.1.6/agilerl/algorithms/dqn.py
+-rw-r--r--   0        0        0    72764 2023-05-05 09:35:55.678696 agilerl-0.1.6/agilerl/algorithms/ilql.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.238404 agilerl-0.1.6/agilerl/components/__init__.py
+-rw-r--r--   0        0        0     3874 2023-05-19 14:45:03.354134 agilerl-0.1.6/agilerl/components/replay_buffer.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.678696 agilerl-0.1.6/agilerl/data/__init__.py
+-rw-r--r--   0        0        0     1688 2023-05-05 09:35:55.686685 agilerl-0.1.6/agilerl/data/language_environment.py
+-rw-r--r--   0        0        0     8013 2023-05-05 09:35:55.686685 agilerl-0.1.6/agilerl/data/rl_data.py
+-rw-r--r--   0        0        0     1303 2023-05-05 09:35:55.686685 agilerl-0.1.6/agilerl/data/tokenizer.py
+-rw-r--r--   0        0        0     1175 2023-05-05 09:35:55.686685 agilerl-0.1.6/agilerl/data/torch_datasets.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.239407 agilerl-0.1.6/agilerl/hpo/__init__.py
+-rw-r--r--   0        0        0    20187 2023-05-19 14:21:08.490783 agilerl-0.1.6/agilerl/hpo/mutation.py
+-rw-r--r--   0        0        0     2153 2023-05-05 09:35:55.695030 agilerl-0.1.6/agilerl/hpo/tournament.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.241395 agilerl-0.1.6/agilerl/networks/__init__.py
+-rw-r--r--   0        0        0    37557 2023-05-05 09:35:55.695030 agilerl-0.1.6/agilerl/networks/evolvable_bert.py
+-rw-r--r--   0        0        0    25101 2023-05-05 09:35:55.695030 agilerl-0.1.6/agilerl/networks/evolvable_cnn.py
+-rw-r--r--   0        0        0    37684 2023-05-05 09:35:55.695030 agilerl-0.1.6/agilerl/networks/evolvable_gpt.py
+-rw-r--r--   0        0        0    14781 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/networks/evolvable_mlp.py
+-rw-r--r--   0        0        0        0 2023-03-06 12:15:09.242405 agilerl-0.1.6/agilerl/training/__init__.py
+-rw-r--r--   0        0        0     7408 2023-05-22 13:31:33.225917 agilerl-0.1.6/agilerl/training/train.py
+-rw-r--r--   0        0        0     8771 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/training/train_bc_lm.py
+-rw-r--r--   0        0        0     9326 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/training/train_ilql.py
+-rw-r--r--   0        0        0     6662 2023-05-22 10:14:40.179051 agilerl-0.1.6/agilerl/training/train_offline.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/utils/__init__.py
+-rw-r--r--   0        0        0     1628 2023-05-05 09:35:55.703476 agilerl-0.1.6/agilerl/utils/cache.py
+-rw-r--r--   0        0        0     3952 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/ilql_utils.py
+-rw-r--r--   0        0        0    10349 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/load_objects.py
+-rw-r--r--   0        0        0     2444 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/log_utils.py
+-rw-r--r--   0        0        0      120 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/mp_cache.py
+-rw-r--r--   0        0        0     2205 2023-05-05 09:35:55.711952 agilerl-0.1.6/agilerl/utils/sampling_utils.py
+-rw-r--r--   0        0        0     3307 2023-05-05 09:35:55.719952 agilerl-0.1.6/agilerl/utils/serve_queue.py
+-rw-r--r--   0        0        0     1496 2023-05-05 09:35:55.719952 agilerl-0.1.6/agilerl/utils/torch_utils.py
+-rw-r--r--   0        0        0     4092 2023-05-22 14:05:48.103293 agilerl-0.1.6/agilerl/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:35:55.719952 agilerl-0.1.6/agilerl/wordle/__init__.py
+-rw-r--r--   0        0        0     7021 2023-05-05 09:35:55.719952 agilerl-0.1.6/agilerl/wordle/policy.py
+-rw-r--r--   0        0        0     5900 2023-05-05 09:35:55.728286 agilerl-0.1.6/agilerl/wordle/wordle_dataset.py
+-rw-r--r--   0        0        0     1119 2023-05-05 09:35:55.728286 agilerl-0.1.6/agilerl/wordle/wordle_env.py
+-rw-r--r--   0        0        0     9110 2023-05-05 09:35:55.728286 agilerl-0.1.6/agilerl/wordle/wordle_evaluators.py
+-rw-r--r--   0        0        0    11117 2023-05-05 09:35:55.728286 agilerl-0.1.6/agilerl/wordle/wordle_game.py
+-rw-r--r--   0        0        0     2510 2023-05-05 09:35:55.736340 agilerl-0.1.6/agilerl/wordle/wordle_tokenizer.py
+-rw-r--r--   0        0        0    11558 2023-03-06 12:15:09.243395 agilerl-0.1.6/LICENSE
+-rw-r--r--   0        0        0      728 2023-05-24 08:41:30.075862 agilerl-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    32090 2023-05-23 16:32:45.722183 agilerl-0.1.6/README.md
+-rw-r--r--   0        0        0    32755 1970-01-01 00:00:00.000000 agilerl-0.1.6/PKG-INFO
```

### Comparing `agilerl-0.1.5/agilerl/algorithms/bc_lm.py` & `agilerl-0.1.6/agilerl/algorithms/bc_lm.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/algorithms/ddpg.py` & `agilerl-0.1.6/agilerl/algorithms/ddpg.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,26 +173,26 @@
         state = torch.from_numpy(state).float().to(self.device)
 
         if self.one_hot:
             state = nn.functional.one_hot(
                 state.long(), num_classes=self.state_dim[0]).float().squeeze()
 
         if len(state.size()) < 2:
-            state = state.unsqueeze(0)
-
-        self.actor.eval()
-        with torch.no_grad():
-            action_values = self.actor(state)
-        self.actor.train()
+            state = state.unsqueeze(0)       
 
         # epsilon-greedy
         if random.random() < epsilon:
             action = (np.random.rand(
                 state.size()[0], self.action_dim).astype('float32') - 0.5) * 2
         else:
+            self.actor.eval()
+            with torch.no_grad():
+                action_values = self.actor(state)
+            self.actor.train()
+
             action = action_values.cpu().data.numpy()
 
         return action
 
     def learn(self, experiences, noise_clip=0.5, policy_noise=0.2):
         """Updates agent network parameters to learn from experiences.
```

### Comparing `agilerl-0.1.5/agilerl/algorithms/dqn.py` & `agilerl-0.1.6/agilerl/algorithms/cqn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import random
 import copy
 import numpy as np
 import torch
 import torch.nn as nn
+from torch.nn.utils import clip_grad_norm_
 import torch.optim as optim
 from agilerl.networks.evolvable_mlp import EvolvableMLP
 from agilerl.networks.evolvable_cnn import EvolvableCNN
 
 
-class DQN():
-    """The DQN algorithm class. DQN paper: https://arxiv.org/abs/1312.5602
+class CQN():
+    """The CQN algorithm class. CQN paper: https://arxiv.org/abs/2006.04779
 
     :param state_dim: State observation dimension
     :type state_dim: int
     :param action_dim: Action dimension
     :type action_dim: int
     :param one_hot: One-hot encoding, used with discrete observation spaces
     :type one_hot: bool
@@ -29,37 +30,40 @@
     :type learn_step: int, optional
     :param gamma: Discount factor, defaults to 0.99
     :type gamma: float, optional
     :param tau: For soft update of target network parameters, defaults to 1e-3
     :type tau: float, optional
     :param mutation: Most recent mutation to agent, defaults to None
     :type mutation: str, optional
+    :param double: Use double Q-learning, defaults to False
+    :type double: bool, optional
     :param device: Device for accelerated computing, 'cpu' or 'cuda', defaults to 'cpu'
     :type device: str, optional
     """
 
     def __init__(
         self,
         state_dim,
         action_dim,
         one_hot,
         index=0,
         net_config={
             'arch': 'mlp',
-            'h_size': [
-            64,
-            64]},
-            batch_size=64,
-            lr=1e-4,
-            learn_step=5,
-            gamma=0.99,
-            tau=1e-3,
-            mutation=None,
-            device='cpu'):
-        self.algo = 'DQN'
+            'h_size': [64, 64]
+            },
+        batch_size=64,
+        lr=1e-4,
+        learn_step=5,
+        gamma=0.99,
+        tau=1e-3,
+        mutation=None,
+        double=False,
+        device='cpu'):
+        
+        self.algo = 'CQN'
         self.state_dim = state_dim
         self.action_dim = action_dim
         self.one_hot = one_hot
         self.net_config = net_config
         self.batch_size = batch_size
         self.lr = lr
         self.learn_step = learn_step
@@ -69,14 +73,16 @@
         self.device = device
 
         self.index = index
         self.scores = []
         self.fitness = []
         self.steps = [0]
 
+        self.double = double
+
         # model
         if self.net_config['arch'] == 'mlp':      # Multi-layer Perceptron
             self.actor = EvolvableMLP(
                 num_inputs=state_dim[0],
                 num_outputs=action_dim,
                 hidden_size=self.net_config['h_size'],
                 device=self.device).to(
@@ -110,15 +116,16 @@
                 self.device)
             self.actor_target.load_state_dict(self.actor.state_dict())
 
         self.optimizer = optim.Adam(self.actor.parameters(), lr=self.lr)
         self.criterion = nn.MSELoss()
 
     def getAction(self, state, epsilon=0):
-        """Returns the next action to take in the environment. Epsilon is the probability of taking a random action, used for exploration.
+        """Returns the next action to take in the environment. Epsilon is the 
+        probability of taking a random action, used for exploration.
         For epsilon-greedy behaviour, set epsilon to 0.
 
         :param state: State observation, or multiple observations in a batch
         :type state: float or List[float]
         :param epsilon: Probablilty of taking a random action for exploration, defaults to 0
         :type epsilon: float, optional
         """
@@ -127,26 +134,23 @@
         if self.one_hot:
             state = nn.functional.one_hot(
                 state.long(), num_classes=self.state_dim[0]).float().squeeze()
 
         if len(state.size()) < 2:
             state = state.unsqueeze(0)
 
-        self.actor.eval()
-        with torch.no_grad():
-            action_values = self.actor(state)
-        self.actor.train()
-
         # epsilon-greedy
         if random.random() < epsilon:
-            action = np.random.randint(
-                0, self.action_dim, size=state.size()[0])
+            action = np.random.randint(0, self.action_dim, size=state.size()[0])[0]
         else:
-            action = np.argmax(action_values.cpu().data.numpy(), axis=1)
-
+            self.actor.eval()
+            with torch.no_grad():
+                action_values = self.actor(state)
+            self.actor.train()
+            action = np.argmax(action_values.cpu().data.numpy(), axis=1)[0]
         return action
 
     def learn(self, experiences):
         """Updates agent network parameters to learn from experiences.
 
         :param experiences: List of batched states, actions, rewards, next_states, dones in that order.
         :type state: List[torch.Tensor[float]]
@@ -155,24 +159,32 @@
 
         if self.one_hot:
             states = nn.functional.one_hot(
                 states.long(), num_classes=self.state_dim[0]).float().squeeze()
             next_states = nn.functional.one_hot(
                 next_states.long(), num_classes=self.state_dim[0]).float().squeeze()
 
-        q_target = self.actor_target(next_states).detach().max(axis=1)[
-            0].unsqueeze(1)
+        if self.double: # Double Q-learning
+            q_idx = self.actor_target(next_states).argmax(dim=1).unsqueeze(1)
+            q_target_next = self.actor(next_states).gather(dim=1, index=q_idx).detach()
+        else:
+            q_target_next = self.actor_target(next_states).detach().max(axis=1)[0].unsqueeze(1)
+
         # target, if terminal then y_j = rewards
-        y_j = rewards + self.gamma * q_target * (1 - dones)
-        q_eval = self.actor(states).gather(1, actions.long())
+        q_target = rewards + self.gamma * q_target_next * (1 - dones)
+        q_a_s = self.actor(states)
+        q_eval = q_a_s.gather(1, actions.long())
 
         # loss backprop
-        loss = self.criterion(q_eval, y_j)
+        cql1_loss = torch.logsumexp(q_a_s, dim=1).mean() - q_a_s.mean()
+        loss = self.criterion(q_eval, q_target)
+        q1_loss = cql1_loss + 0.5 * loss
         self.optimizer.zero_grad()
-        loss.backward()
+        q1_loss.backward()
+        clip_grad_norm_(self.actor.parameters(), 1)
         self.optimizer.step()
 
         # soft update target network
         self.softUpdate()
 
     def softUpdate(self):
         """Soft updates target network.
@@ -201,14 +213,16 @@
                 score = 0
                 for idx_step in range(max_steps):
                     if swap_channels:
                         state = np.moveaxis(state, [3], [1])
                     action = self.getAction(state, epsilon=0)
                     state, reward, done, _, _ = env.step(action)
                     score += reward
+                    if done:
+                        break
                 rewards.append(score)
         mean_fit = np.mean(rewards)
         self.fitness.append(mean_fit)
         return mean_fit
 
     def clone(self, index=None):
         """Returns cloned agent identical to self.
```

### Comparing `agilerl-0.1.5/agilerl/algorithms/ilql.py` & `agilerl-0.1.6/agilerl/algorithms/ilql.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/components/replay_buffer.py` & `agilerl-0.1.6/agilerl/components/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/data/language_environment.py` & `agilerl-0.1.6/agilerl/data/language_environment.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/data/rl_data.py` & `agilerl-0.1.6/agilerl/data/rl_data.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/data/tokenizer.py` & `agilerl-0.1.6/agilerl/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/data/torch_datasets.py` & `agilerl-0.1.6/agilerl/data/torch_datasets.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/hpo/mutation.py` & `agilerl-0.1.6/agilerl/hpo/mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,14 +448,23 @@
                 },
                 'critics': [{
                     'eval': 'critic',
                     'target': 'critic_target',
                     'optimizer': 'critic_optimizer'
                 }]
             }
+        elif algo == 'CQN':
+            nets = {
+                'actor': {
+                    'eval': 'actor',
+                    'target': 'actor_target',
+                    'optimizer': 'optimizer'
+                },
+                'critics': []
+            }
         elif algo == 'ILQL':
             nets = {
                 'actor': {
                     'eval': 'actor',
                     'target': 'actor_target',
                     'optimizer': 'optimizer'
                 },
```

### Comparing `agilerl-0.1.5/agilerl/hpo/tournament.py` & `agilerl-0.1.6/agilerl/hpo/tournament.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/networks/evolvable_bert.py` & `agilerl-0.1.6/agilerl/networks/evolvable_bert.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/networks/evolvable_cnn.py` & `agilerl-0.1.6/agilerl/networks/evolvable_cnn.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/networks/evolvable_gpt.py` & `agilerl-0.1.6/agilerl/networks/evolvable_gpt.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/networks/evolvable_mlp.py` & `agilerl-0.1.6/agilerl/networks/evolvable_mlp.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/training/train.py` & `agilerl-0.1.6/agilerl/training/train.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/training/train_bc_lm.py` & `agilerl-0.1.6/agilerl/training/train_bc_lm.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/training/train_ilql.py` & `agilerl-0.1.6/agilerl/training/train_ilql.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/utils/cache.py` & `agilerl-0.1.6/agilerl/utils/cache.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/utils/ilql_utils.py` & `agilerl-0.1.6/agilerl/utils/ilql_utils.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/utils/load_objects.py` & `agilerl-0.1.6/agilerl/utils/load_objects.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/utils/log_utils.py` & `agilerl-0.1.6/agilerl/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/utils/sampling_utils.py` & `agilerl-0.1.6/agilerl/utils/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/utils/serve_queue.py` & `agilerl-0.1.6/agilerl/utils/serve_queue.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/utils/torch_utils.py` & `agilerl-0.1.6/agilerl/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/utils/utils.py` & `agilerl-0.1.6/agilerl/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import gymnasium as gym
 import numpy as np
 import matplotlib.pyplot as plt
+from agilerl.algorithms.cqn import CQN
 from agilerl.algorithms.dqn import DQN
 from agilerl.algorithms.ddpg import DDPG
 
 
 def makeVectEnvs(env_name, num_envs=1):
     """Returns async-vectorized gym environments.
 
     :param env_name: Gym environment name
     :type env_name: str
-    :param num_ens: Number of vectorized environments, defaults to 1
+    :param num_envs: Number of vectorized environments, defaults to 1
     :type num_envs: int, optional
     """
     return gym.vector.AsyncVectorEnv(
         [lambda: gym.make(env_name) for i in range(num_envs)])
 
 
 def initialPopulation(algo, state_dim, action_dim, one_hot,
@@ -47,14 +48,15 @@
                 index=idx,
                 net_config=net_config,
                 batch_size=INIT_HP['BATCH_SIZE'],
                 lr=INIT_HP['LR'],
                 learn_step=INIT_HP['LEARN_STEP'],
                 gamma=INIT_HP['GAMMA'],
                 tau=INIT_HP['TAU'],
+                double=INIT_HP['DOUBLE'],
                 device=device
             )
             population.append(agent)
 
     elif algo == 'DDPG':
         for idx in range(population_size):
             agent = DDPG(
@@ -69,14 +71,32 @@
                 gamma=INIT_HP['GAMMA'],
                 tau=INIT_HP['TAU'],
                 policy_freq=INIT_HP['POLICY_FREQ'],
                 device=device
             )
             population.append(agent)
 
+    elif algo == 'CQN':
+        for idx in range(population_size):
+            agent = CQN(
+                state_dim=state_dim,
+                action_dim=action_dim,
+                one_hot=one_hot,
+                index=idx,
+                net_config=net_config,
+                batch_size=INIT_HP['BATCH_SIZE'],
+                lr=INIT_HP['LR'],
+                learn_step=INIT_HP['LEARN_STEP'],
+                gamma=INIT_HP['GAMMA'],
+                tau=INIT_HP['TAU'],
+                double=INIT_HP['DOUBLE'],
+                device=device
+            )
+            population.append(agent)
+
     return population
 
 
 def printHyperparams(pop):
     """Prints current hyperparameters of agents in a population and their fitnesses.
 
     :param pop: Population of agents
```

### Comparing `agilerl-0.1.5/agilerl/wordle/policy.py` & `agilerl-0.1.6/agilerl/wordle/policy.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/wordle/wordle_dataset.py` & `agilerl-0.1.6/agilerl/wordle/wordle_dataset.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/wordle/wordle_env.py` & `agilerl-0.1.6/agilerl/wordle/wordle_env.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/wordle/wordle_evaluators.py` & `agilerl-0.1.6/agilerl/wordle/wordle_evaluators.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/wordle/wordle_game.py` & `agilerl-0.1.6/agilerl/wordle/wordle_game.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/agilerl/wordle/wordle_tokenizer.py` & `agilerl-0.1.6/agilerl/wordle/wordle_tokenizer.py`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/LICENSE` & `agilerl-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `agilerl-0.1.5/PKG-INFO` & `agilerl-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: agilerl
-Version: 0.1.5
+Version: 0.1.6
 Summary: AgileRL is a deep reinforcement learning library focused on improving RL development through RLOps.
 License: Apache 2.0
 Author: Nick Ustaran-Anderegg
 Author-email: dev@agilerl.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: accelerate (>=0.18.0,<0.19.0)
 Requires-Dist: fastrand (>=1.3.0,<2.0.0)
-Requires-Dist: gymnasium (>=0.27.1,<0.28.0)
+Requires-Dist: flatten_dict (>=0.4.2,<0.5.0)
+Requires-Dist: gymnasium (>=0.26.3,<0.27.0)
+Requires-Dist: h5py (>=3.8.0,<4.0.0)
+Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
-Requires-Dist: numpy (>=1.22.4,<2.0.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
+Requires-Dist: redis (>=4.4.4,<5.0.0)
+Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: torch (>=1.13.1,<2.0.0)
-Requires-Dist: tqdm (>=4.62.2,<5.0.0)
-Requires-Dist: wandb (>=0.13.1,<0.14.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: transformers (>=4.23.1,<5.0.0)
+Requires-Dist: wandb (>=0.13.10,<0.14.0)
 Description-Content-Type: text/markdown
 
 # AgileRL
 <p align="center">
   <img src=https://user-images.githubusercontent.com/47857277/222710068-e09a4e3c-368c-458a-9e01-b68674806887.png height="120">
 </p>
 <p align="center"><b>Reinforcement learning streamlined.</b><br>Easier and faster reinforcement learning with RLOps. Visit our <a href="https://agilerl.com">website</a>. View <a href="https://agilerl.readthedocs.io/en/latest/">documentation</a>.<br>Join the <a href="https://discord.gg/eB8HyTA2ux">Discord Server</a> to collaborate.</p>
@@ -47,16 +55,18 @@
 </p>
 <p align="center">AgileRL offers 10x faster hyperparameter optimization than SOTA.<br> Global steps is the sum of every step taken by any agent in the environment, including across an entire population, during the entire hyperparameter optimization process.</p>
 
 ## Table of Contents
   * [Benchmarks](#benchmarks)
   * [Get Started](#get-started)
   * [Algorithms implemented](#algorithms-implemented-more-coming-soon)
-  * [Train an agent on a Gym environment](#train-an-agent-on-a-gym-environment)
-    + [Custom Training Loop](#custom-training-loop)
+  * [Train an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-online)
+    + [Custom Online Training Loop](#custom-online-training-loop)
+  * [Train an agent on data (Offline)](#train-an-agent-on-data-offline)
+    + [Custom Offline Training Loop](#custom-offline-training-loop)
   * [Train an agent on a language environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf)
 
 ## Benchmarks
 
 Reinforcement learning algorithms and libraries are usually benchmarked once the optimal hyperparameters for training are known, but it often takes hundreds or thousands of experiments to discover these. This is unrealistic and does not reflect the true, total time taken for training. What if we could remove the need to conduct all these prior experiments?
 
 In the charts below, a single AgileRL run, which automatically tunes hyperparameters, is benchmarked against Optuna's multiple training runs traditionally required for hyperparameter optimization, demonstrating the real time savings possible. Global steps is the sum of every step taken by any agent in the environment, including across an entire population.
@@ -82,22 +92,24 @@
 ```bash
 python demo.py
 ```
 
 ## Algorithms implemented (more coming soon!)
   * DQN
   * DDPG
+  * CQL
   * ILQL
 
-## Train an agent on a Gym environment
+## Train an agent on a Gym environment (Online)
 Before starting training, there are some meta-hyperparameters and settings that must be set. These are defined in <code>INIT_HP</code>, for general parameters, and <code>MUTATION_PARAMS</code>, which define the evolutionary probabilities, and <code>NET_CONFIG</code>, which defines the network architecture. For example:
 ```python
 INIT_HP = {
     'ENV_NAME': 'LunarLander-v2',   # Gym environment name
     'ALGO': 'DQN',                  # Algorithm
+    'DOUBLE': True,                 # Use double Q-learning
     'CHANNELS_LAST': False,         # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
     'BATCH_SIZE': 256,              # Batch size
     'LR': 1e-3,                     # Learning rate
     'EPISODES': 2000,               # Max no. episodes
     'TARGET_SCORE': 200.,           # Early training stop at avg score of last 100 episodes
     'GAMMA': 0.99,                  # Discount factor
     'MEMORY_SIZE': 10000,           # Max memory buffer size
@@ -127,17 +139,17 @@
 ```
 ```python
 NET_CONFIG = {
     'arch': 'mlp',      # Network architecture
     'h_size': [32, 32], # Actor hidden size
 }
 ```
-First, use <code>utils.initialPopulation</code> to create a list of agents - our population that will evolve and mutate to the optimal hyperparameters.
+First, use <code>utils.utils.initialPopulation</code> to create a list of agents - our population that will evolve and mutate to the optimal hyperparameters.
 ```python
-from agilerl.utils import makeVectEnvs, initialPopulation
+from agilerl.utils.utils import makeVectEnvs, initialPopulation
 import torch
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 env = makeVectEnvs(env_name=INIT_HP['ENV_NAME'], num_envs=16)
 try:
     state_dim = env.single_observation_space.n          # Discrete observation space
@@ -189,15 +201,15 @@
                       rl_hp=MUTATION_PARAMS['RL_HP_MUT'],                   # Learning HP mutation
                       rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],   # Learning HPs to choose from
                       mutation_sd=MUTATION_PARAMS['MUT_SD'],                # Mutation strength
                       arch=NET_CONFIG['arch'],                              # Network architecture
                       rand_seed=MUTATION_PARAMS['RAND_SEED'],               # Random seed
                       device=torch.device("cuda"))
 ```
-The easiest training loop implementation is to use our <code>training.train()</code> function. It requires the <code>agent</code> have functions <code>getAction()</code> and <code>learn().</code>
+The easiest training loop implementation is to use our <code>training.train.train()</code> function. It requires the <code>agent</code> have functions <code>getAction()</code> and <code>learn().</code>
 ```python
 from agilerl.training.train import train
 
 trained_pop, pop_fitnesses = train(env=env,                             # Gym-style environment
                                    env_name=INIT_HP['ENV_NAME'],        # Environment name
                                    algo=INIT_HP['ALGO'],                # Algorithm
                                    pop=agent_pop,                       # Population of agents
@@ -209,32 +221,33 @@
                                    target=INIT_HP['TARGET_SCORE'],      # Target score for early stopping
                                    tournament=tournament,               # Tournament selection object
                                    mutation=mutations,                  # Mutations object
                                    wb=INIT_HP['WANDB'],                 # Weights and Biases tracking
                                    device=torch.device("cuda"))
 ```
 
-### Custom Training Loop
+### Custom Online Training Loop
 Alternatively, use a custom training loop. Combining all of the above:
 
 ```python
-from agilerl.utils import makeVectEnvs, initialPopulation
+from agilerl.utils.utils import makeVectEnvs, initialPopulation
 from agilerl.components.replay_buffer import ReplayBuffer
 from agilerl.hpo.tournament import TournamentSelection
 from agilerl.hpo.mutation import Mutations
 import gymnasium as gym
 import numpy as np
 import torch
 
 NET_CONFIG = {
                 'arch': 'mlp',       # Network architecture
                 'h_size': [32, 32],  # Actor hidden size
              }
 
 INIT_HP = {
+            'DOUBLE': True,         # Use double Q-learning
             'BATCH_SIZE': 128,      # Batch size
             'LR': 1e-3,             # Learning rate
             'GAMMA': 0.99,          # Discount factor
             'LEARN_STEP': 1,        # Learning frequency
             'TAU': 1e-3,            # For soft update of target network parameters
             'CHANNELS_LAST': False  # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
           }
@@ -310,14 +323,254 @@
 
     # Now evolve population if necessary
     if (idx_epi+1) % evo_epochs == 0:
         
         # Evaluate population
         fitnesses = [agent.test(env, swap_channels=False, max_steps=max_steps, loop=evo_loop) for agent in pop]
 
+        print(f'Episode {idx_epi+1}/{max_episodes}')
+        print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
+        print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
+
+        # Tournament selection and population mutation
+        elite, pop = tournament.select(pop)
+        pop = mutations.mutation(pop)
+```
+
+## Train an agent on data (Offline)
+Like with online RL, above, there are some meta-hyperparameters and settings that must be set before starting training. These are defined in <code>INIT_HP</code>, for general parameters, and <code>MUTATION_PARAMS</code>, which define the evolutionary probabilities, and <code>NET_CONFIG</code>, which defines the network architecture. For example:
+```python
+INIT_HP = {
+  'ENV_NAME': 'CartPole-v1',      # Gym environment name
+  'DATASET': 'data/cartpole/cartpole_random_v1.1.0.h5', # Offline RL dataset
+  'ALGO': 'CQN',                  # Algorithm
+  'DOUBLE': True,                 # Use double Q-learning
+  # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+  'CHANNELS_LAST': False,
+  'BATCH_SIZE': 256,              # Batch size
+  'LR': 1e-3,                     # Learning rate
+  'EPISODES': 2000,               # Max no. episodes
+  'TARGET_SCORE': 200.,           # Early training stop at avg score of last 100 episodes
+  'GAMMA': 0.99,                  # Discount factor
+  'MEMORY_SIZE': 10000,           # Max memory buffer size
+  'LEARN_STEP': 1,                # Learning frequency
+  'TAU': 1e-3,                    # For soft update of target parameters
+  'TOURN_SIZE': 2,                # Tournament size
+  'ELITISM': True,                # Elitism in tournament selection
+  'POP_SIZE': 6,                  # Population size
+  'EVO_EPOCHS': 20,               # Evolution frequency
+  'POLICY_FREQ': 2,               # Policy network update frequency
+  'WANDB': True                   # Log with Weights and Biases
+}
+```
+```python
+MUTATION_PARAMS = {
+    # Relative probabilities
+    'NO_MUT': 0.4,                              # No mutation
+    'ARCH_MUT': 0.2,                            # Architecture mutation
+    'NEW_LAYER': 0.2,                           # New layer mutation
+    'PARAMS_MUT': 0.2,                          # Network parameters mutation
+    'ACT_MUT': 0,                               # Activation layer mutation
+    'RL_HP_MUT': 0.2,                           # Learning HP mutation
+    'RL_HP_SELECTION': ['lr', 'batch_size'],    # Learning HPs to choose from
+    'MUT_SD': 0.1,                              # Mutation strength
+    'RAND_SEED': 1,                             # Random seed
+}
+```
+```python
+NET_CONFIG = {
+    'arch': 'mlp',      # Network architecture
+    'h_size': [32, 32], # Actor hidden size
+}
+```
+First, use <code>utils.utils.initialPopulation</code> to create a list of agents - our population that will evolve and mutate to the optimal hyperparameters.
+```python
+from agilerl.utils.utils import initialPopulation
+import torch
+import h5py
+import gymnasium as gym
+
+device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+env = gym.make(INIT_HP['ENV_NAME'])
+try:
+    state_dim = env.observation_space.n       # Discrete observation space
+    one_hot = True                            # Requires one-hot encoding
+except Exception:
+    state_dim = env.observation_space.shape   # Continuous observation space
+    one_hot = False                           # Does not require one-hot encoding
+try:
+    action_dim = env.action_space.n           # Discrete action space
+except Exception:
+    action_dim = env.action_space.shape[0]    # Continuous action space
+
+if INIT_HP['CHANNELS_LAST']:
+    state_dim = (state_dim[2], state_dim[0], state_dim[1])
+
+dataset = h5py.File(INIT_HP['DATASET'], 'r')
+
+agent_pop = initialPopulation(algo=INIT_HP['ALGO'],                 # Algorithm
+                              state_dim=state_dim,                  # State dimension
+                              action_dim=action_dim,                # Action dimension
+                              one_hot=one_hot,                      # One-hot encoding
+                              net_config=NET_CONFIG,                # Network configuration
+                              INIT_HP=INIT_HP,                      # Initial hyperparameters
+                              population_size=INIT_HP['POP_SIZE'],  # Population size
+                              device=torch.device("cuda"))
+```
+Next, create the tournament, mutations and experience replay buffer objects that allow agents to share memory and efficiently perform evolutionary HPO.
+```python
+from agilerl.components.replay_buffer import ReplayBuffer
+from agilerl.hpo.tournament import TournamentSelection
+from agilerl.hpo.mutation import Mutations
+import torch
+
+field_names = ["state", "action", "reward", "next_state", "done"]
+memory = ReplayBuffer(action_dim=action_dim,                # Number of agent actions
+                      memory_size=INIT_HP['MEMORY_SIZE'],   # Max replay buffer size
+                      field_names=field_names,              # Field names to store in memory
+                      device=torch.device("cuda"))
+
+tournament = TournamentSelection(tournament_size=INIT_HP['TOURN_SIZE'], # Tournament selection size
+                                 elitism=INIT_HP['ELITISM'],            # Elitism in tournament selection
+                                 population_size=INIT_HP['POP_SIZE'],   # Population size
+                                 evo_step=INIT_HP['EVO_EPOCHS'])        # Evaluate using last N fitness scores
+
+mutations = Mutations(algo=INIT_HP['ALGO'],                                 # Algorithm
+                      no_mutation=MUTATION_PARAMS['NO_MUT'],                # No mutation
+                      architecture=MUTATION_PARAMS['ARCH_MUT'],             # Architecture mutation
+                      new_layer_prob=MUTATION_PARAMS['NEW_LAYER'],          # New layer mutation
+                      parameters=MUTATION_PARAMS['PARAMS_MUT'],             # Network parameters mutation
+                      activation=MUTATION_PARAMS['ACT_MUT'],                # Activation layer mutation
+                      rl_hp=MUTATION_PARAMS['RL_HP_MUT'],                   # Learning HP mutation
+                      rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'],   # Learning HPs to choose from
+                      mutation_sd=MUTATION_PARAMS['MUT_SD'],                # Mutation strength
+                      arch=NET_CONFIG['arch'],                              # Network architecture
+                      rand_seed=MUTATION_PARAMS['RAND_SEED'],               # Random seed
+                      device=torch.device("cuda"))
+```
+The easiest training loop implementation is to use our <code>training.train_offline.train()</code> function. It requires the <code>agent</code> have functions <code>getAction()</code> and <code>learn().</code>
+```python
+from agilerl.training.train_offline import train
+
+trained_pop, pop_fitnesses = train(env=env,                             # Gym-style environment
+                                   env_name=INIT_HP['ENV_NAME'],        # Environment name
+                                   dataset=dataset,                     # Offline dataset
+                                   algo=INIT_HP['ALGO'],                # Algorithm
+                                   pop=agent_pop,                       # Population of agents
+                                   memory=memory,                       # Replay buffer
+                                   swap_channels=False,                 # Swap image channel from last to first
+                                   n_episodes=INIT_HP['EPISODES'],      # Max number of training episodes
+                                   evo_epochs=INIT_HP['EVO_EPOCHS'],    # Evolution frequency
+                                   evo_loop=1,                          # Number of evaluation episodes per agent
+                                   target=INIT_HP['TARGET_SCORE'],      # Target score for early stopping
+                                   tournament=tournament,               # Tournament selection object
+                                   mutation=mutations,                  # Mutations object
+                                   wb=INIT_HP['WANDB'],                 # Weights and Biases tracking
+                                   device=torch.device("cuda"))
+```
+
+### Custom Offline Training Loop
+Alternatively, use a custom training loop. Combining all of the above:
+
+```python
+from agilerl.utils.utils import initialPopulation
+from agilerl.components.replay_buffer import ReplayBuffer
+from agilerl.hpo.tournament import TournamentSelection
+from agilerl.hpo.mutation import Mutations
+import gymnasium as gym
+import h5py
+import numpy as np
+import torch
+
+NET_CONFIG = {
+                'arch': 'mlp',       # Network architecture
+                'h_size': [32, 32],  # Actor hidden size
+             }
+
+INIT_HP = {
+            'DOUBLE': True,         # Use double Q-learning
+            'BATCH_SIZE': 128,      # Batch size
+            'LR': 1e-3,             # Learning rate
+            'GAMMA': 0.99,          # Discount factor
+            'LEARN_STEP': 1,        # Learning frequency
+            'TAU': 1e-3,            # For soft update of target network parameters
+            'CHANNELS_LAST': False  # Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+          }
+
+pop = initialPopulation(algo='CQN',             # Algorithm
+                        state_dim=(4,),         # State dimension
+                        action_dim=2,           # Action dimension
+                        one_hot=False,          # One-hot encoding
+                        net_config=NET_CONFIG,  # Network configuration
+                        INIT_HP=INIT_HP,        # Initial hyperparameters
+                        population_size=6,      # Population size
+                        device=torch.device("cuda"))
+
+field_names = ["state", "action", "reward", "next_state", "done"]
+memory = ReplayBuffer(action_dim=2,             # Number of agent actions
+                      memory_size=10000,        # Max replay buffer size
+                      field_names=field_names,  # Field names to store in memory
+                      device=torch.device("cuda"))
+
+tournament = TournamentSelection(tournament_size=2, # Tournament selection size
+                                 elitism=True,      # Elitism in tournament selection
+                                 population_size=6, # Population size
+                                 evo_step=1)        # Evaluate using last N fitness scores
+
+mutations = Mutations(algo='CQN',                           # Algorithm
+                      no_mutation=0.4,                      # No mutation
+                      architecture=0.2,                     # Architecture mutation
+                      new_layer_prob=0.2,                   # New layer mutation
+                      parameters=0.2,                       # Network parameters mutation
+                      activation=0,                         # Activation layer mutation
+                      rl_hp=0.2,                            # Learning HP mutation
+                      rl_hp_selection=['lr', 'batch_size'], # Learning HPs to choose from
+                      mutation_sd=0.1,                      # Mutation strength
+                      arch=NET_CONFIG['arch'],              # Network architecture
+                      rand_seed=1,                          # Random seed
+                      device=torch.device("cuda"))
+
+max_episodes = 1000 # Max training episodes
+max_steps = 500     # Max steps per episode
+
+evo_epochs = 5      # Evolution frequency
+evo_loop = 1        # Number of evaluation episodes
+
+env = gym.make('CartPole-v1')   # Create environment
+
+dataset = h5py.File('data/cartpole/cartpole_random_v1.1.0.h5', 'r')  # Load dataset
+
+# Save transitions to replay buffer
+dataset_length = dataset['rewards'].shape[0]
+for i in range(dataset_length-1):
+    state = dataset['observations'][i]
+    next_state = dataset['observations'][i+1]
+    if swap_channels:
+        state = np.moveaxis(state, [3], [1])
+        next_state = np.moveaxis(next_state, [3], [1])
+    action = dataset['actions'][i]
+    reward = dataset['rewards'][i]
+    done = bool(dataset['terminals'][i])
+    memory.save2memory(state, action, reward, next_state, done)
+
+# TRAINING LOOP
+for idx_epi in range(max_episodes):
+    for agent in pop:   # Loop through population
+        for idx_step in range(max_steps):
+            experiences = memory.sample(agent.batch_size)   # Sample replay buffer
+            # Learn according to agent's RL algorithm
+            agent.learn(experiences)
+
+    # Now evolve population if necessary
+    if (idx_epi+1) % evo_epochs == 0:
+        
+        # Evaluate population
+        fitnesses = [agent.test(env, swap_channels=False, max_steps=max_steps, loop=evo_loop) for agent in pop]
+
         print(f'Episode {idx_epi+1}/{max_episodes}')
         print(f'Fitnesses: {["%.2f"%fitness for fitness in fitnesses]}')
         print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:]) for agent in pop]}')
 
         # Tournament selection and population mutation
         elite, pop = tournament.select(pop)
         pop = mutations.mutation(pop)
```

#### html2text {}

```diff
@@ -1,19 +1,24 @@
-Metadata-Version: 2.1 Name: agilerl Version: 0.1.5 Summary: AgileRL is a deep
+Metadata-Version: 2.1 Name: agilerl Version: 0.1.6 Summary: AgileRL is a deep
 reinforcement learning library focused on improving RL development through
 RLOps. License: Apache 2.0 Author: Nick Ustaran-Anderegg Author-email:
 dev@agilerl.com Requires-Python: >=3.8,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: fastrand (>=1.3.0,<2.0.0)
-Requires-Dist: gymnasium (>=0.27.1,<0.28.0) Requires-Dist: matplotlib
-(>=3.4.3,<4.0.0) Requires-Dist: numpy (>=1.22.4,<2.0.0) Requires-Dist: torch
-(>=1.13.1,<2.0.0) Requires-Dist: tqdm (>=4.62.2,<5.0.0) Requires-Dist: wandb
-(>=0.13.1,<0.14.0) Description-Content-Type: text/markdown # AgileRL
+Programming Language :: Python :: 3.11 Requires-Dist: accelerate
+(>=0.18.0,<0.19.0) Requires-Dist: fastrand (>=1.3.0,<2.0.0) Requires-Dist:
+flatten_dict (>=0.4.2,<0.5.0) Requires-Dist: gymnasium (>=0.26.3,<0.27.0)
+Requires-Dist: h5py (>=3.8.0,<4.0.0) Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
+Requires-Dist: matplotlib (>=3.4.3,<4.0.0) Requires-Dist: numpy
+(>=1.24.2,<2.0.0) Requires-Dist: omegaconf (>=2.3.0,<3.0.0) Requires-Dist:
+redis (>=4.4.4,<5.0.0) Requires-Dist: termcolor (>=1.1.0,<2.0.0) Requires-Dist:
+torch (>=1.13.1,<2.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist:
+transformers (>=4.23.1,<5.0.0) Requires-Dist: wandb (>=0.13.10,<0.14.0)
+Description-Content-Type: text/markdown # AgileRL
  [https://user-images.githubusercontent.com/47857277/222710068-e09a4e3c-368c-
                           458a-9e01-b68674806887.png]
                       Reinforcement learning streamlined.
  Easier and faster reinforcement learning with RLOps. Visit our website. View
                                 documentation.
                     Join the Discord_Server to collaborate.
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
@@ -37,16 +42,18 @@
                           419f-b019-0be4ddf1ed4a.gif]
        AgileRL offers 10x faster hyperparameter optimization than SOTA.
  Global steps is the sum of every step taken by any agent in the environment,
     including across an entire population, during the entire hyperparameter
                              optimization process.
 ## Table of Contents * [Benchmarks](#benchmarks) * [Get Started](#get-started)
 * [Algorithms implemented](#algorithms-implemented-more-coming-soon) * [Train
-an agent on a Gym environment](#train-an-agent-on-a-gym-environment) + [Custom
-Training Loop](#custom-training-loop) * [Train an agent on a language
+an agent on a Gym environment (Online)](#train-an-agent-on-a-gym-environment-
+online) + [Custom Online Training Loop](#custom-online-training-loop) * [Train
+an agent on data (Offline)](#train-an-agent-on-data-offline) + [Custom Offline
+Training Loop](#custom-offline-training-loop) * [Train an agent on a language
 environment (RLHF)](#train-an-agent-on-a-language-environment-rlhf) ##
 Benchmarks Reinforcement learning algorithms and libraries are usually
 benchmarked once the optimal hyperparameters for training are known, but it
 often takes hundreds or thousands of experiments to discover these. This is
 unrealistic and does not reflect the true, total time taken for training. What
 if we could remove the need to conduct all these prior experiments? In the
 charts below, a single AgileRL run, which automatically tunes hyperparameters,
@@ -60,45 +67,46 @@
 popular reinforcement learning training frameworks combined with Optuna. Remove
          the need for multiple training runs and save yourself hours.
 ## Get Started Install as a package with pip: ```bash pip install agilerl ```
 Or install in development mode: (Recommended due to nascent nature of this
 library) ```bash git clone https://github.com/AgileRL/AgileRL.git && cd AgileRL
 pip install -r requirements.txt ``` If using ILQL on Wordle, download and unzip
 data.zip here. Demo: ```bash python demo.py ``` ## Algorithms implemented (more
-coming soon!) * DQN * DDPG * ILQL ## Train an agent on a Gym environment Before
-starting training, there are some meta-hyperparameters and settings that must
-be set. These are defined in INIT_HP, for general parameters, and
-MUTATION_PARAMS, which define the evolutionary probabilities, and NET_CONFIG,
-which defines the network architecture. For example: ```python INIT_HP =
-{ 'ENV_NAME': 'LunarLander-v2', # Gym environment name 'ALGO': 'DQN', #
-Algorithm 'CHANNELS_LAST': False, # Swap image channels dimension from last to
-first [H, W, C] -> [C, H, W] 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, #
-Learning rate 'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., #
-Early training stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount
-factor 'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, #
-Learning frequency 'TAU': 1e-3, # For soft update of target parameters
-'TOURN_SIZE': 2, # Tournament size 'ELITISM': True, # Elitism in tournament
-selection 'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution
-frequency 'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True #
-Log with Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative
-probabilities 'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture
-mutation 'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network
-parameters mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2,
-# Learning HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs
-to choose from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed
-} ``` ```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
-[32, 32], # Actor hidden size } ``` First, use utils.initialPopulation to
-create a list of agents - our population that will evolve and mutate to the
-optimal hyperparameters. ```python from agilerl.utils import makeVectEnvs,
-initialPopulation import torch device = torch.device("cuda" if
-torch.cuda.is_available() else "cpu") env = makeVectEnvs(env_name=INIT_HP
-['ENV_NAME'], num_envs=16) try: state_dim = env.single_observation_space.n #
-Discrete observation space one_hot = True # Requires one-hot encoding except:
-state_dim = env.single_observation_space.shape # Continuous observation space
-one_hot = False # Does not require one-hot encoding try: action_dim =
+coming soon!) * DQN * DDPG * CQL * ILQL ## Train an agent on a Gym environment
+(Online) Before starting training, there are some meta-hyperparameters and
+settings that must be set. These are defined in INIT_HP, for general
+parameters, and MUTATION_PARAMS, which define the evolutionary probabilities,
+and NET_CONFIG, which defines the network architecture. For example: ```python
+INIT_HP = { 'ENV_NAME': 'LunarLander-v2', # Gym environment name 'ALGO': 'DQN',
+# Algorithm 'DOUBLE': True, # Use double Q-learning 'CHANNELS_LAST': False, #
+Swap image channels dimension from last to first [H, W, C] -> [C, H, W]
+'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, # Learning rate 'EPISODES': 2000, #
+Max no. episodes 'TARGET_SCORE': 200., # Early training stop at avg score of
+last 100 episodes 'GAMMA': 0.99, # Discount factor 'MEMORY_SIZE': 10000, # Max
+memory buffer size 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For
+soft update of target parameters 'TOURN_SIZE': 2, # Tournament size 'ELITISM':
+True, # Elitism in tournament selection 'POP_SIZE': 6, # Population size
+'EVO_EPOCHS': 20, # Evolution frequency 'POLICY_FREQ': 2, # Policy network
+update frequency 'WANDB': True # Log with Weights and Biases } ``` ```python
+MUTATION_PARAMS = { # Relative probabilities 'NO_MUT': 0.4, # No mutation
+'ARCH_MUT': 0.2, # Architecture mutation 'NEW_LAYER': 0.2, # New layer mutation
+'PARAMS_MUT': 0.2, # Network parameters mutation 'ACT_MUT': 0, # Activation
+layer mutation 'RL_HP_MUT': 0.2, # Learning HP mutation 'RL_HP_SELECTION':
+['lr', 'batch_size'], # Learning HPs to choose from 'MUT_SD': 0.1, # Mutation
+strength 'RAND_SEED': 1, # Random seed } ``` ```python NET_CONFIG = { 'arch':
+'mlp', # Network architecture 'h_size': [32, 32], # Actor hidden size } ```
+First, use utils.utils.initialPopulation to create a list of agents - our
+population that will evolve and mutate to the optimal hyperparameters.
+```python from agilerl.utils.utils import makeVectEnvs, initialPopulation
+import torch device = torch.device("cuda" if torch.cuda.is_available() else
+"cpu") env = makeVectEnvs(env_name=INIT_HP['ENV_NAME'], num_envs=16) try:
+state_dim = env.single_observation_space.n # Discrete observation space one_hot
+= True # Requires one-hot encoding except: state_dim =
+env.single_observation_space.shape # Continuous observation space one_hot =
+False # Does not require one-hot encoding try: action_dim =
 env.single_action_space.n # Discrete action space except: action_dim =
 env.single_action_space.shape[0] # Continuous action space if INIT_HP
 ['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1])
 agent_pop = initialPopulation(algo=INIT_HP['ALGO'], # Algorithm
 state_dim=state_dim, # State dimension action_dim=action_dim, # Action
 dimension one_hot=one_hot, # One-hot encoding net_config=NET_CONFIG, # Network
 configuration INIT_HP=INIT_HP, # Initial hyperparameters
@@ -122,44 +130,45 @@
 parameters=MUTATION_PARAMS['PARAMS_MUT'], # Network parameters mutation
 activation=MUTATION_PARAMS['ACT_MUT'], # Activation layer mutation
 rl_hp=MUTATION_PARAMS['RL_HP_MUT'], # Learning HP mutation
 rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], # Learning HPs to choose
 from mutation_sd=MUTATION_PARAMS['MUT_SD'], # Mutation strength arch=NET_CONFIG
 ['arch'], # Network architecture rand_seed=MUTATION_PARAMS['RAND_SEED'], #
 Random seed device=torch.device("cuda")) ``` The easiest training loop
-implementation is to use our training.train() function. It requires the agent
-have functions getAction() and learn(). ```python from agilerl.training.train
-import train trained_pop, pop_fitnesses = train(env=env, # Gym-style
-environment env_name=INIT_HP['ENV_NAME'], # Environment name algo=INIT_HP
-['ALGO'], # Algorithm pop=agent_pop, # Population of agents memory=memory, #
-Replay buffer swap_channels=False, # Swap image channel from last to first
-n_episodes=INIT_HP['EPISODES'], # Max number of training episodes
+implementation is to use our training.train.train() function. It requires the
+agent have functions getAction() and learn(). ```python from
+agilerl.training.train import train trained_pop, pop_fitnesses = train(env=env,
+# Gym-style environment env_name=INIT_HP['ENV_NAME'], # Environment name
+algo=INIT_HP['ALGO'], # Algorithm pop=agent_pop, # Population of agents
+memory=memory, # Replay buffer swap_channels=False, # Swap image channel from
+last to first n_episodes=INIT_HP['EPISODES'], # Max number of training episodes
 evo_epochs=INIT_HP['EVO_EPOCHS'], # Evolution frequency evo_loop=1, # Number of
 evaluation episodes per agent target=INIT_HP['TARGET_SCORE'], # Target score
 for early stopping tournament=tournament, # Tournament selection object
 mutation=mutations, # Mutations object wb=INIT_HP['WANDB'], # Weights and
-Biases tracking device=torch.device("cuda")) ``` ### Custom Training Loop
-Alternatively, use a custom training loop. Combining all of the above:
-```python from agilerl.utils import makeVectEnvs, initialPopulation from
+Biases tracking device=torch.device("cuda")) ``` ### Custom Online Training
+Loop Alternatively, use a custom training loop. Combining all of the above:
+```python from agilerl.utils.utils import makeVectEnvs, initialPopulation from
 agilerl.components.replay_buffer import ReplayBuffer from
 agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
 import Mutations import gymnasium as gym import numpy as np import torch
 NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32], #
-Actor hidden size } INIT_HP = { 'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, #
-Learning rate 'GAMMA': 0.99, # Discount factor 'LEARN_STEP': 1, # Learning
-frequency 'TAU': 1e-3, # For soft update of target network parameters
-'CHANNELS_LAST': False # Swap image channels dimension from last to first [H,
-W, C] -> [C, H, W] } pop = initialPopulation(algo='DQN', # Algorithm state_dim=
-(8,), # State dimension action_dim=4, # Action dimension one_hot=False, # One-
-hot encoding net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, #
-Initial hyperparameters population_size=6, # Population size
-device=torch.device("cuda")) field_names = ["state", "action", "reward",
-"next_state", "done"] memory = ReplayBuffer(action_dim=4, # Number of agent
-actions memory_size=10000, # Max replay buffer size field_names=field_names, #
-Field names to store in memory device=torch.device("cuda")) tournament =
+Actor hidden size } INIT_HP = { 'DOUBLE': True, # Use double Q-learning
+'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, # Learning rate 'GAMMA': 0.99, #
+Discount factor 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For soft
+update of target network parameters 'CHANNELS_LAST': False # Swap image
+channels dimension from last to first [H, W, C] -> [C, H, W] } pop =
+initialPopulation(algo='DQN', # Algorithm state_dim=(8,), # State dimension
+action_dim=4, # Action dimension one_hot=False, # One-hot encoding
+net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
+hyperparameters population_size=6, # Population size device=torch.device
+("cuda")) field_names = ["state", "action", "reward", "next_state", "done"]
+memory = ReplayBuffer(action_dim=4, # Number of agent actions
+memory_size=10000, # Max replay buffer size field_names=field_names, # Field
+names to store in memory device=torch.device("cuda")) tournament =
 TournamentSelection(tournament_size=2, # Tournament selection size
 elitism=True, # Elitism in tournament selection population_size=6, # Population
 size evo_step=1) # Evaluate using last N fitness scores mutations = Mutations
 (algo='DQN', # Algorithm no_mutation=0.4, # No mutation architecture=0.2, #
 Architecture mutation new_layer_prob=0.2, # New layer mutation parameters=0.2,
 # Network parameters mutation activation=0, # Activation layer mutation
 rl_hp=0.2, # Learning HP mutation rl_hp_selection=['lr', 'batch_size'], #
@@ -184,14 +193,140 @@
 Now evolve population if necessary if (idx_epi+1) % evo_epochs == 0: # Evaluate
 population fitnesses = [agent.test(env, swap_channels=False,
 max_steps=max_steps, loop=evo_loop) for agent in pop] print(f'Episode
 {idx_epi+1}/{max_episodes}') print(f'Fitnesses: {["%.2f"%fitness for fitness in
 fitnesses]}') print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:])
 for agent in pop]}') # Tournament selection and population mutation elite, pop
 = tournament.select(pop) pop = mutations.mutation(pop) ``` ## Train an agent on
+data (Offline) Like with online RL, above, there are some meta-hyperparameters
+and settings that must be set before starting training. These are defined in
+INIT_HP, for general parameters, and MUTATION_PARAMS, which define the
+evolutionary probabilities, and NET_CONFIG, which defines the network
+architecture. For example: ```python INIT_HP = { 'ENV_NAME': 'CartPole-v1', #
+Gym environment name 'DATASET': 'data/cartpole/cartpole_random_v1.1.0.h5', #
+Offline RL dataset 'ALGO': 'CQN', # Algorithm 'DOUBLE': True, # Use double Q-
+learning # Swap image channels dimension from last to first [H, W, C] -> [C, H,
+W] 'CHANNELS_LAST': False, 'BATCH_SIZE': 256, # Batch size 'LR': 1e-3, #
+Learning rate 'EPISODES': 2000, # Max no. episodes 'TARGET_SCORE': 200., #
+Early training stop at avg score of last 100 episodes 'GAMMA': 0.99, # Discount
+factor 'MEMORY_SIZE': 10000, # Max memory buffer size 'LEARN_STEP': 1, #
+Learning frequency 'TAU': 1e-3, # For soft update of target parameters
+'TOURN_SIZE': 2, # Tournament size 'ELITISM': True, # Elitism in tournament
+selection 'POP_SIZE': 6, # Population size 'EVO_EPOCHS': 20, # Evolution
+frequency 'POLICY_FREQ': 2, # Policy network update frequency 'WANDB': True #
+Log with Weights and Biases } ``` ```python MUTATION_PARAMS = { # Relative
+probabilities 'NO_MUT': 0.4, # No mutation 'ARCH_MUT': 0.2, # Architecture
+mutation 'NEW_LAYER': 0.2, # New layer mutation 'PARAMS_MUT': 0.2, # Network
+parameters mutation 'ACT_MUT': 0, # Activation layer mutation 'RL_HP_MUT': 0.2,
+# Learning HP mutation 'RL_HP_SELECTION': ['lr', 'batch_size'], # Learning HPs
+to choose from 'MUT_SD': 0.1, # Mutation strength 'RAND_SEED': 1, # Random seed
+} ``` ```python NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size':
+[32, 32], # Actor hidden size } ``` First, use utils.utils.initialPopulation to
+create a list of agents - our population that will evolve and mutate to the
+optimal hyperparameters. ```python from agilerl.utils.utils import
+initialPopulation import torch import h5py import gymnasium as gym device =
+torch.device("cuda" if torch.cuda.is_available() else "cpu") env = gym.make
+(INIT_HP['ENV_NAME']) try: state_dim = env.observation_space.n # Discrete
+observation space one_hot = True # Requires one-hot encoding except Exception:
+state_dim = env.observation_space.shape # Continuous observation space one_hot
+= False # Does not require one-hot encoding try: action_dim =
+env.action_space.n # Discrete action space except Exception: action_dim =
+env.action_space.shape[0] # Continuous action space if INIT_HP
+['CHANNELS_LAST']: state_dim = (state_dim[2], state_dim[0], state_dim[1])
+dataset = h5py.File(INIT_HP['DATASET'], 'r') agent_pop = initialPopulation
+(algo=INIT_HP['ALGO'], # Algorithm state_dim=state_dim, # State dimension
+action_dim=action_dim, # Action dimension one_hot=one_hot, # One-hot encoding
+net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
+hyperparameters population_size=INIT_HP['POP_SIZE'], # Population size
+device=torch.device("cuda")) ``` Next, create the tournament, mutations and
+experience replay buffer objects that allow agents to share memory and
+efficiently perform evolutionary HPO. ```python from
+agilerl.components.replay_buffer import ReplayBuffer from
+agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
+import Mutations import torch field_names = ["state", "action", "reward",
+"next_state", "done"] memory = ReplayBuffer(action_dim=action_dim, # Number of
+agent actions memory_size=INIT_HP['MEMORY_SIZE'], # Max replay buffer size
+field_names=field_names, # Field names to store in memory device=torch.device
+("cuda")) tournament = TournamentSelection(tournament_size=INIT_HP
+['TOURN_SIZE'], # Tournament selection size elitism=INIT_HP['ELITISM'], #
+Elitism in tournament selection population_size=INIT_HP['POP_SIZE'], #
+Population size evo_step=INIT_HP['EVO_EPOCHS']) # Evaluate using last N fitness
+scores mutations = Mutations(algo=INIT_HP['ALGO'], # Algorithm
+no_mutation=MUTATION_PARAMS['NO_MUT'], # No mutation
+architecture=MUTATION_PARAMS['ARCH_MUT'], # Architecture mutation
+new_layer_prob=MUTATION_PARAMS['NEW_LAYER'], # New layer mutation
+parameters=MUTATION_PARAMS['PARAMS_MUT'], # Network parameters mutation
+activation=MUTATION_PARAMS['ACT_MUT'], # Activation layer mutation
+rl_hp=MUTATION_PARAMS['RL_HP_MUT'], # Learning HP mutation
+rl_hp_selection=MUTATION_PARAMS['RL_HP_SELECTION'], # Learning HPs to choose
+from mutation_sd=MUTATION_PARAMS['MUT_SD'], # Mutation strength arch=NET_CONFIG
+['arch'], # Network architecture rand_seed=MUTATION_PARAMS['RAND_SEED'], #
+Random seed device=torch.device("cuda")) ``` The easiest training loop
+implementation is to use our training.train_offline.train() function. It
+requires the agent have functions getAction() and learn(). ```python from
+agilerl.training.train_offline import train trained_pop, pop_fitnesses = train
+(env=env, # Gym-style environment env_name=INIT_HP['ENV_NAME'], # Environment
+name dataset=dataset, # Offline dataset algo=INIT_HP['ALGO'], # Algorithm
+pop=agent_pop, # Population of agents memory=memory, # Replay buffer
+swap_channels=False, # Swap image channel from last to first n_episodes=INIT_HP
+['EPISODES'], # Max number of training episodes evo_epochs=INIT_HP
+['EVO_EPOCHS'], # Evolution frequency evo_loop=1, # Number of evaluation
+episodes per agent target=INIT_HP['TARGET_SCORE'], # Target score for early
+stopping tournament=tournament, # Tournament selection object
+mutation=mutations, # Mutations object wb=INIT_HP['WANDB'], # Weights and
+Biases tracking device=torch.device("cuda")) ``` ### Custom Offline Training
+Loop Alternatively, use a custom training loop. Combining all of the above:
+```python from agilerl.utils.utils import initialPopulation from
+agilerl.components.replay_buffer import ReplayBuffer from
+agilerl.hpo.tournament import TournamentSelection from agilerl.hpo.mutation
+import Mutations import gymnasium as gym import h5py import numpy as np import
+torch NET_CONFIG = { 'arch': 'mlp', # Network architecture 'h_size': [32, 32],
+# Actor hidden size } INIT_HP = { 'DOUBLE': True, # Use double Q-learning
+'BATCH_SIZE': 128, # Batch size 'LR': 1e-3, # Learning rate 'GAMMA': 0.99, #
+Discount factor 'LEARN_STEP': 1, # Learning frequency 'TAU': 1e-3, # For soft
+update of target network parameters 'CHANNELS_LAST': False # Swap image
+channels dimension from last to first [H, W, C] -> [C, H, W] } pop =
+initialPopulation(algo='CQN', # Algorithm state_dim=(4,), # State dimension
+action_dim=2, # Action dimension one_hot=False, # One-hot encoding
+net_config=NET_CONFIG, # Network configuration INIT_HP=INIT_HP, # Initial
+hyperparameters population_size=6, # Population size device=torch.device
+("cuda")) field_names = ["state", "action", "reward", "next_state", "done"]
+memory = ReplayBuffer(action_dim=2, # Number of agent actions
+memory_size=10000, # Max replay buffer size field_names=field_names, # Field
+names to store in memory device=torch.device("cuda")) tournament =
+TournamentSelection(tournament_size=2, # Tournament selection size
+elitism=True, # Elitism in tournament selection population_size=6, # Population
+size evo_step=1) # Evaluate using last N fitness scores mutations = Mutations
+(algo='CQN', # Algorithm no_mutation=0.4, # No mutation architecture=0.2, #
+Architecture mutation new_layer_prob=0.2, # New layer mutation parameters=0.2,
+# Network parameters mutation activation=0, # Activation layer mutation
+rl_hp=0.2, # Learning HP mutation rl_hp_selection=['lr', 'batch_size'], #
+Learning HPs to choose from mutation_sd=0.1, # Mutation strength
+arch=NET_CONFIG['arch'], # Network architecture rand_seed=1, # Random seed
+device=torch.device("cuda")) max_episodes = 1000 # Max training episodes
+max_steps = 500 # Max steps per episode evo_epochs = 5 # Evolution frequency
+evo_loop = 1 # Number of evaluation episodes env = gym.make('CartPole-v1') #
+Create environment dataset = h5py.File('data/cartpole/
+cartpole_random_v1.1.0.h5', 'r') # Load dataset # Save transitions to replay
+buffer dataset_length = dataset['rewards'].shape[0] for i in range
+(dataset_length-1): state = dataset['observations'][i] next_state = dataset
+['observations'][i+1] if swap_channels: state = np.moveaxis(state, [3], [1])
+next_state = np.moveaxis(next_state, [3], [1]) action = dataset['actions'][i]
+reward = dataset['rewards'][i] done = bool(dataset['terminals'][i])
+memory.save2memory(state, action, reward, next_state, done) # TRAINING LOOP for
+idx_epi in range(max_episodes): for agent in pop: # Loop through population for
+idx_step in range(max_steps): experiences = memory.sample(agent.batch_size) #
+Sample replay buffer # Learn according to agent's RL algorithm agent.learn
+(experiences) # Now evolve population if necessary if (idx_epi+1) % evo_epochs
+== 0: # Evaluate population fitnesses = [agent.test(env, swap_channels=False,
+max_steps=max_steps, loop=evo_loop) for agent in pop] print(f'Episode
+{idx_epi+1}/{max_episodes}') print(f'Fitnesses: {["%.2f"%fitness for fitness in
+fitnesses]}') print(f'100 fitness avgs: {["%.2f"%np.mean(agent.fitness[-100:])
+for agent in pop]}') # Tournament selection and population mutation elite, pop
+= tournament.select(pop) pop = mutations.mutation(pop) ``` ## Train an agent on
 a language environment (RLHF) We implement RLHF on Wordle, and use ILQL to
 finetune our model. To create your own language environment, see https://
 github.com/Sea-Snell/Implicit-Language-Q-Learning. The EvolvableGPT class
 allows us to combine LLMs and transformer architectures with evolvable HPO,
 which can massively reduce the time taken to finetune these expensive models.
 Due to the vast number of parameters and settings involved in training a Large
 Language Model (LLM) on human feedback, these are defined in configs. In order
```

