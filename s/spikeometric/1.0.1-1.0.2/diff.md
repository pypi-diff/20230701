# Comparing `tmp/spikeometric-1.0.1.tar.gz` & `tmp/spikeometric-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikeometric-1.0.1.tar", max compression
+gzip compressed data, was "spikeometric-1.0.2.tar", max compression
```

## Comparing `spikeometric-1.0.1.tar` & `spikeometric-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-02-23 21:23:20.295275 spikeometric-1.0.1/LICENSE
--rw-r--r--   0        0        0     1359 2023-02-23 21:23:20.295275 spikeometric-1.0.1/README.md
--rw-r--r--   0        0        0      917 2023-04-20 10:08:25.569925 spikeometric-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      325 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/__init__.py
--rw-r--r--   0        0        0     4251 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/connectivity_dataset.py
--rw-r--r--   0        0        0     1558 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/connectivity_generator.py
--rw-r--r--   0        0        0     1428 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/mexican_hat_connectivity_generator.py
--rw-r--r--   0        0        0     3426 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/normal_connectivity_generator.py
--rw-r--r--   0        0        0     2069 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/datasets/uniform_connectivity_generator.py
--rw-r--r--   0        0        0      534 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/__init__.py
--rw-r--r--   0        0        0    15433 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/base_model.py
--rw-r--r--   0        0        0    12420 2023-04-20 09:56:38.368186 spikeometric-1.0.1/spikeometric/models/bernoulli_glm_model.py
--rw-r--r--   0        0        0     6830 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/poisson_glm_model.py
--rw-r--r--   0        0        0     6928 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/rectified_lnp_model.py
--rw-r--r--   0        0        0     6522 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/rectified_sa_model.py
--rw-r--r--   0        0        0     7782 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/sa_model.py
--rw-r--r--   0        0        0     6353 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/models/threshold_sa_model.py
--rw-r--r--   0        0        0      192 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/stimulus/__init__.py
--rw-r--r--   0        0        0     3052 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/stimulus/poisson_stimulus.py
--rw-r--r--   0        0        0     2205 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/stimulus/regular_stimulus.py
--rw-r--r--   0        0        0     2420 2023-02-23 21:23:20.355275 spikeometric-1.0.1/spikeometric/stimulus/sin_stimulus.py
--rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 spikeometric-1.0.1/setup.py
--rw-r--r--   0        0        0     2407 1970-01-01 00:00:00.000000 spikeometric-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-23 21:23:20.295275 spikeometric-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1359 2023-02-23 21:23:20.295275 spikeometric-1.0.2/README.md
+-rw-r--r--   0        0        0      917 2023-07-01 14:12:24.268477 spikeometric-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-02-23 21:23:20.355275 spikeometric-1.0.2/spikeometric/datasets/__init__.py
+-rw-r--r--   0        0        0     3170 2023-07-01 14:11:55.448479 spikeometric-1.0.2/spikeometric/datasets/connectivity_dataset.py
+-rw-r--r--   0        0        0     1095 2023-07-01 13:30:18.808721 spikeometric-1.0.2/spikeometric/datasets/connectivity_generator.py
+-rw-r--r--   0        0        0     1428 2023-02-23 21:23:20.355275 spikeometric-1.0.2/spikeometric/datasets/mexican_hat_connectivity_generator.py
+-rw-r--r--   0        0        0     3317 2023-07-01 13:30:18.808721 spikeometric-1.0.2/spikeometric/datasets/normal_connectivity_generator.py
+-rw-r--r--   0        0        0     2069 2023-02-23 21:23:20.355275 spikeometric-1.0.2/spikeometric/datasets/uniform_connectivity_generator.py
+-rw-r--r--   0        0        0      534 2023-02-23 21:23:20.355275 spikeometric-1.0.2/spikeometric/models/__init__.py
+-rw-r--r--   0        0        0    15609 2023-07-01 13:30:18.808721 spikeometric-1.0.2/spikeometric/models/base_model.py
+-rw-r--r--   0        0        0    12250 2023-07-01 13:30:18.808721 spikeometric-1.0.2/spikeometric/models/bernoulli_glm_model.py
+-rw-r--r--   0        0        0     6660 2023-07-01 13:30:18.808721 spikeometric-1.0.2/spikeometric/models/poisson_glm_model.py
+-rw-r--r--   0        0        0     6758 2023-07-01 13:30:18.808721 spikeometric-1.0.2/spikeometric/models/rectified_lnp_model.py
+-rw-r--r--   0        0        0     6368 2023-07-01 13:30:18.808721 spikeometric-1.0.2/spikeometric/models/rectified_sa_model.py
+-rw-r--r--   0        0        0     8445 2023-07-01 13:30:18.808721 spikeometric-1.0.2/spikeometric/models/sa_model.py
+-rw-r--r--   0        0        0     6195 2023-07-01 13:30:18.818721 spikeometric-1.0.2/spikeometric/models/threshold_sa_model.py
+-rw-r--r--   0        0        0      318 2023-07-01 13:30:18.818721 spikeometric-1.0.2/spikeometric/stimulus/__init__.py
+-rw-r--r--   0        0        0     1728 2023-07-01 13:30:18.818721 spikeometric-1.0.2/spikeometric/stimulus/base_stimulus.py
+-rw-r--r--   0        0        0     3753 2023-07-01 13:30:18.818721 spikeometric-1.0.2/spikeometric/stimulus/loaded_stimulus.py
+-rw-r--r--   0        0        0     4677 2023-07-01 13:30:18.818721 spikeometric-1.0.2/spikeometric/stimulus/poisson_stimulus.py
+-rw-r--r--   0        0        0     3496 2023-07-01 13:30:18.818721 spikeometric-1.0.2/spikeometric/stimulus/regular_stimulus.py
+-rw-r--r--   0        0        0     3769 2023-07-01 13:30:18.818721 spikeometric-1.0.2/spikeometric/stimulus/sin_stimulus.py
+-rw-r--r--   0        0        0     2349 1970-01-01 00:00:00.000000 spikeometric-1.0.2/setup.py
+-rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 spikeometric-1.0.2/PKG-INFO
```

### Comparing `spikeometric-1.0.1/LICENSE` & `spikeometric-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.1/README.md` & `spikeometric-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.1/pyproject.toml` & `spikeometric-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "spikeometric"
-version = "1.0.1"
+version = "1.0.2"
 description = "Spikeometric is a Pytorch Geometric based framework for simulating Spiking Neural Networks using Linear Non-linear Cascade models"
 authors = ["Jakob Sønstebø <jakobls16@gmail.com>"]
 readme = "README.md"
 license = "GNU General Public License v3.0"
 documentation = "https://spikeometric.readthedocs.io/en/latest/"
 repository = "https://github.com/bioAI-Oslo/Spikeometric"
 packages = [{include = "spikeometric"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = ">=3.8, <3.12"
 numpy = "^1.21.4"
 matplotlib = "^3.5.0"
 tqdm = "^4.62.3"
 scipy = "^1.7.3"
-seaborn = "^0.11.2"
+seaborn = "^0.12.2"
 networkx = "^3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pytest-lazy-fixture = "^0.6.3"
 sphinx = "^4.3.2"
```

### Comparing `spikeometric-1.0.1/spikeometric/datasets/connectivity_generator.py` & `spikeometric-1.0.2/spikeometric/datasets/connectivity_generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,30 +2,25 @@
 from torch_geometric.data import Data
 from torch_geometric.utils import add_remaining_self_loops
 from pathlib import Path
 import torch
 
 class ConnectivityGenerator(object):
     """Base class for generating connectivity matrices W0"""
-    def generate(self, n_examples: int, add_self_loops: bool = False, stimulus_masks=[]) -> list[Data]:
+    def generate(self, n_examples: int) -> List[Data]:
         """Generates a set of connectivity matrices W0 and returns them as a list of torch_geometric.data.Data objects"""
         w0_list = []
         for i in range(n_examples):
             W0_square = self.generate_W0()
             edge_index = W0_square.nonzero().t()
-            if add_self_loops:
-                edge_index, _ = add_remaining_self_loops(edge_index, num_nodes=self.n_neurons)
             W0 = W0_square[edge_index[0], edge_index[1]]
-            data = Data(edge_index=edge_index, W0=W0, num_nodes=self.n_neurons, stimulus_mask=stimulus_masks[i] if len(stimulus_masks) > 0 else None)
+            data = Data(edge_index=edge_index, W0=W0, num_nodes=self.n_neurons)
             w0_list.append(data)
         return w0_list
     
-    def save(self, n_networks, path, stimulus_masks=[]):
+    def save(self, n_networks, path):
         """Saves n_networks square connectivity matrices W0 to the specified path"""
         path = Path(path)
         path.mkdir(parents=True, exist_ok=True)
         for i in range(n_networks):
             w0 = self.generate_W0()
-            torch.save(w0, path / f"{i}.pt")
-        if len(stimulus_masks) > 0:
-            stimulus_masks = [mask.unsqueeze(1).T for mask in stimulus_masks]
-            torch.save(torch.cat(stimulus_masks, dim=0), path / "stimulus_masks.pt")
+            torch.save(w0, path / f"{i}.pt")
```

### Comparing `spikeometric-1.0.1/spikeometric/datasets/mexican_hat_connectivity_generator.py` & `spikeometric-1.0.2/spikeometric/datasets/mexican_hat_connectivity_generator.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.1/spikeometric/datasets/normal_connectivity_generator.py` & `spikeometric-1.0.2/spikeometric/datasets/normal_connectivity_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,21 @@
     Example:
         >>> from spikeometric.datasets import NormalGenerator, ConnectivityDataset
         >>> generator = NormalGenerator(n_neurons=6, mean=0, std=1, sparsity=0.5, glorot=True)
         >>> generator.save(10, "data/w0/6_neurons_10_networks_0_mean_1_std_0.5_sparsity_glorot_0_seed")
         >>> dataset = ConnectivityDataset("data/w0/6_neurons_10_networks_0_mean_1_std_0.5_sparsity_glorot_0_seed")
         >>> data = dataset[0]
         >>> data
-        Data(edge_index=[2, 13], num_nodes=6, W0=[13], stimulus_mask=[6])
+        Data(edge_index=[2, 13], num_nodes=6, W0=[13])
         >>> data.W0
         tensor([ 0.6270,  0.5048,  0.4300, -0.7440, -0.2918, -1.1955, -0.4468,  0.0000,
                  0.0000,  0.0000,  0.0000,  0.0000,  0.0000])
         >>> data.edge_index
         tensor([[0, 0, 1, 3, 3, 4, 5, 0, 1, 2, 3, 4, 5],
                 [2, 4, 3, 1, 5, 5, 4, 0, 1, 2, 3, 4, 5]])
-        >>> data.stimulus_mask
-        tensor([False, False, False, False, False, False])
 
     Parameters:
     ------------
     n_neurons (int):
         The number of neurons in a network (must be even)
     mean (float):
         The mean of the normal distribution from which the weights are drawn
```

### Comparing `spikeometric-1.0.1/spikeometric/datasets/uniform_connectivity_generator.py` & `spikeometric-1.0.2/spikeometric/datasets/uniform_connectivity_generator.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.1/spikeometric/models/__init__.py` & `spikeometric-1.0.2/spikeometric/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeometric-1.0.1/spikeometric/models/base_model.py` & `spikeometric-1.0.2/spikeometric/models/base_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from torch_geometric.nn import MessagePassing
 from torch_geometric.data import Data
 import torch
 from tqdm import tqdm
-from typing import Union
+from typing import Union, Callable
+from spikeometric.stimulus import BaseStimulus
+from typing import List
 
 class BaseModel(MessagePassing):
     """
     Base class for all spiking neural networks.
     
     Extends the MessagePassing class from torch_geometric by adding stimulus support and
     a forward method that calculates the spikes of the network at time t using the following steps:
@@ -23,15 +25,15 @@
     If the models has any tunable parameters, they can be tuned to match a desired firing rate using the tune method.
     For other target functions, the tune method can be overriden by the child classes.
 
     There are also methods for saving and loading the model.
     """
     def __init__(self):
         super().__init__()
-        self.stimulus = lambda t: 0
+        self.stimulus = lambda t: torch.tensor(0.0)
 
     @property
     def tunable_parameters(self) -> dict:
         """Returns a list of the tunable parameters"""
         return dict(self.named_parameters())
     
     def connectivity_filter(self, W0: torch.Tensor, edge_index: torch.Tensor) -> torch.Tensor:
@@ -111,31 +113,29 @@
         Returns
         -------
         message: torch.Tensor
             The message from the j-th neuron to the i-th neuron [n_edges, 1]
         """
         return torch.sum(state_j*W, dim=1, keepdim=True)
 
-    def stimulus_input(self, t: int, stimulus_mask: torch.Tensor, **kwargs) -> torch.Tensor:
+    def stimulus_input(self, t: int, **kwargs) -> torch.Tensor:
         r"""
         Calculates the stimulus input to the network at time t.
 
         Parameters
         ----------
         t: int
             The current time step
-        stimulus_mask: torch.Tensor[bool]
-            A boolean tensor indicating which neurons are targeted by the stimulus [n_neurons]
         
         Returns
         -------
         stimulus_input: torch.Tensor
             The stimulus input to the network [n_neurons]
         """
-        return self.stimulus_filter(self.stimulus(t), **kwargs) * stimulus_mask
+        return self.stimulus_filter(self.stimulus(t), **kwargs)
 
     def stimulus_filter(self, stimulus: torch.Tensor, **kwargs) -> torch.Tensor:
         r"""
         Filters the stimulus to the network. The default stimulus filter is just the stimulus itself.
 
         Parameters
         ----------
@@ -147,18 +147,18 @@
         Returns
         -------
         stimulus: torch.Tensor
             The filtered stimulus to the network [n_neurons]
         """
         return stimulus
 
-    def add_stimulus(self, stimulus: callable):
+    def add_stimulus(self, stimulus: Callable):
         """Adds a stimulus to the network"""
         if not callable(stimulus):
-            raise TypeError("The stimulus must be a callable function")
+            raise TypeError("The stimulus must be a callable object")
         self.stimulus = stimulus
 
     def forward(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, **kwargs) -> torch.Tensor:
         r"""
         Calculates the new state of the network at time t+1 from the state at time t.
 
         Parameters
@@ -180,68 +180,68 @@
             W=W,
             state=state,
             **kwargs
         )
         rate = self.non_linearity(input)
         return self.emit_spikes(rate)
     
-    def simulate(self, data, n_steps, verbose=True, equilibration_steps=100, **kwargs):
+    def simulate(self, data, n_steps: int, verbose: bool = True, equilibration_steps: int = 100, store_as_dtype: torch.dtype = torch.int, **kwargs):
         r"""
         Simulates the network for n_steps time steps given the connectivity.
         Returns the state of the network at each time step.
 
         Parameters
         -----------
         data: torch_geometric.data.Data
             The data containing the connectivity. 
         n_steps: int
             The number of time steps to simulate
         verbose: bool
             If True, a progress bar is shown
         equilibration: int
             The number of time steps to simulate before the we start recording the state of the network.
+        store_as_dtype: torch.dtype
+            The dtype to store the state of the network as.
 
         Returns
         --------
         x: torch.Tensor[n_neurons, n_steps]
             The state of the network at each time step. The state is a binary tensor where 1 means that the neuron is active.
         """
         # Get the parameters of the network
         n_neurons = data.num_nodes
         edge_index = data.edge_index
         W0 = data.W0
         W, edge_index = self.connectivity_filter(W0, edge_index)
         T = W.shape[1]
 
-        if not hasattr(data, "stimulus_mask"):
-            stimulus_mask = torch.zeros(n_neurons, dtype=torch.bool, device=edge_index.device)
-            data.stimulus_mask = stimulus_mask
-        else:
-            stimulus_mask = data.stimulus_mask
-        
         device = edge_index.device
 
         # If verbose is True, a progress bar is shown
         pbar = tqdm(range(T, n_steps + T), colour="#3E5641") if verbose else range(T, n_steps + T)
         
         # Simulate the network
-        x = torch.zeros((n_neurons, n_steps + T), device=device, dtype=torch.int)
-        inital_state = torch.randint(0, 2, device=device, size=(n_neurons,), generator=self._rng)
-        x[:, :T] = self.equilibrate(edge_index, W, inital_state, n_steps=equilibration_steps)
+        x = torch.zeros((n_neurons, n_steps + T), device=device, dtype=store_as_dtype)
+        inital_state = torch.randint(0, 2, device=device, size=(n_neurons,), generator=self._rng, dtype=store_as_dtype)
+        x[:, :T] = self.equilibrate(edge_index, W, inital_state, n_steps=equilibration_steps, store_as_dtype=store_as_dtype)
         for t in pbar:
-            x[:, t] = self(edge_index=edge_index, W=W, state=x[:, t-T:t], t=t-T, stimulus_mask=stimulus_mask)
+            x[:, t] = self(edge_index=edge_index, W=W, state=x[:, t-T:t], t=t-T)
+
+        # If the stimulus is batched, we increment the batch in preparation for the next batch
+        if isinstance(self.stimulus, BaseStimulus) and self.stimulus.n_batches > 1:
+            self.stimulus.next_batch()
         
         # Return the state of the network at each time step
         return x[:, T:]
     
     def tune(
         self,
         data: Data,
         firing_rate: float,
-        tunable_parameters: Union[str, list[str]] = "all",
+        tunable_parameters: Union[str, List[str]] = "all",
         lr: float = 0.1,
         n_steps: int = 100,
         n_epochs: int = 100,
         verbose: bool = True
     ):
         """
         Tunes the model parameters to match a firing rate.
@@ -285,15 +285,14 @@
             
         self.set_tunable(tunable_parameters)
         
         # Get the parameters of the network
         edge_index = data.edge_index
         W0 = data.W0
         n_neurons = data.num_nodes
-        stimulus_mask = data.stimulus_mask if hasattr(data, "stimulus_mask") else False
         optimizer = torch.optim.Adam(self.parameters(), lr=lr)
         loss_fn = torch.nn.MSELoss()
         firing_rate = torch.tensor(firing_rate, device=device, dtype=torch.float)
 
         average_firing_rate = 0
         self.train()
         for epoch in pbar:
@@ -313,15 +312,14 @@
             # Simulate the network
             for t in range(T, n_steps + T):
                 activation[:, t] = self.input(
                     edge_index,
                     W=W,
                     state=x[:, t-T:t],
                     t=t,
-                    stimulus_mask=stimulus_mask,
                 )
                 x[:, t] = self.emit_spikes(
                     self.non_linearity(activation[:, t]),
                 )
 
             # Compute the loss
             firing_rate_hat = self.non_linearity(activation[:, T:]).mean() * 1000 / self.dt
@@ -330,18 +328,22 @@
             loss = loss_fn(firing_rate, firing_rate_hat)
             if verbose:
                 pbar.set_description(f"Tuning... fr={average_firing_rate:.5f}")
             
             # Backpropagate
             loss.backward()
             optimizer.step()
+
+        # If the stimulus is batched, we increment the batch in preparation for the next batch
+        if isinstance(self.stimulus, BaseStimulus) and self.stimulus.n_batches > 1:
+            self.stimulus.next_batch()
+
+        self.requires_grad_(False) # Freeze the parameters
         
-        self.requires_grad_(False)
-        
-    def set_tunable(self, parameters: list):
+    def set_tunable(self, parameters: Union[str, List[str]]):
         """Sets requires_grad to True for the parameters to be tuned"""
         for param in parameters:
             parameter_dict = dict(self.named_parameters())
             if param not in parameter_dict:
                 raise ValueError(f"Parameter {param} not found in the model")
             parameter_dict[param].requires_grad = True
 
@@ -349,51 +351,48 @@
         """Saves the model to the path"""
         torch.save(self.state_dict(), path)
 
     def load(self, path: str):
         """Loads the model from the path"""
         self.load_state_dict(torch.load(path))
 
-    def to(self, device: str):
+    def to(self, device: Union[str, torch.device]):
         """Moves the model to the device, including the random number generator"""
         self = super().to(device)
         if hasattr(self, "_rng"):
-            if device == "cpu":
-                state = self._rng.get_state()
-                self._rng = torch.Generator().set_state(state)
-            else:
-                seed = self._rng.seed()
-                self._rng = torch.Generator(device=device).manual_seed(seed)
-
+            seed = self._rng.initial_seed()
+            self._rng = torch.Generator(device=device).manual_seed(seed)
         return self
 
-    def equilibrate(self, edge_index: torch.Tensor, W: torch.Tensor, inital_state: torch.Tensor, n_steps=100) -> torch.Tensor:
+    def equilibrate(self, edge_index: torch.Tensor, W: torch.Tensor, inital_state: torch.Tensor, n_steps=100, store_as_dtype: torch.dtype = torch.int) -> torch.Tensor:
         """
         Equilibrate the network to a given connectivity matrix.
 
         Parameters
         -----------
         edge_index: torch.Tensor
             The connectivity of the network
         W: torch.Tensor
             The connectivity filter
         inital_state: torch.Tensor
             The initial state of the network
         n_steps: int
             The number of time steps to equilibrate for
+        store_as_dtype: torch.dtype
+            The dtype to store the state of the network as
 
         Returns
         --------
         x: torch.Tensor
             The state of the network at each time step
         """
         n_neurons = inital_state.shape[0]
         device = inital_state.device
         T = W.shape[1]
-        x_equi = torch.zeros((n_neurons, T + n_steps), device=device, dtype=torch.int)
+        x_equi = torch.zeros((n_neurons, T + n_steps), device=device, dtype=store_as_dtype)
         x_equi[:, T-1] = inital_state
 
         # Equilibrate the network
         for t in range(T, T + n_steps):
             x_equi[:, t] = self(edge_index=edge_index, W=W, state=x_equi[:, t-T:t])
         
         return x_equi[:, -T:]
```

### Comparing `spikeometric-1.0.1/spikeometric/models/bernoulli_glm_model.py` & `spikeometric-1.0.2/spikeometric/models/bernoulli_glm_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.register_parameter("beta", nn.Parameter(torch.tensor(beta, dtype=torch.float)))
         self.register_parameter("alpha", nn.Parameter(torch.tensor(alpha, dtype=torch.float)))
         self.register_parameter("rel_ref_strength", nn.Parameter(torch.tensor(rel_ref_strength, dtype=torch.float)))
 
         self._rng = rng if rng is not None else torch.Generator()
         self.requires_grad_(False)
     
-    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1, stimulus_mask: torch.Tensor = 0) -> torch.Tensor:
+    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1) -> torch.Tensor:
         r"""
         Computes the input at time step :obj:`t+1` by adding together the synaptic input from neighboring neurons and the stimulus input.
 
         .. math::
             g_i(t+1) = \sum_{\tau=0}^{T-1} \left(X_i(t-\tau)r(\tau) + \sum_{j \in \mathcal{N}(i)} (W_0)_{j, i} X_j(t-\tau) c(\tau)\right) + \mathcal{E}_i(t+1)
 
         Parameters
@@ -96,23 +96,21 @@
             The connectivity of the network
         W : torch.Tensor [n_edges, T]
             The weights of the edges
         state : torch.Tensor [n_neurons, T]
             The state of the neurons
         t : int
             The current time step
-        stimulus_mask : torch.Tensor [n_stimulated_neurons, 1]
-            The indices of the neurons that are stimulated
 
         Returns
         -------
         synaptic_input : torch.Tensor [n_neurons, 1]
         
         """
-        return self.synaptic_input(edge_index, W, state=state) + self.stimulus_input(t, stimulus_mask)
+        return self.synaptic_input(edge_index, W, state=state) + self.stimulus_input(t)
 
     def non_linearity(self, input: torch.Tensor) -> torch.Tensor:
         r"""
         Computes the probability that a neuron spikes given its input
 
         .. math::
             p_i(t+1) = \sigma(g_i(t+1) - \theta)
```

### Comparing `spikeometric-1.0.1/spikeometric/models/poisson_glm_model.py` & `spikeometric-1.0.2/spikeometric/models/poisson_glm_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.register_parameter("b", torch.nn.Parameter(torch.tensor(b, dtype=torch.float)))
 
         # RNG
         self._rng = rng if rng is not None else torch.Generator()
 
         self.requires_grad_(False)
 
-    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1, stimulus_mask: torch.Tensor = False) -> torch.Tensor:
+    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1) -> torch.Tensor:
         r"""
         The input to the network at time t+1.
 
         .. math:: g_i(t+1) = r \: \sum_{\tau = 0}^{T-1} \sum_{j\in \mathcal{N}(i)} (W_0)_{j, i} X_j(t-\tau)c(\tau) + b_i + \mathcal{E}_i(t+1)
 
         Parameters
         ----------
@@ -77,25 +77,23 @@
             The edge index of the network.
         W : torch.Tensor[float]
             The weights of the network.
         state : torch.Tensor[int]
             The state of the network at time t.
         t : int
             The time step of the simulation.
-        stimulus_mask : torch.Tensor[bool]
-            A boolean mask of the neurons that are stimulated at time t+1.
 
         Returns
         -------
         torch.Tensor
             The input to the network at time t+1.
         """
         return (
             self.r*self.synaptic_input(edge_index, W, state)
-             + self.stimulus_input(t, stimulus_mask)
+             + self.stimulus_input(t)
              + self.b
         )
     
     def non_linearity(self, input: torch.Tensor) -> torch.Tensor:
         r"""
         The exponential non-linearity of the model. Calculates an expected spike count from the input.
```

### Comparing `spikeometric-1.0.1/spikeometric/models/rectified_lnp_model.py` & `spikeometric-1.0.2/spikeometric/models/rectified_lnp_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self.register_parameter("b", torch.nn.Parameter(torch.tensor(b, dtype=torch.float32)))
 
         # RNG
         self._rng = rng if rng is not None else torch.Generator()
 
         self.requires_grad_(False)
     
-    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1, stimulus_mask: torch.Tensor = False) -> torch.Tensor:
+    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1) -> torch.Tensor:
         r"""
         The input to the network at time t+1.
 
         .. math:: g_i(t+1) = r \: \sum_{\tau = 0}^{T-1} \sum_{j\in \mathcal{N}(i)} (W_0)_{j, i} X_j(t-\tau)c(\tau) + b_i + \mathcal{E}_i(t+1)
 
         Parameters
         ----------
@@ -74,25 +74,23 @@
             The edge index of the network.
         W : torch.Tensor[float]
             The weights of the network.
         state : torch.Tensor[int]
             The state of the network at time t.
         t : int
             The time step of the simulation.
-        stimulus_mask : torch.Tensor[bool]
-            A boolean mask of the neurons that are stimulated at time t+1.
 
         Returns
         -------
         torch.Tensor
             The input to the network at time t+1.
         """
         return (
             self.r*self.synaptic_input(edge_index, W, state)
-             + self.stimulus_input(t, stimulus_mask)
+             + self.stimulus_input(t)
              + self.b
         )
 
     def non_linearity(self, input: torch.Tensor) -> torch.Tensor:
         r"""
         Computes the response to the input through a rectified linear nonlinearity:
```

### Comparing `spikeometric-1.0.1/spikeometric/models/rectified_sa_model.py` & `spikeometric-1.0.2/spikeometric/models/rectified_sa_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self.register_parameter("b", torch.nn.Parameter(torch.tensor(b, dtype=torch.float)))
 
         # RNG
         self._rng = rng if rng is not None else torch.Generator()
 
         self.requires_grad_(False)
 
-    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1, stimulus_mask=False) -> torch.Tensor:
+    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1) -> torch.Tensor:
         r"""
         The input to the network at time t+1.
 
         .. math:: g_i(t+1) = r \: \sum_j (W_0)_{j,i}\: s_j(t) + b_i + \mathcal{E}_i(t+1)
 
         Parameters
         ----------
@@ -76,25 +76,23 @@
             The edge index of the network.
         W : torch.Tensor[float]
             The weights of the network.
         state : torch.Tensor[int]
             The state of the network at time t.
         t : int
             The time step of the simulation.
-        stimulus_mask : torch.Tensor[bool]
-            A boolean mask of the neurons that are stimulated at time t+1.
 
         Returns
         -------
         torch.Tensor
             The input to the network at time t+1.
         """
         return (
             self.r*self.synaptic_input(edge_index, W, state)
-             + self.stimulus_input(t, stimulus_mask)
+             + self.stimulus_input(t)
              + self.b
         )
     
     def non_linearity(self, input: torch.Tensor) -> torch.Tensor:
         r"""
         Computes the response to the input through a rectified linear nonlinearity:
```

### Comparing `spikeometric-1.0.1/spikeometric/models/sa_model.py` & `spikeometric-1.0.2/spikeometric/models/sa_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from spikeometric.models.base_model import BaseModel
 import torch
 from tqdm import tqdm
+from spikeometric.stimulus import BaseStimulus
+from torch_geometric.data import Data
 
 class SAModel(BaseModel):
     r"""
     The Synaptic Activation model (SAModel) is a base model
     for models that use the synaptic activation as the state of the network and has an update rule
     for based on previous synaptic activation and spikes.
 
@@ -13,57 +15,62 @@
     def __init__(self):
         super().__init__()
     
     def update_activation(self, spikes, activation):
         r"""The update rule for the synaptic activation."""
         raise NotImplementedError
     
-    def simulate(self, data, n_steps, verbose=True, equilibration_steps=100):
+    def simulate(self, data: Data, n_steps: int, verbose: bool =True, equilibration_steps: int =100, store_as_dtype: torch.dtype = torch.int):
         """
         Simulates the network for n_steps time steps given the connectivity.
         Returns the state of the network at each time step.
 
         Parameters
         -----------
         data: torch_geometric.data.Data
             The data containing the connectivity. 
         n_steps: int
             The number of time steps to simulate
         verbose: bool
             If True, a progress bar is shown
         equilibration: int
             The number of time steps to simulate before starting to record the state of the network.
+        store_as_dtype: torch.dtype
+            The dtype to store the state of the network
 
         Returns
         --------
         x: torch.Tensor[n_neurons, n_steps]
             The state of the network at each time step. The state is a binary tensor where 1 means that the neuron is active.
         """
         # Get the parameters of the network
         n_neurons = data.num_nodes
         edge_index = data.edge_index
         W0 = data.W0
         W = self.connectivity_filter(W0, edge_index)
         T = W.shape[1]
-        stimulus_mask = data.stimulus_mask if hasattr(data, "stimulus_mask") else False
         device = edge_index.device
 
         # If verbose is True, a progress bar is shown
         pbar = tqdm(range(n_steps + equilibration_steps), colour="#3E5641") if verbose else range(n_steps + equilibration_steps)
         
         # Initialize the state of the network
-        x = torch.zeros(n_neurons, n_steps + equilibration_steps, device=device, dtype=torch.uint8)
+        x = torch.zeros(n_neurons, n_steps + equilibration_steps, device=device, dtype=store_as_dtype)
         initial_activation = torch.rand((n_neurons,1), device=device)
-        activation = self.equilibrate(edge_index, W, initial_activation, equilibration_steps)
+        activation = self.equilibrate(edge_index, W, initial_activation, equilibration_steps, store_as_dtype=store_as_dtype)
 
         # Simulate the network
         for t in pbar:
-            x[:, t] = self(edge_index=edge_index, W=W, state=activation, t=t, stimulus_mask=stimulus_mask)
+            x[:, t] = self(edge_index=edge_index, W=W, state=activation, t=t)
             activation = self.update_activation(spikes=x[:, t:t+T], activation=activation)
 
+        # If the stimulus is batched, we increment the batch in preparation for the next batch
+        if isinstance(self.stimulus, BaseStimulus) and self.stimulus.n_batches > 1:
+            self.stimulus.next_batch()
+
         # Return the state of the network at each time step
         return x
 
     def tune(
         self,
         data,
         firing_rate,
@@ -117,15 +124,14 @@
         
         # Get the parameters of the network
         edge_index = data.edge_index
         W0 = data.W0
         W = self.connectivity_filter(W0, edge_index)
         T = W.shape[1]
         n_neurons = data.num_nodes
-        stimulus_mask = data.stimulus_mask if hasattr(data, "stimulus_mask") else False
         optimizer = torch.optim.Adam(self.parameters(), lr=lr)
         loss_fn = torch.nn.MSELoss()
         firing_rate = torch.tensor(firing_rate, device=device, dtype=torch.float)
         self.train()
         average_firing_rate = 0
         for epoch in pbar:
             optimizer.zero_grad()
@@ -139,15 +145,14 @@
             # Simulate the network
             for t in range(1, n_steps):
                 input[:, t] = self.input(
                     edge_index,
                     W=W,
                     state=activation,
                     t=t,
-                    stimulus_mask=stimulus_mask
                 )
                 x[:, t] = self.emit_spikes(
                     self.non_linearity(input[:, t]),
                 )
                 activation = self.update_activation(
                     activation=activation,
                     spikes=x[:, t:t+1]
@@ -161,37 +166,45 @@
             if verbose:
                 pbar.set_description(f"Tuning... fr={average_firing_rate:.5f}")
 
             # Backpropagate
             loss.backward()
             optimizer.step()
 
-    def equilibrate(self, edge_index: torch.Tensor, W: torch.Tensor, inital_state: torch.Tensor, n_steps=100) -> torch.Tensor:
+        # If the stimulus is batched, we increment the batch in preparation for the next batch
+        if isinstance(self.stimulus, BaseStimulus) and self.stimulus.n_batches > 1:
+            self.stimulus.next_batch()
+
+        self.requires_grad_(False) # Freeze the parameters 
+
+    def equilibrate(self, edge_index: torch.Tensor, W: torch.Tensor, inital_state: torch.Tensor, n_steps=100, store_as_dtype: torch.dtype = torch.int) -> torch.Tensor:
         """
         Equilibrate the network to a given connectivity matrix.
 
         Parameters
         -----------
         edge_index: torch.Tensor
             The connectivity of the network
         W: torch.Tensor
             The connectivity filter
         inital_state: torch.Tensor
             The initial state of the network
         n_steps: int
             The number of time steps to equilibrate for
+        store_as_dtype: torch.dtype
+            The dtype to store the state of the network as
 
         Returns
         --------
         x: torch.Tensor
             The state of the network at each time step
         """
         n_neurons = inital_state.shape[0]
         device = inital_state.device
-        x_equi = torch.zeros((n_neurons, self.T + n_steps), device=device, dtype=torch.int)
+        x_equi = torch.zeros((n_neurons, self.T + n_steps), device=device, dtype=store_as_dtype)
         x_equi[:, self.T-1] = inital_state.squeeze()
 
         # Equilibrate the network
         for t in range(self.T, self.T + n_steps):
             x_equi[:, t] = self(edge_index=edge_index, W=W, state=x_equi[:, t-self.T:t])
         
         return x_equi[:, -self.T:]
```

### Comparing `spikeometric-1.0.1/spikeometric/models/threshold_sa_model.py` & `spikeometric-1.0.2/spikeometric/models/threshold_sa_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.register_buffer("dt", torch.tensor(dt, dtype=torch.float))
         self.register_buffer("sigma", torch.tensor(sigma, dtype=torch.float))
         self.register_buffer("rho", torch.tensor(rho, dtype=torch.float))
         self.register_buffer("theta", torch.tensor(theta, dtype=torch.float))
         self.register_buffer("T", torch.tensor(1, dtype=torch.int))
         self._rng = rng
     
-    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1, stimulus_mask=False) -> torch.Tensor:
+    def input(self, edge_index: torch.Tensor, W: torch.Tensor, state: torch.Tensor, t=-1) -> torch.Tensor:
         r"""
         Calculates the input to each neuron as:
 
         .. math:: g_i(t+1) = r \: \sum_j (W_0)_{j,i}\: s_j(t) + b_i + \mathcal{E}_i(t+1)
 
         Parameters
         -----------
@@ -69,23 +69,21 @@
             The connectivity of the network.
         W : torch.Tensor [n_edges, 1]
             The edge weights of the connectivity filter.
         state : torch.Tensor [n_neurons, 1]
             The activation of the neurons at time t.
         t : int
             The current time step.
-        stimulus_mask : torch.Tensor [n_neurons]
-            A boolean mask of the neurons that are stimulated at time t.
         
         Returns
         --------
         input : torch.Tensor [n_neurons]
             The input to each neuron at time t.
         """
-        return self.r*self.synaptic_input(edge_index, W, state=state) + self.background_input(state.shape[0]) + self.stimulus_input(t, stimulus_mask)
+        return self.r*self.synaptic_input(edge_index, W, state=state) + self.background_input(state.shape[0]) + self.stimulus_input(t)
 
     def background_input(self, n_neurons: int):
         r"""
         Generate the background input. This is a uniform excitatory input given by the parameter :math:`b`
         plus a scaled Gaussian noise with standard deviation :math:`\sigma` and some sparsity.
 
         Parameters
```

### Comparing `spikeometric-1.0.1/spikeometric/stimulus/sin_stimulus.py` & `spikeometric-1.0.2/spikeometric/stimulus/sin_stimulus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import torch
 import torch.nn as nn
+from spikeometric.stimulus.base_stimulus import BaseStimulus
+import math
+from typing import Union
 
-class SinStimulus(nn.Module):
+class SinStimulus(BaseStimulus):
     r"""
     Sinusoidal stimulus of neurons.
 
     The stimulus is a sinusoidal function with amplitude :math:`A`, period :math:`T`, and phase :math:`\phi`.
     The stimulus starts at time :math:`t_0` and lasts for a duration :math:`\tau`.
 
     Parameters
     ----------
     amplitude : float
         Amplitude :math:`A` of stimulus.
     period : float
         Period :math:`T` of stimulus
     duration : int
         Duration :math:`\tau` stimulus in total
+    stimulus_mask:
+        A mask of shape (n_neurons,) indicating which neurons to stimulate.
+    batch_size : int
+        The number of networks to stimulate in parallel.
     phase : float
         Phase of stimulus :math:`\phi`
     baseline: float
         The constant baseline of the stimulus.
     start : float
         Start time :math:`t_0` of stimulus.
     dt : float
         Time step :math:`\Delta t` of the simulation in ms.
     """
-    def __init__(self, amplitude: float, period: float, duration: int, phase: float = 0., baseline: float = 0, start: float = 0., dt: float = 1.):
+    def __init__(self, amplitude: float, period: float, duration: int, stimulus_masks: torch.Tensor, batch_size: int = 1, phase: float = 0., baseline: float = 0, start: float = 0., dt: float = 1.):
         super().__init__()
         if amplitude < 0:
             raise ValueError("All amplitudes must be positive.")
         if period < 0:
             raise ValueError("All periods must be positive.")
         if duration < 0:
             raise ValueError("All durations must be positive.")
@@ -37,21 +44,38 @@
         self.register_parameter("amplitude", nn.Parameter(torch.tensor(amplitude, dtype=torch.float)))
         self.register_parameter("period", nn.Parameter(torch.tensor(period, dtype=torch.float)))
         self.register_parameter("phase", nn.Parameter(torch.tensor(phase, dtype=torch.float)))
         self.register_parameter("baseline", nn.Parameter(torch.tensor(baseline, dtype=torch.float)))
         self.register_buffer("duration", torch.tensor(duration, dtype=torch.int))
         self.register_buffer("start", torch.tensor(start, dtype=torch.float))
         self.register_buffer("dt", torch.tensor(dt, dtype=torch.float))
+
+        if isinstance(stimulus_masks, torch.Tensor) and stimulus_masks.ndim == 1:
+            stimulus_masks = [stimulus_masks]
+
+        if isinstance(stimulus_masks, torch.Tensor) and stimulus_masks.ndim == 2:
+            stimulus_masks = [sm.squeeze() for sm in torch.split(stimulus_masks, 1, dim=0)]
+        
+        conc_stimulus_masks, split_points = self.batch_stimulus_masks(stimulus_masks, batch_size)
+        self.n_batches = math.ceil(len(stimulus_masks) / batch_size)
+        self.register_buffer("conc_stimulus_masks", conc_stimulus_masks)
+        self.register_buffer("split_points", torch.tensor(split_points, dtype=torch.int))
+        self._idx = 0
+
         self.requires_grad_(False)
 
-    def __call__(self, t):
+    def __call__(self, t: Union[float, torch.Tensor]) -> torch.Tensor:
         r"""
         Computes stimulus at time t by applying a sinusoidal function.
 
         Between the start time :math:`t_0` and the end time :math:`t_0 + \tau`, the stimulus is given by
 
         .. math::
             f(t) = A \sin \left( \frac{2 \pi}{T} (t - t_0)\Delta t + \phi \right)
         """
+        time_mask = (t < self.duration) * (t >= self.start)
+        if torch.is_tensor(t):
+            stim_mask = self.stimulus_masks[self._idx].unsqueeze(1)
+            return (self.amplitude * torch.sin(2*torch.pi / self.period * (t-self.start)*self.dt + self.phase) + self.baseline) * time_mask * stim_mask
         return (
             self.amplitude * torch.sin(2*torch.pi / self.period * (t-self.start)*self.dt + self.phase) + self.baseline
-        ) * (t < self.duration) * (t >= self.start)
+        ) * time_mask * self.stimulus_masks[self._idx]
```

### Comparing `spikeometric-1.0.1/setup.py` & `spikeometric-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.5.0,<4.0.0',
  'networkx>=3.0,<4.0',
  'numpy>=1.21.4,<2.0.0',
  'scipy>=1.7.3,<2.0.0',
- 'seaborn>=0.11.2,<0.12.0',
+ 'seaborn>=0.12.2,<0.13.0',
  'tqdm>=4.62.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'spikeometric',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Spikeometric is a Pytorch Geometric based framework for simulating Spiking Neural Networks using Linear Non-linear Cascade models',
     'long_description': '# Spikeometric - Linear Non-Linear Cascade Spiking Neural Networks with PyTorch Geometric\n\nThe spikeometric package is a framework for simulating spiking neural networks (SNNs) using generalized linear models (GLMs) and Linear-Nonlinear-Poisson models (LNPs) in Python. It is built on top of the [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/) package and makes use of their powerful graph neural network (GNN) modules and efficient graph representation. It is designed to be fast, flexible and easy to use, and is intended for research purposes.\n\n# Install\nBefore installing `spikeometric` you will need to download versions of PyTorch and PyTorch Geometric that work with your hardware. When you have done that (for example in a conda environment), you are ready to download spikeometric with:\n\n    pip install spikeometric\n\n# Documentation\n\nFor more information about the package and a full API reference check out our [documentation](https://spikeometric.readthedocs.io/en/latest/).\n\n# How to contribute\nWe welcome contributions from users and developers. If you find bugs, please report an issue on github.\nIf you would like to contribute to new features you can either find an issue you would like to work on, or fork this project and develop something great. \nSend pull request for review. We will respond as soon as possible.\n',
     'author': 'Jakob Sønstebø',
     'author_email': 'jakobls16@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bioAI-Oslo/Spikeometric',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `spikeometric-1.0.1/PKG-INFO` & `spikeometric-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: spikeometric
-Version: 1.0.1
+Version: 1.0.2
 Summary: Spikeometric is a Pytorch Geometric based framework for simulating Spiking Neural Networks using Linear Non-linear Cascade models
 Home-page: https://github.com/bioAI-Oslo/Spikeometric
 License: GNU General Public License v3.0
 Author: Jakob Sønstebø
 Author-email: jakobls16@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.5.0,<4.0.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (>=1.21.4,<2.0.0)
 Requires-Dist: scipy (>=1.7.3,<2.0.0)
-Requires-Dist: seaborn (>=0.11.2,<0.12.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Documentation, https://spikeometric.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/bioAI-Oslo/Spikeometric
 Description-Content-Type: text/markdown
 
 # Spikeometric - Linear Non-Linear Cascade Spiking Neural Networks with PyTorch Geometric
```

