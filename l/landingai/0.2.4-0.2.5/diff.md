# Comparing `tmp/landingai-0.2.4.tar.gz` & `tmp/landingai-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.2.4.tar", max compression
+gzip compressed data, was "landingai-0.2.5.tar", max compression
```

## Comparing `landingai-0.2.4.tar` & `landingai-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1063 2023-07-13 17:29:25.948012 landingai-0.2.4/LICENSE.md
--rw-r--r--   0        0        0     6774 2023-07-13 17:29:25.948012 landingai-0.2.4/README.md
--rw-r--r--   0        0        0      354 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/__init__.py
--rw-r--r--   0        0        0     6833 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/client.py
--rw-r--r--   0        0        0    21135 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/media.py
--rw-r--r--   0        0        0     4722 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9730 2023-07-13 17:29:25.984012 landingai-0.2.4/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-13 17:29:25.996012 landingai-0.2.4/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0      419 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0    16392 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/pipeline/frameset.py
--rw-r--r--   0        0        0    16998 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     1339 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/pipeline/postprocessing.py
--rw-r--r--   0        0        0     8389 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/postprocess.py
--rw-r--r--   0        0        0    25559 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/predict.py
--rw-r--r--   0        0        0     6068 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4439 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/storage/data_access.py
--rw-r--r--   0        0        0     4340 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     2657 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/telemetry.py
--rw-r--r--   0        0        0     1685 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/utils.py
--rw-r--r--   0        0        0    13403 2023-07-13 17:29:26.000012 landingai-0.2.4/landingai/visualize.py
--rw-r--r--   0        0        0     2606 2023-07-13 17:29:26.924010 landingai-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 landingai-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-14 12:14:28.628564 landingai-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0     6743 2023-07-14 12:14:28.628564 landingai-0.2.5/README.md
+-rw-r--r--   0        0        0      354 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/__init__.py
+-rw-r--r--   0        0        0     6451 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/client.py
+-rw-r--r--   0        0        0    21135 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9730 2023-07-14 12:14:28.660565 landingai-0.2.5/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-14 12:14:28.668565 landingai-0.2.5/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     4750 2023-07-14 12:14:28.668565 landingai-0.2.5/landingai/notebook_utils.py
+-rw-r--r--   0        0        0      420 2023-07-14 12:14:28.668565 landingai-0.2.5/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0    16449 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/pipeline/frameset.py
+-rw-r--r--   0        0        0    17016 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     1339 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/pipeline/postprocessing.py
+-rw-r--r--   0        0        0     8389 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/postprocess.py
+-rw-r--r--   0        0        0    25559 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/predict.py
+-rw-r--r--   0        0        0     6462 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4439 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/storage/data_access.py
+-rw-r--r--   0        0        0     4340 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1503 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/telemetry.py
+-rw-r--r--   0        0        0     1685 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/utils.py
+-rw-r--r--   0        0        0    13403 2023-07-14 12:14:28.672565 landingai-0.2.5/landingai/visualize.py
+-rw-r--r--   0        0        0     2606 2023-07-14 12:14:29.360574 landingai-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     7988 1970-01-01 00:00:00.000000 landingai-0.2.5/PKG-INFO
```

### Comparing `landingai-0.2.4/LICENSE.md` & `landingai-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/README.md` & `landingai-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,22 +55,21 @@
 
 1. Install the Python library.
 2. Create a `Predictor` class with your Endpoint ID, API Key, and API Secret.
 3. Load your image into a NumPy array (below the image is "image.png")
 4. Call the `predict()` function with an image (using the NumPy array format).
 
 ```python
-import numpy as np
 from PIL import Image
 from landingai.predict import Predictor
 # Enter your API Key and Secret
 endpoint_id = "FILL_YOUR_INFERENCE_ENDPOINT_ID"
 api_key = "FILL_YOUR_API_KEY"
 # Load your image
-image = np.asarray(Image.open("image.png"))
+image = Image.open("image.png")
 # Run inference
 predictor = Predictor(endpoint_id, api_key=api_key)
 predictions = predictor.predict(image)
 ```
 
 See a **working example** [here](https://github.com/landing-ai/landingai-python/blob/main/tests/integration/landingai/test_predict_e2e.py).
```

### Comparing `landingai-0.2.4/landingai/common.py` & `landingai-0.2.5/landingai/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,26 +177,7 @@
     """
     flat_mask = []
     bitmap_list = re.split("(Z|N)", bitmap)
     for num, map_letter in zip(*[iter(bitmap_list)] * 2):
         map_number = encoding_map[map_letter]
         flat_mask.extend([int(map_number)] * int(num))
     return flat_mask
-
-
-def in_notebook() -> bool:
-    """Determine if we are running inside a notebook
-
-    Returns
-    -------
-    bool
-    """
-    try:
-        from IPython import get_ipython
-
-        if "IPKernelApp" not in get_ipython().config:  # pragma: no cover
-            return False
-    except ImportError:
-        return False
-    except AttributeError:
-        return False
-    return True
```

### Comparing `landingai-0.2.4/landingai/data_management/client.py` & `landingai-0.2.5/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/data_management/media.py` & `landingai-0.2.5/landingai/data_management/media.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/data_management/metadata.py` & `landingai-0.2.5/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/data_management/utils.py` & `landingai-0.2.5/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/exceptions.py` & `landingai-0.2.5/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.2.5/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/pipeline/frameset.py` & `landingai-0.2.5/landingai/pipeline/frameset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 """
 
 import logging
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Union, cast
 
 import cv2
+import imageio
 import numpy as np
 from PIL import Image
-import imageio
 from pydantic import BaseModel
 
-from landingai.common import Prediction, ClassificationPrediction, in_notebook
+from landingai.common import ClassificationPrediction, Prediction
+from landingai.notebook_utils import is_running_in_notebook
 from landingai.predict import Predictor
-from landingai.visualize import overlay_predictions
 from landingai.storage.data_access import fetch_from_uri
-
+from landingai.visualize import overlay_predictions
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Frame(BaseModel):
     """A Frame stores a main image, its metadata and potentially other derived images. This class will be mostly used internally by the FrameSet clase. A pipeline will `FrameSet` since it is more general and a can also keep new `Frames` extracted from existing ones"""
 
@@ -301,15 +301,15 @@
         """Open an a window and display all the images.
         Parameters
         ----------
         image_src: if empty the source image will be displayed. Otherwise the image will be selected from `other_images`
         """
         # TODO: Should show be a end leaf?
         # Check if we are on a notebook context
-        if in_notebook():
+        if is_running_in_notebook():
             from IPython import display
 
             for frame in self.frames:
                 if clear_nb_cell:
                     display.clear_output(wait=True)
                 if image_src == "":
                     display.display(frame.image)
```

### Comparing `landingai-0.2.4/landingai/pipeline/image_source.py` & `landingai-0.2.5/landingai/pipeline/image_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """A module that provides a set of abstractions and APIs for reading images from different sources."""
 
-from datetime import datetime
 import glob
-from collections.abc import Iterator
-from pathlib import Path
-import tempfile
 import shutil
+import tempfile
 import threading
 import time
-from typing import Any, Callable, Iterator as IteratorType, Optional, Tuple
-from typing import List, Union
+from collections.abc import Iterator
+from datetime import datetime
+from pathlib import Path
+from typing import Any, Callable
+from typing import Iterator as IteratorType
+from typing import List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 from pydantic import BaseModel, PrivateAttr
 
 from landingai.pipeline.frameset import Frame, FrameSet
 from landingai.storage.data_access import fetch_from_uri
```

### Comparing `landingai-0.2.4/landingai/pipeline/postprocessing.py` & `landingai-0.2.5/landingai/pipeline/postprocessing.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 
-from landingai.postprocess import class_counts
 from landingai.pipeline.frameset import FrameSet
+from landingai.postprocess import class_counts
 
 
 def get_class_counts(
     frs: FrameSet, add_id_to_classname: bool = False
 ) -> Dict[str, int]:
     """This method returns the number of occurrences of each detected class in the FrameSet.
```

### Comparing `landingai-0.2.4/landingai/postprocess.py` & `landingai-0.2.5/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/predict.py` & `landingai-0.2.5/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/st_utils.py` & `landingai-0.2.5/landingai/st_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,25 @@
 from typing import Any, Optional
 
 _DEFAULT_API_KEY_ENV_VAR = "LANDINGAI_API_KEY"
 
 _LOGGER = logging.getLogger(__name__)
 
 
+def is_running_in_streamlit() -> bool:
+    """Return True if the code is running in a streamlit App."""
+    # See: https://discuss.streamlit.io/t/how-to-check-if-code-is-run-inside-streamlit-and-not-e-g-ipython/23439/2
+    try:
+        from streamlit.runtime.scriptrunner import get_script_run_ctx
+
+        return get_script_run_ctx() is not None
+    except ImportError:
+        return False
+
+
 def _import_st() -> Any:
     """Import streamlit and raise an error if it fails."""
     try:
         import streamlit as st
 
         return st
     except ImportError as e:
```

### Comparing `landingai-0.2.4/landingai/storage/data_access.py` & `landingai-0.2.5/landingai/storage/data_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
-import re
 import os
+import re
 import tempfile
 from pathlib import Path
-from typing import Dict, Optional, Any
-from urllib.parse import urlparse, unquote
-import requests
+from typing import Any, Dict, Optional
+from urllib.parse import unquote, urlparse
 
+import requests
 
 _LOGGER = logging.getLogger(__name__)
 
 
 # TODO: support output type stream
 def read_file(url: str) -> Dict[str, Any]:
     """Read bytes from a URL.
```

### Comparing `landingai-0.2.4/landingai/storage/snowflake.py` & `landingai-0.2.5/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/telemetry.py` & `landingai-0.2.5/landingai/telemetry.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 import platform
 import sys
 from functools import lru_cache
 from importlib.metadata import version
 from pathlib import Path
 from typing import Dict
 
+from landingai.notebook_utils import (
+    is_running_in_colab_notebook,
+    is_running_in_jupyter_notebook,
+)
+from landingai.st_utils import is_running_in_streamlit
+
 
 @lru_cache(maxsize=None)
 def get_runtime_environment_info() -> Dict[str, str]:
     """Return a set of runtime environment information in key value pairs."""
     return {
         "lib_type": "pylib",
         "lib_version": version("landingai"),
@@ -26,52 +32,18 @@
 def is_running_in_pytest() -> bool:
     """Return True if the code is running in a pytest session."""
     # See: https://stackoverflow.com/questions/25188119/test-if-code-is-executed-from-within-a-py-test-session
     return "pytest" in sys.modules
 
 
 def _resolve_python_runtime() -> str:
-    if _is_running_in_colab():
+    if is_running_in_colab_notebook():
         runtime = "colab"
-    elif _is_running_in_notebook():
+    elif is_running_in_jupyter_notebook():
         runtime = "notebook"
-    elif _is_running_in_streamlit():
+    elif is_running_in_streamlit():
         runtime = "streamlit"
     elif is_running_in_pytest():
         runtime = "pytest"
     else:
         runtime = Path(os.environ.get("_", "unknown")).name
     return runtime
-
-
-def _is_running_in_colab() -> bool:
-    """Return True if the code is running in a Google Colab notebook."""
-    try:
-        return get_ipython().__class__.__module__ == "google.colab._shell"  # type: ignore
-    except NameError:
-        return False  # Probably standard Python interpreter
-
-
-def _is_running_in_notebook() -> bool:
-    """Return True if the code is running in a Jupyter notebook."""
-    try:
-        # See: https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
-        shell = get_ipython().__class__.__name__  # type: ignore
-        if shell == "ZMQInteractiveShell":
-            return True  # Jupyter notebook or qtconsole
-        elif shell == "TerminalInteractiveShell":
-            return False  # Terminal running IPython
-        else:
-            return False  # Other type (?)
-    except NameError:
-        return False  # Probably standard Python interpreter
-
-
-def _is_running_in_streamlit() -> bool:
-    """Return True if the code is running in a streamlit App."""
-    # See: https://discuss.streamlit.io/t/how-to-check-if-code-is-run-inside-streamlit-and-not-e-g-ipython/23439/2
-    try:
-        from streamlit.runtime.scriptrunner import get_script_run_ctx
-
-        return get_script_run_ctx() is not None
-    except ImportError:
-        return False
```

### Comparing `landingai-0.2.4/landingai/transform.py` & `landingai-0.2.5/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/utils.py` & `landingai-0.2.5/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.2.4/landingai/visualize.py` & `landingai-0.2.5/landingai/visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """The landingai.visualize module contains functions to visualize the prediction results."""
 
 import logging
 import math
-from pathlib import Path
 import random
+from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union, cast
-import cv2
 
+import cv2
 import numpy as np
-from PIL import Image, ImageDraw, ImageFont, ImageColor
+from PIL import Image, ImageColor, ImageDraw, ImageFont
 
 from landingai.common import (
     ClassificationPrediction,
     ObjectDetectionPrediction,
     OcrPrediction,
     Prediction,
     SegmentationPrediction,
```

### Comparing `landingai-0.2.4/pyproject.toml` & `landingai-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.2.4"
+version = "0.2.5"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.2.4/PKG-INFO` & `landingai-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.2.4
+Version: 0.2.5
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -84,22 +84,21 @@
 
 1. Install the Python library.
 2. Create a `Predictor` class with your Endpoint ID, API Key, and API Secret.
 3. Load your image into a NumPy array (below the image is "image.png")
 4. Call the `predict()` function with an image (using the NumPy array format).
 
 ```python
-import numpy as np
 from PIL import Image
 from landingai.predict import Predictor
 # Enter your API Key and Secret
 endpoint_id = "FILL_YOUR_INFERENCE_ENDPOINT_ID"
 api_key = "FILL_YOUR_API_KEY"
 # Load your image
-image = np.asarray(Image.open("image.png"))
+image = Image.open("image.png")
 # Run inference
 predictor = Predictor(endpoint_id, api_key=api_key)
 predictions = predictor.predict(image)
 ```
 
 See a **working example** [here](https://github.com/landing-ai/landingai-python/blob/main/tests/integration/landingai/test_predict_e2e.py).
```

