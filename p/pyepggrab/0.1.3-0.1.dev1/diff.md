# Comparing `tmp/pyepggrab-0.1.3.tar.gz` & `tmp/pyepggrab-0.1.dev1.tar.gz`

## Comparing `pyepggrab-0.1.3.tar` & `pyepggrab-0.1.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/__init__.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/args.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/ask.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/configbase.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/configmanager.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/log.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/pyepggrab.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/utils.py
--rw-r--r--   0        0        0    21727 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/xmltv.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/xmlwriter.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/grabbers/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/__init__.py
--rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/catmap.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/config.py
--rwxr-xr-x   0        0        0    16507 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/hu_porthu.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/request_proc.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/utils.py
--rw-r--r--   0        0        0    18850 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/xml_utils.py
--rw-r--r--   0        0        0    27085 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyepggrab/resources/xmltv.dtd
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/README.md
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 pyepggrab-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/args.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/ask.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/configbase.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/configmanager.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/log.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/pyepggrab.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/utils.py
+-rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/xmltv.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/xmlwriter.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/__init__.py
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/catmap.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/config.py
+-rwxr-xr-x   0        0        0    15937 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/hu_porthu.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/request_proc.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/utils.py
+-rw-r--r--   0        0        0    17379 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/xml_utils.py
+-rw-r--r--   0        0        0    27085 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/resources/xmltv.dtd
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/LICENSE.txt
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/README.md
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/PKG-INFO
```

### Comparing `pyepggrab-0.1.3/pyepggrab/ask.py` & `pyepggrab-0.1.dev1/pyepggrab/ask.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/pyepggrab/configbase.py` & `pyepggrab-0.1.dev1/pyepggrab/configbase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Base classes used in the configuration management.
 
 These also provides the default config functionality
 """
 
+# from __future__ import annotations
+
 from dataclasses import dataclass
 from json import JSONEncoder
 from typing import Any, Dict, Type, TypeVar
 
 try:
     from typing import override  # type: ignore # noqa: F401, RUF100
 except ImportError:
@@ -39,8 +41,9 @@
 
 
 class ConfigEncoder(JSONEncoder):
     """Default config encoder. Saves every member variable of the class."""
 
     @override
     def default(self, o: Any) -> dict:
+        ConfigRootBase.from_dict({})
         return vars(o)
```

### Comparing `pyepggrab-0.1.3/pyepggrab/configmanager.py` & `pyepggrab-0.1.dev1/pyepggrab/configmanager.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import json
 import sys
 from json import JSONDecoder, JSONEncoder
 from pathlib import Path
 from typing import Generic, Optional, Type
 
 from pyepggrab.configbase import ConfigEncoder, ConfigRootBase, T
-from pyepggrab.log import Log
 
 
 class ConfigManager(Generic[T]):
     """Handles reading and writing grabber configurations."""
 
     def __init__(
         self,
@@ -48,48 +47,29 @@
         self._root = root
         self._encoder = encoder
         self._decoder = decoder
 
         if path:
             self._path = Path(path)
         else:
-            self._path = self.get_default_config_path()
+            confname = Path(sys.argv[0]).stem + ".conf"
+            self._path = Path(Path.home(), ".xmltv", confname)
 
     def get_config_path(self) -> Path:
         """Return the path to the config file."""
         return self._path
 
     def is_config_exists(self) -> bool:
         """Return true is the config file exists."""
         return self._path.exists()
 
     def read_config(self) -> T:
         """Read the config file and return the contents as `root` type."""
         with self._path.open("r", encoding="UTF-8") as file:
-            Log.get_pyepggrab_logger().debug("Reading config file %s", self._path)
             conf = json.load(file, cls=self._decoder)
             return self._root.from_dict(conf)
 
     def write_config(self, config: T) -> None:
         """Write the `root` type config to the config file."""
         configstr = json.dumps(config, cls=self._encoder, indent=2, ensure_ascii=False)
         with self._path.open("w", encoding="UTF-8") as file:
-            Log.get_pyepggrab_logger().debug("Writing config file %s", self._path)
             file.write(configstr)
-
-    @staticmethod
-    def get_default_config_directory() -> Path:
-        """Get the default configuration directory."""
-        return Path(Path.home(), ".xmltv")
-
-    @staticmethod
-    def get_default_config_name() -> str:
-        """Get the default configuration file name."""
-        return Path(sys.argv[0]).stem + ".conf"
-
-    @classmethod
-    def get_default_config_path(cls) -> Path:
-        """Get the default configuration path (dir+name)."""
-        return Path(
-            cls.get_default_config_directory(),
-            cls.get_default_config_name(),
-        )
```

### Comparing `pyepggrab-0.1.3/pyepggrab/log.py` & `pyepggrab-0.1.dev1/pyepggrab/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 Loggers created with `create_logger()` are treated as manged loggers.
 The managed loggers are benefit from the delayed logging feature if the loggers
 are not finalized to avoid outputting unwanted log messages.
 """
 
 import logging
 import sys
-from typing import ClassVar, Dict, List, Union
+from typing import Dict, List, Union
 
 from .utils import grabber_name
 
 
 class Log:
     """Logger of pyepggrab."""
 
-    _finalized: ClassVar[bool] = False
-    _delayedlogs: ClassVar[Dict[str, List[logging.LogRecord]]] = {}
-    _managed_loggers: ClassVar[List[logging.Logger]] = []
+    _finalized: bool = False
+    _delayedlogs: Dict[str, List[logging.LogRecord]] = {}
+    _managed_loggers: List[logging.Logger] = []
 
     @classmethod
     def disable_loggers(cls) -> None:
         """Disable any logging output."""
         logging.disable(logging.CRITICAL)
 
     @classmethod
```

### Comparing `pyepggrab-0.1.3/pyepggrab/pyepggrab.py` & `pyepggrab-0.1.dev1/pyepggrab/pyepggrab.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 Writing grabber that not using these are possible but not recommended (if you
 still want to do, use this as a reference).
 """
 
 import sys
 from argparse import Namespace
 from json import JSONDecoder, JSONEncoder
-from typing import Callable, ClassVar, List, NoReturn, Optional, Type
+from typing import Callable, List, NoReturn, Optional, Type
 
 from pyepggrab import __about__
 from pyepggrab.configbase import ConfigEncoder, ConfigRootBase, T
 from pyepggrab.log import Log
 
 from .args import ArgParser, ExtraargsType
 from .configmanager import ConfigManager
 
 MainType = Callable[[Namespace, ConfigManager], Optional[int]]
 
 
 class Pyepggrab:
     """Pyepggrab convenience functions and decorators."""
 
-    _grabber_main: ClassVar[Optional[MainType]] = None
-    _grabber_config: ClassVar[Optional[MainType]] = None
-    _grabber_extraargs: ClassVar[Optional[ExtraargsType]] = None
+    _grabber_main: Optional[MainType] = None
+    _grabber_config: Optional[MainType] = None
+    _grabber_extraargs: Optional[ExtraargsType] = None
 
     @classmethod
     def grabber_main(cls, func: MainType) -> MainType:
         """Decorate the grabber main function with this.
 
         Called when grabber starts in normal operation.
```

### Comparing `pyepggrab-0.1.3/pyepggrab/utils.py` & `pyepggrab-0.1.dev1/pyepggrab/utils.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/pyepggrab/xmltv.py` & `pyepggrab-0.1.dev1/pyepggrab/xmltv.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     from typing_extensions import override  # type: ignore # noqa: F401, RUF100
 
 
 GEN_NAME = Path(sys.argv[0]).stem
 GEN_URL = "https://github.com/pyepggrab/pyepggrab"
 
 
-def to_xmltv_date(datetime: datetime.datetime) -> str:
-    """`datetime` to XMLTV date format."""
-    return datetime.strftime("%Y%m%d%H%M%S %z")
+def to_xmltv_date(date: datetime.date) -> str:
+    """`date` to XMLTV date format."""
+    return date.strftime("%Y%m%d%H%M%S %z")
 
 
 @dataclass(eq=True)
 class _XmltvBase:
     """Base class for all XML objects."""
 
     def to_xml(self, parent: Optional[etree._Element] = None) -> etree._Element:
```

### Comparing `pyepggrab-0.1.3/pyepggrab/xmlwriter.py` & `pyepggrab-0.1.dev1/pyepggrab/xmlwriter.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/catmap.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/catmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,68 +177,63 @@
     "családi kalandfilm": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "családi vígjáték": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "dokumentumfilm": Cat.EDUCATION_SCIENCE_FACTUAL,
     "dokumentumfilm összeállítás": Cat.EDUCATION_SCIENCE_FACTUAL,
     "dokumentumfilm sorozat": Cat.EDUCATION_SCIENCE_FACTUAL,
     "dokureality-sorozat": Cat.SHOW_GAMESHOW,
     "dráma": Cat.MOVIE_DRAMA,
-    "dráma minisorozat": Cat.MOVIE_DRAMA,
     "drámasorozat": Cat.MOVIE_DRAMA,
+    "dráma minisorozat": Cat.MOVIE_DRAMA,
     "életmódmagazin": Cat.LEISURE_HOBBIES,
     "életrajzi dráma": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
     "életrajzi film": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
     "életrajzi minisorozat": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
     "extrém vetélkedő": Cat.GAMESHOW_QUIZ_CONTEST,
     "fantasy": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "fantasy sorozat": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "fantasztikus akciófilm": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "fantasztikus film": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "fantasztikus kalandfilm": Cat.ADVENTURE_WESTERN_WAR,
     "fantasztikus thriller": Cat.DETECTIVE_THRILLER,
     "fekete komédia": Cat.COMEDY,
-    "fikciós dokumentumfilm": Cat.EDUCATION_SCIENCE_FACTUAL,
     "film": Cat.MOVIE_DRAMA,
     "filmdráma": Cat.MOVIE_DRAMA,
     "filmsorozat": Cat.MOVIE_DRAMA,
     "filmszatíra": Cat.MOVIE_DRAMA,
     "főzős műsor": Cat.COOKING,
     "főzőshow": Cat.SHOW_GAMESHOW,
     "gála": Cat.MUSIC_BALLET_DANCE,
     "gasztro-reality": Cat.SHOW_GAMESHOW,
     "gasztronómiai műsor": Cat.COOKING,
-    "gasztroshow": Cat.COOKING,
     "gazdasági műsor": Cat.SOCIAL_POLITICALISSUES_ECONOMICS,
     "gyerekfilm sorozat": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "gyerekműsor": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "gyermekfilm": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "háborús filmdráma": Cat.ADVENTURE_WESTERN_WAR,
     "hírműsor": Cat.NEWS_CURRENTAFFAIRS,
     "horror": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "horror-dráma": Cat.MOVIE_DRAMA,
     "horror-vígjáték": Cat.COMEDY,
     "horrorsorozat": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "ifjúsági film": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "ifjúsági filmsorozat": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "ifjúsági kalandfilm": Cat.CHILDRENS_YOUTH_PROGRAMMES,
-    "ifjúsági kalandfilmsorozat": Cat.CHILDRENS_YOUTH_PROGRAMMES,
-    "ifjúsági vígjáték": Cat.COMEDY,
     "Információs műsor": Cat.DISCUSSION_INTERVIEW_DEBATE,
     "interaktív filmsorozat": Cat.MOVIE_DRAMA,
     "ismeretterjesztő film": Cat.EDUCATION_SCIENCE_FACTUAL,
     "ismeretterjesztő filmsorozat": Cat.EDUCATION_SCIENCE_FACTUAL,
     "ismeretterjesztő magazin": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
     "ismeretterjesztő műsor": Cat.EDUCATION_SCIENCE_FACTUAL,
     "Ismeretterjesztő sorozat": Cat.EDUCATION_SCIENCE_FACTUAL,
     "játékfilm": Cat.MOVIE_DRAMA,
     "kabaréshow": Cat.SHOW_GAMESHOW,
     "kaland minisorozat": Cat.ADVENTURE_WESTERN_WAR,
     "kalandfilm": Cat.ADVENTURE_WESTERN_WAR,
     "kalandfilmsorozat": Cat.ADVENTURE_WESTERN_WAR,
     "katasztrófa film": Cat.SERIOUS_CLASSICAL_RELIGIOUS_HISTORICAL_MOVIE_DRAMA,
-    "kísérleti film": Cat.EXPERIMENTALFILM_VIDEO,
     "kisfilm-összeállítás": Cat.MOVIE_DRAMA,
     "kisjátékfilm": Cat.MOVIE_DRAMA,
     "komédia": Cat.COMEDY,
     "komédia sorozat": Cat.COMEDY,
     "komolyzenei film": Cat.SERIOUSMUSIC_CLASSICALMUSIC,
     "komolyzenei műsor": Cat.SERIOUSMUSIC_CLASSICALMUSIC,
     "koncertfilm": Cat.MUSIC_BALLET_DANCE,
@@ -246,19 +241,17 @@
     "közlekedésbiztonsági sorozat": Cat.NEWS_CURRENTAFFAIRS,
     "krimi": Cat.DETECTIVE_THRILLER,
     "krimi minisorozat": Cat.DETECTIVE_THRILLER,
     "krimi vígjáték": Cat.COMEDY,
     "krimi-dráma": Cat.MOVIE_DRAMA,
     "krimi-vígjáték": Cat.COMEDY,
     "krimisorozat": Cat.DETECTIVE_THRILLER,
-    "kulináris krimi": Cat.DETECTIVE_THRILLER,
     "kulturális magazin": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
     "kvíz-show": Cat.GAMESHOW_QUIZ_CONTEST,
     "magazinműsor": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
-    "melodráma": Cat.SOAP_MELODRAMA_FOLKLORIC,
     "mesefilm": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "mesejáték": Cat.CHILDRENS_YOUTH_PROGRAMMES,
     "miniportré-sorozat": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
     "minisorozat": Cat.MOVIE_DRAMA,
     "misztikus film": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "misztikus sorozat": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "misztikus thriller": Cat.DETECTIVE_THRILLER,
@@ -278,22 +271,21 @@
     "reality műsor": Cat.GAMESHOW_QUIZ_CONTEST,
     "reality show": Cat.GAMESHOW_QUIZ_CONTEST,
     "reality vígjátéksorozat": Cat.GAMESHOW_QUIZ_CONTEST,
     "reality-sorozat": Cat.GAMESHOW_QUIZ_CONTEST,
     "reklámfilm": Cat.ADVERTISEMENT_SHOPPING,
     "riportfilm": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
     "riportműsor": Cat.MAGAZINES_REPORTS_DOCUMENTARY,
-    "road movie": Cat.MOVIE_DRAMA,
     "romantikus dráma": Cat.ROMANCE,
     "romantikus film": Cat.ROMANCE,
     "romantikus kalandfilm": Cat.ADVENTURE_WESTERN_WAR,
     "romantikus komédia": Cat.COMEDY,
     "romantikus sorozat": Cat.ROMANCE,
     "romantikus thriller": Cat.DETECTIVE_THRILLER,
-    "romantikus vígjáték": Cat.COMEDY,
+    "romantikus vígjáték ": Cat.COMEDY,
     "rövidfilm": Cat.MOVIE_DRAMA,
     "rövidfilm összeállítás": Cat.MOVIE_DRAMA,
     "rövidfilmsorozat": Cat.MOVIE_DRAMA,
     "sci-fi": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "sci-fi akciófilm": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "sci-fi dráma": Cat.SCIENCEFICTION_FANTASY_HORROR,
     "sci-fi kalandfilm": Cat.ADVENTURE_WESTERN_WAR,
@@ -301,40 +293,37 @@
     "sci-fi vígjáték": Cat.COMEDY,
     "show műsor": Cat.SHOW_GAMESHOW,
     "show-műsor": Cat.SHOW_GAMESHOW,
     "sportfilm": Cat.SPORTS,
     "sportműsor": Cat.SPORTS,
     "stand-up comedy": Cat.COMEDY,
     "szabadidős műsor": Cat.LEISURE_HOBBIES,
-    "szatíra": Cat.MOVIE_DRAMA,
     "színházi magazin": Cat.ARTS_CULTURE_MAGAZINES,
     "szórakoztató műsor": Cat.COMEDY,
     "szórakoztató sorozat": Cat.COMEDY,
     "szórakoztató vetélkedő": Cat.GAMESHOW_QUIZ_CONTEST,
     "talk show": Cat.TALKSHOW,
     "telenovella": Cat.MOVIE_DRAMA,
     "televíziós vásárlási műsorablak": Cat.ADVERTISEMENT_SHOPPING,
     "természetfilm": Cat.NATURE_ANIMALS_ENVIRONMENT,
     "természetfilm sorozat": Cat.NATURE_ANIMALS_ENVIRONMENT,
     "tévéfilm": Cat.MOVIE_DRAMA,
     "tévéfilmsorozat": Cat.MOVIE_DRAMA,
     "tévéjáték": Cat.MOVIE_DRAMA,
     "thriller": Cat.DETECTIVE_THRILLER,
-    "thriller minisorozat": Cat.DETECTIVE_THRILLER,
     "thrillersorozat": Cat.DETECTIVE_THRILLER,
     "történelmi dokumentumfilm": Cat.EDUCATION_SCIENCE_FACTUAL,
     "történelmi dokumentumfilm-sorozat": Cat.EDUCATION_SCIENCE_FACTUAL,
     "történelmi dráma": Cat.SERIOUS_CLASSICAL_RELIGIOUS_HISTORICAL_MOVIE_DRAMA,
     "történelmi film": Cat.SERIOUS_CLASSICAL_RELIGIOUS_HISTORICAL_MOVIE_DRAMA,
     "történelmi filmsorozat": Cat.SERIOUS_CLASSICAL_RELIGIOUS_HISTORICAL_MOVIE_DRAMA,
     "történelmi kalandfilm": Cat.ADVENTURE_WESTERN_WAR,
     "történelmi sorozat": Cat.SERIOUS_CLASSICAL_RELIGIOUS_HISTORICAL_MOVIE_DRAMA,
     "történelmi vígjáték": Cat.COMEDY,
-    "útifilm": Cat.FOREIGNCOUNTRIES_EXPEDITIONS,
-    "útifilm-sorozat": Cat.FOREIGNCOUNTRIES_EXPEDITIONS,
+    "útifilm-sorozat": Cat.MOVIE_DRAMA,
     "vallási műsor": Cat.RELIGION,
     "valóságshow": Cat.GAMESHOW_QUIZ_CONTEST,
     "vetélkedő": Cat.GAMESHOW_QUIZ_CONTEST,
     "videóklipek": Cat.MOVIE_DRAMA,
     "vígjáték": Cat.COMEDY,
     "vígjátéksorozat": Cat.COMEDY,
     "western": Cat.ADVENTURE_WESTERN_WAR,
```

### Comparing `pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/config.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Classes used in the configuration file."""
 
+# from __future__ import annotations
+
 from dataclasses import asdict, dataclass
-from json import JSONEncoder
-from typing import Any, List, Type
+from typing import List, Type
 
 from pyepggrab.configbase import ConfigBase, ConfigRootBase, T
-from pyepggrab.utils import remove_suffix
 
 try:
     from typing import override  # type: ignore # noqa: F401, RUF100
 except ImportError:
     from typing_extensions import override  # type: ignore # noqa: F401, RUF100
 
 
@@ -20,15 +20,15 @@
     id_: str
     name: str
     enabled: bool
 
     @override
     @classmethod
     def from_dict(cls: Type[T], d: dict) -> "Channel":
-        id_ = d.get("id", "")  # Stored without '_' in config
+        id_ = d.get("id", "")
         name = d.get("name", "")
         enabled = d.get("enabled", False)
         return Channel(id_, name, enabled)
 
 
 @dataclass
 class GrabberConfig(ConfigRootBase):
@@ -38,16 +38,7 @@
 
     @override
     @classmethod
     def from_dict(cls: Type[T], d: dict) -> "GrabberConfig":
         channels = [Channel.from_dict(ch) for ch in d.get("channels", [])]
         conf = ConfigRootBase.from_dict(d)
         return GrabberConfig(**asdict(conf), channels=channels)
-
-
-class GrabberConfigEncoder(JSONEncoder):
-    """Save every member variable of the class, but without the '_' suffixes."""
-
-    @override
-    def default(self, o: Any) -> dict:
-        """Encode keys without '_' suffixes."""
-        return {remove_suffix(k, "_"): v for k, v in vars(o).items()}
```

### Comparing `pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/hu_porthu.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/hu_porthu.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 from typing import Dict, List, NoReturn, Optional, Tuple
 
 import requests
 from fake_useragent import UserAgent  # type: ignore[import]
 
 from pyepggrab.ask import ask_boolean, ask_many_boolean
 from pyepggrab.configmanager import ConfigManager
-from pyepggrab.grabbers.hu_porthu.config import (
-    Channel,
-    GrabberConfig,
-    GrabberConfigEncoder,
-)
+from pyepggrab.grabbers.hu_porthu.config import Channel, GrabberConfig
 from pyepggrab.grabbers.hu_porthu.request_proc import ProcessCtx
 from pyepggrab.grabbers.hu_porthu.utils import (
     INIT_URL,
     PROGLIST_URL,
     portid_to_xmlid,
     xmlid_to_portid,
 )
@@ -181,36 +177,36 @@
             # recv is xmlid style
             portrecv = xmlid_to_portid(recv)
             if portrecv not in expected_ids:
                 log.debug("Extra channel: %s", recv)
 
 
 def extract_channel_prog(ch: Dict) -> List[Dict]:
-    """Extract the list of programs on a channel from the port.hu api json."""
+    """Extract the list of programs on a chennel from the port.hu api json."""
     ret_json: List[Dict] = []
     prog: dict
     for prog in ch["programs"]:
         ret_json.append(prog)
     return ret_json
 
 
-def add_new_progs(progjsons: List[dict], expectedday: date, ch: dict) -> None:
+def add_new_progs(progjsons: List[dict], exceptedday: date, ch: dict) -> None:
     """Add new programs on `ch` to `progjsons` if they are on the `expectedday`."""
     log = Log.get_grabber_logger()
 
     for progjson in extract_channel_prog(ch):
         if "start_datetime" in progjson:
             start_date = datetime.fromisoformat(progjson["start_datetime"]).date()
-            if start_date == expectedday:
+            if start_date == exceptedday:
                 progjsons.append(progjson)
             else:
                 log.debug(
                     "Program start time is outside of the day. "
                     "Skipped. day: %s, program: %s (%s) - %s",
-                    str(expectedday),
+                    str(exceptedday),
                     str(progjson["title"]),
                     str(progjson["id"]),
                     str(progjson["start_datetime"]),
                 )
         else:
             log.warning("Invalid program. Skipped. program: %s", str(progjson))
 
@@ -417,40 +413,24 @@
 
 @Pyepggrab.grabber_extraargs
 def extraargs(argp: argparse.ArgumentParser) -> None:
     """Add grabber specific arguments to argparser.
 
     Called by pyepggrab
     """
-    argp.add_argument(
-        "--slow",
-        action="store_true",
-        help=(
-            "Use a significantly slower, but more detailed mode to download the guide. "
-            "This adds information like description, actors, etc"
-        ),
-    )
-    argp.add_argument(
-        "--jobs",
-        type=int,
-        default=1,
-        help=(
-            "Number of parallel processes used to download the guide. "
-            "Only used in --slow mode. Setting this value too high may result in "
-            "high resource usage and/or getting banned from port.hu"
-        ),
-    )
+    argp.add_argument("--slow", action="store_true")
+    argp.add_argument("--jobs", type=int, default=1)
 
 
 @Pyepggrab.grabber_main
 def main(
     args: argparse.Namespace,
     confman: ConfigManager[GrabberConfig],
 ) -> Optional[int]:
-    """Start grabber in normal operation (not configuring).
+    """Start graber in normal operation (not configuring).
 
     Called by pyepggrab
     """
     log = Log.get_grabber_logger()
 
     if not confman.is_config_exists():
         log.error(
@@ -509,20 +489,19 @@
 
     guide = retrieve_guide(enabled_ch_portids, days, args.offset, args.slow, args.jobs)
     writexml(guide, args.output)
     return 0
 
 
 def run(**kwargs) -> NoReturn:
-    """Entrypoint to start the grabber by calling `Pyepggrab.main()`."""
+    """Entrypoint to start the grabber by calling `pyepggrab_main()`."""
     Pyepggrab.main(
         version=GRABBER_VERSION,
         description=GRABBER_DESCRIPTION,
         caps=GRABBER_CAPABILITIES,
         config_root=GrabberConfig,
-        config_encoder=GrabberConfigEncoder,
         **kwargs,
     )
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/request_proc.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/request_proc.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/utils.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/utils.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/pyepggrab/grabbers/hu_porthu/xml_utils.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/xml_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,43 +37,30 @@
     XmltvTitle,
     XmltvUrl,
     XmltvValue,
     to_xmltv_date,
 )
 
 RE_JSONDESC = re.compile(
-    r"^(?P<countries>[A-Za-zÁáÉéÍíÓóÖöŐőÚúÜüŰű -]+)?"
-    r"(?:(?: |^)(?P<categories>[A-Za-zÁáÉéÍíÓóÖöŐőÚúÜüŰű, -]+)(?:, |$))?"
+    r"^(?P<countries>[A-Za-zÁáÉéÍíÓóÖöŐőÚúÜüŰű-]+)? ?"
+    r"(?:(?:(?<= )|^)(?P<categories>[A-Za-zÁáÉéÍíÓóÖöŐőÚúÜüŰű, -]+)(?:, |$))?"
     r"(?:(?:(?<=, )|^)(?P<season>[IVXLCDM]+)(?: / ))?"
     r"(?:(?P<episode>[0-9]+)\. rész)?(?:, )?"
     r"(?P<year>[0-9]{4})?$",
 )
 """`countries` captures the first part of the `categories` if no country present
 because it's impossible to distinguish between a county name and a category name
 
-`countries` also captures the first part of the `categories` if the first
-category contains space
-
-example 1:
+example:
 
 angol tévéfilmsorozat, IV / 15. rész -> angol | tévéfilmsorozat | IV | 15
 
 talk show, I / 9. rész -> talk | show | I | 9
 
-example 2:
-
-török romantikus vígjáték , I / 13. rész -> török romantikus | vígjáték  | I | 13
-                         ^ extra space came from port.hu
-
-example 3:
-
-venezuelai-amerikai-Puerto Rico-i filmsorozat, 230. rész ->
-    venezuelai-amerikai-Puerto Rico-i | filmsorozat | 230
-
-if the `countries` can be categorized then it's a category not a country
+if the `countres` can be categorized then it's a category not a country
 """
 
 RE_DESC_TAG = re.compile(r"<div class=\"description\">([\s\S]+?)</div>")
 RE_EXTRACT_TEXT = re.compile(r">([\s\S]+?)<")
 
 RE_HTML_TAG = re.compile(r"<[^>]*>")
 
@@ -114,15 +101,15 @@
     for cat in cats:
         # match category
         if cat in CATDICT:
             encats.append(XmltvCategory(CATDICT[cat].value[0], "en"))
             hucats.append(XmltvCategory(CATDICT[cat].value[1], "hu"))
         # TODO: elif try to match unknown catergory
         else:
-            log.warning("Unknown category: '%s'", cat)
+            log.warning("Unknown category: %s", cat)
 
         # try to match mythtv category if not already
         if mythcat is None:
             for re_cat in RE_MYTHTVCAT:
                 if re_cat[0].search(cat) is not None:
                     mythcat = XmltvCategory(re_cat[1], "en")
                     break
@@ -185,15 +172,16 @@
     if season_num in (None, ""):
         subt = append_if_not_empty(subt, ", ", episode_num, ". rész")
     else:
         subt = append_if_not_empty(subt, "/", episode_num, ". rész")
     subt = append_if_not_empty(subt, ", ", release_date)
     if subt not in (None, ""):
         subt = f"({subt})"
-    return append_if_not_empty(episode_title, " - ", subt)
+    subt = append_if_not_empty(episode_title, " - ", subt)
+    return subt
 
 
 def create_xprogramme(  # noqa: PLR0912, PLR0915
     progjsons: List[Dict],
     response: Optional[requests.Response] = None,
 ) -> List[XmltvProgramme]:
     """Build an XMLTV program from json and by scraping the page of the program."""
@@ -246,20 +234,14 @@
         og_duration = page_opengraph.get("video:duration")
         og_release_date = page_opengraph.get("video:release_date")
 
     if page_jsonld:
         # From json-ld data
         # jld_desc = page_jsonld.get("description")
         jld_genre = page_jsonld.get("genre")
-        if jld_genre:
-            # Sometimes there is a leading space before the comma
-            # or trailing space after the last category.
-            # Causes failed category matches.
-            jld_genre = jld_genre.replace(" , ", ", ").strip()
-
         jld_episode_num = page_jsonld.get("episodeNumber")
         jld_season_num = page_jsonld.get("partOfSeason", {}).get("seasonNumber")
 
         country: Dict
         for country in page_jsonld.get("countryOfOrigin", []):
             name = country.get("name")
             if name:
@@ -351,49 +333,31 @@
                 jld_genre,
                 og_release_date,
                 jld_season_num,
                 jld_episode_num,
             ]
             and j_short_desc is not None
         ):
-            # Sometimes there is a leading space before the comma
-            # or trailing space if the categories are on the end.
-            # Causes incorrect matches
-            j_short_desc = j_short_desc.replace(" , ", ", ").strip()
-
             match = RE_JSONDESC.search(j_short_desc)
             if match and len(match.group(0)) > 0:
                 j_re_countries = match.group("countries")
                 j_re_categories = match.group("categories")
                 j_re_season = match.group("season")
                 j_re_episode = match.group("episode")
                 j_re_year = match.group("year")
 
-                # Country may be the first part of the category, not a country.
-                # First try all parts of the country to see if is a category
-                # if not decrease the number of parts.
-                # Search is stopped after the first successful match
-
-                j_re_country_splits = (
-                    j_re_countries.split(" ") if j_re_countries else ""
-                )
-                cat_str = j_re_categories if j_re_categories else ""
-
-                for i in range(len(j_re_country_splits)):
-                    concat_country = " ".join(j_re_country_splits[i:])
-                    if is_category(
-                        f"{concat_country} {cat_str}".rstrip().split(", ")[0],
-                    ):
-                        if j_re_categories:
-                            j_re_categories = f"{concat_country} {cat_str}"
-                        else:
-                            j_re_categories = concat_country
-                        j_re_countries = " ".join(j_re_country_splits[:i])
-
-                        break
+                # country may be the first part of the category, not a country
+                if j_re_countries and is_category(
+                    f"{j_re_countries} {j_re_categories}".split(", ")[0],
+                ):
+                    if j_re_categories:
+                        j_re_categories = f"{j_re_countries} {j_re_categories}"
+                    else:
+                        j_re_categories = j_re_countries
+                    j_re_countries = None
 
         j_episode_title = progjson.get("episode_title")
         j_porturl = progjson.get("film_url")
         j_prev_shown = progjson.get("is_repeat", False)
         if "restriction" in progjson:
             restr: dict = progjson["restriction"]
             j_age_limit = restr.get("age_limit")
```

### Comparing `pyepggrab-0.1.3/pyepggrab/resources/xmltv.dtd` & `pyepggrab-0.1.dev1/pyepggrab/resources/xmltv.dtd`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/.gitignore` & `pyepggrab-0.1.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/LICENSE.txt` & `pyepggrab-0.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/README.md` & `pyepggrab-0.1.dev1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,65 +9,40 @@
 original XMLTV project, and any software uses the original XMLTV project
 can use these grabbers without any modification.
 
 To avoid name conflicts, pyepggrab grabbers use the prefix `tv_grab_pyepg_`.
 
 ## Installation
 
+Currently, there are no premade packages available, but this expected to change
+in the future.
+
 If the functionality of `tv_find_grabbers` is required the one in the
 original [XMLTV][xmltv] project can be used until we provide an alternative.
 (On the [Roadmap](#roadmap))
 
-### From package
-
-pyepggrab is available on PyPi: https://pypi.org/project/pyepggrab/
-
-Install it with your preferred package manager.
-
-For example, with `pip`
-```
-pip install pyepggrab
-```
-
-or with `pipx`
-```
-pipx install pyepggrab
-```
+To install from source, create a wheel package (this requires `hatch`):
 
-### From source
+> `hatch build`
 
-To install from source, create a wheel package (this requires `hatch`):
+and install it with your preferred package manager (`pipx` in the example):
 
-```
-hatch build
-```
-
-and install it with your preferred package manager.
-
-For example, with `pip`
-```
-pip install dist/pyepggrab-*.whl
-```
-
-or with `pipx`
-```
-pipx install dist/pyepggrab-*.whl
-```
+> `pipx install dist/pyepggrab-*.whl`
 
 ## Available grabbers:
 
 | Country | Guide source      | Grabber                |
 |:-------:|-------------------|------------------------|
 | HU      | [port.hu][porthu] | [hu_porthu][hu_porthu] |
 
 [porthu]: https://port.hu
 [hu_porthu]: pyepggrab/grabbers/hu_porthu
 
 ## Roadmap
 
 In no particular order
 
-- [x] Upload a package to PyPi
-- [x] Write an example grabber to demonstrate the usage of pyepggrab (see [example](example) directory)
+- [ ] Upload a package to PyPi
+- [ ] Write an example grabber to demonstrate the usage of pyepggrab
 - [ ] Write tools to make it standalone (`tv_find_grabbers`, `tv_validate_*`)
 
 [xmltv]: https://github.com/XMLTV/xmltv
```

### Comparing `pyepggrab-0.1.3/pyproject.toml` & `pyepggrab-0.1.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.3/PKG-INFO` & `pyepggrab-0.1.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepggrab
-Version: 0.1.3
+Version: 0.1.dev1
 Summary: Drop in replacement/extension to xmltv grabbers
 Project-URL: Documentation, https://github.com/pyepggrab/pyepggrab#readme
 Project-URL: Issues, https://github.com/pyepggrab/pyepggrab/issues
 Project-URL: Source, https://github.com/pyepggrab/pyepggrab
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: XMLTV,epg,tv
@@ -43,65 +43,40 @@
 original XMLTV project, and any software uses the original XMLTV project
 can use these grabbers without any modification.
 
 To avoid name conflicts, pyepggrab grabbers use the prefix `tv_grab_pyepg_`.
 
 ## Installation
 
+Currently, there are no premade packages available, but this expected to change
+in the future.
+
 If the functionality of `tv_find_grabbers` is required the one in the
 original [XMLTV][xmltv] project can be used until we provide an alternative.
 (On the [Roadmap](#roadmap))
 
-### From package
-
-pyepggrab is available on PyPi: https://pypi.org/project/pyepggrab/
-
-Install it with your preferred package manager.
-
-For example, with `pip`
-```
-pip install pyepggrab
-```
-
-or with `pipx`
-```
-pipx install pyepggrab
-```
+To install from source, create a wheel package (this requires `hatch`):
 
-### From source
+> `hatch build`
 
-To install from source, create a wheel package (this requires `hatch`):
+and install it with your preferred package manager (`pipx` in the example):
 
-```
-hatch build
-```
-
-and install it with your preferred package manager.
-
-For example, with `pip`
-```
-pip install dist/pyepggrab-*.whl
-```
-
-or with `pipx`
-```
-pipx install dist/pyepggrab-*.whl
-```
+> `pipx install dist/pyepggrab-*.whl`
 
 ## Available grabbers:
 
 | Country | Guide source      | Grabber                |
 |:-------:|-------------------|------------------------|
 | HU      | [port.hu][porthu] | [hu_porthu][hu_porthu] |
 
 [porthu]: https://port.hu
 [hu_porthu]: pyepggrab/grabbers/hu_porthu
 
 ## Roadmap
 
 In no particular order
 
-- [x] Upload a package to PyPi
-- [x] Write an example grabber to demonstrate the usage of pyepggrab (see [example](example) directory)
+- [ ] Upload a package to PyPi
+- [ ] Write an example grabber to demonstrate the usage of pyepggrab
 - [ ] Write tools to make it standalone (`tv_find_grabbers`, `tv_validate_*`)
 
 [xmltv]: https://github.com/XMLTV/xmltv
```

