# Comparing `tmp/blacklight-0.1.8.tar.gz` & `tmp/blacklight-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacklight-0.1.8.tar", max compression
+gzip compressed data, was "blacklight-0.1.9.tar", max compression
```

## Comparing `blacklight-0.1.8.tar` & `blacklight-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,59 @@
--rw-r--r--   0        0        0    35149 2023-07-06 22:26:37.027562 blacklight-0.1.8/LICENSE
--rw-r--r--   0        0        0     3589 2023-07-06 22:26:37.027726 blacklight-0.1.8/README.md
--rw-r--r--   0        0        0       67 2023-07-06 22:26:37.028342 blacklight-0.1.8/blacklight/__init__.py
--rw-r--r--   0        0        0       74 2023-07-06 22:26:37.028739 blacklight-0.1.8/blacklight/autoML/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 22:26:37.029046 blacklight-0.1.8/blacklight/autoML/_convolutional_nn.py
--rw-r--r--   0        0        0     6585 2023-07-06 22:26:37.029190 blacklight-0.1.8/blacklight/autoML/_feed_forward.py
--rw-r--r--   0        0        0        0 2023-07-06 22:26:37.029265 blacklight-0.1.8/blacklight/autoML/tests/__init__.py
--rw-r--r--   0        0        0     5105 2023-07-06 22:26:37.030033 blacklight-0.1.8/blacklight/autoML/tests/data/Iris.csv
--rw-r--r--   0        0        0      409 2023-07-06 22:26:37.030130 blacklight-0.1.8/blacklight/autoML/tests/end_to_end_feed_forward_test.py
--rw-r--r--   0        0        0      186 2023-07-06 22:26:37.030217 blacklight-0.1.8/blacklight/autoML/tests/test_CI_CD.py
--rw-r--r--   0        0        0     6129 2023-07-06 23:01:51.776809 blacklight-0.1.8/blacklight/autoML/tests/test_feed_forward_population.py
--rw-r--r--   0        0        0      191 2023-07-06 22:26:37.030452 blacklight-0.1.8/blacklight/base/__init__.py
--rw-r--r--   0        0        0      168 2023-07-06 22:26:37.030949 blacklight-0.1.8/blacklight/base/chromosomes/__init__.py
--rw-r--r--   0        0        0     1423 2023-07-06 22:26:37.031388 blacklight-0.1.8/blacklight/base/chromosomes/base_chromosome.py
--rw-r--r--   0        0        0     7888 2023-07-06 22:26:37.031526 blacklight-0.1.8/blacklight/base/chromosomes/convolutional_chromosome.py
--rw-r--r--   0        0        0     5836 2023-07-06 22:26:37.031627 blacklight-0.1.8/blacklight/base/chromosomes/feed_forward_chromosome.py
--rw-r--r--   0        0        0        0 2023-07-06 22:26:37.031717 blacklight-0.1.8/blacklight/base/chromosomes/tests/__init__.py
--rw-r--r--   0        0        0     2310 2023-07-06 22:26:37.032326 blacklight-0.1.8/blacklight/base/chromosomes/tests/test_feed_forward_chromosome.py
--rw-r--r--   0        0        0     1523 2023-07-06 22:26:37.032418 blacklight-0.1.8/blacklight/base/individual.py
--rw-r--r--   0        0        0      171 2023-07-06 22:26:37.032540 blacklight-0.1.8/blacklight/base/individuals/__init__.py
--rw-r--r--   0        0        0     2470 2023-07-06 22:26:37.032872 blacklight-0.1.8/blacklight/base/individuals/convolution_individual.py
--rw-r--r--   0        0        0     4490 2023-07-06 22:26:37.032961 blacklight-0.1.8/blacklight/base/individuals/feed_forward_individual.py
--rw-r--r--   0        0        0        0 2023-07-06 22:26:37.033047 blacklight-0.1.8/blacklight/base/individuals/tests/__init__.py
--rw-r--r--   0        0        0     2139 2023-07-06 22:26:37.033466 blacklight-0.1.8/blacklight/base/individuals/tests/test_feedforwardindividual.py
--rw-r--r--   0        0        0     2260 2023-07-06 22:26:37.033553 blacklight-0.1.8/blacklight/base/population.py
--rw-r--r--   0        0        0       75 2023-07-06 22:26:37.033677 blacklight-0.1.8/blacklight/base/populations/__init__.py
--rw-r--r--   0        0        0      139 2023-07-06 22:26:37.033935 blacklight-0.1.8/blacklight/base/utils/__init__.py
--rw-r--r--   0        0        0     2673 2023-07-06 22:26:37.034342 blacklight-0.1.8/blacklight/base/utils/model_creator.py
--rw-r--r--   0        0        0     5856 2023-07-06 22:26:37.034439 blacklight-0.1.8/blacklight/base/utils/model_options.py
--rw-r--r--   0        0        0        0 2023-07-06 22:26:37.034513 blacklight-0.1.8/blacklight/base/utils/tests/__init__.py
--rw-r--r--   0        0        0     2462 2023-07-06 22:26:37.034914 blacklight-0.1.8/blacklight/base/utils/tests/test_model_creator.py
--rw-r--r--   0        0        0     4673 2023-07-06 22:26:37.034984 blacklight-0.1.8/blacklight/base/utils/tests/test_model_options.py
--rw-r--r--   0        0        0       89 2023-07-06 22:26:37.035103 blacklight-0.1.8/blacklight/blacklightDataLoader/__init__.py
--rw-r--r--   0        0        0     6530 2023-07-06 23:01:51.777227 blacklight-0.1.8/blacklight/blacklightDataLoader/blacklight_dataset.py
--rw-r--r--   0        0        0        0 2023-07-06 22:26:37.035616 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/__init__.py
--rw-r--r--   0        0        0     5105 2023-07-06 22:26:37.036062 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.csv
--rw-r--r--   0        0        0    10170 2023-07-06 22:26:37.036218 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.json
--rw-r--r--   0        0        0     4794 2023-07-06 22:26:37.036335 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.parquet
--rw-r--r--   0        0        0     9183 2023-07-06 22:26:37.036456 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.xlsx
--rw-r--r--   0        0        0        0 2023-07-06 22:26:37.036483 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/__init__.py
--rw-r--r--   0        0        0      343 2023-07-06 22:26:37.036689 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/csv_to_other_datatypes.py
--rw-r--r--   0        0        0     4076 2023-07-06 23:01:51.777624 blacklight-0.1.8/blacklight/blacklightDataLoader/tests/test_blacklight_dataset.py
--rw-r--r--   0        0        0      594 2023-07-06 23:08:14.456493 blacklight-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4226 1970-01-01 00:00:00.000000 blacklight-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 02:29:57.726020 blacklight-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3624 2023-07-14 02:29:57.726020 blacklight-0.1.9/README.md
+-rw-r--r--   0        0        0     6148 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/.DS_Store
+-rw-r--r--   0        0        0       56 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/autoML/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/autoML/_convolutional_nn.py
+-rw-r--r--   0        0        0     6148 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/.DS_Store
+-rw-r--r--   0        0        0      139 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/adapters/__init__.py
+-rw-r--r--   0        0        0     1858 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/adapters/adapter.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/adapters/tests/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/adapters/tests/test_adapter.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/analyzers/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/__init__.py
+-rw-r--r--   0        0        0     6530 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/blacklight_dataset.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/tests/__init__.py
+-rw-r--r--   0        0        0     5105 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/tests/data/Iris.csv
+-rw-r--r--   0        0        0    10170 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/tests/data/Iris.json
+-rw-r--r--   0        0        0     4794 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/tests/data/Iris.parquet
+-rw-r--r--   0        0        0     9183 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/tests/data/Iris.xlsx
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/tests/data/__init__.py
+-rw-r--r--   0        0        0      343 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/tests/data/csv_to_other_datatypes.py
+-rw-r--r--   0        0        0     3633 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/data/tests/test_blacklight_dataset.py
+-rw-r--r--   0        0        0     2741 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/model_creator.py
+-rw-r--r--   0        0        0     5928 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/model_options.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/tests/__init__.py
+-rw-r--r--   0        0        0     2440 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/tests/test_model_creator.py
+-rw-r--r--   0        0        0     4669 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/tests/test_model_options.py
+-rw-r--r--   0        0        0     6148 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/utils/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/utils/data_utils.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/engine/utils/tests/test_data_utils.py
+-rw-r--r--   0        0        0     6148 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/.DS_Store
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/__init__.py
+-rw-r--r--   0        0        0      174 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/base/__init__.py
+-rw-r--r--   0        0        0     1419 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/base/chromosome.py
+-rw-r--r--   0        0        0     1523 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/base/individual.py
+-rw-r--r--   0        0        0     2317 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/base/population.py
+-rw-r--r--   0        0        0     6148 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/chromosomes/.DS_Store
+-rw-r--r--   0        0        0      102 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/chromosomes/__init__.py
+-rw-r--r--   0        0        0     7804 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/chromosomes/convolutional_chromosome.py
+-rw-r--r--   0        0        0     5876 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/chromosomes/feed_forward_chromosome.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/chromosomes/tests/__init__.py
+-rw-r--r--   0        0        0     2309 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/chromosomes/tests/test_feed_forward_chromosome.py
+-rw-r--r--   0        0        0      103 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/individuals/__init__.py
+-rw-r--r--   0        0        0     2470 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/individuals/convolution_individual.py
+-rw-r--r--   0        0        0     4524 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/individuals/feed_forward_individual.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/individuals/tests/__init__.py
+-rw-r--r--   0        0        0     2117 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/individuals/tests/test_feedforwardindividual.py
+-rw-r--r--   0        0        0       74 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/populations/__init__.py
+-rw-r--r--   0        0        0     7370 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/populations/_feed_forward.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/populations/tests/__init__.py
+-rw-r--r--   0        0        0     5105 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/populations/tests/data/Iris.csv
+-rw-r--r--   0        0        0      868 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/populations/tests/end_to_end_feed_forward_test.py
+-rw-r--r--   0        0        0      186 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/populations/tests/test_CI_CD.py
+-rw-r--r--   0        0        0     6129 2023-07-14 02:29:57.726020 blacklight-0.1.9/blacklight/genetic/populations/tests/test_feed_forward_population.py
+-rw-r--r--   0        0        0      755 2023-07-14 02:29:57.758022 blacklight-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4392 1970-01-01 00:00:00.000000 blacklight-0.1.9/PKG-INFO
```

### Comparing `blacklight-0.1.8/LICENSE` & `blacklight-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.8/README.md` & `blacklight-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     - ```pip install tensorflow-macos``` 
     - ```pip install tensorflow-metal```
 6. Install the package:
    - ```pip install blacklight```
     
 ## Hypothesis
 
-The hypothesis of this project is that DNN topologies will converge to either a local maximum or an absolute maximum over the evolution process, offering better performance than a DNN with randomly selected topology. For this experiment, the project will use equivalent activation functions (ReLU) and SGD for back-propagation, holding everything except the topology constant.
+The hypothesis of this project is that DNN topologies will converge to either a local maximum or an absolute maximum over the evolution process, offering better performance than a DNN with randomly selected topology. For this experiment, the project will use equivalent activation functions (ReLU) and SGD for back-propagation, holding everything except the topology constant. Updated documentation coming soon.
 
 ## Methodology
 
 The project utilizes a genetic algorithm to evolve the topology of the DNN. The algorithm starts with a randomly generated population of DNN topologies and evaluates their fitness using the accuracy of the model. The fittest individuals are selected for reproduction, while the weaker ones are discarded. The offspring of the selected individuals are then created through crossover and mutation. This process is repeated for a specified number of generations, and the best-performing topology is chosen as the final output.
 
 ## Documentation 
 Documentation can be found at https://blacklightlabs.github.io/blacklight/html/index.html
```

### Comparing `blacklight-0.1.8/blacklight/autoML/_feed_forward.py` & `blacklight-0.1.9/blacklight/genetic/populations/_feed_forward.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from blacklight.base.individuals import FeedForwardIndividual
-from blacklight.blacklightDataLoader import BlacklightDataset
-from blacklight.base.population import Population
-from blacklight.base.utils import ModelConfig
+from blacklight.genetic.individuals import FeedForwardIndividual
+from blacklight.engine.data import BlacklightDataset
+from blacklight.genetic.base import Population
+from blacklight.engine import ModelConfig
 from collections import OrderedDict
-import numpy as np
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 from sklearn.model_selection import train_test_split
 import logging
 
 
 class FeedForward(Population):
@@ -15,98 +14,120 @@
     A population of Feed Forward DNN topologies that will be evaluated utilizing a genetic search.
 
     Parameters:
             number_of_individuals (int): The number of individuals that the user wants in the population.
             num_parents_mating (int): The number of parents that will be used to mate and create the next generation.
             death_percentage (float): The percentage of individuals that will die off each generation.
             number_of_generations (int): The number of generations that the population will be simulated for.
+            options (ModelConfig): ModelConfig Object containing options for the model (e.g. number of layers, number of neurons, etc.).
     """
 
     def __init__(
-            self,
-            number_of_individuals,
-            num_parents_mating,
-            death_percentage,
-            number_of_generations,
-            options):
+        self,
+        number_of_individuals,
+        num_parents_mating,
+        death_percentage,
+        number_of_generations,
+        options,
+    ):
         super().__init__(
             number_of_individuals,
             num_parents_mating,
             death_percentage,
             number_of_generations,
-            options)
+            options,
+        )
         self.num_classes = None
         self.test_data = None
         self.problem_type_individual = None
         self.model_history = None
         self.model = None
         self.data = None
         self.num_individuals = number_of_individuals
         self.num_parents_mating = num_parents_mating
         self.num_generations = number_of_generations
         self.death_percentage = death_percentage
         self.problem_type = None
         self.options = ModelConfig.parse_options_to_model_options(options)
 
     def _initialize_individuals(self):
-        self.individuals = OrderedDict({FeedForwardIndividual(
-            self.options, self, None): f"{i}" for i in range(self.num_individuals)})
+        """
+        Initialize the individuals in this population.
+        Returns:
+
+        """
+        self.individuals = OrderedDict(
+            {
+                FeedForwardIndividual(self.options, self, None): f"{i}"
+                for i in range(self.num_individuals)
+            }
+        )
 
     def fit(self, X_train, y_train=None, X_test=None, y_test=None, **kwargs):
         """
         Fit this population of FeedForward Individuals to the given data, and return the best model.
+        You can pass ONLY x if and only if you have a column in your dataset (if pandas) called labels or label.
+        You can also do this if you have a numpy array with the label column at position -1.
+        Otherwise, you must pass X_train and y_train. If you pass X_test and y_test, then the model will be evaluated
+        on the test data after each generation. If not, then test train split will be applied with an 80/20 split.
 
         Parameters:
                 X: The data to fit this population to. Has to be either a pandas dataframe with columns: [feature1, feature2, ..., featureN, label] or a file path to a file of formats specified in `ref: dataLoaders.dataLoader.choose_data_loader` that have the same layout.
                 **kwargs: Any additional arguments to pass to each :class:`~blacklight.autoML.individuals.FeedForwardIndividual` which is a Keras model.
                 y: The labels of the data. If None, then the labels are assumed to be the last column of the data.
         """
         # Disable tensorflow logging
         import os
-        logging.getLogger('tensorflow').disabled = True
-        os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
+
+        logging.getLogger("tensorflow").disabled = True
+        os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 
         if X_test is not None and y_test is not None:
             self.test_data = BlacklightDataset(
-                X_test, y_test, kwargs.get("batch_size", None))
+                X_test, y_test, kwargs.get("batch_size", None)
+            )
             self.train_data = BlacklightDataset(
-                X_train, y_train, kwargs.get("batch_size", None))
+                X_train, y_train, kwargs.get("batch_size", None)
+            )
         else:
-            data = BlacklightDataset(
-                X_train, y_train, kwargs.get(
-                    "batch_size", None))
+            data = BlacklightDataset(X_train, y_train, kwargs.get("batch_size", None))
             X_train, X_test, y_train, y_test = train_test_split(
-                data.X, data.y, test_size=0.2)
+                data.X, data.y, test_size=0.2
+            )
             self.test_data = BlacklightDataset(
-                X_test, y_test, kwargs.get("batch_size", None))
+                X_test, y_test, kwargs.get("batch_size", None)
+            )
             self.train_data = BlacklightDataset(
-                X_train, y_train, kwargs.get(
-                    "batch_size", None))
+                X_train, y_train, kwargs.get("batch_size", None)
+            )
 
         # Initialize individuals
         self._initialize_individuals()
 
         # Simulate the population for the specified number of generations
         self._simulate()
 
         # Get the best individual
         self.best_individual = list(self.individuals.keys())[0]
-        self.model, self.model_history = self.best_individual.model, self.best_individual.model_history
+        self.model, self.model_history = (
+            self.best_individual.model,
+            self.best_individual.model_history,
+        )
 
     def print_model_summary(self):
         """
         Print the summary of the best model.
         """
         self.model.summary()
 
     def print_model_training_history(self):
-        plt.plot(self.model_history.history['accuracy'])
-        plt.title('model accuracy')
-        plt.ylabel('accuracy')
-        plt.xlabel('epoch')
+        plt.plot(self.model_history.history["accuracy"])
+        plt.title("model accuracy")
+        plt.ylabel("accuracy")
+        plt.xlabel("epoch")
         plt.show()
 
     def predict(self, X):
         """
         Predict the labels of the given data, utilizing the best found model.
 
         Parameters:
@@ -127,29 +148,33 @@
     def _simulate(self):
         """
         Simulate the population for the number of generations.
         Callable method.
         :return:
         """
         print(
-            f"\nSimulating feed forward neural network population with {self.num_individuals} individuals for {self.num_generations} generations.")
+            f"\nSimulating feed forward neural network population with {self.num_individuals} individuals for {self.num_generations} generations."
+        )
         for gen in range(self.num_generations):
             print(f"\nGeneration {gen}")
             print(f"Evaluating Individuals in generation {gen}")
             self._evaluate()
             print(f"\nReproducing Individuals in generation {gen}")
             self._reproduce()
 
     def _evaluate(self):
         """
         Evaluate the fitness of all individuals in the population.
         :return:
         """
-        evaluated_individuals = OrderedDict({individual: individual.get_fitness(
-        ) for individual in tqdm(self.individuals.keys())})
-        self.individuals = OrderedDict(sorted(
-            evaluated_individuals.items(),
-            key=lambda x: x[1],
-            reverse=True))
+        evaluated_individuals = OrderedDict(
+            {
+                individual: individual.get_fitness()
+                for individual in tqdm(self.individuals.keys())
+            }
+        )
+        self.individuals = OrderedDict(
+            sorted(evaluated_individuals.items(), key=lambda x: x[1], reverse=True)
+        )
 
     def _get_fitness(self):
         pass
```

### Comparing `blacklight-0.1.8/blacklight/autoML/tests/data/Iris.csv` & `blacklight-0.1.9/blacklight/engine/data/tests/data/Iris.csv`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.8/blacklight/autoML/tests/test_feed_forward_population.py` & `blacklight-0.1.9/blacklight/genetic/populations/tests/test_feed_forward_population.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from blacklight.autoML._feed_forward import FeedForward
+from blacklight.genetic.populations import FeedForward
+from blacklight.genetic.individuals import FeedForwardIndividual
+from blacklight.engine import ModelConfig
+
 import numpy as np
 import pandas as pd
+
 import unittest.mock
 import pytest
 from unittest.mock import MagicMock
 from collections import OrderedDict
-from blacklight.base.utils import ModelConfig
-from blacklight.base.individuals import FeedForwardIndividual
 import random
 
 
 @pytest.fixture
 def getdata():
     X = np.array([[5.1, 3.5, 1.4, 0.2], [4.9, 3.0, 1.4, 0.2], [4.7, 3.2, 1.3, 0.2], [
         4.6, 3.1, 1.5, 0.2], [4.7, 3.2, 1.3, 0.2], [4.7, 3.2, 1.3, 0.2], [4.7, 3.2, 1.3, 0.2]])
```

### Comparing `blacklight-0.1.8/blacklight/base/chromosomes/base_chromosome.py` & `blacklight-0.1.9/blacklight/genetic/base/chromosome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 
-class BaseChromosome(ABC):
+class Chromosome(ABC):
     """
     Abstract class for a chromosome in an individual. Implements common traits between all chromosomes.
     """
 
     def __init__(self):
         self.genes = None
         self.length = None
```

### Comparing `blacklight-0.1.8/blacklight/base/chromosomes/convolutional_chromosome.py` & `blacklight-0.1.9/blacklight/genetic/chromosomes/convolutional_chromosome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 import random
 from abc import ABC
 import tensorflow as tf
-from tensorflow import keras
-from blacklight.base.chromosomes import BaseChromosome
-from blacklight.base.utils import ModelConfig
-from blacklight.base.utils import BlacklightModel
+from blacklight.genetic.base.chromosome import Chromosome
+from blacklight.engine import BlacklightModel
 
 
-class ConvolutionalChromosome(BaseChromosome, ABC):
+class ConvolutionalChromosome(Chromosome, ABC):
     """
     Convolutional chromosome class, which represents a convolutional neural network architecture.
 
     The class inherits from BaseChromosome and implements methods to generate random genes, mutate
     the chromosome, and create a Keras model based on the genes. The genes represent both the
     convolutional and dense layers of the neural network.
 
@@ -116,15 +114,15 @@
 
             Returns:
                 ConvolutionalChromosome: A new ConvolutionalChromosome instances created through crossover.
 
             Raises:
                 ValueError: If the "flatten" layer is not found in the genes or if the input chromosomes have different input shapes.
             """
-        shorter_chromosome, longer_chromosome = BaseChromosome.get_shortest_chromosome(
+        shorter_chromosome, longer_chromosome = Chromosome.get_shortest_chromosome(
             chromosome_a, chromosome_b)
 
         shorter_conv_part, shorter_dense_part = ConvolutionalChromosome.split_convolutional_dense(
             shorter_chromosome.genes)
         longer_conv_part, longer_dense_part = ConvolutionalChromosome.split_convolutional_dense(
             longer_chromosome.genes)
```

### Comparing `blacklight-0.1.8/blacklight/base/chromosomes/feed_forward_chromosome.py` & `blacklight-0.1.9/blacklight/genetic/chromosomes/feed_forward_chromosome.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
-from blacklight.base.chromosomes.base_chromosome import BaseChromosome
-from blacklight.base.utils import BlacklightModel
-from blacklight.base.utils import ModelConfig
+from blacklight.genetic.base import Chromosome
+from blacklight.engine import BlacklightModel
+from blacklight.engine import ModelConfig
 from typing import List, Optional, Tuple
 from keras import Sequential
 
 import random
 
 
-class FeedForwardChromosome(BaseChromosome):
+class FeedForwardChromosome(Chromosome):
     """
     Feed forward chromosome class representing a feed forward neural network.
 
     Args:
         model_params ModelConfig: The parameters for the Keras model. Defaults to None.
         genes (Optional[List[Tuple[int, str]]], optional): The list of genes representing the neural network structure. Defaults to None.
         mutation_prob (Optional[int], optional): The probability of mutation for the chromosome. Defaults to None.
@@ -88,15 +88,15 @@
             FeedForwardChromosome: A new chromosome created by cross over between the input chromosomes.
 
         Examples:
             >>> chromosome_a = FeedForwardChromosome(input_shape=10)
             >>> chromosome_b = FeedForwardChromosome(input_shape=10)
             >>> new_chromosome = FeedForwardChromosome.cross_over(chromosome_a,chromosome_b)
         """
-        shorter_chromosome, longer_chromosome = BaseChromosome.get_shortest_chromosome(
+        shorter_chromosome, longer_chromosome = Chromosome.get_shortest_chromosome(
             chromosome_a, chromosome_b)
 
         points = random.randint(1, len(shorter_chromosome.genes))
         base_one = shorter_chromosome.genes[:points]
         link_one = longer_chromosome.genes[points:]
 
         base_two = longer_chromosome.genes[:points]
@@ -149,12 +149,15 @@
 
         Examples:
             >>> chromosome = FeedForwardChromosome(input_shape=10)
             >>> model = chromosome.get_model()
         """
         return self.model.get_model()
 
+    def get_model_history(self):
+        return self.model.get_model_history()
+
     def __repr__(self):
         return f"FeedForwardChromosome with genes: {self.genes}"
 
     def __str__(self):
         return f"FeedForwardChromosome with genes: {self.genes} \n and model: {self.model.summary()}"
```

### Comparing `blacklight-0.1.8/blacklight/base/chromosomes/tests/test_feed_forward_chromosome.py` & `blacklight-0.1.9/blacklight/genetic/chromosomes/tests/test_feed_forward_chromosome.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import pytest
-from blacklight.base.chromosomes import FeedForwardChromosome
-from blacklight.base.utils import ModelConfig
+from blacklight.genetic.chromosomes import FeedForwardChromosome
+from blacklight.engine import ModelConfig
 from unittest.mock import MagicMock
 
 
 def get_model_config() -> ModelConfig:
     model_options = {
         "layer_information": {
             "problem_type": "binary_classification",
```

### Comparing `blacklight-0.1.8/blacklight/base/individual.py` & `blacklight-0.1.9/blacklight/genetic/base/individual.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         return True
     return False
 
 
 class Individual(ABC):
     """
     Abstract class for an individual in a population. Implements common traits between all individuals.
-    An individual is a KERAS model.
+    An individual is a KERAS Model.
     Genes are passed down from parents, or instantiated randomly.
     Individual is a base class that implements the basic functionality of an individual.
     Child classes hold specific information for different types of models.
     """
 
     fitness = 0
```

### Comparing `blacklight-0.1.8/blacklight/base/individuals/convolution_individual.py` & `blacklight-0.1.9/blacklight/genetic/individuals/convolution_individual.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.8/blacklight/base/individuals/feed_forward_individual.py` & `blacklight-0.1.9/blacklight/genetic/individuals/feed_forward_individual.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from blacklight.base.individual import Individual
-from blacklight.base.population import Population
-from blacklight.base.chromosomes.feed_forward_chromosome import FeedForwardChromosome
-from blacklight.base.utils import ModelConfig
+from blacklight.genetic.base import Individual
+from blacklight.genetic.base import Population
+from blacklight.genetic.chromosomes import FeedForwardChromosome
+from blacklight.engine import ModelConfig
 
 
 class FeedForwardIndividual(Individual):
     """
     Individual for a feed forward neural network.
 
     Attributes:
@@ -91,14 +91,15 @@
             float: The fitness of the individual.
         """
         # Evaluate the model
         self.model = self.chromosome.get_model()
         fitness = self.chromosome.evaluate_model(
             self.train_data, self.test_data)
         self.fitness = fitness
+        self.model_history = self.chromosome.get_model_history()
 
         return fitness
 
     def mate(self, other_individual):
         """
         Mate with another individual to produce a child.
```

### Comparing `blacklight-0.1.8/blacklight/base/individuals/tests/test_feedforwardindividual.py` & `blacklight-0.1.9/blacklight/genetic/individuals/tests/test_feedforwardindividual.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from unittest.mock import MagicMock
-from blacklight.base.chromosomes.feed_forward_chromosome import FeedForwardChromosome
-from blacklight.base.utils import ModelConfig
-from blacklight.base.individuals import FeedForwardIndividual
+from blacklight.genetic.chromosomes import FeedForwardChromosome
+from blacklight.genetic.individuals import FeedForwardIndividual
+from blacklight.engine import ModelConfig
 
 
 @pytest.fixture
 def model_config():
     model_options = {
         "layer_information": {
             "problem_type": "binary_classification",
```

### Comparing `blacklight-0.1.8/blacklight/base/population.py` & `blacklight-0.1.9/blacklight/genetic/base/population.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
     def _reproduce(self):
         self._kill_off_worst()
         for i in range(self.num_parents_mating):
             parents = np.random.choice(
                 list(self.individuals.keys()), size=2, replace=False)
             child = parents[0].mate(parents[1])
+            # Add individual from Bayesian Optimization.
             self.individuals[child] = f"new_child_{i}"
             self.num_individuals += 1
 
     def get_training_data(self):
         return self.train_data if self.train_data else None
 
     def get_testing_data(self):
```

### Comparing `blacklight-0.1.8/blacklight/base/utils/model_creator.py` & `blacklight-0.1.9/blacklight/engine/model_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
             class_weight=self.model_config.get("class_weight"),
             validation_data=self.model_config.get("validation_data"),
             callbacks=self.model_config.get("callbacks") if self.model_config.get("early_stopping") else None)
 
     def get_model(self):
         return self.model
 
+    def get_model_history(self):
+        return self.model_history
+
     def evaluate_model(self, train_data, test_data):
         # first train the model
         if self.model_history is None:
             self.train_model(train_data)
         # then evaluate the model
         results = self.model.evaluate(
             test_data,
```

### Comparing `blacklight-0.1.8/blacklight/base/utils/model_options.py` & `blacklight-0.1.9/blacklight/engine/model_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,9 +122,10 @@
         config["validation_data"] = options.get("validation_data", None)
         config["use_multiprocessing"] = options.get(
             "use_multiprocessing", False)
         config["early_stopping"] = options.get("early_stopping", True)
         config["callbacks"] = options.get(
             "callbacks", ModelConfig.get_default_callbacks())
         config["output_bias"] = options.get("output_bias", None)
+        config["fitness_metric"] = options.get("fitness_metric", "auc")
 
         return ModelConfig(config)
```

### Comparing `blacklight-0.1.8/blacklight/base/utils/tests/test_model_creator.py` & `blacklight-0.1.9/blacklight/engine/tests/test_model_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import pytest
 import tensorflow as tf
 from unittest.mock import MagicMock
-from blacklight.base.utils import BlacklightModel
-from blacklight.base.utils import ModelConfig
+from blacklight.engine import BlacklightModel
+from blacklight.engine import ModelConfig
 
 # Helper function to create a ModelConfig instance
 
 
 def get_model_config():
     config = {
         "target_layer": (1, "sigmoid"),
```

### Comparing `blacklight-0.1.8/blacklight/base/utils/tests/test_model_options.py` & `blacklight-0.1.9/blacklight/engine/tests/test_model_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from blacklight.base.utils import ModelConfig
+from blacklight.engine import ModelConfig
 
 
 def test_model_config_init():
     config = {
         "target_layer": (1, "sigmoid"),
         "loss": "binary_crossentropy",
         "optimizer": "adam",
```

### Comparing `blacklight-0.1.8/blacklight/blacklightDataLoader/blacklight_dataset.py` & `blacklight-0.1.9/blacklight/engine/data/blacklight_dataset.py`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.csv` & `blacklight-0.1.9/blacklight/genetic/populations/tests/data/Iris.csv`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.json` & `blacklight-0.1.9/blacklight/engine/data/tests/data/Iris.json`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.parquet` & `blacklight-0.1.9/blacklight/engine/data/tests/data/Iris.parquet`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.8/blacklight/blacklightDataLoader/tests/data/Iris.xlsx` & `blacklight-0.1.9/blacklight/engine/data/tests/data/Iris.xlsx`

 * *Files identical despite different names*

### Comparing `blacklight-0.1.8/pyproject.toml` & `blacklight-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "blacklight"
-version = "0.1.8"
+version = "0.1.9"
 description = "AutoML utilizing Genetic Algorithms and Neural Networks"
 authors = ["Cole Agard <ctagard19@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 numpy = "*"
 pandas = "*"
 fastparquet = "*"
 openpyxl = "*"
 matplotlib = "*"
 tqdm = "*"
 scikit-learn = "*"
-scipy = "*"
-tensorflow = {version = "*", markers = "platform_machine != 'arm64'"}
+tensorflow = "*"
+tensorflow-macos = {version = "*", markers = "platform_machine == 'arm64' and sys.platform == 'darwin'"}
+tensorflow-metal = {version = "*", markers = "platform_machine == 'arm64' and sys.platform == 'darwin'"}
+
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 flake8 = "*"
 autopep8 = "*"
+coverage = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `blacklight-0.1.8/PKG-INFO` & `blacklight-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: blacklight
-Version: 0.1.8
+Version: 0.1.9
 Summary: AutoML utilizing Genetic Algorithms and Neural Networks
 Author: Cole Agard
 Author-email: ctagard19@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: fastparquet
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
-Requires-Dist: scipy
-Requires-Dist: tensorflow ; platform_machine != "arm64"
+Requires-Dist: tensorflow
+Requires-Dist: tensorflow-macos ; platform_machine == "arm64" and sys_platform == "darwin"
+Requires-Dist: tensorflow-metal ; platform_machine == "arm64" and sys_platform == "darwin"
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # Blacklight  
 
 [![test](https://github.com/BlackLightLabs/blacklight/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/BlackLightLabs/blacklight/actions/workflows/test.yml) [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/449f7ff90fcb4340a4c90884d15f700a)](https://www.codacy.com/gh/BlackLightLabs/blacklight/dashboard?utm_source=github.com&utm_medium=referral&utm_content=BlackLightLabs/blacklight&utm_campaign=Badge_Coverage) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/449f7ff90fcb4340a4c90884d15f700a)](https://www.codacy.com/gh/BlackLightLabs/blacklight/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=BlackLightLabs/blacklight&amp;utm_campaign=Badge_Grade)![PyPI - Downloads](https://img.shields.io/pypi/dm/blacklight?color=lime&label=Downloads%20from%20PyPi&logoColor=blue)
 
@@ -65,15 +66,15 @@
     - ```pip install tensorflow-macos``` 
     - ```pip install tensorflow-metal```
 6. Install the package:
    - ```pip install blacklight```
     
 ## Hypothesis
 
-The hypothesis of this project is that DNN topologies will converge to either a local maximum or an absolute maximum over the evolution process, offering better performance than a DNN with randomly selected topology. For this experiment, the project will use equivalent activation functions (ReLU) and SGD for back-propagation, holding everything except the topology constant.
+The hypothesis of this project is that DNN topologies will converge to either a local maximum or an absolute maximum over the evolution process, offering better performance than a DNN with randomly selected topology. For this experiment, the project will use equivalent activation functions (ReLU) and SGD for back-propagation, holding everything except the topology constant. Updated documentation coming soon.
 
 ## Methodology
 
 The project utilizes a genetic algorithm to evolve the topology of the DNN. The algorithm starts with a randomly generated population of DNN topologies and evaluates their fitness using the accuracy of the model. The fittest individuals are selected for reproduction, while the weaker ones are discarded. The offspring of the selected individuals are then created through crossover and mutation. This process is repeated for a specified number of generations, and the best-performing topology is chosen as the final output.
 
 ## Documentation 
 Documentation can be found at https://blacklightlabs.github.io/blacklight/html/index.html
```

