# Comparing `tmp/cftsdata-0.1.2.tar.gz` & `tmp/cftsdata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cftsdata-0.1.2.tar", last modified: Mon May 22 21:42:36 2023, max compression
+gzip compressed data, was "cftsdata-0.1.3.tar", last modified: Fri Jul 14 17:50:31 2023, max compression
```

## Comparing `cftsdata-0.1.2.tar` & `cftsdata-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.077678 cftsdata-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.069678 cftsdata-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.069678 cftsdata-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-22 21:42:26.000000 cftsdata-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-22 21:42:26.000000 cftsdata-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 21:42:26.000000 cftsdata-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-22 21:42:36.077678 cftsdata-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 21:42:26.000000 cftsdata-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.073678 cftsdata-0.1.2/cftsdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/abr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/dpoae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/efr.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/iec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/memr.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/microphone_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_abr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_abr_gui.enaml
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_dpoae.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_efr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_iec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/summarize_memr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-22 21:42:26.000000 cftsdata-0.1.2/cftsdata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 21:42:35.000000 cftsdata-0.1.2/cftsdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.073678 cftsdata-0.1.2/cftsdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 21:42:36.000000 cftsdata-0.1.2/cftsdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-22 21:42:26.000000 cftsdata-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 21:42:36.077678 cftsdata-0.1.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-22 21:42:26.000000 cftsdata-0.1.2/scripts/validate_abr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-22 21:42:26.000000 cftsdata-0.1.2/scripts/validate_dpoae.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 21:42:36.077678 cftsdata-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:50:31.772893 cftsdata-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:50:31.768893 cftsdata-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:50:31.768893 cftsdata-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-14 17:50:20.000000 cftsdata-0.1.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-14 17:50:20.000000 cftsdata-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-14 17:50:20.000000 cftsdata-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-14 17:50:31.772893 cftsdata-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-14 17:50:20.000000 cftsdata-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:50:31.772893 cftsdata-0.1.3/cftsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/abr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/dpoae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/efr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/iec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/memr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/microphone_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/summarize_abr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/summarize_abr_gui.enaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/summarize_dpoae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/summarize_efr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/summarize_iec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/summarize_memr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-14 17:50:20.000000 cftsdata-0.1.3/cftsdata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 17:50:31.000000 cftsdata-0.1.3/cftsdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:50:31.772893 cftsdata-0.1.3/cftsdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-14 17:50:31.000000 cftsdata-0.1.3/cftsdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-14 17:50:31.000000 cftsdata-0.1.3/cftsdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:50:31.000000 cftsdata-0.1.3/cftsdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-14 17:50:31.000000 cftsdata-0.1.3/cftsdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 17:50:31.000000 cftsdata-0.1.3/cftsdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 17:50:31.000000 cftsdata-0.1.3/cftsdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 17:50:20.000000 cftsdata-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:50:31.772893 cftsdata-0.1.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-14 17:50:20.000000 cftsdata-0.1.3/scripts/validate_abr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-14 17:50:20.000000 cftsdata-0.1.3/scripts/validate_dpoae.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:50:31.772893 cftsdata-0.1.3/setup.cfg
```

### Comparing `cftsdata-0.1.2/.github/workflows/publish-to-pypi.yml` & `cftsdata-0.1.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.2/.gitignore` & `cftsdata-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.2/LICENSE.txt` & `cftsdata-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.2/PKG-INFO` & `cftsdata-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cftsdata
-Version: 0.1.2
+Version: 0.1.3
 Summary: Lightweight tools for managing CFTS data
 Author-email: Brad Buran <buran@ohsu.edu>, Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <buran@ohsu.edu>, Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2022 CFTS development team
```

### Comparing `cftsdata-0.1.2/cftsdata/abr.py` & `cftsdata-0.1.3/cftsdata/abr.py`

 * *Files 17% similar despite different names*

```diff
@@ -330,14 +330,100 @@
     try:
         result = load(base_path, allow_superset)
         return True
     except Exception as e:
         return False
 
 
+P_TH = re.compile('Threshold \(dB SPL\): ([\w.-]+)')
+P_FREQ = re.compile('Frequency \(kHz\): ([\d.]+)')
+P_RATER = re.compile(r'.*[\d.]+kHz-(?:(\w+)-)?analyzed.txt')
+
+def load_abr_analysis(filename):
+    '''
+    Load ABR analysis from file
+
+    Parameters
+    ----------
+    filename : {str, pathlib.Path}
+        Name of file to load.
+
+    Returns
+    -------
+
+    '''
+    rename = {
+        'Level': 'level',
+        '1msec Avg': 'baseline',
+        '1msec StDev': 'baseline_std',
+        'P1 Latency': 'p1_latency',
+        'P1 Amplitude': 'p1_amplitude',
+        'N1 Latency': 'n1_latency',
+        'N1 Amplitude': 'n1_amplitude',
+        'P2 Latency': 'p2_latency',
+        'P2 Amplitude': 'p2_amplitude',
+        'N2 Latency': 'n2_latency',
+        'N2 Amplitude': 'n2_amplitude',
+        'P3 Latency': 'p3_latency',
+        'P3 Amplitude': 'p3_amplitude',
+        'N3 Latency': 'n3_latency',
+        'N3 Amplitude': 'n3_amplitude',
+        'P4 Latency': 'p4_latency',
+        'P4 Amplitude': 'p4_amplitude',
+        'N4 Latency': 'n4_latency',
+        'N4 Amplitude': 'n4_amplitude',
+        'P5 Latency': 'p5_latency',
+        'P5 Amplitude': 'p5_amplitude',
+        'N5 Latency': 'n5_latency',
+        'N5 Amplitude': 'n5_amplitude',
+    }
+
+    filename = Path(filename)
+
+    with filename.open() as fh:
+        for line in fh:
+            # Parse the threshold string
+            if line.startswith('Threshold'):
+                th_string = P_TH.search(line).group(1)
+                if th_string == 'None':
+                    th = -np.inf
+                elif th_string == 'inf':
+                    th = np.inf
+                elif th_string == '-inf':
+                    th = -np.inf
+                else:
+                    th = float(th_string)
+
+            if line.startswith('Frequency'):
+                freq = float(P_FREQ.search(line).group(1))*1e3
+
+            if line.startswith('NOTE'):
+                break
+
+        data = pd.io.parsers.read_csv(fh, sep='\t')
+        data.rename(columns=rename, inplace=True)
+
+    # Discard all sub-threshold data
+    m = data['level'] >= th
+    data = data.loc[m]
+
+    keep_cols = list(rename.values())
+    keep = [c for c in data.columns if c in keep_cols]
+    data = data[keep] \
+        .set_index('level', verify_integrity=True) \
+        .sort_index()
+
+    try:
+        rater = P_RATER.match(filename.name).group(1)
+    except AttributeError:
+        raise ValueError(f'Could not parser rater from {filename.name}')
+
+    return freq, th, rater, data
+
+
 filter_docstring = '''
         filter_lb : float
             Lower bound of filter passband, in Hz.
         filter_ub : float
             Upper bound of filter passband, in Hz.
         filter_order : int
             Filter order. Note that the effective order will be double this
```

### Comparing `cftsdata-0.1.2/cftsdata/efr.py` & `cftsdata-0.1.3/cftsdata/efr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from psidata.api import Recording
 
 
 class EFR(Recording):
 
     def __init__(self, filename, setting_table='analyze_efr_metadata'):
         super().__init__(filename, setting_table)
-        self.efr_type = 'ram' if self.base_path.stem.endswith('ram') else 'sam'
+        self.efr_type = 'ram' if 'efr_ram' in self.base_path.stem else 'sam'
 
     def _get_epochs(self, signal):
         duration = self.get_setting('duration')
         offset = 0
         result = signal.get_epochs(self.analyze_efr_metadata, offset, duration)
         print(result)
         if self.efr_type == 'sam':
```

### Comparing `cftsdata-0.1.2/cftsdata/memr.py` & `cftsdata-0.1.3/cftsdata/memr.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,44 +33,55 @@
 
     def __init__(self, base_path, setting_table='memr_metadata'):
         if 'memr' not in Path(base_path).stem:
             raise ValueError(f'{base_path} is not a MEMR recording')
         super().__init__(base_path, setting_table)
 
     @property
+    def probe_fs(self):
+        return self.probe_microphone.fs
+
+    @property
+    def elicitor_fs(self):
+        return self.elicitor_microphone.fs
+
+    @property
     def probe_microphone(self):
         # A refactor of the cfts suite resulted in microphone being renamed to
         # system_microphone.
         try:
             return self.__getattr__('probe_microphone')
         except AttributeError:
             return self.__getattr__('microphone')
 
     @property
     @lru_cache(maxsize=MAXSIZE)
     def memr_metadata(self):
-        data = self.__getattr__('memr_metadata')
+        try:
+            data = self.__getattr__('memr_metadata')
+        except AttributeError:
+            data = self.__getattr__('memr_probe_metadata')
         # We need to check what needs to be renamed since an update to the MEMR
         # paradigm now includes the renamed column names.
         rename = {k: v for k, v in RENAME.items() if v not in data}
         return data.rename(columns=rename)
 
     @lru_cache(maxsize=MAXSIZE)
     def get_epochs(self, columns='auto', signal_name='probe_microphone',
-                   add_trial=True):
+                   add_trial=True, cb=None):
         signal = getattr(self, signal_name)
         epochs = signal.get_epochs(
             self.memr_metadata, 0, self.trial_duration,
-            columns=columns).sort_index()
+            columns=columns, cb=cb).sort_index()
         if add_trial:
             epochs = util.add_trial(epochs, epochs.index.names[:-1])
         return epochs
 
     @lru_cache(maxsize=MAXSIZE)
-    def get_repeats(self, columns='auto', signal_name='probe_microphone'):
+    def _get_repeats(self, columns='auto', signal_name='probe_microphone'):
         fs = getattr(self, signal_name).fs
         epochs = self.get_epochs(columns, signal_name).copy()
         s_repeat = int(round(self.repeat_period * fs))
         n_probe = self.get_setting('probe_n')
         t_probe = np.arange(s_repeat) / fs
 
         repeats = []
@@ -99,52 +110,78 @@
     def trial_duration(self):
         return self.get_setting('probe_n') * self.get_setting('repeat_period')
 
     @property
     def repeat_period(self):
         return self.get_setting('repeat_period')
 
+    @lru_cache(maxsize=MAXSIZE)
+    def get_elicitor(self, signal_name='elicitor_microphone'):
+        repeats = self._get_repeats(signal_name=signal_name)
+        elicitor_delay = self.get_setting('elicitor_envelope_start_time')
+        m = repeats.columns >= elicitor_delay
+        return repeats.loc[:, m].reset_index(['probe_t0', 't0'], drop=True)
+
+    @lru_cache(maxsize=MAXSIZE)
+    def get_probe(self, acoustic_delay=0.75e-3, signal_name='probe_microphone'):
+        repeats = self._get_repeats(signal_name=signal_name)
+        probe_delay = self.get_setting('probe_delay')
+        probe_duration = self.get_setting('probe_duration')
+        probe_lb = acoustic_delay + probe_delay
+        probe_ub = acoustic_delay + probe_delay + probe_duration
+        m = (repeats.columns >= probe_lb) & (repeats.columns < probe_ub)
+        return repeats.loc[:, m].reset_index(['probe_t0', 't0'], drop=True)
+
+    @lru_cache(maxsize=MAXSIZE)
+    def get_silence(self, acoustic_delay=0.75e-3, signal_name='probe_microphone'):
+        probe_delay = self.get_setting('probe_delay')
+        probe_duration = self.get_setting('probe_duration')
+        silence_lb = acoustic_delay + probe_delay + probe_duration
+        silence_ub = silence_lb + probe_duration
+        repeats = self._get_repeats(signal_name=signal_name)
+        m = (repeats.columns >= silence_lb) & (repeats.columns < silence_ub)
+        return repeats.loc[:, m].reset_index(['probe_t0', 't0'], drop=True)
+
 
 class SimultaneousMEMRFile(BaseMEMRFile):
 
     @property
     def trial_duration(self):
         return self.get_setting('trial_duration')
 
     @property
     def repeat_period(self):
         return 1 / self.get_setting('probe_rate')
 
-    @lru_cache(maxsize=MAXSIZE)
-    def get_repeats(self, columns='auto', signal_name='probe_microphone'):
+    def get_repeats(self, columns='auto', signal_name='probe_microphone',
+                    norm_window=None):
         repeats = super().get_repeats(columns, signal_name)
 
         probe_n = self.get_setting('probe_n')
         onset = self.get_setting('elicitor_onset')
         duration = self.get_setting('elicitor_duration')
         rise = self.get_setting('elicitor_noise_rise_time')
+        if norm_window is None:
+            norm_window = self.get_setting('norm_window')
 
+        def to_repeat(x):
+            return int(round(x / self.repeat_period))
 
-        def to_repeat(x, p): 
-            return int(round(x / p))
-
-        rp = self.repeat_period
-        e_start = to_repeat(onset, rp)
-        e_ss_start = to_repeat(onset + rise, rp)
-        e_ss_end = to_repeat(onset + duration - rise, rp)
-        e_end =  to_repeat(onset + duration, rp)
-
-        nw_start = to_repeat(onset - duration + rise * 2, rp)
-        nw_end = to_repeat(onset, rp)
+        # Mark elicitor portions
+        e_start = to_repeat(onset + rise)
+        e_end = to_repeat(onset + duration - rise)
+
+        # Norm window is just before the elicitor begins
+        nw_start = to_repeat(onset - norm_window)
+        nw_end = to_repeat(onset)
 
         # Create a mapping of repeat number to the probe type (e.g., baseline,
         # elicitor, recovery).
         probe_map = pd.Series('', index=range(probe_n))
         probe_map[e_start:e_end] = 'elicitor'
-        probe_map[e_ss_start:e_ss_end] = 'elicitor_ss'
         probe_map[nw_start:nw_end] = 'baseline'
         probe_map[e_end:] = 'recovery'
 
         ix = repeats.index.to_frame(index=False)
         ix['epoch_t0'] = ix['t0']
         ix['t0'] = ix.eval('epoch_t0 + probe_t0')
         ix['group'] = ix['repeat'].map(probe_map)
```

### Comparing `cftsdata-0.1.2/cftsdata/microphone_calibration.py` & `cftsdata-0.1.3/cftsdata/microphone_calibration.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.2/cftsdata/postprocess.py` & `cftsdata-0.1.3/cftsdata/postprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,30 +13,35 @@
 def zip_data():
     import argparse
     parser = argparse.ArgumentParser('cfts-zip-data')
     parser.add_argument('path', nargs='?', default=get_config('DATA_ROOT'), type=Path)
     parser.add_argument('-d', '--destination', type=Path)
     args = parser.parse_args()
 
+    # Make zip archives first
     dirs = [p for p in args.path.iterdir() if p.is_dir()]
     for path in tqdm(dirs):
         shutil.make_archive(str(path), 'zip', str(path))
         try:
             zippath = validate(path)
             zipmd5 = md5sum(zippath.open('rb'))
             md5path = zippath.with_suffix('.md5')
             md5path.write_text(zipmd5)
             shutil.rmtree(path)
-            if args.destination is not None:
-                for file in (zippath, md5path):
-                    new_file = args.destination / file.name
-                    file.rename(new_file)
         except IOError as e:
             print(e)
 
+    # Now, move all zip and md5 files if a destination is specified
+    if args.destination is not None:
+        for zippath in tqdm(args.path.glob('*.zip')):
+            md5path = zippath.with_suffix('.md5')
+            for file in (zippath, md5path):
+                new_file = args.destination / file.name
+                file.rename(new_file)
+
 
 def md5sum(stream, blocksize=1024**2):
     '''
     Generates md5sum from byte stream
 
     Parameters
     ----------
```

### Comparing `cftsdata-0.1.2/cftsdata/summarize_abr.py` & `cftsdata-0.1.3/cftsdata/summarize_abr.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,16 +78,15 @@
 
 def _get_epochs(fh, offset, duration, filter_settings, reject_ratio=None,
                 downsample=None, cb=None):
     # We need to do the rejects in this code so that we can obtain the
     # information for generating the CSV files. Set reject_threshold to np.inf
     # to ensure that nothing gets rejected.
     kwargs = {'offset': offset, 'duration': duration, 'columns': COLUMNS,
-              'reject_threshold': np.inf, 'downsample': downsample, 'cb': cb,
-              'bypass_cache': True}
+              'reject_threshold': np.inf, 'downsample': downsample, 'cb': cb}
 
     if filter_settings is None:
         return fh.get_epochs(**kwargs)
 
     if filter_settings == 'saved':
         settings = _get_filter(fh)
         if not settings['digital_filter']:
```

### Comparing `cftsdata-0.1.2/cftsdata/summarize_abr_gui.enaml` & `cftsdata-0.1.3/cftsdata/summarize_abr_gui.enaml`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.2/cftsdata/summarize_dpoae.py` & `cftsdata-0.1.3/cftsdata/summarize_dpoae.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,91 +3,33 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from psiaudio import util
 
-from .dpoae import DPOAEFile
+from .dpoae import DPOAEFile, isodp_th_criterions
 from .util import add_default_options, DatasetManager, process_files
 
 
-def isodp_th(l2, dp, nf, criterion):
-    '''
-    Computes iso-DP threshold for a level sweep at a single frequency
-
-    Parameters
-    ----------
-    l2 : array-like
-        Requested F2 levels
-    dp : array-like
-        Measured DPOAE levels
-    nf : array-like
-        Measured DPOAE noise floor
-    criterion : float
-        Threshold criterion (e.g., value that the input-output function must
-        exceed)
-
-    Returns
-    -------
-    threshold : float
-        If no threshold is identified, NaN is returned
-    '''
-    # First, discard up to the first level where the DPOAE exceeds one standard
-    # deviation from the noisne floor
-    nf_crit = np.mean(nf) + np.std(nf)
-    i = np.flatnonzero(dp < nf_crit)
-    if len(i):
-        dp = dp[i[-1]:]
-        l2 = l2[i[-1]:]
-
-    # Now, loop through every pair of points until we find the first pair that
-    # brackets criterion (for non-Python programmers, this uses chained
-    # comparision operators and is not a bug)
-    for l_lb, l_ub, d_lb, d_ub in zip(l2[:-1], l2[1:], dp[:-1], dp[1:]):
-        if d_lb < criterion <= d_ub:
-            return np.interp(criterion, [d_lb, d_ub], [l_lb, l_ub])
-    return np.nan
-
-
-def isodp_th_criterions(df, criterions=None, debug=False):
-    '''
-    Helper function that takes dataframe containing a single frequency and
-    calculates threshold for each criterion.
-    '''
-    if criterions is None:
-        criterions = [-5, 0, 5, 10, 15, 20, 25]
-
-    if ':dB' in df.columns:
-        # This is used for thresholding data already in EPL CFTS format
-        l2 = df.loc[:, ':dB']
-        dp = df.loc[:, '2f1-f2(dB)']
-        nf = df.loc[:, '2f1-f2Nse(dB)']
-    else:
-        # This is used for thresholding data from the psi DPOAE IO.
-        if debug:
-            # Use a measurable signal to estimate threshold.
-            l2 = df.loc[:, 'secondary_tone_level'].values
-            dp = df.loc[:, 'f2_level'].values
-            nf = df.loc[:, 'dpoae_noise_floor'].values
-        else:
-            l2 = df.loc[:, 'secondary_tone_level'].values
-            dp = df.loc[:, 'dpoae_level'].values
-            nf = df.loc[:, 'dpoae_noise_floor'].values
-
-    th = [isodp_th(l2, dp, nf, c) for c in criterions]
-    index = pd.Index(criterions, name='criterion')
-    return pd.Series(th, index=index, name='threshold')
+expected_suffixes = [
+    'io.csv',
+    'th.csv',
+    'io.pdf',
+    'mic spectrum.pdf',
+    'th.pdf'
+]
 
 
 def process_file(filename, cb, reprocess=False):
     manager = DatasetManager(filename)
-    if not reprocess and manager.is_processed('io.csv'):
+    if not reprocess and manager.is_processed(expected_suffixes):
         return
-    manager.clear()
+    manager.clear(expected_suffixes)
+
     with manager.create_cb(cb) as cb:
         fh = DPOAEFile(filename)
         fs = fh.system_microphone.fs
         ramp_time = fh.get_setting('primary_tone_rise_time')
         n_time = fh.get_setting('n_time')
         n_fft = fh.get_setting('n_fft')
         window = fh.get_setting('response_window')
@@ -159,46 +101,37 @@
         n_level = len(level)
 
         measured = pd.DataFrame(
             measured.values(),
             index=pd.MultiIndex.from_tuples(measured.keys(), names=['f2', 'l2'])
         )
 
-        figure, axes = plt.subplots(2, n_freq, figsize=(4 * n_freq, 8),
-                                    sharex=True, sharey=True, squeeze=False)
+        io_figure, axes = plt.subplots(1, n_freq, figsize=(4 * n_freq, 4),
+                                       sharex=True, sharey=True, squeeze=False)
         for fi, f2 in enumerate(freq):
             col = axes[:, fi]
             m = measured.loc[f2]
 
             ax = col[0]
             ax.axhline(0, ls='-', color='k')
             ax.plot(m['f2_level'], marker='o', color='0.5')
             ax.plot(m['f1_level'], marker='o', color='k')
             ax.plot(m['dp_level'], marker='o', color='darkturquoise')
             ax.plot(m['dp_nf'], marker='x', color='lightblue')
             ax.set_title(f'{f2} Hz')
-            ax.grid()
-
-            ax = col[1]
-            ax.axhline(0, ls='-', color='k')
-            ax.plot(m['f2_level'], marker='o', color='0.5')
-            ax.plot(m['f1_level'], marker='o', color='k')
-            ax.plot(m['online_dp_level'], marker='o', color='darkorange')
-            ax.plot(m['online_dp_nf'], marker='x', color='coral')
-            ax.grid()
             ax.set_xlabel('F2 level (dB SPL)')
+            ax.grid()
 
         for ax in axes[:, 0]:
             ax.set_ylabel('Measured level (dB SPL)')
 
-        manager.save_fig(figure, 'io.pdf')
-
-        figure, axes = plt.subplots(n_level, n_freq,
-                                    figsize=(4 * n_freq, 4 * n_level),
-                                    sharex=True, sharey=True, squeeze=False)
+        mic_figure, axes = plt.subplots(n_level, n_freq,
+                                        figsize=(4 * n_freq, 4 * n_level),
+                                        sharex=True, sharey=True,
+                                        squeeze=False)
         for fi, f2 in enumerate(freq):
             for li, l2 in enumerate(level[::-1]):
                 ax = axes[li, fi]
                 f1 = f2 / f2_f1_ratio
                 dp = 2 * f1 - f2
                 ax.axvline(f2, lw=2, color='lightblue')
                 ax.axvline(f1, lw=2, color='lightblue')
@@ -215,16 +148,28 @@
         axes[0, 0].set_xscale('octave')
 
         for ax in axes[-1]:
             ax.set_xlabel('Frequency (kHz)')
         for ax in axes[:, 0]:
             ax.set_xlabel('PSD (dB)')
 
-        manager.save_fig(figure, 'mic spectrum.pdf')
+        th = measured.groupby('f2').apply(isodp_th_criterions)
+        th_figure, ax = plt.subplots(1, 1, figsize=(4, 4))
+        for c, row in th.T.iterrows():
+            ax.plot(row, 'o-', label=str(c))
+        ax.set_xscale('octave', octaves=0.5)
+        ax.set_xlabel('$f_2$ frequency (kHz)')
+        ax.set_ylabel('IsoDP threshold (dB SPL)')
+        ax.legend()
+
         manager.save_dataframe(measured, 'io.csv')
+        manager.save_dataframe(th, 'th.csv')
+        manager.save_fig(mic_figure, 'mic spectrum.pdf')
+        manager.save_fig(io_figure, 'io.pdf')
+        manager.save_fig(th_figure, 'th.pdf')
         plt.close('all')
 
 
 def main_folder():
     import argparse
     parser = argparse.ArgumentParser('Summarize DPOAE IO data in folder')
     add_default_options(parser)
```

### Comparing `cftsdata-0.1.2/cftsdata/summarize_efr.py` & `cftsdata-0.1.3/cftsdata/summarize_efr.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,145 +4,152 @@
 
 from psiaudio import util
 
 from .efr import EFR
 from .util import add_default_options, DatasetManager, process_files
 
 
-def process_file(filename, cb='tqdm', reprocess=False, segment_duration=0.2,
+expected_suffixes = [
+    'EEG bootstrapped.csv',
+    'mic bootstrapped.csv',
+    'EFR.csv',
+    'EFR.pdf',
+    'spectrum.pdf',
+]
+
+
+def process_file(filename, cb='tqdm', reprocess=False, segment_duration=0.5,
                  n_draw=10, n_bootstrap=100):
     manager = DatasetManager(filename)
-    if not reprocess and manager.is_processed('psd.csv'):
+    if not reprocess and manager.is_processed(expected_suffixes):
         return
-    manager.clear()
-    cb = manager.create_cb(cb)
-    cb(0)
-
-    fh = EFR(filename)
-    print(fh.analyze_efr_metadata.iloc[0])
-    n_segments = fh.get_setting('duration') / segment_duration
-    if n_segments != int(n_segments):
-        raise ValueError(f'Cannot analyze {filename} using default settings')
-    n_segments = int(n_segments)
-
-    mic_grouped = fh.get_mic_epochs().groupby(['fm', 'fc'])
-    eeg_grouped = fh.get_eeg_epochs().groupby(['fm', 'fc'])
-    cal = fh.system_microphone.get_calibration()
-
-    keys = []
-    eeg_bs_all = []
-    mic_bs_all = []
-
-    n = len(eeg_grouped)
-    for i, ((fm, fc), eeg) in enumerate(eeg_grouped):
-        figure, axes = plt.subplots(3, 2, sharex=True, figsize=(12, 18))
-        for ax1, ax2 in axes[1:]:
-            ax1.sharey(ax2)
-
-        if len(eeg) != 1:
-            raise ValueError('Cannot analyze {filename} using default settings')
-
-        mic = mic_grouped.get_group((fm, fc))
-        eeg = eeg.values[0].reshape((n_segments, -1))[1:-1]
-        mic = mic.values[0].reshape((n_segments, -1))[1:-1]
-        mic_psd = util.psd_df(mic, fs=fh.mic.fs, window='hann').mean(axis=0)
-        eeg_psd = util.db(util.psd_df(eeg, fs=fh.eeg.fs, window='hann').mean(axis=0))
-        mic_spl = cal.get_db(mic_psd)
-
-        axes[0, 0].plot(mic_spl, color='k')
-        axes[0, 0].axhline(fh.level, color='lightblue')
-        axes[0, 1].plot(eeg_psd, color='k')
-
-        mic_bs = util.psd_bootstrap_loop(mic, fs=fh.mic.fs, n_draw=n_draw, n_bootstrap=n_bootstrap)
-        eeg_bs = util.psd_bootstrap_loop(eeg, fs=fh.eeg.fs, n_draw=n_draw, n_bootstrap=n_bootstrap)
-        mic_bs_all.append(mic_bs)
-        eeg_bs_all.append(eeg_bs)
-        keys.append((fm, fc))
-
-        axes[1, 0].plot(mic_bs['psd_norm'], color='k')
-        axes[1, 1].plot(eeg_bs['psd_norm'], color='k')
-        axes[2, 0].plot(mic_bs['plv'], color='k')
-        axes[2, 1].plot(eeg_bs['plv'], color='k')
-
-        for ax in axes.flat:
-            for i in range(1, 5):
-                ls = ':' if i != 1 else '-'
-                ax.axvline(60 * i, color='lightgray', ls=ls, zorder=-1)
-                ax.axvline(fm * i, color='lightblue', ls=ls, zorder=-1)
-            ax.axvline(fc, color='pink', zorder=-1)
-            ax.axvline(fc+fm, color='pink', zorder=-1)
-            ax.axvline(fc-fm, color='pink', zorder=-1)
-
-        axes[0, 1].set_xscale('octave')
-        axes[0, 1].axis(xmin=50, xmax=50e3)
-
-        for ax in axes[-1]:
-            ax.set_xlabel('Frequency (kHz)')
-        axes[0, 0].set_title('Microphone')
-        axes[0, 1].set_title('EEG')
-        axes[0, 0].set_ylabel('Stimulus (dB SPL)')
-        axes[0, 1].set_ylabel('Response (dB re 1Vrms)')
-        axes[1, 0].set_ylabel('Norm. amplitude (dB re noise floor)')
-        axes[2, 0].set_ylabel('Phase-locking value')
-
-        figure.suptitle(f'{fc} Hz modulated @ {fm} Hz')
-        manager.save_fig(figure, f'spectrum for {fc} Hz modulated at {fm} Hz.pdf')
-        plt.close(figure)
-        cb((i + 1) / n)
-
-    eeg_bs_all = pd.concat(eeg_bs_all, keys=keys, names=['fm', 'fc'])
-    mic_bs_all = pd.concat(mic_bs_all, keys=keys, names=['fm', 'fc'])
-    manager.save_df(eeg_bs_all, 'EEG boostrapped.csv')
-    manager.save_df(mic_bs_all, 'mic boostrapped.csv')
-
-    fft_resolution = 1 / segment_duration
-    noise_bins = np.array([-2, -1, 1, 2]) * fft_resolution
-
-    efr = []
-    for fm, df in eeg_bs_all.groupby('fm'):
-        ix = pd.IndexSlice[:, :, fm+noise_bins]
-        noise = df.loc[ix].groupby(['fm', 'fc']).mean().add_suffix('_noise')
-        signal = df.xs(fm, level='frequency')
-        harmonics = np.array([1, 2, 3, 4, 5]) * fm
-        ix = pd.IndexSlice[:, :, harmonics]
-        harmonics = df.loc[ix].groupby(['fm', 'fc'])[['psd', 'psd_norm']].sum().add_suffix('_harmonics')
-        efr.append(pd.concat((noise, signal, harmonics), axis=1))
-
-    figure, axes = plt.subplots(2, 2, figsize=(12, 12), sharex=True)
-    efr = pd.concat(efr, axis=0).reset_index()
-    manager.save_df(efr, 'EFR.csv')
-
-    for fm, efr_df in efr.groupby('fm'):
-        p, = axes[0, 0].plot(efr_df['fc'], efr_df['psd'], 'o-', label=f'{fm} Hz')
-        c = p.get_color()
-        axes[0, 0].plot(efr_df['fc'], efr_df['psd_noise'], ':')
-        axes[0, 1].plot(efr_df['fc'], efr_df['psd_norm'], 'o-', label=f'{fm} Hz')
-        axes[0, 1].plot(efr_df['fc'], efr_df['psd_norm_noise'], ':', color=c)
-        axes[1, 0].plot(efr_df['fc'], efr_df['plv'], 'o-', color=c)
-        axes[1, 0].plot(efr_df['fc'], efr_df['plv_noise'], ':', color=c)
-        axes[1, 1].plot(efr_df['fc'], efr_df['psd_norm_harmonics'], 'o-', color=c)
-
-    axes[0, 0].legend()
-    axes[0, 0].set_xscale('octave')
-    for ax in axes[1]:
-        ax.set_xlabel('Frequency (kHz)')
-    axes[0, 0].set_ylabel('EFR (dB re 1V)')
-    axes[0, 1].set_ylabel('EFR (dB re noise floor)')
-    axes[1, 0].set_ylabel('Phase-locking value (frac.)')
-    axes[1, 1].set_ylabel('EFR with harmonics (dB re noise floor)')
-    axes[1, 0].axis(ymin=0, ymax=1)
-    manager.save_fig(figure, 'EFR.pdf')
+    #manager.clear(expected_suffixes)
+    with manager.create_cb(cb) as cb:
+        fh = EFR(filename)
+        n_segments = fh.get_setting('duration') / segment_duration
+        if n_segments != int(n_segments):
+            raise ValueError(f'Cannot analyze {filename} using default settings')
+        n_segments = int(n_segments)
+
+        mic_grouped = fh.get_mic_epochs().dropna().groupby(['fm', 'fc'])
+        eeg_grouped = fh.get_eeg_epochs().dropna().groupby(['fm', 'fc'])
+        cal = fh.system_microphone.get_calibration()
+
+        keys = []
+        eeg_bs_all = []
+        mic_bs_all = []
+
+        spectrum_figures = []
+        n = len(eeg_grouped)
+        for i, ((fm, fc), eeg) in enumerate(eeg_grouped):
+            figure, axes = plt.subplots(3, 2, sharex=True, figsize=(12, 18))
+            for ax1, ax2 in axes[1:]:
+                ax1.sharey(ax2)
+
+            mic = mic_grouped.get_group((fm, fc))
+
+            n = len(eeg) * n_segments
+            eeg = eeg.values.reshape((n, -1))
+
+            n = len(mic) * n_segments
+            mic = mic.values.reshape((n, -1))
+
+            mic_psd = util.psd_df(mic, fs=fh.mic.fs, window='hann').mean(axis=0)
+            eeg_psd = util.db(util.psd_df(eeg, fs=fh.eeg.fs, window='hann').mean(axis=0))
+            mic_spl = cal.get_db(mic_psd)
+
+            axes[0, 0].plot(mic_spl, color='k')
+            axes[0, 0].axhline(fh.level, color='lightblue')
+            axes[0, 1].plot(eeg_psd, color='k')
+
+            mic_bs = util.psd_bootstrap_loop(mic, fs=fh.mic.fs, n_draw=n_draw, n_bootstrap=n_bootstrap)
+            eeg_bs = util.psd_bootstrap_loop(eeg, fs=fh.eeg.fs, n_draw=n_draw, n_bootstrap=n_bootstrap)
+            mic_bs_all.append(mic_bs)
+            eeg_bs_all.append(eeg_bs)
+            keys.append((fm, fc))
+
+            axes[1, 0].plot(mic_bs['psd_norm'], color='k')
+            axes[1, 1].plot(eeg_bs['psd_norm'], color='k')
+            axes[2, 0].plot(mic_bs['plv'], color='k')
+            axes[2, 1].plot(eeg_bs['plv'], color='k')
+
+            for ax in axes.flat:
+                for i in range(1, 5):
+                    ls = ':' if i != 1 else '-'
+                    ax.axvline(60 * i, color='lightgray', ls=ls, zorder=-1)
+                    ax.axvline(fm * i, color='lightblue', ls=ls, zorder=-1)
+                ax.axvline(fc, color='pink', zorder=-1)
+                ax.axvline(fc+fm, color='pink', zorder=-1)
+                ax.axvline(fc-fm, color='pink', zorder=-1)
+
+            axes[0, 1].set_xscale('octave')
+            axes[0, 1].axis(xmin=50, xmax=50e3)
+
+            for ax in axes[-1]:
+                ax.set_xlabel('Frequency (kHz)')
+            axes[0, 0].set_title('Microphone')
+            axes[0, 1].set_title('EEG')
+            axes[0, 0].set_ylabel('Stimulus (dB SPL)')
+            axes[0, 1].set_ylabel('Response (dB re 1Vrms)')
+            axes[1, 0].set_ylabel('Norm. amplitude (dB re noise floor)')
+            axes[2, 0].set_ylabel('Phase-locking value')
+            figure.suptitle(f'{fc} Hz modulated @ {fm} Hz')
+            spectrum_figures.append(figure)
+
+            cb((i + 1) / n)
+
+        eeg_bs_all = pd.concat(eeg_bs_all, keys=keys, names=['fm', 'fc'])
+        mic_bs_all = pd.concat(mic_bs_all, keys=keys, names=['fm', 'fc'])
+
+        fft_resolution = 1 / segment_duration
+        noise_bins = np.array([-2, -1, 1, 2]) * fft_resolution
+
+        efr = []
+        for fm, df in eeg_bs_all.groupby('fm'):
+            ix = pd.IndexSlice[:, :, fm+noise_bins]
+            noise = df.loc[ix].groupby(['fm', 'fc']).mean().add_suffix('_noise')
+            signal = df.xs(fm, level='frequency')
+            harmonics = np.array([1, 2, 3, 4, 5]) * fm
+            ix = pd.IndexSlice[:, :, harmonics]
+            harmonics = df.loc[ix].groupby(['fm', 'fc'])[['psd', 'psd_norm']].sum().add_suffix('_harmonics')
+            efr.append(pd.concat((noise, signal, harmonics), axis=1))
+        efr = pd.concat(efr, axis=0).reset_index()
+
+        efr_figure, axes = plt.subplots(1, 3, figsize=(12, 4), sharex=True)
+        for fm, efr_df in efr.reset_index().groupby('fm'):
+            p, = axes[0].plot(efr_df['fc'], efr_df['psd'], 'o-', label=f'{fm} Hz')
+            c = p.get_color()
+            axes[0].plot(efr_df['fc'], efr_df['psd_noise'], ':', color=c, label=f'{fm} nse')
+            axes[1].plot(efr_df['fc'], efr_df['psd_norm'], '--', label=f'{fm} Hz ($f_0$)', color=c)
+            axes[1].plot(efr_df['fc'], efr_df['psd_norm_harmonics'], 'o-', color=c, label=f'{fm} Hz ($f_{{0-4}})$')
+            axes[2].plot(efr_df['fc'], efr_df['plv'], 'o-', color=c, label=f'{fm} Hz')
+            axes[2].plot(efr_df['fc'], efr_df['plv_noise'], ':', color=c, label=f'{fm} Hz nse')
+
+        axes[1].legend()
+        axes[2].legend()
+        axes[0].set_xscale('octave')
+        for ax in axes:
+            ax.set_xlabel('Carrier Freq. (kHz)')
+        axes[0].set_ylabel('EFR (dB re 1V)')
+        axes[1].set_ylabel('EFR (dB re noise floor)')
+        axes[2].set_ylabel('Phase-locking value (frac.)')
+        axes[2].axis(ymin=0, ymax=1.1)
+        efr_figure.tight_layout()
+
+        manager.save_df(eeg_bs_all, 'EEG bootstrapped.csv')
+        manager.save_df(mic_bs_all, 'mic bootstrapped.csv')
+        manager.save_df(efr, 'EFR.csv')
+        manager.save_fig(efr_figure, 'EFR.pdf')
+        manager.save_figs(spectrum_figures, 'spectrum.pdf')
 
 
 def main_folder():
     import argparse
-    parser = argparse.ArgumentParser('Summarize IEC data in folder')
+    parser = argparse.ArgumentParser('Summarize EFR in folder')
     add_default_options(parser)
     args = parser.parse_args()
-    process_files(args.folder, '**/*inear_speaker_calibration_chirp*',
-                  process_file, reprocess=args.reprocess)
-
-
-if __name__ == '__main__':
-    #process_file(r'C:\Users\mmm\projects\psi1\data\data\20230127-124721 Sean Sean left 151122 1 efr_sam.zip')
-    #process_file(r'C:\Users\mmm\projects\psi1\data\data\20230208-113146 Sean B018-1 left 400uM efr_sam.zip')
-    process_file(r'C:\Users\mmm\projects\psi1\data\data\20230208-113941 Sean B018-1 left 400uM efr_ram.zip')
+    process_files(args.folder, '**/*efr_ram_epoch*',
+                  process_file, reprocess=args.reprocess,
+                  halt_on_error=args.halt_on_error)
+    process_files(args.folder, '**/*efr_sam_epoch*',
+                  process_file, reprocess=args.reprocess,
+                  halt_on_error=args.halt_on_error)
```

### Comparing `cftsdata-0.1.2/cftsdata/summarize_iec.py` & `cftsdata-0.1.3/cftsdata/summarize_iec.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.2/cftsdata/util.py` & `cftsdata-0.1.3/cftsdata/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import os
 from pathlib import Path
 
+from matplotlib.backends.backend_pdf import PdfPages
+import matplotlib.pyplot as plt
+
 
 class CallbackManager:
 
-    def __init__(self, cb):
+    def __init__(self, cb, autoclose_figures=True):
         self._cb = cb
+        self._autoclose_figures = autoclose_figures
 
     def __enter__(self):
         self._cb(0)
         return self
 
     def __call__(self, value):
         return self._cb(value)
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         self._cb(1)
+        if self._autoclose_figures:
+            plt.close('all')
 
 
 def get_cb(cb, suffix=None):
     # Define the callback as a no-op if not provided or sets up tqdm if requested.
     if cb is None:
         cb = lambda x: x
     elif cb == 'tqdm':
@@ -38,18 +44,19 @@
         raise ValueError(f'Unsupported callback: {cb}')
     return cb
 
 
 def add_default_options(parser):
     parser.add_argument('folder', type=str, help='Folder containing data')
     parser.add_argument('--reprocess', action='store_true', help='Reprocess all data in folder')
+    parser.add_argument('--halt-on-error', action='store_true', help='Stop on error?')
 
 
 def process_files(folder, glob_pattern, fn, cb='tqdm', reprocess=False,
-                  halt_on_error=True):
+                  halt_on_error=False):
     success = []
     errors = []
     for filename in Path(folder).glob(glob_pattern):
         if filename.suffix == '.md5':
             continue
         try:
             fn(filename, cb=cb, reprocess=reprocess)
@@ -134,16 +141,24 @@
                 return False
         return True
 
     def save_fig(self, figure, suffix):
         filename = self.get_proc_filename(suffix)
         figure.savefig(filename, bbox_inches='tight')
 
+    def save_figs(self, figures, suffix):
+        filename = self.get_proc_filename(suffix).with_suffix('.pdf')
+        with PdfPages(filename) as pdf:
+            for figure in figures:
+                pdf.savefig(figure, bbox_inches='tight')
+
     def save_dataframe(self, df, suffix):
         filename = self.get_proc_filename(suffix)
         df.to_csv(filename)
 
     save_df = save_dataframe
 
-    def clear(self):
-        for filename in self.get_proc_path().iterdir():
-            filename.unlink()
+    def clear(self, suffixes):
+        for suffix in suffixes:
+            filename = self.get_proc_filename(suffix)
+            if filename.exists():
+                filename.unlink()
```

### Comparing `cftsdata-0.1.2/cftsdata.egg-info/PKG-INFO` & `cftsdata-0.1.3/cftsdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cftsdata
-Version: 0.1.2
+Version: 0.1.3
 Summary: Lightweight tools for managing CFTS data
 Author-email: Brad Buran <buran@ohsu.edu>, Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <buran@ohsu.edu>, Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 License: MIT License
         
         Copyright (c) 2022 CFTS development team
```

### Comparing `cftsdata-0.1.2/cftsdata.egg-info/SOURCES.txt` & `cftsdata-0.1.3/cftsdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.2/scripts/validate_abr.py` & `cftsdata-0.1.3/scripts/validate_abr.py`

 * *Files identical despite different names*

### Comparing `cftsdata-0.1.2/scripts/validate_dpoae.py` & `cftsdata-0.1.3/scripts/validate_dpoae.py`

 * *Files identical despite different names*

