# Comparing `tmp/b2sim-1.1.0.tar.gz` & `tmp/b2sim-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.1.0.tar", last modified: Tue Jul 11 04:30:16 2023, max compression
+gzip compressed data, was "b2sim-1.1.1.tar", last modified: Fri Jul 14 02:57:14 2023, max compression
```

## Comparing `b2sim-1.1.0.tar` & `b2sim-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-12 23:51:19.069376 b2sim-1.1.0/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.1.0/LICENSE
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.1.0/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-12 23:51:19.054637 b2sim-1.1.0/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    13601 2023-07-12 23:50:40.000000 b2sim-1.1.0/README.md
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-12 23:51:18.482022 b2sim-1.1.0/b2sim/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.1.0/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    10817 2023-07-12 23:37:31.000000 b2sim-1.1.0/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     8804 2023-07-12 20:35:37.000000 b2sim-1.1.0/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   103530 2023-07-12 23:42:28.000000 b2sim-1.1.0/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     3818 2023-07-04 23:08:48.000000 b2sim-1.1.0/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-12 23:51:18.923626 b2sim-1.1.0/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-07-12 20:07:14.000000 b2sim-1.1.0/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      418 2023-07-11 02:24:19.000000 b2sim-1.1.0/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-12 23:51:18.772886 b2sim-1.1.0/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-12 23:51:19.073328 b2sim-1.1.0/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-12 19:38:52.000000 b2sim-1.1.0/setup.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-14 02:57:14.893132 b2sim-1.1.1/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.1.1/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.1.1/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-14 02:57:14.884618 b2sim-1.1.1/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    12903 2023-07-12 18:41:22.000000 b2sim-1.1.1/README.md
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-14 02:57:14.265361 b2sim-1.1.1/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.1.1/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    10817 2023-07-12 23:37:31.000000 b2sim-1.1.1/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     8804 2023-07-12 20:35:37.000000 b2sim-1.1.1/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   103703 2023-07-14 02:24:33.000000 b2sim-1.1.1/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     4135 2023-07-14 02:54:35.000000 b2sim-1.1.1/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-14 02:57:14.768344 b2sim-1.1.1/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-07-12 20:07:14.000000 b2sim-1.1.1/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      418 2023-07-12 18:41:22.000000 b2sim-1.1.1/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-14 02:57:14.524260 b2sim-1.1.1/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-14 02:57:13.000000 b2sim-1.1.1/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-14 02:57:14.896128 b2sim-1.1.1/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-14 02:25:19.000000 b2sim-1.1.1/setup.py
```

### Comparing `b2sim-1.1.0/LICENSE` & `b2sim-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.1.0/README.md` & `b2sim-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 ## For noobs:
 1. Install python on your computer here: https://www.anaconda.com/download/
 2. Open the anaconda prompt and type `pip install b2sim`.
 3. Your installation of anaconda came with a program called "Jupyter Notebook", which allows you to create and edit .ipynb files which you will use to operate the code. Open Jupyter, and create a new .ipynb file wherever you wish on your computer.
 4. In the first cell of this new .ipynb file you've created, type `import b2sim as b2` and hit enter. 
 5. Congratulations, you now have a file which you can use to generate simulations! Check out the tutorial files in this repo (examples folder) for more info on how to operate the library.
-6. (Bonus step) Instead of Jupyter Notebook, I recommend using [Visual Studio Code](https://code.visualstudio.com/) to operate the code. VS Code comes with a number of bells and whistles and QOL features that can speed up the code-writing process.
 
 ## For experienced coders:
 1. Type `pip install b2sim` in the terminal to download.
 2. Check out the tutorial files in this repo (tutorials folder) for more info on how to operate the library.
 
 ## Alternative installation instructions:
 If for whatever reason pip installation does not work, try the following:
@@ -28,21 +27,14 @@
 3. **Complete Farm support:** The simulator supports IMF Loans and Monkeyopolis. Also, the simulator supports compound purchases, such as selling into Monkey Wall Street.
 4. **Advanced Optimization Potential:** The code can be used in conjuction with optimization or nonlinear root-finding methods to determine the absolute best times to makes your moves during the game.
 
 # Contributing to the Code
 
 Potential contributors are urged to join the [b2 popology discord](https://discord.gg/YBkvcdBN4H) where I can be easily reached with a ping. Look in the "issues" section of this repo for tasks which need to be completed but have not yet been tended to.
 
-## First-Time Contributors
-
-If it's your first time ever contributing to the code, follow these steps to made the contribution process easy and hassle-free:
-1. Download [GitHub Desktop](https://desktop.github.com/).
-2. Clone the repository to your desktop.
-3. When you're ready to make changes after working on the code, [create a pull request](https://www.nexmo.com/legacy-blog/2020/10/01/how-to-create-a-pull-request-with-github-desktop).
-
 # Update Log
 - (July 11, 2023 - v1.0.9)
    - Adjusted the lengths of some of the rounds in `nat_send_lengths.csv`
    - Fixed an error in `eco_send_info.csv` which caused Grouped Reds and Grouped Blues to be unavailable in the simulator on Round 11
    - Fixed a bug which made the code throw an error if a fail-safe was triggered as a consequence of the simulator attempting to use an eco send after it became unavailable.
    - Renamed "examples" folder to "tutorials". Revised the tutorial files so that they are more instructive.
    - Updated `GameState.viewCashEcoHistory` so that it is easier to see when key transactions or changes in eco occur during the simulation.
```

### Comparing `b2sim-1.1.0/b2sim/actions.py` & `b2sim-1.1.1/b2sim/actions.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.1.0/b2sim/info.py` & `b2sim-1.1.1/b2sim/info.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.1.0/b2sim/main.py` & `b2sim-1.1.1/b2sim/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,21 +184,24 @@
         # }
 
         # Max send amount is useful if we need to simulate sending a precise number of sets of bloons
         # Max eco amount is useful for eco strategies which may demand strategy decisions like "stop eco at 3000 eco"
 
         self.eco_queue = initial_state.get('Eco Queue')
         if self.eco_queue is None:
-            self.eco_queue = [ecoSend(time = 0, send_name = 'Zero')]
+            self.eco_queue = []
         self.number_of_sends = 0
 
         eco_send = initial_state.get('Eco Send')
         if eco_send is not None:
             eco_send['Time'] = 0
             self.eco_queue.insert(0,eco_send)
+
+        if len(self.eco_queue) == 0: #I'm gonna be honest, I'm not proud of myself for writing code like this, but it works so fuck you.
+            self.eco_queue = [ecoSend(time = 0, send_name = 'Zero')]
         
         #Upgrade queue
         self.buy_queue = initial_state.get('Buy Queue')
         self.buy_cost = None
         self.buffer = 0
         self.min_buy_time = None
```

### Comparing `b2sim-1.1.0/b2sim/rounds.py` & `b2sim-1.1.1/b2sim/rounds.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,54 +4,62 @@
 
 import os
 
 nat_dirname = os.path.dirname(__file__)
 nat_filename = os.path.join(nat_dirname, "templates/nat_send_lengths.csv")
 
 #DEFINITION OF THE ROUNDS CLASS
+
+# There are two ways to set round times:
+# 1. Stall Factor - stall factors are given to rounds with a list of tuples
+# 2. Stall Times - stall times are given to rounds witha list of tuples
+
 class Rounds():
-    def __init__(self, stall_factor_info):
+    def __init__(self, info, mode = 'Stall Factor'):
         
         #Logging system
         self.logs = []
 
         #Determine natural send lengths, max stall times, and max anti-stall times
         df = pd.read_csv(nat_filename)
         self.nat_send_lens = list(df['Nat Send Len'])
 
         max_antistall_time = 5.5
         max_stall_times = [8.5 + i for i in range(51)]
         max_stall_times[0] = max_antistall_time
 
         #Backwards compatability with the old system:
-        if type(stall_factor_info) == float:
-            stall_factor_info = [(0,stall_factor_info)]
+        if type(info) == float:
+            info = [(0,info)]
 
         #If the users fails to specify stall factor info for round 0...
-        if stall_factor_info[0][0] > 0:
-            stall_factor_info[0] = (0,stall_factor_info[0][1])
+        if info[0][0] > 0:
+            info[0] = (0,info[0][1])
 
         #Compute the round times given the stall factor info
         val = 0
         self.round_starts = [0]
 
         ind_of_interest = 0
-        stall_factor = stall_factor_info[ind_of_interest][1]
+        stall_info = info[ind_of_interest][1]
         for i in range(len(self.nat_send_lens)):
 
-            #If we have reached a round where the stall factor changes, change the stall factor
-            if len(stall_factor_info) >= ind_of_interest + 2 and i >= stall_factor_info[ind_of_interest+1][0]:
+            #If we have reached a round where the stall info changes, change the stall info
+            if len(info) >= ind_of_interest + 2 and i >= info[ind_of_interest+1][0]:
                 ind_of_interest += 1
-                stall_factor = stall_factor_info[ind_of_interest][1]
-                #print("Changed stall factor to %s"%(stall_factor))
-
-            #Determine the round length based on the current stall factor.
-            round_len = self.nat_send_lens[i] + (1-stall_factor)*max_antistall_time + stall_factor*max_stall_times[i]
+                stall_info = info[ind_of_interest][1]
+            
+            if mode == 'Stall Times':
+                #Interpret the stall info as meaning, "the given round is stalled for this many seconds"
+                round_len = self.nat_send_lens[i] + max(max_antistall_time,min(max_stall_times[i],stall_info))
+            elif mode == 'Stall Factor':
+                #Interpret the stall info as meaning, "the given round has this stall factor"
+                round_len = self.nat_send_lens[i] + (1-stall_info)*max_antistall_time + stall_info*max_stall_times[i]
             val += round_len
-            self.round_starts.append(val)            
+            self.round_starts.append(val)
             
     def getRoundFromTime(self, time, get_frac_part = False):
         ind = 0
         while self.round_starts[ind] <= time and ind < 50:
             ind += 1
         
         if get_frac_part:
```

### Comparing `b2sim-1.1.0/b2sim/templates/eco_send_info.csv` & `b2sim-1.1.1/b2sim/templates/eco_send_info.csv`

 * *Files identical despite different names*

