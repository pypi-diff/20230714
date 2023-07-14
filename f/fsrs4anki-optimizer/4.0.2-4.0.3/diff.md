# Comparing `tmp/fsrs4anki_optimizer-4.0.2.tar.gz` & `tmp/fsrs4anki_optimizer-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.0.2.tar", last modified: Fri Jul 14 02:23:31 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.0.3.tar", last modified: Fri Jul 14 06:13:39 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.0.2.tar` & `fsrs4anki_optimizer-4.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49737 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50026 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 06:13:39.000000 fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:13:39.965233 fsrs4anki_optimizer-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 06:13:24.000000 fsrs4anki_optimizer-4.0.3/setup.py
```

### Comparing `fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.0.3/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,14 +508,19 @@
                 plt.ylabel('Recall')
                 plt.title(f'Forgetting curve for first rating {first_rating} (n={total_count}, s={stability:.2f})')
                 plt.show()
                 tqdm.write(str(rating_stability))
 
         if len(rating_stability) < 2:
             raise Exception("Not enough data for pretraining!")
+        elif len(rating_stability) == 4:
+            for rating, stability in rating_stability.items():
+                self.init_w[rating-1] = round(stability, 2)
+            tqdm.write(f"Pretrain finished!")
+            return
 
         def S0_rating_curve(rating, a, b, c):
             return np.exp(a + b * rating) + c
 
         params, covs = curve_fit(S0_rating_curve, list(rating_stability.keys()), list(rating_stability.values()), sigma=1/np.sqrt(list(rating_count.values())), method='dogbox', bounds=((-15, 0.03, -5), (15, 7, 30)))
         if verbose:
             tqdm.write(f'Weighted fit parameters: {params}')
@@ -572,19 +577,21 @@
             sgkf = StratifiedGroupKFold(n_splits=n_splits)
             for train_index, test_index in sgkf.split(self.dataset, self.dataset['i'], self.dataset['group']):
                 tqdm.write(f"TRAIN: {len(train_index)} TEST: {len(test_index)}")
                 train_set = self.dataset.iloc[train_index].copy()
                 test_set = self.dataset.iloc[test_index].copy()
                 trainer = Trainer(train_set, test_set, self.init_w, n_epoch=n_epoch, lr=lr, batch_size=batch_size)
                 w.append(trainer.train(verbose=verbose))
-                plots.append(trainer.plot())
+                if verbose:
+                    plots.append(trainer.plot())
         else:
             trainer = Trainer(self.dataset, self.dataset, self.init_w, n_epoch=n_epoch, lr=lr, batch_size=batch_size)
             w.append(trainer.train(verbose=verbose))
-            plots.append(trainer.plot())
+            if verbose:
+                plots.append(trainer.plot())
 
         w = np.array(w)
         avg_w = np.round(np.mean(w, axis=0), 4)
         self.w = avg_w.tolist()
 
         tqdm.write("\nTraining finished!")
         return plots
```

