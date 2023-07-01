# Comparing `tmp/fogLedger-1.1.2.tar.gz` & `tmp/fogLedger-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fogLedger-1.1.2.tar", last modified: Sat Jul  1 13:53:27 2023, max compression
+gzip compressed data, was "fogLedger-2.0.0.tar", last modified: Sat Jul  1 13:43:03 2023, max compression
```

## Comparing `fogLedger-1.1.2.tar` & `fogLedger-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:53:27.273877 fogLedger-1.1.2/
--rw-r--r--   0 matheus   (1000) matheus   (1000)      477 2023-07-01 13:53:27.273877 fogLedger-1.1.2/PKG-INFO
--rw-r--r--   0 matheus   (1000) matheus   (1000)     2054 2023-05-27 11:43:06.000000 fogLedger-1.1.2/README.md
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:53:27.273877 fogLedger-1.1.2/fogLedger.egg-info/
--rw-r--r--   0 matheus   (1000) matheus   (1000)      477 2023-07-01 13:53:27.000000 fogLedger-1.1.2/fogLedger.egg-info/PKG-INFO
--rw-r--r--   0 matheus   (1000) matheus   (1000)      291 2023-07-01 13:53:27.000000 fogLedger-1.1.2/fogLedger.egg-info/SOURCES.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2023-07-01 13:53:27.000000 fogLedger-1.1.2/fogLedger.egg-info/dependency_links.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2023-07-01 13:52:27.000000 fogLedger-1.1.2/fogLedger.egg-info/not-zip-safe
--rw-r--r--   0 matheus   (1000) matheus   (1000)       14 2023-07-01 13:53:27.000000 fogLedger-1.1.2/fogLedger.egg-info/requires.txt
--rw-r--r--   0 matheus   (1000) matheus   (1000)       10 2023-07-01 13:53:27.000000 fogLedger-1.1.2/fogLedger.egg-info/top_level.txt
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:53:27.273877 fogLedger-1.1.2/fogledger/
--rw-r--r--   0 matheus   (1000) matheus   (1000)        0 2023-05-25 23:56:28.000000 fogLedger-1.1.2/fogledger/__init__.py
-drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:53:27.273877 fogLedger-1.1.2/fogledger/indy/
--rw-r--r--   0 matheus   (1000) matheus   (1000)     4819 2023-07-01 13:52:01.000000 fogLedger-1.1.2/fogledger/indy/IndyBasic.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)       48 2023-05-25 23:57:43.000000 fogLedger-1.1.2/fogledger/indy/__init__.py
--rw-r--r--   0 matheus   (1000) matheus   (1000)       38 2023-07-01 13:53:27.273877 fogLedger-1.1.2/setup.cfg
--rw-r--r--   0 matheus   (1000) matheus   (1000)      753 2023-07-01 13:53:21.000000 fogLedger-1.1.2/setup.py
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:43:03.820892 fogLedger-2.0.0/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     1062 2023-07-01 13:29:47.000000 fogLedger-2.0.0/LICENSE.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      515 2023-07-01 13:43:03.820892 fogLedger-2.0.0/PKG-INFO
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     2054 2023-05-27 11:43:06.000000 fogLedger-2.0.0/README.md
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:43:03.820892 fogLedger-2.0.0/fogLedger.egg-info/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      515 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/PKG-INFO
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      318 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/SOURCES.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/dependency_links.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)        1 2023-07-01 13:33:01.000000 fogLedger-2.0.0/fogLedger.egg-info/not-zip-safe
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       14 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/requires.txt
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       10 2023-07-01 13:43:03.000000 fogLedger-2.0.0/fogLedger.egg-info/top_level.txt
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:43:03.820892 fogLedger-2.0.0/fogledger/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)        0 2023-05-25 23:56:28.000000 fogLedger-2.0.0/fogledger/__init__.py
+drwxr-xr-x   0 matheus   (1000) matheus   (1000)        0 2023-07-01 13:43:03.820892 fogLedger-2.0.0/fogledger/indy/
+-rw-r--r--   0 matheus   (1000) matheus   (1000)     5235 2023-06-28 13:38:45.000000 fogLedger-2.0.0/fogledger/indy/IndyBasic.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       48 2023-05-25 23:57:43.000000 fogLedger-2.0.0/fogledger/indy/__init__.py
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       84 2023-07-01 13:32:06.000000 fogLedger-2.0.0/pyproject.toml
+-rw-r--r--   0 matheus   (1000) matheus   (1000)       38 2023-07-01 13:43:03.820892 fogLedger-2.0.0/setup.cfg
+-rw-r--r--   0 matheus   (1000) matheus   (1000)      765 2023-07-01 13:42:57.000000 fogLedger-2.0.0/setup.py
```

### Comparing `fogLedger-1.1.2/README.md` & `fogLedger-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fogLedger-1.1.2/fogledger/indy/IndyBasic.py` & `fogLedger-2.0.0/fogledger/indy/IndyBasic.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,88 +9,99 @@
 import numpy
 
 
 class IndyBasic:
     def __init__(
         self,
         exp: FogbedDistributedExperiment,
-        nodes_number: int = 4,
-        prefix: str = 'node',
-        trustees_path='tmp/trustees.csv'
+        trustees_path='tmp/trustees.csv',
+        config_nodes: List[dict] = []
     ) -> None:
         self.ledgers: List[VirtualInstance] = []
         self.nodes: List[Container] = []
         self.exp = exp
         self.genesis_content = ''
         self.trustees_path = trustees_path
-        self._create_ledgers(prefix, nodes_number)
+        self._create_ledgers(config_nodes)
         self._create_dir()
 
-    def _create_ledgers(self, prefix: str = 'node', nodes_number: int = 4):
-        self.ledgers = self._create_virtual_instances(nodes_number, prefix)
-        self.nodes = self._create_nodes(prefix)
+    def _create_ledgers(self, config_nodes: List[dict] = []):
+        self.ledgers = self._create_virtual_instances(config_nodes)
+        self.nodes = self._create_nodes(config_nodes)
         return self.ledgers, self.nodes
 
     def create_links(self, target: VirtualInstance, devices: List[VirtualInstance]) -> None:
         for device in devices:
             self.exp.add_link(device, target)
 
-    def _create_virtual_instances(self, number: int, prefix: str) -> List[VirtualInstance]:
-        return [self.exp.add_virtual_instance(f'{prefix}{i+1}') for i in range(number)]
+    def _create_virtual_instances(self, config_nodes: List[dict] = []) -> List[VirtualInstance]:
+        return [self.exp.add_virtual_instance(config['name']) for i, config in enumerate(config_nodes)]
 
-    def _create_nodes(self, prefix: str) -> List[Container]:
+    def _create_nodes(self, config_nodes: List[dict]) -> List[Container]:
         nodes = []
         for i, ledger in enumerate(self.ledgers):
-            name = f'{prefix}{i+1}'
+
+            name = config_nodes[i]['name'] if (
+                "name" in config_nodes[i]) else str(i)
+            
+            ip = config_nodes[i]['ip'] if ("ip" in config_nodes[i]) else None
+            
+            port_bindings = config_nodes[i]['port_bindings'] if ("port_bindings" in config_nodes[i]) else {}
+            
             node = Container(
                 name=name,
                 dimage='larsid/fogbed-indy-node:v1.0.2-beta',
+                ip=ip,
+                port_bindings=port_bindings
             )
             nodes.append(node)
             self.exp.add_docker(
                 container=node,
                 datacenter=ledger)
         return nodes
-    def _create_dir(self) -> None: 
-        if not os.path.exists("tmp/indy/"):   
+
+    def _create_dir(self) -> None:
+        if not os.path.exists("tmp/indy/"):
             os.makedirs("tmp/indy/")
 
     def _get_content_trustees(self) -> str:
         content = ''
         with open(self.trustees_path, newline='') as csvfile:
             # read csv file and save in a string
             spamreader = csv.reader(csvfile, delimiter=',')
             for row in spamreader:
                 content += ','.join(row) + '\n'
         return content
-        
-        
 
     def start_network(self) -> None:
         print('Initializing Network... ⏳')
 
         genesis_file_name = uuid.uuid4()
         array_genesis = numpy.array([['Steward name', 'Validator alias', 'Node IP address', 'Node port', 'Client IP address',
                                     'Client port', 'Validator verkey', 'Validator BLS key', 'Validator BLS POP', 'Steward DID', 'Steward verkey']])
         for i, node in enumerate(self.nodes):
             print(f'Configuring {node.name}... ⏳')
             seed = node.cmd("pwgen -s 32 1")
             node.cmd(f"printf 'wallet create fogbed key=key \nexit\n' | indy-cli")
             info_cli = node.cmd(
                 f"printf 'wallet open fogbed key=key\n did new seed={seed}\nexit\n' | indy-cli")
+            print(info_cli)
             matches = re.findall(
                 r'Did "(\S+)" has been created with "(\S+)" verkey', info_cli)
             did = ''
             verkey = ''
+            print(matches)
             if matches:
                 did = matches[0][0]
                 verkey = matches[0][1]
             aux = node.cmd(
                 f'init_indy_node {node.name} {node.ip} 9701 {node.ip} 9702')
+            print(aux)
             lines = aux.splitlines()
+
             array_genesis = numpy.append(array_genesis, [[node.name, node.name, node.ip, 9701, node.ip, 9702, lines[5].split(
                 ' ')[3], lines[9].split(' ')[4], lines[10].split(' ')[7], did, verkey]], axis=0)
             print(f'Configured {node.name} ✅')
         print('Configured Nodes ✅')
         # create a list of formatted rows
         rows = [','.join(str(field) for field in row) for row in array_genesis]
 
@@ -103,12 +114,13 @@
             node.cmd(f'echo "{text}" >> /tmp/indy/{genesis_file_name}.csv')
             node.cmd(f'echo "{trustees_content}" >> /tmp/indy/trustees.csv')
             node.cmd(
                 f'/opt/indy/scripts/genesis_from_files.py --stewards /tmp/indy/{genesis_file_name}.csv --trustees /tmp/indy/trustees.csv')
             node.cmd(
                 f'cp domain_transactions_genesis /var/lib/indy/$NETWORK_NAME/ && cp pool_transactions_genesis /var/lib/indy/$NETWORK_NAME/')
             node.cmd(
-                f'start_indy_node {node.name} {node.ip} 9701 {node.ip} 9702 > output.log 2>&1 &')
+                f'start_indy_node {node.name} 0.0.0.0 9701 0.0.0.0 9702 > output.log 2>&1 &')
             print(f'Started {node.name} ✅')
         # save genesis content in memory
-        self.genesis_content = self.nodes[0].cmd('cat pool_transactions_genesis')
+        self.genesis_content = self.nodes[0].cmd(
+            'cat pool_transactions_genesis')
         print('Indy Network Started ✅')
```

### Comparing `fogLedger-1.1.2/setup.py` & `fogLedger-2.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="fogLedger",
-    version="1.1.2",
+    version="2.0.0",
     description='Plugin to build DLTs in Fogbed.',
     long_description='Plugin to build DLT in Fogbed. Suport Hyperledger Indy',
     keywords=['networking', 'emulator', 'protocol', 'Internet', 'dlt', 'indy', 'fog'],
-    url='https://github.com/larsid/FogLedger',
+    url='https://github.com/larsid/FogLedger/tree/v2.0.0',
     author='Matheus Nascimento',
     author_email='matheusnascimentoti99@gmail.com',
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

