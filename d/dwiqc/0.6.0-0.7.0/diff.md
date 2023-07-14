# Comparing `tmp/dwiqc-0.6.0-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.7.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,26 @@
-Zip file size: 25957 bytes, number of entries: 22
+Zip file size: 27288 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      225 b- defN 23-Jul-05 14:23 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-13 14:27 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jul-14 14:57 dwiqc/__version__.py
 -rw-r--r--  2.0 unx     1352 b- defN 23-Jul-05 14:23 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       61 b- defN 23-Jul-05 14:23 dwiqc/cli/__init__.py
--rw-r--r--  2.0 unx     6941 b- defN 23-Jul-06 18:14 dwiqc/cli/get.py
--rw-r--r--  2.0 unx     6009 b- defN 23-Jul-07 14:09 dwiqc/cli/process.py
--rw-r--r--  2.0 unx     4180 b- defN 23-Jul-06 18:14 dwiqc/cli/tandem.py
--rw-r--r--  2.0 unx      160 b- defN 23-Jul-06 18:14 dwiqc/config/__init__.py
+-rw-r--r--  2.0 unx     6941 b- defN 23-Jul-13 14:52 dwiqc/cli/get.py
+-rw-r--r--  2.0 unx     6105 b- defN 23-Jul-14 14:57 dwiqc/cli/process.py
+-rw-r--r--  2.0 unx     4185 b- defN 23-Jul-14 14:57 dwiqc/cli/tandem.py
+-rw-r--r--  2.0 unx      383 b- defN 23-Jul-13 14:56 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jul-05 14:23 dwiqc/config/dwiqc.yaml
+-rw-r--r--  2.0 unx     1029 b- defN 23-Jul-13 14:57 dwiqc/config/prequal.yaml
+-rw-r--r--  2.0 unx      634 b- defN 23-Jul-13 14:58 dwiqc/config/qsiprep.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jul-05 14:23 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jul-05 14:23 dwiqc/tasks/__init__.py
--rw-r--r--  2.0 unx    15219 b- defN 23-Jul-12 15:57 dwiqc/tasks/prequal.py
+-rw-r--r--  2.0 unx    15699 b- defN 23-Jul-14 14:57 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4656 b- defN 23-Jul-05 14:23 dwiqc/tasks/prequal_EQ.py
--rw-r--r--  2.0 unx     7849 b- defN 23-Jul-13 14:00 dwiqc/tasks/qsiprep.py
+-rw-r--r--  2.0 unx     8188 b- defN 23-Jul-14 14:57 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jul-05 14:23 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13087 b- defN 23-Jul-05 14:23 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     6046 b- defN 23-Jul-13 14:28 dwiqc-0.6.0.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jul-13 14:28 dwiqc-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      439 b- defN 23-Jul-13 14:28 dwiqc-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-13 14:28 dwiqc-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-13 14:28 dwiqc-0.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1718 b- defN 23-Jul-13 14:28 dwiqc-0.6.0.dist-info/RECORD
-22 files, 75982 bytes uncompressed, 23205 bytes compressed:  69.5%
+-rwxr-xr-x  2.0 unx     6571 b- defN 23-Jul-14 14:58 dwiqc-0.7.0.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jul-14 14:58 dwiqc-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      460 b- defN 23-Jul-14 14:58 dwiqc-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-14 14:58 dwiqc-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-14 14:58 dwiqc-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1881 b- defN 23-Jul-14 14:58 dwiqc-0.7.0.dist-info/RECORD
+24 files, 79497 bytes uncompressed, 24284 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -21,14 +21,20 @@
 
 Filename: dwiqc/config/__init__.py
 Comment: 
 
 Filename: dwiqc/config/dwiqc.yaml
 Comment: 
 
+Filename: dwiqc/config/prequal.yaml
+Comment: 
+
+Filename: dwiqc/config/qsiprep.yaml
+Comment: 
+
 Filename: dwiqc/state/__init__.py
 Comment: 
 
 Filename: dwiqc/tasks/__init__.py
 Comment: 
 
 Filename: dwiqc/tasks/prequal.py
@@ -42,26 +48,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.6.0.data/scripts/dwiQC.py
+Filename: dwiqc-0.7.0.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.6.0.dist-info/LICENSE
+Filename: dwiqc-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.6.0.dist-info/METADATA
+Filename: dwiqc-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.6.0.dist-info/WHEEL
+Filename: dwiqc-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.6.0.dist-info/top_level.txt
+Filename: dwiqc-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.6.0.dist-info/RECORD
+Filename: dwiqc-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.6.0'
+__version__ = '0.7.0'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/cli/process.py

```diff
@@ -67,14 +67,15 @@
         prequal_outdir = os.path.join(args.bids_dir, 'derivatives', 'dwiqc-prequal', f'sub-{args.sub}', f'ses-{args.ses}', basename, 'OUTPUTS')
         prequal_task = prequal.Task(
             sub=args.sub,
             ses=args.ses,
             run=args.run,
             bids=args.bids_dir,
             outdir=prequal_outdir,
+            prequal_config=args.prequal_config,
             no_gpu=args.no_gpu,
             tempdir=tempfile.gettempdir(),
             pipenv='/sw/apps/prequal'
         )
         os.environ['OPENBLAS_NUM_THREADS'] = '1'
         logger.info(json.dumps(prequal_task.command, indent=1))
         jarray.add(prequal_task.job)
@@ -87,14 +88,15 @@
         #os.symlink(qsiprep_outdir, f"{qsiprep_trick}/q")
         qsiprep_task = qsiprep.Task(
             sub=args.sub,
             ses=args.ses,
             run=args.run,
             bids=args.bids_dir,
             outdir=qsiprep_outdir,
+            qsiprep_config=args.qsiprep_config,
             no_gpu=args.no_gpu,
             tempdir=tempfile.gettempdir(),
             pipenv='/sw/apps/qsiprep'
         )
         os.environ['OPENBLAS_NUM_THREADS'] = '1'
         logger.info(json.dumps(qsiprep_task.command, indent=1))
         #check_for_output(args, qsiprep_outdir)
```

## dwiqc/cli/tandem.py

```diff
@@ -49,15 +49,15 @@
         args.xnat_user,
         args.xnat_pass
     )
     os.environ['XNAT_HOST'] = auth.url
     os.environ['XNAT_USER'] = auth.username
     os.environ['XNAT_PASS'] = auth.password
 
-    conf = yaml.safe_load(open(args.config)) # load 
+    conf = yaml.safe_load(open(args.xnat_config)) # load 
 
     # config file under anatqc/config/anatqc.yaml
 
     # query DWI, T1 and fieldmap scans from XNAT
     with yaxil.session(auth) as ses:
         scans = col.defaultdict(dict)
         for scan in ses.scans(label=args.label, project=args.project):
```

## dwiqc/config/__init__.py

```diff
@@ -1,11 +1,25 @@
 import os
 import yaml
 
 __dir__ = os.path.dirname(__file__)
 
-def default():
+def xnat_download():
     conf = os.path.join(
         __dir__,
         'dwiqc.yaml'
     )
     return conf
+
+def prequal_command():
+    cmd = os.path.join(
+        __dir__,
+        'prequal.yaml'
+    )
+    return cmd
+
+def qsiprep_command():
+    cmd = os.path.join(
+        __dir__,
+        'qsiprep.yaml'
+    )
+    return cmd
```

## dwiqc/tasks/prequal.py

```diff
@@ -1,36 +1,40 @@
 
 #### load necessary libraries
 import tempfile
 import subprocess
+import yaml
 import os
 import logging
 from bids import BIDSLayout
 import sys
 import json
 import dwiqc.tasks as tasks
 import shutil
 from executors.models import Job
 sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
 from env_modules_python import module
+import dwiqc.config as config
+import numpy as np
 
 
 logger = logging.getLogger(__name__)
 
 
 module('load', 'cuda/9.1.85-fasrc01')
 
 # pull in some parameters from the BaseTask class in the __init__.py directory
 
 class Task(tasks.BaseTask):
-	def __init__(self, sub, ses, run, bids, outdir, no_gpu=False, tempdir=None, pipenv=None):
+	def __init__(self, sub, ses, run, bids, outdir, prequal_config=False, no_gpu=False, tempdir=None, pipenv=None):
 		self._sub = sub
 		self._ses = ses
 		self._run = run
 		self._bids = bids
+		self._prequal_config = prequal_config
 		self._no_gpu = no_gpu
 		self._layout = BIDSLayout(bids)
 		super().__init__(outdir, tempdir, pipenv)
 
 
 	# create an INPUTS dir next to the OUTPUTS dir
 	def copy_inputs(self, inputs_dir):
@@ -191,15 +195,15 @@
 			col3.append(col3_num)
 		col3 = np.array(col3)
 
 		all_cols = np.column_stack([col1, col2, col3])
 
 		spec_file = f"{inputs_dir}/odd_slices_slspec.txt"
 
-		np.savetxt(spec_file, data, fmt=['%d', '%d', '%d'])
+		np.savetxt(spec_file, all_cols, fmt=['%d', '%d', '%d'])
 
 		os.makedirs(self._outdir)
 		shutil.copy(f"{inputs_dir}/odd_slices_slspec.txt", self._outdir)
 		self._spec = "odd"
 
 	# this method will grab the manufacturer name and model and the max bval value. 
 	# if it is a Siemens Skyra and the max bval is 2000, the non-zero_shells argument needs to be passed to prequal
@@ -310,209 +314,213 @@
 	# build the prequal sbatch command and create job
 
 	def build(self):
 		self.add_intended_for()
 		self._tempdir = tempfile.gettempdir()
 		inputs_dir = f'{self._tempdir}/INPUTS/'
 		self.copy_inputs(inputs_dir)
-		if self._nonzero_shells == False:
-			if self._no_gpu:
-				self._command = [
-					'selfie',
-					'--lock',
-					'--output-file', self._prov,
-					'singularity',
-					'run',
-					'-e',
-					'--contain',
-					'-B',
-					f'{inputs_dir}:/INPUTS/',
-					'-B',
-					f'{self._outdir}:/OUTPUTS',
-					'-B',
-					f'{self._tempdir}:/tmp',
-					'-B',
-					'/n/sw/ncf/apps/freesurfer/6.0.0/license.txt:/APPS/freesurfer/license.txt',
-					'-B',
-					'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/run_dtiQA.py:/CODE/dtiQA_v7/run_dtiQA.py',
-					'-B',
-					'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/vis.py:/CODE/dtiQA_v7/vis.py',
-					'/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif',
-					'--save_component_pngs',
-					'j',
-					'--num_threads',
-					'2',
-					'--denoise',
-					'off',
-					'--degibbs',
-					'off',
-					'--rician',
-					'off',
-					'--prenormalize',
-					'on',
-					'--correct_bias',
-					'on',
-					'--topup_first_b0s_only',
-					'--subject',
-					self._sub,
-					'--project',
-					'SSBC',
-					'--session',
-					self._ses
-				]
-			else:
-				self._command = [
-					'selfie',
-					'--lock',
-					'--output-file', self._prov,
-					'singularity',
-					'run',
-					'-e',
-					'--contain',
-					'--nv',
-					'-B',
-					f'{inputs_dir}:/INPUTS/',
-					'-B',
-					f'{self._outdir}:/OUTPUTS',
-					'-B',
-					f'{self._tempdir}:/tmp',
-					'-B',
-					'/n/sw/ncf/apps/freesurfer/6.0.0/license.txt:/APPS/freesurfer/license.txt',
-					'-B',
-					'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
-					'-B',
-					'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/run_dtiQA.py:/CODE/dtiQA_v7/run_dtiQA.py',
-					'-B',
-					'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/vis.py:/CODE/dtiQA_v7/vis.py',
-					'/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif',
-					'--save_component_pngs',
-					'j',
-					'--eddy_cuda',
-					'9.1',
-					'--num_threads',
-					'2',
-					'--denoise',
-					'off',
-					'--degibbs',
-					'off',
-					'--rician',
-					'off',
-					'--prenormalize',
-					'on',
-					'--correct_bias',
-					'on',
-					'--topup_first_b0s_only',
-					'--subject',
-					self._sub,
-					'--project',
-					'SSBC',
-					'--session',
-					self._ses
-				]
-
-		elif self._nonzero_shells == True:
-			if self._no_gpu:
-
-				self._command = [
-					'selfie',
-					'--lock',
-					'--output-file', self._prov,
-					'singularity',
-					'run',
-					'-e',
-					'--contain',
-					'-B',
-					f'{inputs_dir}:/INPUTS/',
-					'-B',
-					f'{self._outdir}:/OUTPUTS',
-					'-B',
-					f'{self._tempdir}:/tmp',
-					'-B',
-					'/n/sw/ncf/apps/freesurfer/6.0.0/license.txt:/APPS/freesurfer/license.txt',
-					'-B',
-					'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/run_dtiQA.py:/CODE/dtiQA_v7/run_dtiQA.py',
-					'-B',
-					'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/vis.py:/CODE/dtiQA_v7/vis.py',
-					'/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif',
-					'--save_component_pngs',
-					'j',
-					'--num_threads',
-					'2',
-					'--denoise',
-					'off',
-					'--degibbs',
-					'off',
-					'--rician',
-					'off',
-					'--prenormalize',
-					'on',
-					'--correct_bias',
-					'on',
-					'--topup_first_b0s_only',
-					'--nonzero_shells',
-					'350,650,1350,2000',
-					'--subject',
-					self._sub,
-					'--project',
-					'SSBC',
-					'--session',
-					self._ses
-				]
-			else:
-
-				self._command = [
-					'selfie',
-					'--lock',
-					'--output-file', self._prov,
-					'singularity',
-					'run',
-					'-e',
-					'--contain',
-					'--nv',
-					'-B',
-					f'{inputs_dir}:/INPUTS/',
-					'-B',
-					f'{self._outdir}:/OUTPUTS',
-					'-B',
-					f'{self._tempdir}:/tmp',
-					'-B',
-					'/n/sw/ncf/apps/freesurfer/6.0.0/license.txt:/APPS/freesurfer/license.txt',
-					'-B',
-					'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
-					'-B',
-					'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/run_dtiQA.py:/CODE/dtiQA_v7/run_dtiQA.py',
-					'-B',
-					'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/vis.py:/CODE/dtiQA_v7/vis.py',
-					'/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif',
-					'--save_component_pngs',
-					'j',
-					'--eddy_cuda',
-					'9.1',
-					'--num_threads',
-					'2',
-					'--denoise',
-					'off',
-					'--degibbs',
-					'off',
-					'--rician',
-					'off',
-					'--prenormalize',
-					'on',
-					'--correct_bias',
-					'on',
-					'--topup_first_b0s_only',
-					'--nonzero_shells',
-					'350,650,1350,2000',
-					'--subject',
-					self._sub,
-					'--project',
-					'SSBC',
-					'--session',
-					self._ses
-				]
+		if self._prequal_config:
+			prequal_command = yaml.safe_load(open(config.prequal_command()))
+			self._command = prequal_command['prequal']['shell']
+		else:
+			if self._nonzero_shells == False:
+				if self._no_gpu:
+					self._command = [
+						'selfie',
+						'--lock',
+						'--output-file', self._prov,
+						'singularity',
+						'run',
+						'-e',
+						'--contain',
+						'-B',
+						f'{inputs_dir}:/INPUTS/',
+						'-B',
+						f'{self._outdir}:/OUTPUTS',
+						'-B',
+						f'{self._tempdir}:/tmp',
+						'-B',
+						'/n/sw/ncf/apps/freesurfer/6.0.0/license.txt:/APPS/freesurfer/license.txt',
+						'-B',
+						'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/run_dtiQA.py:/CODE/dtiQA_v7/run_dtiQA.py',
+						'-B',
+						'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/vis.py:/CODE/dtiQA_v7/vis.py',
+						'/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif',
+						'--save_component_pngs',
+						'j',
+						'--num_threads',
+						'2',
+						'--denoise',
+						'off',
+						'--degibbs',
+						'off',
+						'--rician',
+						'off',
+						'--prenormalize',
+						'on',
+						'--correct_bias',
+						'on',
+						'--topup_first_b0s_only',
+						'--subject',
+						self._sub,
+						'--project',
+						'SSBC',
+						'--session',
+						self._ses
+					]
+				else:
+					self._command = [
+						'selfie',
+						'--lock',
+						'--output-file', self._prov,
+						'singularity',
+						'run',
+						'-e',
+						'--contain',
+						'--nv',
+						'-B',
+						f'{inputs_dir}:/INPUTS/',
+						'-B',
+						f'{self._outdir}:/OUTPUTS',
+						'-B',
+						f'{self._tempdir}:/tmp',
+						'-B',
+						'/n/sw/ncf/apps/freesurfer/6.0.0/license.txt:/APPS/freesurfer/license.txt',
+						'-B',
+						'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
+						'-B',
+						'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/run_dtiQA.py:/CODE/dtiQA_v7/run_dtiQA.py',
+						'-B',
+						'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/vis.py:/CODE/dtiQA_v7/vis.py',
+						'/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif',
+						'--save_component_pngs',
+						'j',
+						'--eddy_cuda',
+						'9.1',
+						'--num_threads',
+						'2',
+						'--denoise',
+						'off',
+						'--degibbs',
+						'off',
+						'--rician',
+						'off',
+						'--prenormalize',
+						'on',
+						'--correct_bias',
+						'on',
+						'--topup_first_b0s_only',
+						'--subject',
+						self._sub,
+						'--project',
+						'SSBC',
+						'--session',
+						self._ses
+					]	
+
+			elif self._nonzero_shells == True:
+				if self._no_gpu:	
+
+					self._command = [
+						'selfie',
+						'--lock',
+						'--output-file', self._prov,
+						'singularity',
+						'run',
+						'-e',
+						'--contain',
+						'-B',
+						f'{inputs_dir}:/INPUTS/',
+						'-B',
+						f'{self._outdir}:/OUTPUTS',
+						'-B',
+						f'{self._tempdir}:/tmp',
+						'-B',
+						'/n/sw/ncf/apps/freesurfer/6.0.0/license.txt:/APPS/freesurfer/license.txt',
+						'-B',
+						'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/run_dtiQA.py:/CODE/dtiQA_v7/run_dtiQA.py',
+						'-B',
+						'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/vis.py:/CODE/dtiQA_v7/vis.py',
+						'/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif',
+						'--save_component_pngs',
+						'j',
+						'--num_threads',
+						'2',
+						'--denoise',
+						'off',
+						'--degibbs',
+						'off',
+						'--rician',
+						'off',
+						'--prenormalize',
+						'on',
+						'--correct_bias',
+						'on',
+						'--topup_first_b0s_only',
+						'--nonzero_shells',
+						'350,650,1350,2000',
+						'--subject',
+						self._sub,
+						'--project',
+						'SSBC',
+						'--session',
+						self._ses
+					]
+				else:	
+
+					self._command = [
+						'selfie',
+						'--lock',
+						'--output-file', self._prov,
+						'singularity',
+						'run',
+						'-e',
+						'--contain',
+						'--nv',
+						'-B',
+						f'{inputs_dir}:/INPUTS/',
+						'-B',
+						f'{self._outdir}:/OUTPUTS',
+						'-B',
+						f'{self._tempdir}:/tmp',
+						'-B',
+						'/n/sw/ncf/apps/freesurfer/6.0.0/license.txt:/APPS/freesurfer/license.txt',
+						'-B',
+						'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
+						'-B',
+						'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/run_dtiQA.py:/CODE/dtiQA_v7/run_dtiQA.py',
+						'-B',
+						'/n/nrg_l3/Lab/users/nrgadmin/PreQual/src/CODE/dtiQA_v7/vis.py:/CODE/dtiQA_v7/vis.py',
+						'/n/sw/ncf/containers/masilab/prequal/1.0.8/prequal.sif',
+						'--save_component_pngs',
+						'j',
+						'--eddy_cuda',
+						'9.1',
+						'--num_threads',
+						'2',
+						'--denoise',
+						'off',
+						'--degibbs',
+						'off',
+						'--rician',
+						'off',
+						'--prenormalize',
+						'on',
+						'--correct_bias',
+						'on',
+						'--topup_first_b0s_only',
+						'--nonzero_shells',
+						'350,650,1350,2000',
+						'--subject',
+						self._sub,
+						'--project',
+						'SSBC',
+						'--session',
+						self._ses
+					]
 
 		logdir = self.logdir()
 		logfile = os.path.join(logdir, 'dwiqc-prequal.log')
 		if self._no_gpu:
 			self.job = Job(
 				name='dwiqc-prequal',
 				time='3000',
```

## dwiqc/tasks/qsiprep.py

```diff
@@ -1,36 +1,40 @@
 
 #### load necessary libraries
 
 import subprocess
 import os
+import yaml
 import logging
 from bids import BIDSLayout
 import sys
 import json
 import nibabel as nib
 import dwiqc.tasks as tasks
 sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
 from env_modules_python import module
 import shutil
 from executors.models import Job
+import dwiqc.config as config
+import numpy as np
 
 
 #module('load', 'cuda/9.1.85-fasrc01')
 
 
 logger = logging.getLogger(__name__)
 
 
 class Task(tasks.BaseTask):
-	def __init__(self, sub, ses, run, bids, outdir, no_gpu=False, output_resolution=None, tempdir=None, pipenv=None):
+	def __init__(self, sub, ses, run, bids, outdir, qsiprep_config=False, no_gpu=False, output_resolution=None, tempdir=None, pipenv=None):
 		self._sub = sub
 		self._ses = ses
 		self._run = run
 		self._bids = bids
+		self._qsiprep_config = qsiprep_config
 		self._no_gpu = no_gpu
 		self._layout = BIDSLayout(bids)
 		self._output_resolution = output_resolution
 		super().__init__(outdir, tempdir, pipenv)
 
 
 
@@ -104,15 +108,15 @@
 		num_slices = len(slice_timing)
 
 		# check if there's an even or odd number of slices, run corresponding helper method
 		if num_slices % 2 == 0:
 			self.even_slices(json_file)
 
 		else:
-			self.odd_slices(json_file)
+			self.odd_slices(json_file, num_slices)
 
 	# helper method that creates slspec file for an acquisition with an even number of slices
 
 	# if the number of slices is even, create spec file accordingly. source = https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/eddy/Faq#How_should_my_--slspec_file_look.3F
     # line 138 edited from `item - 1` to `item - 0`
 
 	def even_slices(self, json_file):
@@ -139,15 +143,15 @@
 				fp.write('\n')
 
 		self._spec = spec_file
 
 
 	# helper method that generates slspec file for an acquisition with an odd number of slices
 
-	def odd_slices(self, json_file):
+	def odd_slices(self, json_file, num_slices):
 		## build the first column
 
 		col1 = []
 
 		for i in range(0, num_slices, 2):
 			col1.append(i)
 
@@ -177,15 +181,15 @@
 			col3.append(col3_num)
 		col3 = np.array(col3)
 
 		all_cols = np.column_stack([col1, col2, col3])
 
 		spec_file = f"{self._bids}/odd_slices_slspec.txt"
 
-		np.savetxt(spec_file, data, fmt=['%d', '%d', '%d'])
+		np.savetxt(spec_file, all_cols, fmt=['%d', '%d', '%d'])
 
 		self._spec = spec_file
 
 	# create necessary fsl eddy parameters json file using output from create_spec and calc_mporder
 
 	def create_eddy_params(self):
 		mporder = self.calc_mporder()
@@ -219,44 +223,48 @@
 
 	# create qsiprep command to be executed
 
 	def build(self):
 		self.create_eddy_params()
 		#self.create_nipype()
 		self.check_output_resolution()
-		self._command = [
-			'selfie',
-			'--lock',
-			'--output-file', self._prov,
-			'singularity',
-			'run',
-			'--nv',
-			#'-B',
-			#'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
-			'/n/sw/ncf/containers/hub.docker.io/pennbbl/qsiprep/0.18.0/qsiprep.sif',			
-			self._bids,
-			self._outdir,
-			'participant',
-			'--output-resolution',
-			self._output_resolution,
-			'--separate-all-dwis',
-			'--eddy-config',
-			f'{self._bids}/eddy_params_s2v_mbs.json',
-			'--recon-spec',
-			'reorient_fslstd',
-			'--notrack',
-			'--n_cpus',
-			'2',
-			'--mem_mb',
-			'40000',
-			'--fs-license-file',
-			'/n/helmod/apps/centos7/Core/freesurfer/6.0.0-fasrc01/license.txt',
-			'-w',
-			self._tempdir
-		]
+		if self._qsiprep_config:
+			qsiprep_command = yaml.safe_load(open(config.qsiprep_command()))
+			self._command = qsiprep_command['qsiprep']['shell']
+		else:
+			self._command = [
+				'selfie',
+				'--lock',
+				'--output-file', self._prov,
+				'singularity',
+				'run',
+				'--nv',
+				#'-B',
+				#'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
+				'/n/sw/ncf/containers/hub.docker.io/pennbbl/qsiprep/0.18.0/qsiprep.sif',			
+				self._bids,
+				self._outdir,
+				'participant',
+				'--output-resolution',
+				self._output_resolution,
+				'--separate-all-dwis',
+				'--eddy-config',
+				f'{self._bids}/eddy_params_s2v_mbs.json',
+				'--recon-spec',
+				'reorient_fslstd',
+				'--notrack',
+				'--n_cpus',
+				'2',
+				'--mem_mb',
+				'40000',
+				'--fs-license-file',
+				'/n/helmod/apps/centos7/Core/freesurfer/6.0.0-fasrc01/license.txt',
+				'-w',
+				self._tempdir
+			]
 
 		if self._no_gpu:
 			logdir = self.logdir()
 			logfile = os.path.join(logdir, 'dwiqc-qsiprep.log')
 			self.job = Job(
 				name='dwiqc-qsiprep',
 				time='3000',
```

## Comparing `dwiqc-0.6.0.data/scripts/dwiQC.py` & `dwiqc-0.7.0.data/scripts/dwiQC.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 
 def main():
     parser = ap.ArgumentParser()
     parser.add_argument('-v', '--verbose', action='store_true',
         help='Enable verbose logging')
-    parser.add_argument('-c', '--config', default=config.default(),
+    parser.add_argument('-c', '--xnat-config', default=config.xnat_download(),
         help='dwiQC configuration file')
     parser.add_argument('--insecure', action='store_true',
         help='Disable SSL certificate verification')
     subparsers = parser.add_subparsers(help='sub-command help')
     
     # get mode
     parser_get = subparsers.add_parser('get', help='get -h')
@@ -60,14 +60,18 @@
         help='BIDS run')
     parser_process.add_argument('--bids-dir', required=True,
         help='BIDS root directory')
     parser_process.add_argument('--output-resolution-process',
         help='Resolution of output data. Defaut is resolution of input data.')
     parser_process.add_argument('--dry-run', action='store_true',
         help='Do not execute any jobs')
+    parser_process.add_argument('--prequal-config', action='store_true',
+        help='Config file for custom prequal command.')
+    parser_process.add_argument('--qsiprep-config', action='store_true',
+        help='Config file for custom qsiprep command.')
     parser_process.add_argument('--no-gpu', action='store_true',
         help='Run prequal and qsiprep without gpu functionality.')
     parser_process.add_argument('--sub-tasks', nargs='+', default=['prequal', 'qsiprep'],
         help='Run only certain sub tasks')
     parser_process.add_argument('--fs-license',
         help='Base64 encoded FreeSurfer license file')
     parser_process.add_argument('--xnat-alias',
@@ -100,14 +104,18 @@
         help='Job scheduler partition')
     parser_tandem.add_argument('--scheduler', default=None,
         help='Choose a specific job scheduler')
     parser_tandem.add_argument('--rate-limit', type=int, default=None, 
         help='Rate limit the number of tasks executed in parallel (1=serial)')
     parser_tandem.add_argument('--dry-run', action='store_true',
         help='Do not execute any jobs')
+    parser_tandem.add_argument('--prequal-config', action='store_true',
+        help='Config file for custom prequal command.')
+    parser_tandem.add_argument('--qsiprep-config', action='store_true',
+        help='Config file for custom qsiprep command.')
     parser_tandem.add_argument('--no-gpu', action='store_true',
         help='Run prequal and qsiprep without gpu functionality.')
     parser_tandem.add_argument('--sub-tasks', nargs='+', default=['prequal', 'qsiprep'],
         help='Run only certain sub tasks')
     parser_tandem.add_argument('--fs-license',
         help='Base64 encoded FreeSurfer license')
     parser_tandem.add_argument('--xnat-alias',
```

## Comparing `dwiqc-0.6.0.dist-info/LICENSE` & `dwiqc-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.6.0.dist-info/RECORD` & `dwiqc-0.7.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=KtmgDXlNbapHhH_Ac9yg-GV1JKh3fCN1lwAOKacGdU8,247
+dwiqc/__version__.py,sha256=bsQDI73mru8_hF7YcoWhDmY8VGZXgcwwocqPpsv5eQ8,247
 dwiqc/browser/__init__.py,sha256=4lK-1-VH4l6ppP_5Ju6MeYIctiQmFQfGA7gclqh8euE,1352
 dwiqc/cli/__init__.py,sha256=1Y4dYEbkHH-jZ3cwbFnlb6TthH_K0t4xT_-IphRBu6k,61
 dwiqc/cli/get.py,sha256=w2jLbFA7unwfZ-DghKG-_3vPb1RhZPAYX-nXOEbC8wk,6941
-dwiqc/cli/process.py,sha256=HYnB49FFYXOq2NZzWR5RfiLe824coWKQndXxDo-AiDs,6009
-dwiqc/cli/tandem.py,sha256=18t_cn0VrXeAhohg8ukBnDydsR8ZiB8vM0_AZI1Ohkg,4180
-dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
+dwiqc/cli/process.py,sha256=l7nOFDR6cvshAR41k78GiVGqHkaSEy9yyrUxBMLG5nQ,6105
+dwiqc/cli/tandem.py,sha256=Y9IQV33w6TTgFkyJcAs-obe66oKob0w4lwQdYv3Vzf0,4185
+dwiqc/config/__init__.py,sha256=X33iA2gj1lDc6fsIYPUcqvZUDV--IphhJY4JTNd-Yg0,383
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
+dwiqc/config/prequal.yaml,sha256=tm6Jrb5aj7M2EqD87oXXG1VWryws44hn-uzRISeGNkM,1029
+dwiqc/config/qsiprep.yaml,sha256=QlGuIa2jAwNSWkv8CirhWVk50eRoIGVvieiUWGk9k-8,634
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
-dwiqc/tasks/prequal.py,sha256=B4X2kQkumV1RE0-IyxTHkDNR4zHJ3l2B0QHLL80FVBE,15219
+dwiqc/tasks/prequal.py,sha256=eDg53UOQU_RZVbuWoVmo81V2kdB9rFaIzb5L2t1J18Q,15699
 dwiqc/tasks/prequal_EQ.py,sha256=hvs6qjRNoJXuCzdvP-9BnaZc4xwvI9LHSgmueRobt1Q,4656
-dwiqc/tasks/qsiprep.py,sha256=nDxcKcyBvHknRz8ddR2vJmSygRXuNBlhN3RklmsBNU8,7849
+dwiqc/tasks/qsiprep.py,sha256=yw5V1JAbcPFve_L0NMMA_eMpxHLFWNJ_FZkk1oadcRI,8188
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=fjdic3dblSWMag4vOwCcgyHgD2pBcu7qICNrt7HBwVU,13087
-dwiqc-0.6.0.data/scripts/dwiQC.py,sha256=4ZHaJbGDMCkY-CHztDoBK2NmY78Xq9wA_nUV_PtlZUw,6046
-dwiqc-0.6.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.6.0.dist-info/METADATA,sha256=r-AgOxeOLd5NEB6aaBOsCkO-5c1TcZ9vIUiNVQYN9n0,439
-dwiqc-0.6.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-dwiqc-0.6.0.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.6.0.dist-info/RECORD,,
+dwiqc-0.7.0.data/scripts/dwiQC.py,sha256=-hJstgYajn6nQS_QvZgtA1usqEjK1XJHBWutlyphqAs,6571
+dwiqc-0.7.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.7.0.dist-info/METADATA,sha256=AfUXvqzTixJa6qaEPBW7DMb2EJ1nSXVZr6fMHfLzNkw,460
+dwiqc-0.7.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+dwiqc-0.7.0.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.7.0.dist-info/RECORD,,
```

