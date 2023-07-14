# Comparing `tmp/ex4nicegui-0.1.6.tar.gz` & `tmp/ex4nicegui-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.6.tar", last modified: Wed Jul 12 13:33:11 2023, max compression
+gzip compressed data, was "ex4nicegui-0.1.7.tar", last modified: Fri Jul 14 15:34:28 2023, max compression
```

## Comparing `ex4nicegui-0.1.6.tar` & `ex4nicegui-0.1.7.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.376175 ex4nicegui-0.1.6/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-12 13:33:11.374181 ex4nicegui-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.295793 ex4nicegui-0.1.6/ex4nicegui/
--rw-rw-rw-   0        0        0      337 2023-07-12 13:32:55.000000 ex4nicegui-0.1.6/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.310648 ex4nicegui-0.1.6/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.6/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.6/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.328109 ex4nicegui-0.1.6/ex4nicegui/reactive/
--rw-rw-rw-   0        0        0      998 2023-07-10 14:31:39.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.334095 ex4nicegui-0.1.6/ex4nicegui/reactive/draggable/
--rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/draggable/UseDraggable.js
--rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/draggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/draggable/__init__.py
--rw-rw-rw-   0        0        0     1365 2023-07-10 14:31:39.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/drawer.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.344066 ex4nicegui-0.1.6/ex4nicegui/reactive/echarts/
--rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/echarts/ECharts.js
--rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/echarts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/echarts/__init__.py
--rw-rw-rw-   0        0        0     6106 2023-07-10 14:31:39.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0    31607 2023-07-12 13:32:36.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/officials.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/rxui.py
--rw-rw-rw-   0        0        0      803 2023-07-05 06:10:00.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/signature.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.349528 ex4nicegui-0.1.6/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.6/ex4nicegui/reactive/useMouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.359501 ex4nicegui-0.1.6/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.6/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.6/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.372185 ex4nicegui-0.1.6/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.6/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.6/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.6/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:11.307657 ex4nicegui-0.1.6/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-12 13:33:10.000000 ex4nicegui-0.1.6/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2023-07-12 13:33:10.000000 ex4nicegui-0.1.6/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:33:10.000000 ex4nicegui-0.1.6/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-12 13:33:10.000000 ex4nicegui-0.1.6/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-07-12 13:33:10.000000 ex4nicegui-0.1.6/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 13:33:10.000000 ex4nicegui-0.1.6/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 13:33:11.377172 ex4nicegui-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2088 2023-07-10 14:33:48.000000 ex4nicegui-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.808192 ex4nicegui-0.1.7/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-14 15:34:28.805831 ex4nicegui-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.689114 ex4nicegui-0.1.7/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-14 15:34:04.000000 ex4nicegui-0.1.7/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.705072 ex4nicegui-0.1.7/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.721301 ex4nicegui-0.1.7/ex4nicegui/reactive/
+-rw-rw-rw-   0        0        0     1217 2023-07-14 15:33:47.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.742602 ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/
+-rw-rw-rw-   0        0        0     4851 2023-07-05 09:28:02.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     3041 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/__init__.py
+-rw-rw-rw-   0        0        0     1365 2023-07-10 14:31:39.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/drawer.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.775627 ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/ECharts.js
+-rw-rw-rw-   0        0        0     2685 2023-07-09 14:56:08.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/__init__.py
+-rw-rw-rw-   0        0        0     6106 2023-07-10 14:31:39.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0    35637 2023-07-14 15:33:47.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/officials.py
+-rw-rw-rw-   0        0        0     1224 2023-07-14 15:33:47.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/rxui.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.795887 ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2244 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2093 2023-07-14 15:33:47.000000 ex4nicegui-0.1.7/ex4nicegui/reactive/usePagination.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.798846 ex4nicegui-0.1.7/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.7/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.803832 ex4nicegui-0.1.7/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.7/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.7/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.7/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:34:28.701083 ex4nicegui-0.1.7/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 15:34:28.000000 ex4nicegui-0.1.7/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:34:28.808192 ex4nicegui-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2088 2023-07-10 14:33:48.000000 ex4nicegui-0.1.7/setup.py
```

### Comparing `ex4nicegui-0.1.6/LICENSE` & `ex4nicegui-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/README.md` & `ex4nicegui-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.1.7/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/__index.py` & `ex4nicegui-0.1.7/ex4nicegui/reactive/__index.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,19 @@
     ColorPickerBindableUi as color_picker,
     ColorPickerLazyBindableUi as lazy_color_picker,
     EChartsBindableUi as echarts,
     RowBindableUi as row,
     CardBindableUi as card,
     CardSectionBindableUi as card_section,
     CardActionsBindableUi as card_actions,
+    SliderBindableUi as slider,
+    LazySliderBindableUi as lazy_slider,
+    HtmlBindableUi as html,
 )
+from .q_pagination import QPagination as q_pagination
 from .local_file_picker import local_file_picker
 from ex4nicegui.utils.signals import ref_computed
 from signe import effect
 from .draggable.UseDraggable import use_draggable
 from .useMouse.UseMouse import use_mouse
 from .drawer import drawer
+from .usePagination import PaginationRef as use_pagination
```

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/draggable/UseDraggable.js` & `ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/draggable/UseDraggable.py` & `ex4nicegui-0.1.7/ex4nicegui/reactive/draggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.1.7/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/echarts/ECharts.js` & `ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/echarts/ECharts.py` & `ex4nicegui-0.1.7/ex4nicegui/reactive/echarts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.1.7/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/officials.py` & `ex4nicegui-0.1.7/ex4nicegui/reactive/officials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+import asyncio
 
 from typing import (
     Any,
     Callable,
     List,
     Optional,
     TypeVar,
@@ -64,14 +65,23 @@
         *,
         remove: Optional[str] = None,
         replace: Optional[str] = None,
     ):
         cast(ui.element, self.element).style(add, remove=remove, replace=replace)
         return self
 
+    def add_slot(self, name: str, template: Optional[str] = None):
+        """Add a slot to the element.
+
+        :param name: name of the slot
+        :param template: Vue template of the slot
+        :return: the slot
+        """
+        return cast(ui.element, self.element).add_slot(name, template)
+
     @property
     def element(self):
         return self.__element
 
     def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
         if prop == "visible":
             return self.bind_visible(ref_ui)
@@ -171,15 +181,15 @@
 
         binder.element.on("update:modelValue", handler=onValueChanged)
 
     def __init__(
         self,
         options: Union[TMaybeRef[List], TMaybeRef[Dict]],
         *,
-        label: TMaybeRef[Optional[str]] = None,
+        label: Optional[TMaybeRef[str]] = None,
         value: TMaybeRef[Any] = None,
         on_change: Optional[Callable[..., Any]] = None,
         with_input: TMaybeRef[bool] = False,
         multiple: TMaybeRef[bool] = False,
         clearable: TMaybeRef[bool] = False,
     ) -> None:
         kws = {
@@ -385,22 +395,22 @@
 
         return self
 
 
 class InputBindableUi(SingleValueBindableUi[str, ui.input]):
     def __init__(
         self,
-        label: TMaybeRef[Optional[str]] = None,
+        label: Optional[TMaybeRef[str]] = None,
         *,
-        placeholder: TMaybeRef[Optional[str]] = None,
+        placeholder: Optional[TMaybeRef[str]] = None,
         value: TMaybeRef[str] = "",
         password: TMaybeRef[bool] = False,
         password_toggle_button: TMaybeRef[bool] = False,
         on_change: Optional[Callable[..., Any]] = None,
-        autocomplete: TMaybeRef[Optional[List[str]]] = None,
+        autocomplete: Optional[TMaybeRef[List[str]]] = None,
         validation: Dict[str, Callable[..., bool]] = {},
     ) -> None:
         kws = {
             "label": label,
             "placeholder": placeholder,
             "value": value,
             "password": password,
@@ -426,15 +436,15 @@
         ele = self.element
 
         @effect
         def _():
             ele.value = self.value
 
         def onModelValueChanged(args):
-            self._ref.value = args["args"]  # type: ignore
+            self._ref.value = args["args"] or ""  # type: ignore
 
         ele.on("update:modelValue", handler=onModelValueChanged)
 
     def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
         if prop == "value":
             return self.bind_value(ref_ui)
 
@@ -447,22 +457,22 @@
 
         return self
 
 
 class LazyInputBindableUi(InputBindableUi):
     def __init__(
         self,
-        label: TMaybeRef[Optional[str]] = None,
+        label: Optional[TMaybeRef[str]] = None,
         *,
-        placeholder: TMaybeRef[Optional[str]] = None,
+        placeholder: Optional[TMaybeRef[str]] = None,
         value: TMaybeRef[str] = "",
         password: TMaybeRef[bool] = False,
         password_toggle_button: TMaybeRef[bool] = False,
         on_change: Optional[Callable[..., Any]] = None,
-        autocomplete: TMaybeRef[Optional[List[str]]] = None,
+        autocomplete: Optional[TMaybeRef[List[str]]] = None,
         validation: Dict[str, Callable[..., bool]] = {},
     ) -> None:
         super().__init__(
             label,
             placeholder=placeholder,
             value=value,
             password=password,
@@ -476,26 +486,108 @@
         ele = self.element
 
         @effect
         def _():
             ele.value = self.value
 
         def onValueChanged():
-            self._ref.value = ele.value
+            self._ref.value = ele.value or ""
 
         ele.on("blur", onValueChanged)
         ele.on("keyup.enter", onValueChanged)
 
 
+_TSliderValue = TypeVar("_TSliderValue", float, int)
+
+
+class SliderBindableUi(SingleValueBindableUi[Optional[_TSliderValue], ui.slider]):
+    def __init__(
+        self,
+        min: TMaybeRef[_TSliderValue],
+        max: TMaybeRef[_TSliderValue],
+        step: TMaybeRef[_TSliderValue] = 1.0,
+        value: Optional[TMaybeRef[_TSliderValue]] = None,
+        on_change: Optional[Callable[..., Any]] = None,
+    ) -> None:
+        kws = {
+            "min": min,
+            "max": max,
+            "step": step,
+            "value": value,
+            "on_change": on_change,
+        }
+
+        value_kws = _convert_kws_ref2value(kws)
+
+        element = ui.slider(**value_kws).props("label label-always switch-label-side")
+
+        super().__init__(value, element)  # type: ignore
+
+        for key, value in kws.items():
+            if is_ref(value) and key != "value":
+                self.bind_prop(key, value)  # type: ignore
+
+        self._ex_setup()
+
+    def _ex_setup(self):
+        ele = self.element
+
+        @effect
+        def _():
+            ele.value = self.value
+
+        def onModelValueChanged(args):
+            self._ref.value = args["args"]  # type: ignore
+
+        ele.on("update:modelValue", handler=onModelValueChanged)
+
+    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+        if prop == "value":
+            return self.bind_value(ref_ui)
+
+        return super().bind_prop(prop, ref_ui)
+
+    def bind_value(self, ref_ui: ReadonlyRef[float]):
+        @effect
+        def _():
+            self.element.on_value_change(ref_ui.value)
+
+        return self
+
+
+class LazySliderBindableUi(SliderBindableUi):
+    def __init__(
+        self,
+        min: TMaybeRef[float],
+        max: TMaybeRef[float],
+        step: TMaybeRef[float] = 1,
+        value: TMaybeRef[float | None] = None,
+        on_change: Callable[..., Any] | None = None,
+    ) -> None:
+        super().__init__(min, max, step, value, on_change)
+
+    def _ex_setup(self):
+        ele = self.element
+
+        @effect
+        def _():
+            ele.value = self.value
+
+        def onValueChanged():
+            self._ref.value = ele.value
+
+        ele.on("change ", onValueChanged)
+
+
 class TextareaBindableUi(SingleValueBindableUi[str, ui.textarea]):
     def __init__(
         self,
-        label: TMaybeRef[Optional[str]] = None,
+        label: Optional[TMaybeRef[str]] = None,
         *,
-        placeholder: TMaybeRef[Optional[str]] = None,
+        placeholder: Optional[TMaybeRef[str]] = None,
         value: TMaybeRef[str] = "",
         on_change: Optional[Callable[..., Any]] = None,
         validation: Dict[str, Callable[..., bool]] = {},
     ) -> None:
         kws = {
             "label": label,
             "placeholder": placeholder,
@@ -541,17 +633,17 @@
 
         return self
 
 
 class LazyTextareaBindableUi(TextareaBindableUi):
     def __init__(
         self,
-        label: TMaybeRef[Optional[str]] = None,
+        label: Optional[TMaybeRef[str]] = None,
         *,
-        placeholder: TMaybeRef[Optional[str]] = None,
+        placeholder: Optional[TMaybeRef[str]] = None,
         value: TMaybeRef[str] = "",
         on_change: Optional[Callable[..., Any]] = None,
         validation: Dict[str, Callable[..., bool]] = {},
     ) -> None:
         super().__init__(
             label,
             placeholder=placeholder,
@@ -633,16 +725,16 @@
 
 
 class IconBindableUi(SingleValueBindableUi[str, ui.icon]):
     def __init__(
         self,
         name: TMaybeRef[str],
         *,
-        size: TMaybeRef[Optional[str]] = None,
-        color: TMaybeRef[Optional[str]] = None,
+        size: Optional[TMaybeRef[str]] = None,
+        color: Optional[TMaybeRef[str]] = None,
     ) -> None:
         kws = {
             "name": name,
             "size": size,
             "color": color,
         }
 
@@ -680,16 +772,16 @@
 
 class ButtonBindableUi(SingleValueBindableUi[str, ui.button]):
     def __init__(
         self,
         text: TMaybeRef[str] = "",
         *,
         on_click: Optional[Callable[..., Any]] = None,
-        color: TMaybeRef[Optional[str]] = "primary",
-        icon: TMaybeRef[Optional[str]] = None,
+        color: Optional[TMaybeRef[str]] = "primary",
+        icon: Optional[TMaybeRef[str]] = None,
     ) -> None:
         kws = {
             "text": text,
             "color": color,
             "icon": icon,
             "on_click": on_click,
         }
@@ -893,17 +985,17 @@
 
 class TableBindableUi(BindableUi[ui.table]):
     def __init__(
         self,
         columns: TMaybeRef[List[Dict]],
         rows: TMaybeRef[List[Dict]],
         row_key: TMaybeRef[str] = "id",
-        title: TMaybeRef[Optional[str]] = None,
-        selection: TMaybeRef[Optional[Literal["single", "multiple"]]] = None,
-        pagination: TMaybeRef[Optional[int]] = 15,
+        title: Optional[TMaybeRef[str]] = None,
+        selection: Optional[TMaybeRef[Literal["single", "multiple"]]] = None,
+        pagination: Optional[TMaybeRef[int]] = 15,
         on_select: Optional[Callable[..., Any]] = None,
     ) -> None:
         kws = {
             "columns": columns,
             "rows": rows,
             "row_key": row_key,
             "title": title,
@@ -1149,7 +1241,63 @@
 
     def __enter__(self):
         self.element.__enter__()
         return self
 
     def __exit__(self, *_: Any):
         self.element.__exit__(*_)
+
+
+class HtmlBindableUi(SingleValueBindableUi[str, ui.html]):
+    @staticmethod
+    def _setup_(binder: "HtmlBindableUi"):
+        first = True
+
+        @effect
+        def _():
+            nonlocal first
+
+            async def task():
+                pass
+                await ui.run_javascript(
+                    f"getElement({binder.element.id}).innerText= '{binder.value}' ",
+                    respond=False,
+                )
+
+            if not first:
+                asyncio.run(task())
+            else:
+                first = False
+
+    def __init__(
+        self,
+        content: TMaybeRef[str] = "",
+    ) -> None:
+        kws = {
+            "content": content,
+        }
+
+        value_kws = _convert_kws_ref2value(kws)
+
+        element = ui.html(**value_kws)
+
+        super().__init__(content, element)
+
+        for key, value in kws.items():
+            if is_ref(value):
+                self.bind_prop(key, value)  # type: ignore
+
+        HtmlBindableUi._setup_(self)
+
+    def bind_prop(self, prop: str, ref_ui: ReadonlyRef):
+        if prop == "color":
+            return self.bind_color(ref_ui)
+
+        return super().bind_prop(prop, ref_ui)
+
+    def bind_color(self, ref_ui: ReadonlyRef):
+        @effect
+        def _():
+            ele = self.element
+            color = ref_ui.value
+            ele._style["color"] = color
+            ele.update()
```

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.1.7/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/tools/debug.py` & `ex4nicegui-0.1.7/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui/utils/signals.py` & `ex4nicegui-0.1.7/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.6/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.1.7/ex4nicegui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 ex4nicegui/layout/__init__.py
 ex4nicegui/layout/gridbox.py
 ex4nicegui/reactive/__index.py
 ex4nicegui/reactive/__init__.py
 ex4nicegui/reactive/drawer.py
 ex4nicegui/reactive/local_file_picker.py
 ex4nicegui/reactive/officials.py
+ex4nicegui/reactive/q_pagination.py
 ex4nicegui/reactive/rxui.py
-ex4nicegui/reactive/signature.py
+ex4nicegui/reactive/usePagination.py
 ex4nicegui/reactive/draggable/UseDraggable.js
 ex4nicegui/reactive/draggable/UseDraggable.py
 ex4nicegui/reactive/draggable/__init__.py
 ex4nicegui/reactive/echarts/ECharts.js
 ex4nicegui/reactive/echarts/ECharts.py
 ex4nicegui/reactive/echarts/__init__.py
 ex4nicegui/reactive/useMouse/UseMouse.js
```

### Comparing `ex4nicegui-0.1.6/setup.py` & `ex4nicegui-0.1.7/setup.py`

 * *Files identical despite different names*

