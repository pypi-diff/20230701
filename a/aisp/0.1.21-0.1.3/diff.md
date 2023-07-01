# Comparing `tmp/aisp-0.1.21.tar.gz` & `tmp/aisp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisp-0.1.21.tar", last modified: Mon Jun 12 18:30:51 2023, max compression
+gzip compressed data, was "aisp-0.1.3.tar", last modified: Sat Jul  1 13:23:43 2023, max compression
```

## Comparing `aisp-0.1.21.tar` & `aisp-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:30:51.276323 aisp-0.1.21/
--rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.21/LICENSE
--rw-rw-rw-   0        0        0     7908 2023-06-12 18:30:51.275325 aisp-0.1.21/PKG-INFO
--rw-rw-rw-   0        0        0     6854 2023-06-08 16:13:42.000000 aisp-0.1.21/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:30:51.248329 aisp-0.1.21/aisp/
-drwxrwxrwx   0        0        0        0 2023-06-12 18:30:51.272324 aisp-0.1.21/aisp/NSA/
--rw-rw-rw-   0        0        0      140 2023-06-12 18:29:52.000000 aisp-0.1.21/aisp/NSA/__init__.py
--rw-rw-rw-   0        0        0    50866 2023-06-12 18:20:04.000000 aisp-0.1.21/aisp/NSA/_negativeSelection.py
--rw-rw-rw-   0        0        0     8811 2023-06-12 16:38:13.000000 aisp-0.1.21/aisp/_base.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:30:51.262325 aisp-0.1.21/aisp.egg-info/
--rw-rw-rw-   0        0        0     7908 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-12 18:30:51.000000 aisp-0.1.21/aisp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1443 2023-06-12 18:29:11.000000 aisp-0.1.21/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 18:30:51.277328 aisp-0.1.21/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-01 13:23:43.587263 aisp-0.1.3/
+-rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7907 2023-07-01 13:23:43.585257 aisp-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6854 2023-06-08 16:13:42.000000 aisp-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 13:23:43.559216 aisp-0.1.3/aisp/
+drwxrwxrwx   0        0        0        0 2023-07-01 13:23:43.582253 aisp-0.1.3/aisp/NSA/
+-rw-rw-rw-   0        0        0      140 2023-06-12 18:29:52.000000 aisp-0.1.3/aisp/NSA/__init__.py
+-rw-rw-rw-   0        0        0    51156 2023-06-29 19:12:53.000000 aisp-0.1.3/aisp/NSA/_negativeSelection.py
+-rw-rw-rw-   0        0        0     8811 2023-06-12 16:38:13.000000 aisp-0.1.3/aisp/_base.py
+drwxrwxrwx   0        0        0        0 2023-07-01 13:23:43.575236 aisp-0.1.3/aisp.egg-info/
+-rw-rw-rw-   0        0        0     7907 2023-07-01 13:23:43.000000 aisp-0.1.3/aisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-01 13:23:43.000000 aisp-0.1.3/aisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 13:23:43.000000 aisp-0.1.3/aisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-01 13:23:43.000000 aisp-0.1.3/aisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-01 13:23:43.000000 aisp-0.1.3/aisp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1442 2023-06-28 13:22:23.000000 aisp-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-01 13:23:43.587263 aisp-0.1.3/setup.cfg
```

### Comparing `aisp-0.1.21/LICENSE` & `aisp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aisp-0.1.21/PKG-INFO` & `aisp-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.21
+Version: 0.1.3
 Summary: Package with techniques of artificial immune systems.
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
```

### Comparing `aisp-0.1.21/README.md` & `aisp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aisp-0.1.21/aisp/NSA/_negativeSelection.py` & `aisp-0.1.3/aisp/NSA/_negativeSelection.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,15 @@
             self.max_discards: int = 1000
 
         # Obtém as variáveis do kwargs.
         self.p: float = kwargs.get('p', 2)
         self._cell_bounds: bool = kwargs.get('cell_bounds', False)
         self.non_self_label: str = kwargs.get('non_self_label', 'non-self')
         
+        # Inicializa as demais variáveis da classe como None
         self.detectors: Union[dict, None] = None
         self.classes: npt.NDArray = None
 
     def fit(self, X: npt.NDArray, y: npt.NDArray, verbose: bool = True):
         """
         The function ``fit(...)``, performs the training according to ``X`` and ``y``, using the method
         negative selection method(``NegativeSelect``).
@@ -370,20 +371,19 @@
                 class_found = True
 
             # Se possuir apenas uma classe e não classificar a amostra define a saída como não-própria.
             if not class_found and len(self.classes) == 1:
                 C = np.append(C, [self.non_self_label])
             # Se não identificar a classe com os detectores, coloca a classe com a maior distância da média dos seus detectores.
             elif not class_found:
-                average_distance = dict()
+                average_distance: dict = {}
                 for _class_ in self.classes:
                     detectores = list(
                         map(lambda x: x.position, self.detectors[_class_]))
-                    average_distance[_class_] = self.__distance(
-                        np.average(detectores, axis=0), line)
+                    average_distance[_class_] = np.average([self.__distance(detector, line) for detector in detectores])
                 C = np.append(
                     C, [max(average_distance, key=average_distance.get)])
         return C
 
     def __checks_valid_detector(self, X: npt.NDArray = None, vector_x: npt.NDArray = None, samples_index_class: npt.NDArray = None):
         """
         Function to check if the detector has a valid non-proper ``r`` radius for the class.
@@ -709,15 +709,16 @@
             'N': self.N,
             'r': self.r,
             'k': self.k,
             'metric': self.metric,
             'seed': self.seed,
             'algorithm': self._algorithm,
             'r_s': self.r_s,
-            'cell_bounds': self._cell_bounds
+            'cell_bounds': self._cell_bounds,
+            'p': self.p
         }
 
 class BNSA(Base):
     """
     The ``BNSA`` (Binary Negative Selection Algorithm) class is for classification and identification purposes.
     of anomalies through the self and not self method.
 
@@ -841,18 +842,20 @@
             * y (``npt.NDArray``):  Array com as classes alvos de ``X`` com [``N amostras`` (linhas)].
             * verbose (``bool``): Feedback da geração de detectores para o usuário.
         Returns:
         ---
             (``self``): Retorna a própria instância.
         """
         super()._check_and_raise_exceptions_fit(X, y, 'BNSA')
-
+        
+        # Converte todo o array X para booleano
         if X.dtype != bool:
             X = X.astype(bool)
 
+        # Identificando as classes possíveis, dentro do array de saídas ``y``.
         self.classes = np.unique(y)
         # Dict que armazenará os detectores com as classes como key.
         list_detectors_by_class = dict()
         # Separa as classes para o treinamento.
         sample_index: dict = self.__slice_index_list_by_class(y)
         # Barra de progresso para a geração de todos os detectores.
         if verbose:
@@ -867,15 +870,15 @@
             if verbose:
                 progress.set_description_str(
                     f'Generating the detectors for the {_class_} class:')
             while len(valid_detectors_set) < self.N:
                 
                 is_valid_detector: bool = True
                 # Gera um vetor candidato a detector aleatoriamente com valores 0 e 1.
-                vector_x = np.random.randint(0, 2, X.shape[1], dtype=bool)
+                vector_x = np.random.choice([False, True], size=X.shape[1])
                 for i in sample_index[_class_]:
                     # Verifica a validade do detector para o não-próprio com relação às amostras da classe.
                     if hamming(X[i], vector_x) <= self.aff_thresh:
                         is_valid_detector = False
                         break
                 # Se o detector for válido, adicione a lista dos válidos.
                 if is_valid_detector:
@@ -941,58 +944,59 @@
         elif len(self.detectors[self.classes[0]][0]) != len(X[0]):
             raise Exception('X does not have {} features to make the prediction'.format(
                 len(self.detectors[self.classes[0]][0])))
         # Verifica se a matriz X contém apenas amostras binárias. Caso contrário, lança uma exceção.
         if not np.isin(X, [0, 1]).all():
             raise ValueError(
                 "The array X contains values that are not composed only of 0 and 1.")
-
+        
+        # Converte todo o array X para booleano
         if X.dtype != bool:
             X = X.astype(bool)
             
         # Inicia um array vazio.
         C = np.empty(shape=(0))
         # Para cada linha de amostra em X.
         for line in X:
             class_found: bool = True
             # Lista para armazenar as possíveis classes às quais a amostra se adequou ao self na comparação com os detectores non-self.
             possible_classes: list = [] 
             for _class_ in self.classes:
                 # Lista para armzenar as taxas de similaridade entre a amostra e os detectores.
-                similarity_list: list = []
+                similarity_sum: float = 0
                 for detector in self.detectors[_class_]:
                     similarity = hamming(line, detector)
                     if similarity <= self.aff_thresh:
                         class_found = False
                         break
                     else:
-                        similarity_list.append(similarity)
+                        similarity_sum += similarity
                 # Se a amostra passar por todos os detectores de uma classe, adiciona a classe como possivel previsão e sua media de similaridade.
                 if class_found:
-                    possible_classes.append([_class_, min(similarity_list)])
+                    possible_classes.append([_class_, similarity_sum / self.N])
         
             # Se, pertencer a uma ou mais classes, adiciona a classe com a distância média mais distante.
             if len(possible_classes) > 0 :
                 C = np.append(C, [max(possible_classes, key=lambda x: x[1])[0]])
                 class_found = True
             else:
                 class_found = False
 
             # Se possuir apenas uma classe e não classificar a amostra define a saída como não-própria.
             if not class_found and len(self.classes) == 1:
                 C = np.append(C, ['non-self'])
             # Se não identificar a classe com os detectores, coloca a classe com a maior distância da média dos seus detectores.
             elif not class_found:
-                class_differences = []
+                class_differences: dict = {}
                 for _class_ in self.classes:
-                    differences = []
+                    difference_sum: float = 0
                     for detector in self.detectors[_class_]:
-                        differences.append(hamming(line, detector))
-                    class_differences.append(min(differences))
-                C = np.append(C, [self.classes[class_differences.index(max(class_differences))]])
+                        difference_sum += hamming(line, detector)
+                    class_differences[_class_] = (difference_sum / self.N)
+                C = np.append(C, [max(class_differences, key=class_differences.get)])
  
         return C
 
     def __slice_index_list_by_class(self, y: npt.NDArray) -> dict:
         """
         The function ``__slice_index_list_by_class(...)``, separates the indices of the lines according to the output class,
         to loop through the sample array, only in positions where the output is the class being trained.
```

### Comparing `aisp-0.1.21/aisp/_base.py` & `aisp-0.1.3/aisp/_base.py`

 * *Files identical despite different names*

### Comparing `aisp-0.1.21/aisp.egg-info/PKG-INFO` & `aisp-0.1.3/aisp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.21
+Version: 0.1.3
 Summary: Package with techniques of artificial immune systems.
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
```

### Comparing `aisp-0.1.21/pyproject.toml` & `aisp-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aisp"
-version = "0.1.21"
+version = "0.1.3"
 authors = [
   { name="João Paulo da Silva Barros", email="jpsilvabarr@gmail.com" },
 ]
 
 maintainers = [
   { name="Alison Zille Lopes",  email="alisonzille@gmail.com"},
 ]
```

