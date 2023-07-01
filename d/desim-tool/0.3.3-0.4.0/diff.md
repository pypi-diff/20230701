# Comparing `tmp/desim-tool-0.3.3.tar.gz` & `tmp/desim-tool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desim-tool-0.3.3.tar", last modified: Thu May 25 11:16:25 2023, max compression
+gzip compressed data, was "desim-tool-0.4.0.tar", last modified: Sat Jul  1 14:16:39 2023, max compression
```

## Comparing `desim-tool-0.3.3.tar` & `desim-tool-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-05-25 11:16:25.900635 desim-tool-0.3.3/
--rw-r--r--   0 oscarbennet   (501) staff       (20)     1089 2023-05-18 16:32:34.000000 desim-tool-0.3.3/LICENSE.md
--rw-r--r--   0 oscarbennet   (501) staff       (20)      211 2023-05-25 11:16:25.900866 desim-tool-0.3.3/PKG-INFO
--rw-r--r--   0 oscarbennet   (501) staff       (20)     1561 2023-05-18 16:32:34.000000 desim-tool-0.3.3/README.md
-drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-05-25 11:16:25.895666 desim-tool-0.3.3/desim/
--rw-r--r--   0 oscarbennet   (501) staff       (20)        0 2023-05-18 16:32:34.000000 desim-tool-0.3.3/desim/__init__.py
--rw-r--r--   0 oscarbennet   (501) staff       (20)     2363 2023-05-18 16:32:34.000000 desim-tool-0.3.3/desim/data.py
--rw-r--r--   0 oscarbennet   (501) staff       (20)     6831 2023-05-18 16:32:34.000000 desim-tool-0.3.3/desim/interface.py
--rw-r--r--   0 oscarbennet   (501) staff       (20)    10085 2023-05-25 11:12:25.000000 desim-tool-0.3.3/desim/simulation.py
-drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-05-25 11:16:25.899912 desim-tool-0.3.3/desim_tool.egg-info/
--rw-r--r--   0 oscarbennet   (501) staff       (20)      211 2023-05-25 11:16:25.000000 desim-tool-0.3.3/desim_tool.egg-info/PKG-INFO
--rw-r--r--   0 oscarbennet   (501) staff       (20)      279 2023-05-25 11:16:25.000000 desim-tool-0.3.3/desim_tool.egg-info/SOURCES.txt
--rw-r--r--   0 oscarbennet   (501) staff       (20)        1 2023-05-25 11:16:25.000000 desim-tool-0.3.3/desim_tool.egg-info/dependency_links.txt
--rw-r--r--   0 oscarbennet   (501) staff       (20)       12 2023-05-25 11:16:25.000000 desim-tool-0.3.3/desim_tool.egg-info/requires.txt
--rw-r--r--   0 oscarbennet   (501) staff       (20)        6 2023-05-25 11:16:25.000000 desim-tool-0.3.3/desim_tool.egg-info/top_level.txt
--rw-r--r--   0 oscarbennet   (501) staff       (20)      106 2023-05-25 11:16:25.901989 desim-tool-0.3.3/setup.cfg
--rw-r--r--   0 oscarbennet   (501) staff       (20)      283 2023-05-25 11:16:18.000000 desim-tool-0.3.3/setup.py
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-01 14:16:39.576171 desim-tool-0.4.0/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     1089 2023-05-18 16:32:34.000000 desim-tool-0.4.0/LICENSE.md
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      211 2023-07-01 14:16:39.576536 desim-tool-0.4.0/PKG-INFO
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     1561 2023-05-18 16:32:34.000000 desim-tool-0.4.0/README.md
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-01 14:16:39.572118 desim-tool-0.4.0/desim/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        0 2023-05-18 16:32:34.000000 desim-tool-0.4.0/desim/__init__.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     2363 2023-05-18 16:32:34.000000 desim-tool-0.4.0/desim/data.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      110 2023-07-01 12:22:15.000000 desim-tool-0.4.0/desim/helper.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     6804 2023-07-01 12:52:47.000000 desim-tool-0.4.0/desim/interface.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)    10439 2023-07-01 12:22:15.000000 desim-tool-0.4.0/desim/simulation.py
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-01 14:16:39.575600 desim-tool-0.4.0/desim_tool.egg-info/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      211 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/PKG-INFO
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      295 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        1 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)       12 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/requires.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        6 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/top_level.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      106 2023-07-01 14:16:39.578268 desim-tool-0.4.0/setup.cfg
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      284 2023-07-01 13:03:18.000000 desim-tool-0.4.0/setup.py
```

### Comparing `desim-tool-0.3.3/LICENSE.md` & `desim-tool-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `desim-tool-0.3.3/README.md` & `desim-tool-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `desim-tool-0.3.3/desim/data.py` & `desim-tool-0.4.0/desim/data.py`

 * *Files identical despite different names*

### Comparing `desim-tool-0.3.3/desim/interface.py` & `desim-tool-0.4.0/desim/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import List
-import numpy as np
 import multiprocessing as mp
 from desim.data import SimResults, TimeFormat
-from desim.simulation import Process, Simulation, Entity, NonTechCost
+from desim.simulation import Process, Simulation, NonTechCost
 
 
 class Des(object):
   """
   This is a class for running a discrete event simulation. 
 
   It is an interface of the different types of simulations that can be run.
```

### Comparing `desim-tool-0.3.3/desim/simulation.py` & `desim-tool-0.4.0/desim/simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,227 +1,238 @@
 from dataclasses import dataclass
 import random as r
 import numpy as np
 from typing import Optional, List
 
 import simpy
-#import pandas as pd
+# import pandas as pd
 
 from desim.data import NonTechCost, TimeFormat
+from desim.helper import isfloat
+
+TIMESTEP = 0.25  # TODO change this to be a param in Simulation where it is dependent on the time_format
 
-TIMESTEP = 0.25 #TODO change this to be a param in Simulation where it is dependent on the time_format
 
 class Simulation(object):
-    #@param:
-    #flow_time = the time that entities will flow in the system
-    #interarrival_time = the rate at which entities will flow in the system
-    #interarrival_process = the process at which the entities will start flowing
-    #until = the total simulation time
-    def __init__(self, flow_time: float, flow_rate: float, flow_process: str, simulation_runtime: float, discount_rate: float, processes, non_tech_processes, non_tech_addition, dsm, time_format: TimeFormat) -> None:
+    # @param:
+    # flow_time = the time that entities will flow in the system
+    # interarrival_time = the rate at which entities will flow in the system
+    # interarrival_process = the process at which the entities will start flowing
+    # until = the total simulation time
+    def __init__(self, flow_time: float, flow_rate: float, flow_process: str, simulation_runtime: float,
+                 discount_rate: float, processes, non_tech_processes, non_tech_addition, dsm,
+                 time_format: TimeFormat) -> None:
         self.flow_time = flow_time
         self.flow_rate = flow_rate
-        self.interarrival_time = 0 if flow_rate <= 0 else 1 / (flow_rate * time_format.value) #Causes the interarrival time to be in years.
+        self.interarrival_time = 0 if flow_rate <= 0 else 1 / (
+                    flow_rate * time_format.value)  # Causes the interarrival time to be in years.
         self.interarrival_process = flow_process
-        self.until = simulation_runtime / time_format.value #Causes the runtime to be in years. 
+        self.until = simulation_runtime / time_format.value  # Causes the runtime to be in years.
         self.discount_rate = discount_rate
         self.cum_NPV = [0]
         self.total_costs = [0]
         self.total_revenue = [0]
         self.time_steps = [0]
         self.entities = []
-        self.processes = processes 
+        self.processes = processes
         self.non_tech_costs = sum([p.cost for p in non_tech_processes])
         self.non_tech_revenues = sum([p.revenue for p in non_tech_processes])
         self.add_non_tech = non_tech_addition
         self.dsm_before_flow, self.dsm_after_flow = self.get_dsm_separation(dsm)
         self.time_format = time_format
-        #r.seed(0) #Remove for production
-        #np.random.seed(0) #Remove for production
+        # r.seed(0) #Remove for production
+        # np.random.seed(0) #Remove for production
 
-    #Sets up the simpy environment and runs the simulation
+    # Sets up the simpy environment and runs the simulation
     def run_simulation(self):
         env = simpy.Environment()
         env.process(self.lifecycle(env))
         env.process(self.observe_costs(env))
         env.run(until=self.until)
-    
-    #Initializes the lifecycle in each of the entities. Runs everything before the interarrival
-    #process as a single entity. 
+
+    # Initializes the lifecycle in each of the entities. Runs everything before the interarrival
+    # process as a single entity.
     def lifecycle(self, env):
         interarrival_process = list(filter(lambda p: p.name == self.interarrival_process, self.processes))
-        total_ent_amount =  0 if self.interarrival_time <= 0 else (1 / self.interarrival_time) * self.flow_time
-        
+        total_ent_amount = 0 if self.interarrival_time <= 0 else (1 / self.interarrival_time) * self.flow_time
+
         e = Entity(env, self.processes, self.non_tech_costs)
         self.entities.append(e)
         yield env.process(e.lifecycle(self.dsm_before_flow, [self.processes[0]], 1))
-        
+
         end_flow = env.now + self.flow_time
         while env.now < end_flow:
             for i in range(int(self.flow_rate)):
                 e = Entity(env, self.processes, self.non_tech_costs)
                 self.entities.append(e)
                 env.process(e.lifecycle(self.dsm_after_flow, interarrival_process, total_ent_amount))
             yield env.timeout(1)
-        
 
-        #print('Done')
-            
-            
-    #Observes the total time, cost, revenue, and NPV for each entity in each timestep. 
-    def observe_costs(self, env): #TODO fix calculation of NPV. Currently it's bonkers
-        #total_costs = [0]
-        #total_revenue = [0]
+        # print('Done')
+
+    # Observes the total time, cost, revenue, and NPV for each entity in each timestep.
+    def observe_costs(self, env):  # TODO fix calculation of NPV. Currently it's bonkers
+        # total_costs = [0]
+        # total_revenue = [0]
 
         if self.add_non_tech == NonTechCost.LUMP_SUM:
-            #print('Lump sum')
+            # print('Lump sum')
             self.total_costs[0] += self.non_tech_costs
 
-        while True:         
+        while True:
 
             if self.add_non_tech == NonTechCost.CONTINOUSLY:
-                #print('Added static costs')
+                # print('Added static costs')
                 self.add_static_costs_to_entities()
 
             self.total_costs.append(sum([e.cost for e in self.entities]))
             self.total_revenue.append(sum([e.revenue for e in self.entities]))
             self.time_steps.append(env.now)
 
-
             self.calculate_NPV(self.total_costs, self.total_revenue, self.time_steps)
             yield env.timeout(TIMESTEP)
 
-
-    #Generates the waiting time as interarrival rate on an exponential distribution
+    # Generates the waiting time as interarrival rate on an exponential distribution
     def generate_interarrival(self):
         return np.random.exponential(self.interarrival_time)
 
-
-    def add_static_costs_to_entities(self): #Adds the costs of the non-technical processes to all active entities. 
+    def add_static_costs_to_entities(self):  # Adds the costs of the non-technical processes to all active entities.
         for e in self.entities:
-            e.cost +=  self.non_tech_costs * TIMESTEP/ (len(self.entities) * self.until)  #This works in the margin of 0.00000002 euros
+            e.cost += self.non_tech_costs * TIMESTEP / (
+                        len(self.entities) * self.until)  # This works in the margin of 0.00000002 euros
 
     def calculate_NPV(self, total_costs, total_revenue, time_steps):
-        timestep_revenue = total_revenue[len(time_steps) -1] - total_revenue[len(time_steps) - 2]
+        timestep_revenue = total_revenue[len(time_steps) - 1] - total_revenue[len(time_steps) - 2]
         timestep_cost = total_costs[len(time_steps) - 1] - total_costs[len(time_steps) - 2]
-        #print(timestep_revenue, timestep_cost)
+        # print(timestep_revenue, timestep_cost)
 
-        net_revenue = timestep_revenue - timestep_cost #Cashflow for the timestep
+        net_revenue = timestep_revenue - timestep_cost  # Cashflow for the timestep
         npv = net_revenue / ((1 + self.discount_rate) ** time_steps[-1])
         self.cum_NPV.append(self.cum_NPV[-1] + npv)
 
-    #Separates the given DSM into two dictionaries with the before flow and after flow parts of the dsm
+    # Separates the given DSM into two dictionaries with the before flow and after flow parts of the dsm
     def get_dsm_separation(self, dsm):
         before_dsm = dict()
         dsm = dsm.copy()
+        for key, row in dsm.items():
+            dsm[key] = [float(x) if isfloat(x) else 0 for x in row]
         for p in self.processes:
             if p.name == self.interarrival_process:
                 break
             before_dsm.update({p.name: dsm.pop(p.name)})
-        return before_dsm,dsm
+        return before_dsm, dsm
+
 
 class Entity(object):
-    #@param
-    #env = the simpy environment
-    #processes = the processes that the entity will go through
+    # @param
+    # env = the simpy environment
+    # processes = the processes that the entity will go through
     def __init__(self, env, processes, total_non_tech_costs) -> None:
         self.env = env
         self.processes = processes
         self.total_time = [0]
         self.total_cost = [0]
         self.total_revenue = [0]
         self.cost = 0
         self.revenue = 0
         self.total_non_tech_costs = total_non_tech_costs
-    
-    #Runs the lifecycle for this entity. 
-    #Can choose between processes but cannot run multiple processes in parallell
+
+    # Runs the lifecycle for this entity.
+    # Can choose between processes but cannot run multiple processes in parallell
     def lifecycle(self, dsm, current_processes, ent_amount):
         active_activities = current_processes
         while len(active_activities) > 0:
-            #print(f'curr time {self.env.now}')
-            min_time = active_activities[0].time #For yielding in case there are multiple processes running in parallell
+            # print(f'curr time {self.env.now}')
+            min_time = active_activities[
+                0].time  # For yielding in case there are multiple processes running in parallell
             for activity in active_activities:
                 self.env.process(activity.run_process(self.env, self, ent_amount, self.total_non_tech_costs))
                 if activity.time < min_time:
                     min_time = activity.time
-            
-            #start_time = self.env.now
+
+            # start_time = self.env.now
             yield self.env.timeout(min_time)
-       
-            #for activity in active_activities: #This loop is probably unneccessary since we do not check W anywhere atm
+
+            # for activity in active_activities: #This loop is probably unneccessary since we do not check W anywhere atm
             #    if activity.W > 0:
             #        activity.W = (self.env.now - start_time) / activity.time
-            active_activities = self.find_active_activities(dsm, active_activities) #Find subsequent activities
+            active_activities = self.find_active_activities(dsm, active_activities)  # Find subsequent activities
+
+        # print(f'Entity: {self} done, total time: {sum([p.time for p in self.processes])}')
 
-        #print(f'Entity: {self} done, total time: {sum([p.time for p in self.processes])}')
-    
-    #Finds the active processes for the lifecycle based on the dsm and the current state
-    #That the lifecycle is in. 
+    # Finds the active processes for the lifecycle based on the dsm and the current state
+    # That the lifecycle is in.
     def find_active_activities(self, dsm: dict, current_processes):
         active_activities = []
         for process in current_processes:
-            if(process.name not in dsm.keys()):
+            if (process.name not in dsm.keys()):
                 break
 
             transitions = dsm.get(process.name)
-            
-            if(all([p==0 for p in transitions])): #Checks if all rows are 0, if that is the case then there is nothing more to be done after this process 
+
+            if (all([p == 0 for p in
+                     transitions])):  # Checks if all rows are 0, if that is the case then there is nothing more to be done after this process
+                continue
+
+            process_index = self.choose_process_from_row(transitions)  # Select the process index from its row
+            if process_index >= len(self.processes):  # Simulation has reached the end
                 continue
+            active_activities.append(self.processes[process_index])
 
-            process_index = self.choose_process_from_row(transitions) #Select the process index from its row
-            active_activities.append(self.processes[process_index]) 
-                 
         return active_activities
-    
-    #Selects a process index from a row of transitional probabilities
+
+    # Selects a process index from a row of transitional probabilities
     def choose_process_from_row(self, row):
-        return r.choices([i for i,_ in enumerate(row)], row, k=1)[0]
+        return r.choices([i for i, _ in enumerate(row)], row, k=1)[0] - 1  # -1 because the first column is the start
+
 
 @dataclass
 class Process(object):
-    #@param
-    #id = the id of a process
-    #time = the time a process will take in years. 
-    #cost = the cost of a process
-    #revenue = the revenue of a process
-    #name = the name of a process
-    #time_format = the unit in which the time is given. 
-    def __init__(self, id, time, cost, revenue, name, add_non_tech: NonTechCost, time_format: Optional[TimeFormat] = None) -> None:
+    # @param
+    # id = the id of a process
+    # time = the time a process will take in years.
+    # cost = the cost of a process
+    # revenue = the revenue of a process
+    # name = the name of a process
+    # time_format = the unit in which the time is given.
+    def __init__(self, id, time, cost, revenue, name, add_non_tech: NonTechCost,
+                 time_format: Optional[TimeFormat] = None) -> None:
         self.time = self.convert_time_format_to_default(time, time_format)
         self.cost = cost
         self.revenue = revenue
         self.W = 1
         self.WN = False
         self.id = id
         self.name = name
         self.add_non_tech = add_non_tech
-    
-    #Converts all times to the correct (default: Years) time format
+
+    # Converts all times to the correct (default: Years) time format
     def convert_time_format_to_default(self, time, time_format: Optional[TimeFormat] = None):
         return (time / time_format.value) if time_format is not None else 0
 
-    #Runs a process and adds the cost and the revenue to the entity
+    # Runs a process and adds the cost and the revenue to the entity
     def run_process(self, env, entity, ent_amount, non_tech_costs):
-        #print(f'Started working on process: {self.name}')
+        # print(f'Started working on process: {self.name}')
         yield env.timeout(self.time * self.W)
-        #print(f'Time after step in lifecycle: {env.now}')
-        #non_tech_costs = total_non_tech_cost * self.time / (process_time * amount_of_entities) #Add this to the total cost in order to add non tech costs to processes
-        
+        # print(f'Time after step in lifecycle: {env.now}')
+        # non_tech_costs = total_non_tech_cost * self.time / (process_time * amount_of_entities) #Add this to the total cost in order to add non tech costs to processes
+
         entity.cost += self.cost
         entity.revenue += self.revenue
-        
+
         if self.add_non_tech == NonTechCost.TO_TECHNICAL_PROCESS:
-            #print('Process add')
+            # print('Process add')
             added_cost = non_tech_costs * self.time / (sum([p.time for p in entity.processes]) * ent_amount)
             entity.cost += added_cost
 
-        #total_cost.append(total_cost[-1] + self.cost)
-        #total_revenue.append(total_revenue[-1] + self.revenue)
-        
+        # total_cost.append(total_cost[-1] + self.cost)
+        # total_revenue.append(total_revenue[-1] + self.revenue)
+
         self.W = 0
 
+
 @dataclass
 class NonTechnicalProcess(object):
-  def __init__(self, name: str, cost: float, revenue: float) -> None:
-      self.name = name
-      self.cost = cost
-      self.revenue = revenue
+    def __init__(self, name: str, cost: float, revenue: float) -> None:
+        self.name = name
+        self.cost = cost
+        self.revenue = revenue
```

