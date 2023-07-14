# Comparing `tmp/crandr-1.2.0.tar.gz` & `tmp/crandr-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crandr-1.2.0.tar", last modified: Sun Oct  2 07:18:19 2022, max compression
+gzip compressed data, was "crandr-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `crandr-1.2.0.tar` & `crandr-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      187 2022-07-22 16:42:44.109466 crandr-1.2.0/.gitignore
--rw-r--r--   0        0        0      657 2022-06-29 11:38:44.648366 crandr-1.2.0/LICENSE
--rw-r--r--   0        0        0     2659 2022-10-02 07:18:12.296683 crandr-1.2.0/README.md
--rw-r--r--   0        0        0       58 2022-02-06 17:03:56.463432 crandr-1.2.0/_test-output/config/test
--rw-r--r--   0        0        0     4680 2022-02-05 07:58:35.781701 crandr-1.2.0/_test-output/swaymsg/DP-4_ON_eDP-1_OFF.json
--rw-r--r--   0        0        0     5571 2022-02-05 07:58:35.781701 crandr-1.2.0/_test-output/swaymsg/default_eDP-1_DP-4.json
--rw-r--r--   0        0        0     4677 2022-02-05 07:58:35.781701 crandr-1.2.0/_test-output/swaymsg/eDP-1_ON_DP-4_OFF.json
--rw-r--r--   0        0        0     2786 2022-01-31 14:33:45.399284 crandr-1.2.0/_test-output/xrandr/eDP-1_OFF_DP-1-1_OFF_DP-1-2_ON_.txt
--rw-r--r--   0        0        0     2785 2022-01-31 12:14:28.061322 crandr-1.2.0/_test-output/xrandr/eDP-1_OFF_DP-1-1_ON__DP-1-2_OFF.txt
--rw-r--r--   0        0        0     2783 2022-01-31 12:15:08.925069 crandr-1.2.0/_test-output/xrandr/eDP-1_ON__DP-1-1_OFF_DP-1-2_OFF.txt
--rw-r--r--   0        0        0     2291 2022-02-02 12:59:29.668002 crandr-1.2.0/_test-output/xrandr/eDP-1_ON__HDMI-1_OFF.txt
--rw-r--r--   0        0        0     2469 2022-02-02 14:48:34.106464 crandr-1.2.0/_test-output/xrandr/eDP-1_left-of_DP-1-2.txt
--rw-r--r--   0        0        0     2321 2022-02-02 12:59:29.668002 crandr-1.2.0/_test-output/xrandr/eDP-1_mirror_HDMI-1_original.txt
--rw-r--r--   0        0        0      159 2022-02-06 13:50:40.498323 crandr-1.2.0/mypy.ini
--rw-r--r--   0        0        0      501 2022-02-11 13:52:49.286208 crandr-1.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     8524 2022-10-02 07:18:12.296683 crandr-1.2.0/release.sh
--rw-r--r--   0        0        0        5 2022-07-22 16:42:44.109466 crandr-1.2.0/requirements-release.txt
--rw-r--r--   0        0        0       30 2022-07-22 16:42:44.109466 crandr-1.2.0/requirements-test.txt
--rw-r--r--   0        0        0        0 2022-07-22 16:42:44.109466 crandr-1.2.0/requirements.txt
--rw-r--r--   0        0        0      217 2022-02-09 06:51:34.298206 crandr-1.2.0/src/crandr/__init__.py
--rw-r--r--   0        0        0       83 2022-09-30 17:43:24.370020 crandr-1.2.0/src/crandr/__main__.py
--rw-r--r--   0        0        0     4107 2022-09-30 17:26:26.526753 crandr-1.2.0/src/crandr/api_swaymsg.py
--rw-r--r--   0        0        0     3481 2022-02-11 14:08:49.300990 crandr-1.2.0/src/crandr/api_xrandr.py
--rw-r--r--   0        0        0     1346 2022-02-06 16:29:54.393428 crandr-1.2.0/src/crandr/config_paths.py
--rw-r--r--   0        0        0      378 2022-10-02 07:18:12.296683 crandr-1.2.0/src/crandr/doc/example_config
--rw-r--r--   0        0        0    19630 2022-10-02 07:18:12.296683 crandr-1.2.0/src/crandr/main.py
--rw-r--r--   0        0        0     3458 2022-10-02 07:18:12.296683 crandr-1.2.0/src/crandr/model.py
--rw-r--r--   0        0        0        0 2022-03-17 12:10:17.984443 crandr-1.2.0/src/crandr/py.typed
--rw-r--r--   0        0        0     2402 2022-02-06 13:08:30.493335 crandr-1.2.0/src/crandr/utils.py
--rw-r--r--   0        0        0       22 2022-10-02 07:18:12.296683 crandr-1.2.0/src/crandr/version.py
--rw-r--r--   0        0        0     5384 2022-10-02 07:18:12.300016 crandr-1.2.0/tests/test_config.py
--rw-r--r--   0        0        0     9209 2022-02-09 06:43:13.214657 crandr-1.2.0/tests/test_sway.py
--rw-r--r--   0        0        0     2398 2022-02-09 06:43:19.215073 crandr-1.2.0/tests/test_utils.py
--rw-r--r--   0        0        0      237 2022-02-07 08:02:05.214922 crandr-1.2.0/tests/test_without_config.py
--rw-r--r--   0        0        0     8027 2022-10-01 07:52:21.970426 crandr-1.2.0/tests/test_xrandr.py
--rw-r--r--   0        0        0      369 2022-03-17 08:16:11.790988 crandr-1.2.0/tox.ini
--rw-r--r--   0        0        0     3117 1970-01-01 00:00:00.000000 crandr-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      187 2022-11-03 16:33:34.583339 crandr-1.2.1/.gitignore
+-rw-r--r--   0        0        0      657 2022-11-03 16:33:34.583339 crandr-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2659 2022-11-03 16:33:34.583339 crandr-1.2.1/README.md
+-rw-r--r--   0        0        0       58 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/config/test
+-rw-r--r--   0        0        0     4680 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/swaymsg/DP-4_ON_eDP-1_OFF.json
+-rw-r--r--   0        0        0     5571 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/swaymsg/default_eDP-1_DP-4.json
+-rw-r--r--   0        0        0     4677 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/swaymsg/eDP-1_ON_DP-4_OFF.json
+-rw-r--r--   0        0        0     2786 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/xrandr/eDP-1_OFF_DP-1-1_OFF_DP-1-2_ON_.txt
+-rw-r--r--   0        0        0     2785 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/xrandr/eDP-1_OFF_DP-1-1_ON__DP-1-2_OFF.txt
+-rw-r--r--   0        0        0     2783 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/xrandr/eDP-1_ON__DP-1-1_OFF_DP-1-2_OFF.txt
+-rw-r--r--   0        0        0     2291 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/xrandr/eDP-1_ON__HDMI-1_OFF.txt
+-rw-r--r--   0        0        0     2469 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/xrandr/eDP-1_left-of_DP-1-2.txt
+-rw-r--r--   0        0        0     2321 2022-11-03 16:33:34.583339 crandr-1.2.1/_test-output/xrandr/eDP-1_mirror_HDMI-1_original.txt
+-rw-r--r--   0        0        0      177 2023-07-14 07:44:07.668873 crandr-1.2.1/mypy.ini
+-rw-r--r--   0        0        0      501 2022-11-03 16:33:34.583339 crandr-1.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     8524 2022-11-03 16:33:34.586672 crandr-1.2.1/release.sh
+-rw-r--r--   0        0        0        5 2022-11-03 16:33:34.586672 crandr-1.2.1/requirements-release.txt
+-rw-r--r--   0        0        0       30 2022-11-03 16:33:34.586672 crandr-1.2.1/requirements-test.txt
+-rw-r--r--   0        0        0        0 2022-11-03 16:33:34.586672 crandr-1.2.1/requirements.txt
+-rw-r--r--   0        0        0      217 2022-11-03 16:33:34.586672 crandr-1.2.1/src/crandr/__init__.py
+-rw-r--r--   0        0        0       83 2022-11-03 16:33:34.586672 crandr-1.2.1/src/crandr/__main__.py
+-rw-r--r--   0        0        0     4155 2023-07-14 07:44:07.668873 crandr-1.2.1/src/crandr/api_swaymsg.py
+-rw-r--r--   0        0        0     4128 2023-07-14 07:44:07.668873 crandr-1.2.1/src/crandr/api_xrandr.py
+-rw-r--r--   0        0        0     1346 2022-11-03 16:33:34.586672 crandr-1.2.1/src/crandr/config_paths.py
+-rw-r--r--   0        0        0      378 2022-11-03 16:33:34.586672 crandr-1.2.1/src/crandr/doc/example_config
+-rw-r--r--   0        0        0    19657 2023-07-14 07:44:07.668873 crandr-1.2.1/src/crandr/main.py
+-rw-r--r--   0        0        0     3500 2023-07-14 07:44:07.668873 crandr-1.2.1/src/crandr/model.py
+-rw-r--r--   0        0        0        0 2022-11-03 16:33:34.586672 crandr-1.2.1/src/crandr/py.typed
+-rw-r--r--   0        0        0     2402 2022-11-03 16:33:34.586672 crandr-1.2.1/src/crandr/utils.py
+-rw-r--r--   0        0        0       22 2023-07-14 07:44:07.668873 crandr-1.2.1/src/crandr/version.py
+-rw-r--r--   0        0        0     5384 2022-11-03 16:33:34.586672 crandr-1.2.1/tests/test_config.py
+-rw-r--r--   0        0        0     9209 2022-11-03 16:33:34.586672 crandr-1.2.1/tests/test_sway.py
+-rw-r--r--   0        0        0     2398 2022-11-03 16:33:34.586672 crandr-1.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0      237 2022-11-03 16:33:34.586672 crandr-1.2.1/tests/test_without_config.py
+-rw-r--r--   0        0        0     8129 2023-07-14 07:44:07.668873 crandr-1.2.1/tests/test_xrandr.py
+-rw-r--r--   0        0        0      358 2023-07-14 07:44:07.668873 crandr-1.2.1/tox.ini
+-rw-r--r--   0        0        0     3117 1970-01-01 00:00:00.000000 crandr-1.2.1/PKG-INFO
```

### Comparing `crandr-1.2.0/LICENSE` & `crandr-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/README.md` & `crandr-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/swaymsg/DP-4_ON_eDP-1_OFF.json` & `crandr-1.2.1/_test-output/swaymsg/DP-4_ON_eDP-1_OFF.json`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/swaymsg/default_eDP-1_DP-4.json` & `crandr-1.2.1/_test-output/swaymsg/default_eDP-1_DP-4.json`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/swaymsg/eDP-1_ON_DP-4_OFF.json` & `crandr-1.2.1/_test-output/swaymsg/eDP-1_ON_DP-4_OFF.json`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/xrandr/eDP-1_OFF_DP-1-1_OFF_DP-1-2_ON_.txt` & `crandr-1.2.1/_test-output/xrandr/eDP-1_OFF_DP-1-1_OFF_DP-1-2_ON_.txt`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/xrandr/eDP-1_OFF_DP-1-1_ON__DP-1-2_OFF.txt` & `crandr-1.2.1/_test-output/xrandr/eDP-1_OFF_DP-1-1_ON__DP-1-2_OFF.txt`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/xrandr/eDP-1_ON__DP-1-1_OFF_DP-1-2_OFF.txt` & `crandr-1.2.1/_test-output/xrandr/eDP-1_ON__DP-1-1_OFF_DP-1-2_OFF.txt`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/xrandr/eDP-1_ON__HDMI-1_OFF.txt` & `crandr-1.2.1/_test-output/xrandr/eDP-1_ON__HDMI-1_OFF.txt`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/xrandr/eDP-1_left-of_DP-1-2.txt` & `crandr-1.2.1/_test-output/xrandr/eDP-1_left-of_DP-1-2.txt`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/_test-output/xrandr/eDP-1_mirror_HDMI-1_original.txt` & `crandr-1.2.1/_test-output/xrandr/eDP-1_mirror_HDMI-1_original.txt`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/release.sh` & `crandr-1.2.1/release.sh`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/src/crandr/api_swaymsg.py` & `crandr-1.2.1/src/crandr/api_swaymsg.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 		model.Rotation.INVERTED : '180',
 		model.Rotation.LEFT : '270',
 	}
 
 	def turn_off_and_on(self,
 			monitors_to_be_turned_off: typing.Iterable[model.Monitor],
 			monitors_to_be_turned_on: typing.Iterable[model.Monitor],
-			*, verbose: bool, dry_run: bool) -> None:
+			*, primary: typing.Optional[model.Monitor] = None, verbose: bool, dry_run: bool) -> None:
 		get_name: typing.Callable[[model.Monitor], str]
 		if self.use_short_names:
 			get_name = lambda m: m.name
 		else:
 			get_name = lambda m: m.long_name
 		for monitor in monitors_to_be_turned_on:
 			x, y = self._calc_position(monitor)
```

### Comparing `crandr-1.2.0/src/crandr/api_xrandr.py` & `crandr-1.2.1/src/crandr/api_xrandr.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 		model.Rotation.LEFT : 'left',
 		model.Rotation.RIGHT : 'right',
 	}
 
 	def turn_off_and_on(self,
 			monitors_to_be_turned_off: typing.Iterable[model.Monitor],
 			monitors_to_be_turned_on: typing.Iterable[model.Monitor],
-			*, verbose: bool, dry_run: bool) -> None:
+			*, primary: typing.Optional[model.Monitor] = None, verbose: bool, dry_run: bool) -> None:
 		cmd = ['xrandr']
 		for monitor in monitors_to_be_turned_off:
 			cmd.extend(['--output', monitor.name, '--off'])
 		for monitor in monitors_to_be_turned_on:
 			cmd.extend(['--output', monitor.name])
 			if monitor.position:
 				cmd.append(self.direction_map[monitor.position.direction])
@@ -110,17 +110,37 @@
 			if monitor.scale:
 				cmd.append('--scale')
 				cmd.append(f'{monitor.scale.x}x{monitor.scale.y}')
 			if monitor.rotation:
 				cmd.append('--rotate')
 				cmd.append(self.rotation_map[monitor.rotation])
 
+		if primary:
+			cmd.extend(['--output', primary.name, '--primary'])
+
 		if verbose:
 			print(shlex.join(cmd))
 		if not dry_run:
-			subprocess.run(cmd, check=True)
+			try:
+				subprocess.run(cmd, check=True, text=True, stderr=subprocess.PIPE)
+			except subprocess.CalledProcessError as e:
+				m = re.match('xrandr: Configure crtc ([0-9]) failed', e.stderr)
+				if m:
+					crtc = m.group(1)
+					if crtc == '0':
+						crtc = '1'
+					else:
+						crtc = '0'
+					#https://askubuntu.com/questions/136139/xrandr-configure-crtc-0-failed-when-trying-to-change-resolution-on-external-m
+					cmd.extend(['--crtc',  '1'])
+					if verbose:
+						print(shlex.join(cmd))
+					subprocess.run(cmd, check=True)
+				else:
+					print(e.stderr)
+
 
 
 if __name__ == '__main__':
 	api = Api()
 	for m in api.iter_connected_monitors():
 		print(m)
```

### Comparing `crandr-1.2.0/src/crandr/config_paths.py` & `crandr-1.2.1/src/crandr/config_paths.py`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/src/crandr/main.py` & `crandr-1.2.1/src/crandr/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 		print("no further monitor to be turned on in %s" % ",".join(args.connections))
 		sys.exit(1)
 	
 	monitors_to_be_turned_on = monitors_to_be_turned_on[:1]
 	monitors_to_be_turned_on[0].position = model.Position(direction, reference_monitor)
 	monitors_to_be_turned_on[0].scale = model.Scale(1, 1)
 	
-	api.turn_off_and_on(monitors_to_be_turned_off, monitors_to_be_turned_on, verbose=args.verbose, dry_run=args.dry_run)
+	api.turn_off_and_on(monitors_to_be_turned_off, monitors_to_be_turned_on, primary=reference_monitor, verbose=args.verbose, dry_run=args.dry_run)
 
 def mirror(api: model.Api, args: argparse.Namespace) -> None:
 	'''turn on all monitors and mirror the content'''
 	monitors = list(api.iter_connected_monitors(test_input=args.test_input))
 	if not monitors:
 		print("no monitors connected", file=sys.stderr)
 		sys.exit(1)
@@ -379,18 +379,18 @@
 				raise argparse.ArgumentTypeError(f'invalid connection {c!r}, should be one of {possible_connections}')
 		return connections_list
 
 	root_parser.set_defaults(func=default)
 	root_parser.add_argument('--version', action='store_true', help=print_version.__doc__)
 	root_parser.add_argument('-n', '--dry-run', action='store_true', help='do not run the command to change the monitors (implies --verbose)')
 	root_parser.add_argument('-v', '--verbose', action='store_true', help='print the command to change the monitors')
-	root_parser.add_argument('--wait', type=float, help='time to wait before starting, this may help if you are experiencing trouble when binding this command to a key on sway')
 	root_parser.add_argument('--test-input', help='a file which contains the output of the backend')
 	root_parser.add_argument('--backend', default=DEFAULT_BACKEND, choices=BACKENDS.keys(), help='the command used to configure the monitors')
 	root_parser.add_argument('--use-short-names-on-sway', action='store_true', help='[swaymsg only] use names like eDP-1 and DP-4. These names can change when disconnecting and reconnecting a monitor which can lead to a situation where all monitors are disabled even after reconnecting a previously enabled monitor. Therefore the default behavior is to use longer names based on make, model and serial, see man sway-output.')
+	root_parser.add_argument('--wait', type=float, help='time to wait before starting, this may help if you are experiencing trouble when binding this command to a key on sway')
 
 	parser = add_subparser(cycle)
 	parser.add_argument('connections', type=connection, nargs='?', default=CONNECTION_ANY, help=f'a comma separated list of connections which should be considered for activation: {possible_connections}')
 
 	parser = add_subparser(toggle)
 	parser.add_argument('connections1', type=connection, nargs='?', default=CONNECTION_EXTERNAL, help=f'one of {possible_connections}')
 	parser.add_argument('connections2', type=connection, nargs='?', default=model.CONNECTION_INTERNAL, help=f'one of {possible_connections}')
```

### Comparing `crandr-1.2.0/src/crandr/model.py` & `crandr-1.2.1/src/crandr/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,13 +141,13 @@
 
 	def iter_connected_monitors(self, test_input: typing.Optional[str] = None) -> typing.Iterator[Monitor]:
 		raise NotImplementedError()
 
 	def turn_off_and_on(self,
 			monitors_to_be_turned_off: typing.Iterable[Monitor],
 			monitors_to_be_turned_on: typing.Iterable[Monitor],
-			*, verbose: bool, dry_run: bool) -> None:
+			*, primary: typing.Optional[Monitor] = None, verbose: bool, dry_run: bool) -> None:
 		raise NotImplementedError()
 
 
 if __name__ == '__main__':
 	pass
```

### Comparing `crandr-1.2.0/src/crandr/utils.py` & `crandr-1.2.1/src/crandr/utils.py`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/tests/test_config.py` & `crandr-1.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/tests/test_sway.py` & `crandr-1.2.1/tests/test_sway.py`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/tests/test_utils.py` & `crandr-1.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `crandr-1.2.0/tests/test_xrandr.py` & `crandr-1.2.1/tests/test_xrandr.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,39 +112,39 @@
 
 	def test_extend_left(self, use_xrandr, capsys):
 		fn = '_test-output/xrandr/eDP-1_OFF_DP-1-1_ON__DP-1-2_OFF.txt'
 		args = ['--dry-run', '--test-input', fn, 'extend', 'left']
 		main.main(args)
 
 		cmd = capsys.readouterr().out.rstrip()
-		assert cmd == 'xrandr --output eDP-1 --left-of DP-1-1 --auto --scale 1x1'
+		assert cmd == 'xrandr --output eDP-1 --left-of DP-1-1 --auto --scale 1x1 --output DP-1-1 --primary'
 
 	def test_extend_right(self, use_xrandr, capsys):
 		fn = '_test-output/xrandr/eDP-1_OFF_DP-1-1_ON__DP-1-2_OFF.txt'
 		args = ['--dry-run', '--test-input', fn, 'extend', 'right', 'external']
 		main.main(args)
 
 		cmd = capsys.readouterr().out.rstrip()
-		assert cmd == 'xrandr --output DP-1-2 --right-of DP-1-1 --auto --scale 1x1'
+		assert cmd == 'xrandr --output DP-1-2 --right-of DP-1-1 --auto --scale 1x1 --output DP-1-1 --primary'
 
 	def test_extend_above(self, use_xrandr, capsys):
 		fn = '_test-output/xrandr/eDP-1_ON__DP-1-1_OFF_DP-1-2_OFF.txt'
 		args = ['--dry-run', '--test-input', fn, 'extend', 'above']
 		main.main(args)
 
 		cmd = capsys.readouterr().out.rstrip()
-		assert cmd == 'xrandr --output DP-1-1 --above eDP-1 --auto --scale 1x1'
+		assert cmd == 'xrandr --output DP-1-1 --above eDP-1 --auto --scale 1x1 --output eDP-1 --primary'
 
 	def test_extend_below(self, use_xrandr, capsys):
 		fn = '_test-output/xrandr/eDP-1_ON__DP-1-1_OFF_DP-1-2_OFF.txt'
 		args = ['--dry-run', '--test-input', fn, 'extend', 'below', 'external']
 		main.main(args)
 
 		cmd = capsys.readouterr().out.rstrip()
-		assert cmd == 'xrandr --output DP-1-1 --below eDP-1 --auto --scale 1x1'
+		assert cmd == 'xrandr --output DP-1-1 --below eDP-1 --auto --scale 1x1 --output eDP-1 --primary'
 
 
 class TestMirror:
 
 	def test_mirror_one(self, use_xrandr, capsys):
 		fn = '_test-output/xrandr/eDP-1_ON__HDMI-1_OFF.txt'
 		args = ['--dry-run', '--test-input', fn, 'mirror']
```

### Comparing `crandr-1.2.0/PKG-INFO` & `crandr-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crandr
-Version: 1.2.0
+Version: 1.2.1
 Summary: This is a unifying wrapper around xrandr and swaymsg to control your monitors/outputs,
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
```

