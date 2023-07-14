# Comparing `tmp/fsrs4anki_optimizer-4.0.1.tar.gz` & `tmp/fsrs4anki_optimizer-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.0.1.tar", last modified: Thu Jul 13 16:01:56 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.0.2.tar", last modified: Fri Jul 14 02:23:31 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.0.1.tar` & `fsrs4anki_optimizer-4.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49531 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 16:01:56.000000 fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:01:56.713581 fsrs4anki_optimizer-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 16:01:41.000000 fsrs4anki_optimizer-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49737 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 02:23:31.000000 fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 02:23:31.110863 fsrs4anki_optimizer-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 02:23:21.000000 fsrs4anki_optimizer-4.0.2/setup.py
```

### Comparing `fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.0.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.0.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         self.train_set = RevlogDataset(train_set)
         sampler = RevlogSampler(self.train_set, batch_size=self.batch_size)
         self.train_data_loader = DataLoader(self.train_set, batch_sampler=sampler, collate_fn=collate_fn)
 
         self.test_set = RevlogDataset(test_set)
         sampler = RevlogSampler(self.test_set, batch_size=self.batch_size)
         self.test_data_loader = DataLoader(self.test_set, batch_sampler=sampler, collate_fn=collate_fn)
-        print("dataset built")
+        tqdm.write("dataset built")
 
     def train(self, verbose: bool=True):
         best_loss = np.inf
         epoch_len = len(self.next_train_data_loader)
         pbar = tqdm(desc="train", colour="red", total=epoch_len*self.n_epoch)
         print_len = max(self.batch_nums*self.n_epoch // 10, 1)
         for k in range(self.n_epoch):
@@ -258,24 +258,22 @@
             sequences, delta_ts, labels, seq_lens = self.train_set.x_train, self.train_set.t_train, self.train_set.y_train, self.train_set.seq_len
             real_batch_size = seq_lens.shape[0]
             outputs, _ = self.model(sequences.transpose(0, 1))
             stabilities = outputs[seq_lens-1, torch.arange(real_batch_size), 0]
             retentions = power_forgetting_curve(delta_ts, stabilities)
             tran_loss = self.loss_fn(retentions, labels).mean()
             self.avg_train_losses.append(tran_loss)
-            tqdm.write(f"Loss in trainset: {tran_loss:.4f}")
 
             sequences, delta_ts, labels, seq_lens = self.test_set.x_train, self.test_set.t_train, self.test_set.y_train, self.test_set.seq_len
             real_batch_size = seq_lens.shape[0]
             outputs, _ = self.model(sequences.transpose(0, 1))
             stabilities = outputs[seq_lens-1, torch.arange(real_batch_size), 0]
             retentions = power_forgetting_curve(delta_ts, stabilities)
             test_loss = self.loss_fn(retentions, labels).mean()
             self.avg_eval_losses.append(test_loss)
-            tqdm.write(f"Loss in testset: {test_loss:.4f}")
 
             w = list(map(lambda x: round(float(x), 4), dict(self.model.named_parameters())['w'].data))
 
             weighted_loss = (tran_loss * len(self.train_set) + test_loss * len(self.test_set)) / (len(self.train_set) + len(self.test_set))
 
             return weighted_loss, w
 
@@ -314,15 +312,15 @@
 
     @staticmethod
     def anki_extract(filename: str):
         """Step 1"""
         # Extract the collection file or deck file to get the .anki21 database.
         with zipfile.ZipFile(f'{filename}', 'r') as zip_ref:
             zip_ref.extractall('./')
-            print("Deck file extracted successfully!")
+            tqdm.write("Deck file extracted successfully!")
 
     def create_time_series(self, timezone: str, revlog_start_date: str, next_day_starts_at: int, filter_out_suspended_cards: bool = False):
         """Step 2"""
         if os.path.isfile("collection.anki21b"):
             os.remove("collection.anki21b")
             raise Exception(
                 "Please export the file with `support older Anki versions` if you use the latest version of Anki.")
@@ -370,15 +368,15 @@
         df = df[df['mask'] == True].copy()
         df.drop(columns=['is_learn_start', 'sequence_group', 'last_learn_start', 'mask'], inplace=True)
         df = df[(df['type'] != 4)].copy()
 
         self.type_sequence = np.array(df['type'])
         self.time_sequence = np.array(df['time'])
         df.to_csv("revlog.csv", index=False)
-        print("revlog.csv saved.")
+        tqdm.write("revlog.csv saved.")
 
         df = df[(df['type'] != 3) | (df['factor'] != 0)].copy()
         df['real_days'] = df['review_date'] - timedelta(hours=int(next_day_starts_at))
         df['real_days'] = pd.DatetimeIndex(df['real_days'].dt.floor('D', ambiguous='infer', nonexistent='shift_forward')).to_julian_date()
         df.drop_duplicates(['cid', 'real_days'], keep='first', inplace=True)
         df['delta_t'] = df.real_days.diff()
         df.dropna(inplace=True)
@@ -398,22 +396,22 @@
         t_history = df.groupby('cid', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[int(i)] for i in x]))
         df['t_history']=[','.join(map(str, item[:-1])) for sublist in t_history for item in sublist]
         r_history = df.groupby('cid', group_keys=False)['r'].apply(lambda x: cum_concat([[i] for i in x]))
         df['r_history']=[','.join(map(str, item[:-1])) for sublist in r_history for item in sublist]
         df = df.groupby('cid').filter(lambda group: group['id'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
         df['y'] = df['r'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
         df.to_csv('revlog_history.tsv', sep="\t", index=False)
-        print("Trainset saved.")
+        tqdm.write("Trainset saved.")
 
         S0_dataset = df[df['i'] == 2]
         self.S0_dataset_group = S0_dataset.groupby(by=['r_history', 'delta_t'], group_keys=False).agg({'y': ['mean', 'count']}).reset_index()
 
         df['retention'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['y'].transform('mean')
         df['total_cnt'] = df.groupby(by=['r_history', 'delta_t'], group_keys=False)['id'].transform('count')
-        print("Retention calculated.")
+        tqdm.write("Retention calculated.")
 
         df = df.drop(columns=['id', 'cid', 'usn', 'ivl', 'last_ivl', 'factor', 'time', 'type', 'create_date', 'review_date', 'real_days', 'r', 't_history', 'y'])
         df.drop_duplicates(inplace=True)
         df['retention'] = df['retention'].map(lambda x: max(min(0.99, x), 0.01))
 
         def cal_stability(group: pd.DataFrame) -> pd.DataFrame:
             group_cnt = sum(group['total_cnt'])
@@ -430,30 +428,30 @@
             group['avg_interval'] = round(sum(group['delta_t'] * pow(group['total_cnt'], 2)) / sum(pow(group['total_cnt'], 2)), 1)
             del group['total_cnt']
             del group['retention']
             del group['delta_t']
             return group
 
         df = df.groupby(by=['r_history'], group_keys=False).progress_apply(cal_stability)
-        print("Stability calculated.")
+        tqdm.write("Stability calculated.")
         df.reset_index(drop = True, inplace = True)
         df.drop_duplicates(inplace=True)
         df.sort_values(by=['r_history'], inplace=True, ignore_index=True)
 
         if df.shape[0] > 0:
             for idx in tqdm(df.index, desc="analysis"):
                 item = df.loc[idx]
                 index = df[(df['i'] == item['i'] + 1) & (df['r_history'].str.startswith(item['r_history']))].index
                 df.loc[index, 'last_stability'] = item['stability']
             df['factor'] = round(df['stability'] / df['last_stability'], 2)
             df = df[(df['i'] >= 2) & (df['group_cnt'] >= 100)].copy()
             df['last_recall'] = df['r_history'].map(lambda x: x[-1])
             df = df[df.groupby(['i', 'r_history'], group_keys=False)['group_cnt'].transform(max) == df['group_cnt']]
             df.to_csv('./stability_for_analysis.tsv', sep='\t', index=None)
-            print("Analysis saved!")
+            tqdm.write("Analysis saved!")
             caption = "1:again, 2:hard, 3:good, 4:easy\n"
             analysis = df[df['r_history'].str.contains(r'^[1-4][^124]*$', regex=True)][['r_history', 'avg_interval', 'avg_retention', 'stability', 'factor', 'group_cnt']].to_string(index=False)
             return caption + analysis
 
     def define_model(self):
         """Step 3"""
         self.init_w = [1, 2, 3, 4, 5, 0.5, 0.5, 0.2, 1.4, 0.2, 0.8, 2, 0.2, 0.2, 1, 0.5, 2]
@@ -471,72 +469,74 @@
         w[10]: next_stability_difficulty_decay_after_success
         w[11]: next_stability_stability_gain_after_failure
         w[12]: next_stability_retrievability_gain_after_failure
         For more details about the parameters, please see: 
         https://github.com/open-spaced-repetition/fsrs4anki/wiki/Free-Spaced-Repetition-Scheduler
         '''
 
-    def pretrain(self):
+    def pretrain(self, verbose=True):
         rating_stability = {}
         rating_count = {}
 
         for first_rating in ("1", "2", "3", "4"):
             group = self.S0_dataset_group[self.S0_dataset_group['r_history'] == first_rating]
             if group.empty:
                 continue
             delta_t = group['delta_t']
             recall = group['y']['mean']
             count = group['y']['count']
-            if sum(count) < 100:
-                print(f'Not enough data for first rating {first_rating}. Expected at least 100, got {sum(count)}.')
+            total_count = sum(count)
+            if total_count < 100:
+                tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got {total_count}.')
                 continue
-            params, covs = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (3650)))
-            rating_stability[int(first_rating)] = params[0]
-            rating_count[int(first_rating)] = sum(count)
-            print('Weighted fit parameters:', params)
-            print('Number of reviews:', sum(count))
+            params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (365)))
+            stability = params[0]
+            rating_stability[int(first_rating)] = stability
+            rating_count[int(first_rating)] = total_count
             predict_recall = power_forgetting_curve(delta_t, *params)
-            print(f'RMSE: {mean_squared_error(recall, predict_recall, sample_weight=count, squared=False):.4f}')
+            rmse = mean_squared_error(recall, predict_recall, sample_weight=count, squared=False)
 
-            plt.plot(delta_t, recall, label='Exact')
-            plt.plot(np.linspace(0, 30), power_forgetting_curve(np.linspace(0, 30), *params), label='Weighted fit')
-            count_percent = np.array([x/sum(count) for x in count])
-            plt.scatter(delta_t, recall, s=count_percent * 1000, alpha=0.5)
-            plt.legend(loc='upper right', fancybox=True, shadow=False)
-            plt.grid(True)
-            plt.ylim(0, 1)
-            plt.xlim(0, 30)
-            plt.xlabel('Interval')
-            plt.ylabel('Recall')
-            plt.title('Forgetting curve for first rating ' + first_rating)
-            plt.show()
+            if verbose:
+                plt.plot(delta_t, recall, label='Exact')
+                plt.plot(np.linspace(0, 30), power_forgetting_curve(np.linspace(0, 30), *params), label=f'Weighted fit (RMSE: {rmse:.4f})')
+                count_percent = np.array([x/total_count for x in count])
+                plt.scatter(delta_t, recall, s=count_percent * 1000, alpha=0.5)
+                plt.legend(loc='upper right', fancybox=True, shadow=False)
+                plt.grid(True)
+                plt.ylim(0, 1)
+                plt.xlim(0, 30)
+                plt.xlabel('Interval')
+                plt.ylabel('Recall')
+                plt.title(f'Forgetting curve for first rating {first_rating} (n={total_count}, s={stability:.2f})')
+                plt.show()
+                tqdm.write(str(rating_stability))
 
-        print(rating_stability)
         if len(rating_stability) < 2:
             raise Exception("Not enough data for pretraining!")
 
         def S0_rating_curve(rating, a, b, c):
             return np.exp(a + b * rating) + c
 
         params, covs = curve_fit(S0_rating_curve, list(rating_stability.keys()), list(rating_stability.values()), sigma=1/np.sqrt(list(rating_count.values())), method='dogbox', bounds=((-15, 0.03, -5), (15, 7, 30)))
-        print('Weighted fit parameters:', params)
-        predict_stability = S0_rating_curve(np.array(list(rating_stability.keys())), *params)
-        print("Fit stability:", predict_stability)
-        print(f'RMSE: {mean_squared_error(list(rating_stability.values()), predict_stability, sample_weight=list(rating_count.values()), squared=False):.4f}')
-        plt.plot(list(rating_stability.keys()), list(rating_stability.values()), label='Exact')
-        plt.plot(list(rating_stability.keys()), predict_stability, label='Weighted fit')
-        plt.legend(loc='upper right', fancybox=True, shadow=False)
-        plt.grid(True)
-        plt.xlabel('First rating')
-        plt.ylabel('Stability')
-        plt.title('Stability for first rating')
-        plt.show()
+        if verbose:
+            tqdm.write(f'Weighted fit parameters: {params}')
+            predict_stability = S0_rating_curve(np.array(list(rating_stability.keys())), *params)
+            tqdm.write(f"Fit stability: {predict_stability}")
+            tqdm.write(f'RMSE: {mean_squared_error(list(rating_stability.values()), predict_stability, sample_weight=list(rating_count.values()), squared=False):.4f}')
+            plt.plot(list(rating_stability.keys()), list(rating_stability.values()), label='Exact')
+            plt.plot(list(rating_stability.keys()), predict_stability, label='Weighted fit')
+            plt.legend(loc='upper right', fancybox=True, shadow=False)
+            plt.grid(True)
+            plt.xlabel('First rating')
+            plt.ylabel('Stability')
+            plt.title('Stability for first rating')
+            plt.show()
 
         for rating in (1, 2, 3, 4):
-            again_extrap = max(min(S0_rating_curve(1, *params), 3650), 0.1)
+            again_extrap = max(min(S0_rating_curve(1, *params), 365), 0.1)
             # if there isn't enough data to calculate the value for "Again" exactly
             if 1 not in rating_stability:
                 # then check if there exists an exact value for "Hard"
                 if 2 in rating_stability:
                     # if it exists, then check whether the extrapolation breaks monotonicity
                     # Again > Hard is possible, but we should allow it only for exact values, otherwise we should assume monotonicity
                     if again_extrap > rating_stability[2]:
@@ -545,52 +545,52 @@
                     else:
                         # if it doesn't break monotonicity, then use the extrapolated value
                         rating_stability[1] = again_extrap
                 # if an exact value for "Hard" doesn't exist, then just use the extrapolation, there's nothing else we can do
                 else:
                     rating_stability[1] = again_extrap
             elif rating not in rating_stability:
-                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 3650), 0.1)
+                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 365), 0.1)
 
         rating_stability = {k: round(v, 2) for k, v in sorted(rating_stability.items(), key=lambda item: item[0])}
         for rating, stability in rating_stability.items():
             self.init_w[rating-1] = stability
-        
+        tqdm.write(f"Pretrain finished!")
 
     def train(self, lr: float = 4e-2, n_epoch: int = 5, n_splits: int = 5, batch_size: int = 512, verbose: bool = True):
         """Step 4"""
         self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
         self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
         if self.dataset.empty:
             raise ValueError('Training data is inadequate.')
         self.dataset['tensor'] = self.dataset.progress_apply(lambda x: lineToTensor(list(zip([x['t_history']], [x['r_history']]))[0]), axis=1)
         self.dataset['group'] = self.dataset['r_history'] + self.dataset['t_history']
-        print("Tensorized!")
+        tqdm.write("Tensorized!")
 
         w = []
         plots = []
         if n_splits > 1:
             sgkf = StratifiedGroupKFold(n_splits=n_splits)
             for train_index, test_index in sgkf.split(self.dataset, self.dataset['i'], self.dataset['group']):
-                print("TRAIN:", len(train_index), "TEST:",  len(test_index))
+                tqdm.write(f"TRAIN: {len(train_index)} TEST: {len(test_index)}")
                 train_set = self.dataset.iloc[train_index].copy()
                 test_set = self.dataset.iloc[test_index].copy()
                 trainer = Trainer(train_set, test_set, self.init_w, n_epoch=n_epoch, lr=lr, batch_size=batch_size)
                 w.append(trainer.train(verbose=verbose))
                 plots.append(trainer.plot())
         else:
             trainer = Trainer(self.dataset, self.dataset, self.init_w, n_epoch=n_epoch, lr=lr, batch_size=batch_size)
             w.append(trainer.train(verbose=verbose))
             plots.append(trainer.plot())
 
         w = np.array(w)
         avg_w = np.round(np.mean(w, axis=0), 4)
         self.w = avg_w.tolist()
 
-        print("\nTraining finished!")
+        tqdm.write("\nTraining finished!")
         return plots
 
     def preview(self, requestRetention: float):
         my_collection = Collection(self.w)
         preview_text = "1:again, 2:hard, 3:good, 4:easy\n"
         for first_rating in (1,2,3,4):
             preview_text += f'\nfirst rating: {first_rating}\n'
@@ -616,15 +616,14 @@
         my_collection = Collection(self.w)
 
         t_history = "0"
         d_history = "0"
         for i in range(len(test_rating_sequence.split(','))):
             r_history = test_rating_sequence[:2*i+1]
             states = my_collection.predict(t_history, r_history)
-            print(states)
             next_t = next_interval(states[0], requestRetention)
             t_history += f',{int(next_t)}'
             difficulty = round(float(states[1]), 1)
             d_history += f',{difficulty}'
         preview_text = f"rating history: {test_rating_sequence}\n"
         preview_text += f"interval history: {t_history}\n"
         preview_text += f"difficulty history: {d_history}"
@@ -639,15 +638,15 @@
         self.dataset['stability'] = list(stabilities)
         self.dataset['difficulty'] = list(difficulties)
         prediction = self.dataset.groupby(by=['t_history', 'r_history']).agg({"stability": "mean", "difficulty": "mean", "id": "count"})
         prediction.reset_index(inplace=True)
         prediction.sort_values(by=['r_history'], inplace=True)
         prediction.rename(columns={"id": "count"}, inplace=True)
         prediction.to_csv("./prediction.tsv", sep='\t', index=None)
-        print("prediction.tsv saved.")
+        tqdm.write("prediction.tsv saved.")
         prediction['difficulty'] = prediction['difficulty'].map(lambda x: int(round(x)))
         self.difficulty_distribution = prediction.groupby(by=['difficulty'])['count'].sum() / prediction['count'].sum()
         self.difficulty_distribution_padding = np.zeros(10)
         for i in range(10):
             if i+1 in self.difficulty_distribution.index:
                 self.difficulty_distribution_padding[i] = self.difficulty_distribution.loc[i+1]
         return self.difficulty_distribution
@@ -679,16 +678,16 @@
             last_t = t
 
         r_time = round(type_time[1]/type_count[1]/1000, 1)
 
         if 2 in type_count and 2 in type_block:
             f_time = round(type_time[2]/type_block[2]/1000 + r_time, 1)
 
-        print(f"average time for failed cards: {f_time}s")
-        print(f"average time for recalled cards: {r_time}s")
+        tqdm.write(f"average time for failed cards: {f_time}s")
+        tqdm.write(f"average time for recalled cards: {r_time}s")
 
         def stability2index(stability):
             return (np.log(stability) / np.log(base)).round().astype(int) + index_offset
 
         def cal_next_recall_stability(s, r, d, response):
             if response == 1:
                 return s * (1 + np.exp(self.w[8]) * (11 - d) * np.power(s, -self.w[9]) * (np.exp((1 - r) * self.w[10]) - 1))
@@ -696,15 +695,15 @@
                 return np.minimum(self.w[11] * np.power(d, -self.w[12]) * (np.power(s + 1, self.w[13]) - 1) * np.exp((1 - r) * self.w[14]), s)
 
         terminal_stability = minimum_stability
         for _ in range(128):
             terminal_stability = cal_next_recall_stability(terminal_stability, 0.96, d_range, 1)
         index_len = stability2index(terminal_stability)
         stability_list = np.array([np.power(base, i - index_offset) for i in range(index_len)])
-        print(f"terminal stability: {stability_list.max(): .2f}")
+        tqdm.write(f"terminal stability: {stability_list.max(): .2f}")
         df = pd.DataFrame(columns=["retention", "difficulty", "time"])
 
         for percentage in tqdm(range(96, 66, -2), desc="find optimal retention"):
             recall = percentage / 100
             time_list = np.zeros((d_range, index_len))
             time_list[:,:-1] = max_time
             for d in range(d_range, 0, -1):
@@ -731,29 +730,29 @@
                     time_list[d - 1][s_indices[mask]] = exp_times[mask]
                     diff = total_time - time_list[d - 1].sum()
                     s0_time = time_list[d - 1][s0_index]
                 df.loc[0 if pd.isnull(df.index.max()) else df.index.max() + 1] = [recall, d, s0_time]
 
         df.sort_values(by=["difficulty", "retention"], inplace=True)
         df.to_csv("./expected_time.csv", index=False)
-        print("expected_time.csv saved.")
+        tqdm.write("expected_time.csv saved.")
 
         optimal_retention_list = np.zeros(10)
         fig = plt.figure()
         ax = fig.gca()
         for d in range(1, d_range+1):
             retention = df[df["difficulty"] == d]["retention"]
             cost = df[df["difficulty"] == d]["time"]
             optimal_retention = retention.iat[cost.argmin()]
             optimal_retention_list[d-1] = optimal_retention
             ax.plot(retention, cost, label=f"d={d}, r={optimal_retention}")
         
         self.optimal_retention = np.inner(self.difficulty_distribution_padding, optimal_retention_list)
 
-        print(f"\n-----suggested retention (experimental): {self.optimal_retention:.2f}-----")
+        tqdm.write(f"\n-----suggested retention (experimental): {self.optimal_retention:.2f}-----")
 
         ax.set_ylabel("expected time (second)")
         ax.set_xlabel("retention")
         ax.legend()
         ax.grid()
         ax.semilogy()
         return (fig, )
@@ -786,15 +785,15 @@
         return loss_before, loss_after
 
     def calibration_graph(self):
         fig1 = plt.figure()
         plot_brier(self.dataset['p'], self.dataset['y'], bins=40, ax=fig1.add_subplot(111))
         fig2 = plt.figure(figsize=(16, 12))
         for last_rating in ("1","2","3","4"):
-            print(f"\nLast rating: {last_rating}")
+            tqdm.write(f"\nLast rating: {last_rating}")
             plot_brier(self.dataset[self.dataset['r_history'].str.endswith(last_rating)]['p'], self.dataset[self.dataset['r_history'].str.endswith(last_rating)]['y'], bins=40, ax=fig2.add_subplot(2, 2, int(last_rating)), title=f"Last rating: {last_rating}")
 
         def to_percent(temp, position):
             return '%1.0f' % (100 * temp) + '%'
 
         fig3 = plt.figure()
         ax1 = fig3.add_subplot(111)
@@ -871,15 +870,15 @@
         B_W_Metric_pivot = B_W_Metric[B_W_Metric_count['p'] > max(50, n / (3 * bins))].pivot(index="s_bin", columns='d_bin', values='B-W')
         return B_W_Metric_pivot.apply(pd.to_numeric).style.background_gradient(cmap='seismic', axis=None, vmin=-0.2, vmax=0.2).format("{:.2%}", na_rep='')
 
     def compare_with_sm2(self):
         self.dataset['sm2_ivl'] = self.dataset['tensor'].map(sm2)
         self.dataset['sm2_p'] = np.exp(np.log(0.9) * self.dataset['delta_t'] / self.dataset['sm2_ivl'])
         self.dataset['log_loss'] = self.dataset.apply(lambda row: - np.log(row['sm2_p']) if row['y'] == 1 else - np.log(1 - row['sm2_p']), axis=1)
-        print(f"Loss of SM-2: {self.dataset['log_loss'].mean():.4f}")
+        tqdm.write(f"Loss of SM-2: {self.dataset['log_loss'].mean():.4f}")
         cross_comparison = self.dataset[['sm2_p', 'p', 'y']].copy()
         fig1 = plt.figure()
         plot_brier(cross_comparison['sm2_p'], cross_comparison['y'], bins=40, ax=fig1.add_subplot(111))
 
         fig2 = plt.figure(figsize=(6, 6))
         ax = fig2.gca()
 
@@ -887,21 +886,21 @@
         cross_comparison['SM2_bin'] = cross_comparison['sm2_p'].map(lambda x: round(x, 1))
         cross_comparison['FSRS_B-W'] = cross_comparison['p'] - cross_comparison['y']
         cross_comparison['FSRS_bin'] = cross_comparison['p'].map(lambda x: round(x, 1))
 
         ax.axhline(y = 0.0, color = 'black', linestyle = '-')
 
         cross_comparison_group = cross_comparison.groupby(by='SM2_bin').agg({'y': ['mean'], 'FSRS_B-W': ['mean'], 'p': ['mean', 'count']})
-        print(f"Universal Metric of FSRS: {mean_squared_error(cross_comparison_group['y', 'mean'], cross_comparison_group['p', 'mean'], sample_weight=cross_comparison_group['p', 'count'], squared=False):.4f}")
+        tqdm.write(f"Universal Metric of FSRS: {mean_squared_error(cross_comparison_group['y', 'mean'], cross_comparison_group['p', 'mean'], sample_weight=cross_comparison_group['p', 'count'], squared=False):.4f}")
         cross_comparison_group['p', 'percent'] = cross_comparison_group['p', 'count'] / cross_comparison_group['p', 'count'].sum()
         ax.scatter(cross_comparison_group.index, cross_comparison_group['FSRS_B-W', 'mean'], s=cross_comparison_group['p', 'percent'] * 1024, alpha=0.5)
         ax.plot(cross_comparison_group['FSRS_B-W', 'mean'], label='FSRS by SM2')
 
         cross_comparison_group = cross_comparison.groupby(by='FSRS_bin').agg({'y': ['mean'], 'SM2_B-W': ['mean'], 'sm2_p': ['mean', 'count']})
-        print(f"Universal Metric of SM2: {mean_squared_error(cross_comparison_group['y', 'mean'], cross_comparison_group['sm2_p', 'mean'], sample_weight=cross_comparison_group['sm2_p', 'count'], squared=False):.4f}")
+        tqdm.write(f"Universal Metric of SM2: {mean_squared_error(cross_comparison_group['y', 'mean'], cross_comparison_group['sm2_p', 'mean'], sample_weight=cross_comparison_group['sm2_p', 'count'], squared=False):.4f}")
         cross_comparison_group['sm2_p', 'percent'] = cross_comparison_group['sm2_p', 'count'] / cross_comparison_group['sm2_p', 'count'].sum()
         ax.scatter(cross_comparison_group.index, cross_comparison_group['SM2_B-W', 'mean'], s=cross_comparison_group['sm2_p', 'percent'] * 1024, alpha=0.5)
         ax.plot(cross_comparison_group['SM2_B-W', 'mean'], label='SM2 by FSRS')
 
         ax.legend(loc='lower center')
         ax.grid(linestyle='--')
         ax.set_title("SM2 vs. FSRS")
@@ -943,21 +942,21 @@
 def plot_brier(predictions, real, bins=20, ax=None, title=None):
     brier = load_brier(predictions, real, bins=bins)
     bin_prediction_means = brier['detail']['bin_prediction_means']
     bin_correct_means = brier['detail']['bin_correct_means']
     bin_counts = brier['detail']['bin_counts']
     r2 = r2_score(bin_correct_means, bin_prediction_means, sample_weight=bin_counts)
     rmse = np.sqrt(mean_squared_error(bin_correct_means, bin_prediction_means, sample_weight=bin_counts))
-    print(f"R-squared: {r2:.4f}")
-    print(f"RMSE: {rmse:.4f}")
+    tqdm.write(f"R-squared: {r2:.4f}")
+    tqdm.write(f"RMSE: {rmse:.4f}")
     ax.set_xlim([0, 1])
     ax.set_ylim([0, 1])
     ax.grid(True)
     fit_wls = sm.WLS(bin_correct_means, sm.add_constant(bin_prediction_means), weights=bin_counts).fit()
-    print(fit_wls.params)
+    tqdm.write(str(fit_wls.params))
     y_regression = [fit_wls.params[0] + fit_wls.params[1]*x for x in bin_prediction_means]
     ax.plot(bin_prediction_means, y_regression, label='Weighted Least Squares Regression', color="green")
     ax.plot(bin_prediction_means, bin_correct_means, label='Actual Calibration', color="#1f77b4")
     ax.plot((0, 1), (0, 1), label='Perfect Calibration', color="#ff7f0e")
     bin_count = brier['detail']['bin_count']
     counts = np.array(bin_counts)
     bins = (np.arange(bin_count) + 0.5) / bin_count
```

