# Comparing `tmp/gecs-0.22.0.tar.gz` & `tmp/gecs-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.22.0.tar", max compression
+gzip compressed data, was "gecs-0.27.tar", max compression
```

## Comparing `gecs-0.22.0.tar` & `gecs-0.27.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.22.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-06 08:53:47.610205 gecs-0.22.0/README.md
--rw-r--r--   0        0        0      697 2023-06-26 18:40:00.063336 gecs-0.22.0/pyproject.toml
--rw-r--r--   0        0        0    42972 2023-06-27 16:27:27.188690 gecs-0.22.0/src/gecs/gec.py
--rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.22.0/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 gecs-0.22.0/setup.py
--rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 gecs-0.22.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-06 09:38:20.465352 gecs-0.27/LICENSE
+-rw-r--r--   0        0        0     2454 2023-07-01 12:49:31.528724 gecs-0.27/README.md
+-rw-r--r--   0        0        0      695 2023-06-30 08:00:55.534668 gecs-0.27/pyproject.toml
+-rw-r--r--   0        0        0    42244 2023-06-30 07:59:27.571454 gecs-0.27/src/gecs/gec.py
+-rw-r--r--   0        0        0     2112 2023-06-19 14:54:28.150721 gecs-0.27/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0     3437 1970-01-01 00:00:00.000000 gecs-0.27/setup.py
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 gecs-0.27/PKG-INFO
```

### Comparing `gecs-0.22.0/LICENSE` & `gecs-0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.22.0/pyproject.toml` & `gecs-0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.22.0"
+version = "0.27"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.22.0/src/gecs/gec.py` & `gecs-0.27/src/gecs/gec.py`

 * *Files 4% similar despite different names*

```diff
@@ -330,24 +330,20 @@
 
         self._real_hypermarameter_types = [
             np.array(s).dtype for _, s in self._real_hyperparameters
         ]
 
     def _set_gec_fields(self):
         self.kernel = RBF(self.gec_hyperparameters["l"])
-        self.hyperparameter_scores = {
-            c: {"inputs": [], "output": [], "means": [], "sigmas": []}
-            for c in ["all-models"]
-        }
+        self.hyperparameter_scores = {"inputs": [], "output": [], "means": [], "sigmas": []}
+
         self.kernel_bagging = RBF(self.gec_hyperparameters["l_bagging"])
 
-        self.bagging_scores = {
-            c: {"inputs": [], "output": [], "means": [], "sigmas": []}
-            for c in ["all-models"]
-        }
+        self.bagging_scores = {"inputs": [], "output": [], "means": [], "sigmas": []}
+
         self._bagging_combinations = list(
             itertools.product(
                 *[
                     list(range(1, 11, 1)),
                     np.arange(0.5, 1.0, 0.01),
                 ]
             )
@@ -383,19 +379,15 @@
     @kernel_bagging.setter
     def kernel_bagging(self, value):
         self._kernel_bagging = value
         self.gaussian_bagging = GaussianProcessRegressor(kernel=value)
 
     @property
     def gec_iter(self):
-        return int(
-            np.sum(
-                [len(value["output"]) for value in self.hyperparameter_scores.values()]
-            )
-        )
+        return len(self.hyperparameter_scores)
 
     @classmethod
     def _cast_to_type(cls, value, type_):
         if type_ == np.float64:
             return float(value)
         elif type_ == np.int64:
             return int(value)
@@ -446,18 +438,15 @@
             warnings.warn(
                 "If X and y are not provided, the GEC model is not fitted for inference"
             )
         return gec
 
     @classmethod
     def _convert_gaussian_process_data_from_deserialisation(cls, data_dict):
-        converted_dict = {
-            k: {k2: list(v) for k2, v in values.items()}
-            for k, values in data_dict.items()
-        }
+        converted_dict = {k: list(v) for k, v in data_dict.items()}
         return converted_dict
 
     def serialise(self, path):
         """Serialise GEC model object
 
         Parameters
         ----------
@@ -475,18 +464,16 @@
             if not isinstance(value, np.ndarray):
                 return value
             elif key != "inputs":
                 return list(value)
             else:
                 return list(value.astype(np.float64))
 
-        converted_dict = {
-            k: {k2: [process_value(k2, vv) for vv in v] for k2, v in values.items()}
-            for k, values in data_dict.items()
-        }
+        converted_dict = {k2: [process_value(k2, vv) for vv in v] for k2, v in data_dict.items()}
+
         return converted_dict
 
     def _get_representation(self):
         hyperparameter_scores = self._convert_gaussian_process_data_for_serialisation(
             self.hyperparameter_scores
         )
         bagging_scores = self._convert_gaussian_process_data_for_serialisation(
@@ -591,33 +578,34 @@
         # self.hyperparameter_scores, self.rewards = hyperparameter_scores, rewards
         # self.selected_arms = selected_arms
 
         return self
 
     def _calculate_cv_score(self, X, y, params):
         clf = LGBMClassifier(**params)
-        with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
-            score = np.mean(cross_val_score(clf, X, y, cv=5))
+        try:
+            with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
+                cross_val_scores = cross_val_score(clf, X, y, cv=5)
+                score = np.mean(cross_val_scores)
+        except:
+            warnings.warn(f"Could not calculate cross val scores for parameters: {params}")
+            score = 0.0
         return score
 
 
     def _optimise_hyperparameters(
         self,
         n_iter,
         X,
         Y,
         best_score,
         best_params,
         **kwargs,
     ):
 
-        assert np.all(
-            np.array(sorted(list(self.hyperparameter_scores.keys())))
-            == np.array(["all-models"])
-        )
         if self.gec_hyperparameters["randomize"]:
             np.random.seed(int(datetime.now().timestamp() % 1 * 1e7))
 
         for i in tqdm(list(range(n_iter))):
             if (i + self.gec_iter) < min(
                 self.gec_hyperparameters["n_random_exploration"], int(n_iter / 2)
             ):
@@ -652,45 +640,51 @@
                         for _, reward in self.rewards.items()
                     ]
                 )
                 selected_arm_index = sampled_reward.argmax()
                 selected_arm = self._categorical_hyperparameter_combinations[
                     selected_arm_index
                 ]
-                n_best = max(
-                    3, int(self.gec_iter * self.gec_hyperparameters["best_share"])
-                )
-                best_interactions = np.argsort(
-                    np.array(self.hyperparameter_scores["all-models"]["output"])
-                )[::-1][:n_best]
-
-                best_hyperparameters = np.array(
-                    self.hyperparameter_scores["all-models"]["inputs"]
-                )[best_interactions, :]
+
 
                 sets = np.array(
                     [
                         np.random.choice(
                             range_, self.gec_hyperparameters["n_sample_initial"]
                         )
                         for _, range_ in self._real_hyperparameters_linear
                     ]
                 )
-                closest_hyperparameters = best_hyperparameters.dot(sets).argsort(1)[
-                    :, : int(self.gec_hyperparameters["n_sample"] / n_best)
-                ]
-                selected_hyperparameter_indices = np.unique(
-                    closest_hyperparameters.flatten()
-                )
 
-                combinations = list(sets[:, selected_hyperparameter_indices].T)
+                if len(self.hyperparameter_scores["inputs"]):
+                    n_best = max(
+                        3, int(self.gec_iter * self.gec_hyperparameters["best_share"])
+                    )
+                    best_interactions = np.argsort(
+                        np.array(self.hyperparameter_scores["output"])
+                    )[::-1][:n_best]
+
+                    best_hyperparameters = np.array(
+                        self.hyperparameter_scores["inputs"]
+                    )[best_interactions, :]
+
+                    closest_hyperparameters = best_hyperparameters.dot(sets).argsort(1)[
+                        :, : self.gec_hyperparameters["n_sample"]
+                    ]
+                    selected_hyperparameter_indices = np.unique(
+                        closest_hyperparameters.flatten()
+                    )
+
+                    combinations = list(sets[:, selected_hyperparameter_indices].T)
+                else:
+                    combinations = list(sets[:, :self.gec_hyperparameters["n_sample"]].T)
 
                 assert len(combinations), sets
 
-                if len(self.hyperparameter_scores["all-models"]["inputs"]) > 0:
+                if len(self.hyperparameter_scores["inputs"]) > 0:
                     self._fit_gaussian()
 
                 mean, sigma = self.gaussian.predict(combinations, return_std=True)
 
                 predicted_rewards = np.array(
                     [
                         scipy.stats.norm.ppf(
@@ -707,15 +701,15 @@
                 best_predicted_combination = combinations[np.argmax(predicted_rewards)]
                 selected_combination = best_predicted_combination
                 arguments = self._build_arguments(
                     selected_arm.split("-"), selected_combination
                 )
 
                 if "yes_bagging" in selected_arm:
-                    if len(self.bagging_scores["all-models"]["inputs"]) > 0:
+                    if len(self.bagging_scores["inputs"]) > 0:
                         self._fit_gaussian_bagging()
                     mean_bagging, sigma_bagging = self.gaussian_bagging.predict(
                         self._bagging_combinations_rescaled, return_std=True
                     )
 
                     predicted_rewards_bagging = np.array(
                         [
@@ -747,39 +741,40 @@
                     score = 0
 
                 if best_score is None or score > best_score:
                     best_score = score
                     best_params = arguments
 
                 self.selected_arms.append(selected_arm)
-                self.hyperparameter_scores["all-models"]["inputs"].append(
+                self.hyperparameter_scores["inputs"].append(
                     [float(f) for f in selected_combination]
                 )
-                self.hyperparameter_scores["all-models"]["output"].append(score)
-                self.hyperparameter_scores["all-models"]["means"].append(mean)
-                self.hyperparameter_scores["all-models"]["sigmas"].append(sigma)
+                self.hyperparameter_scores["output"].append(score)
+                self.hyperparameter_scores["means"].append(mean)
+                self.hyperparameter_scores["sigmas"].append(sigma)
 
                 if "bagging_freq" in arguments:
-                    self.bagging_scores["all-models"]["inputs"].append(
+                    self.bagging_scores["inputs"].append(
                         list(self._rescale_bagging_combination(*selected_combination_bagging))
                     )
-                    self.bagging_scores["all-models"]["output"].append(score)
-                    self.bagging_scores["all-models"]["means"].append(mean_bagging)
-                    self.bagging_scores["all-models"]["sigmas"].append(sigma_bagging)
+                    self.bagging_scores["output"].append(score)
+                    self.bagging_scores["means"].append(mean_bagging)
+                    self.bagging_scores["sigmas"].append(sigma_bagging)
 
                 if self.best_score is not None:
                     score_delta = score - self.best_score
                     weighted_score_delta = (
                         score_delta * self.gec_hyperparameters["bandit_greediness"]
                     )
                     if score_delta > 0:
                         self.rewards[selected_arm]["a"] = (
                             self.rewards[selected_arm]["a"] + weighted_score_delta
                         )
                         self.best_params_ = arguments
+                        self.best_score = score
                     else:
                         self.rewards[selected_arm]["b"] = (
                             self.rewards[selected_arm]["b"] - weighted_score_delta
                         )
                 else:
                     self.best_score = score
                     self.best_params_ = arguments
@@ -825,22 +820,22 @@
             if k not in self.__dict__ or self.__dict__[k] is None:
                 self.__dict__[k] = v
 
         super().fit(X, y)
 
     def _fit_gaussian(self):
         self.gaussian.fit(
-            np.array(self.hyperparameter_scores["all-models"]["inputs"]),
-            np.array(self.hyperparameter_scores["all-models"]["output"]) - np.mean(self.hyperparameter_scores["all-models"]["output"]),
+            np.array(self.hyperparameter_scores["inputs"]),
+            np.array(self.hyperparameter_scores["output"]) - np.mean(self.hyperparameter_scores["output"]),
         )
 
     def _fit_gaussian_bagging(self):
         self.gaussian_bagging.fit(
-            np.array(self.bagging_scores["all-models"]["inputs"]),
-            np.array(self.bagging_scores["all-models"]["output"]) - np.mean(self.bagging_scores["all-models"]["output"]),
+            np.array(self.bagging_scores["inputs"]),
+            np.array(self.bagging_scores["output"]) - np.mean(self.bagging_scores["output"]),
         )
 
     def _get_best_arm(self):
         mean_reward = np.array(
             [
                 reward["a"]/ ( reward["a"] + reward["b"])
                 for _, reward in self.rewards.items()
@@ -989,89 +984,83 @@
         -------
             figs : dict[str, fig]
                 a dictionary of figures
         """
 
         figs = {}
 
-        for categorical_combination in ["all-models"]:
-            fig, axes = plt.subplots(
-                nrows=2, ncols=2, sharex=True, sharey=False, figsize=(12, 12)
-            )
-            ax1, ax2, ax3, ax4 = axes.flatten()
+        fig, axes = plt.subplots(
+            nrows=2, ncols=2, sharex=True, sharey=False, figsize=(12, 12)
+        )
+        ax1, ax2, ax3, ax4 = axes.flatten()
 
-            x = np.arange(
-                len(self.hyperparameter_scores[categorical_combination]["means"])
-            )
-            self._plot_mean_prediction_and_mean_variance(
-                categorical_combination, ax1, x
-            )
-            self._plot_prediction_std_and_variance_std(categorical_combination, ax2, x)
-            self._plot_prediction_mean_variance_correlation(
-                categorical_combination, ax3, x
-            )
-            self._plot_linear_scaled_parameter_samples(categorical_combination, ax4, x)
+        x = np.arange(
+            len(self.hyperparameter_scores["means"])
+        )
+        self._plot_mean_prediction_and_mean_variance(ax1, x)
+        self._plot_prediction_std_and_variance_std(ax2, x)
+        self._plot_prediction_mean_variance_correlation(ax3, x)
+        self._plot_linear_scaled_parameter_samples(ax4, x)
 
-            figs[f"{categorical_combination}-parameters"] = fig
+        figs["parameters"] = fig
 
-            fig2 = self._plot_boosting_parameter_surface(categorical_combination)
-            figs[f"{categorical_combination}-bagging"] = fig2
+        fig2 = self._plot_boosting_parameter_surface()
+        figs["bagging"] = fig2
 
         return figs
 
-    def _plot_mean_prediction_and_mean_variance(self, cat, ax, x):
+    def _plot_mean_prediction_and_mean_variance(self, ax, x):
         gp_mean_prediction = [
-            np.mean(x) for x in self.hyperparameter_scores[cat]["means"]
+            np.mean(x) for x in self.hyperparameter_scores["means"]
         ]
-        gp_mean_sigma = [np.mean(x) for x in self.hyperparameter_scores[cat]["sigmas"]]
+        gp_mean_sigma = [np.mean(x) for x in self.hyperparameter_scores["sigmas"]]
 
         ax.plot(x, gp_mean_prediction, label="mean_prediction")
         ax.plot(x, gp_mean_sigma, label="mean_sigma")
         ax.legend(loc="upper right")
 
-    def _plot_prediction_std_and_variance_std(self, cat, ax, x):
+    def _plot_prediction_std_and_variance_std(self, ax, x):
         gp_prediction_variance = [
-            np.std(x) for x in self.hyperparameter_scores[cat]["means"]
+            np.std(x) for x in self.hyperparameter_scores["means"]
         ]
         gp_sigma_variance = [
-            np.std(x) for x in self.hyperparameter_scores[cat]["sigmas"]
+            np.std(x) for x in self.hyperparameter_scores["sigmas"]
         ]
 
         ax.plot(x, gp_prediction_variance, label="prediction_variance")
         ax.plot(x, gp_sigma_variance, label="sigma_variance")
         ax.legend(loc="lower right")
 
-    def _plot_prediction_mean_variance_correlation(self, cat, ax, x):
+    def _plot_prediction_mean_variance_correlation(self, ax, x):
         correlation = [
             np.corrcoef(
-                self.hyperparameter_scores[cat]["means"][i],
-                self.hyperparameter_scores[cat]["sigmas"][i],
+                self.hyperparameter_scores["means"][i],
+                self.hyperparameter_scores["sigmas"][i],
             )[0, 1]
             for i in x
         ]
 
         ax.plot(
             x,
             correlation,
             label="corr(preds mean, preds variance)",
         )
         ax.legend(loc="lower right")
 
-    def _plot_linear_scaled_parameter_samples(self, cat, ax, x):
-        inputs_ = np.array(self.hyperparameter_scores[cat]["inputs"])
+    def _plot_linear_scaled_parameter_samples(self, ax, x):
+        inputs_ = np.array(self.hyperparameter_scores["inputs"])
         assert (
             (len(self._real_hyperparameter_names) == inputs_.shape[1]), 
             f"{len(self._real_hyperparameter_names)}!={inputs_.shape[1]}"
         )
         for i in range(inputs_.shape[1]):
             ax.plot(x, inputs_[:, i], label=self._real_hyperparameter_names[i])
 
     def _plot_boosting_parameter_surface(
         self,
-        cat,
         plot_bounds=True,
     ):
         self._fit_gaussian_bagging()
 
         X_range = np.array(self._bagging_combinations_rescaled)[0,:]
         Y_range = np.array(self._bagging_combinations_rescaled)[1,:]
         Z_range = np.arange(-0.5, 1.5, 0.1)
```

### Comparing `gecs-0.22.0/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.27/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

