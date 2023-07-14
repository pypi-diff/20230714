# Comparing `tmp/pyDolarVenezuela-1.0.5-py3-none-any.whl.zip` & `tmp/pyDolarVenezuela-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4967 bytes, number of entries: 9
+Zip file size: 4997 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       68 b- defN 23-Jul-14 18:45 pyDolarVenezuela/__init__.py
 -rw-rw-rw-  2.0 fat      216 b- defN 23-Jul-14 18:45 pyDolarVenezuela/request.py
--rw-rw-rw-  2.0 fat     1522 b- defN 23-Jul-14 18:45 pyDolarVenezuela/scraping_bcv.py
--rw-rw-rw-  2.0 fat     1351 b- defN 23-Jul-14 18:45 pyDolarVenezuela/scraping_monitor.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-14 18:49 pyDolarVenezuela-1.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2576 b- defN 23-Jul-14 18:49 pyDolarVenezuela-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 18:49 pyDolarVenezuela-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-14 18:49 pyDolarVenezuela-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      779 b- defN 23-Jul-14 18:49 pyDolarVenezuela-1.0.5.dist-info/RECORD
-9 files, 7715 bytes uncompressed, 3607 bytes compressed:  53.2%
+-rw-rw-rw-  2.0 fat     1597 b- defN 23-Jul-14 18:58 pyDolarVenezuela/scraping_bcv.py
+-rw-rw-rw-  2.0 fat     1351 b- defN 23-Jul-14 18:56 pyDolarVenezuela/scraping_monitor.py
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2579 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      779 b- defN 23-Jul-14 19:00 pyDolarVenezuela-1.0.6.dist-info/RECORD
+9 files, 7793 bytes uncompressed, 3637 bytes compressed:  53.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: pyDolarVenezuela/scraping_bcv.py
 Comment: 
 
 Filename: pyDolarVenezuela/scraping_monitor.py
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.5.dist-info/LICENSE
+Filename: pyDolarVenezuela-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.5.dist-info/METADATA
+Filename: pyDolarVenezuela-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.5.dist-info/WHEEL
+Filename: pyDolarVenezuela-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.5.dist-info/top_level.txt
+Filename: pyDolarVenezuela-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.5.dist-info/RECORD
+Filename: pyDolarVenezuela-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyDolarVenezuela/scraping_bcv.py

```diff
@@ -11,15 +11,15 @@
     
     def _get_content(self, web_site: str) -> bytes:
         return _get_response_content(requests.get(web_site))
     
     def _get_value_by_id(self, tag_id: str, soup: BeautifulSoup):
         return soup.find(id=tag_id).find("strong").text.strip().replace(',', '.')
     
-    def get_rates(self, currency_code: str):
+    def get_rates(self, currency_code: str, prettify: bool = False):
         content = self._get_content(self.page_bcv)
         soup = BeautifulSoup(content, "html.parser")
         section_tipo_de_cambio_oficial = soup.find("div", "view-tipo-de-cambio-oficial-del-bcv")
 
         rates = {
             "EUR": self._get_value_by_id("euro", section_tipo_de_cambio_oficial),
             "CNY": self._get_value_by_id("yuan", section_tipo_de_cambio_oficial),
@@ -27,9 +27,9 @@
             "RUB": self._get_value_by_id("rublo", section_tipo_de_cambio_oficial),
             "USD": self._get_value_by_id("dolar", section_tipo_de_cambio_oficial)
         }
 
         if not currency_code:
             return rates
         if currency_code not in rates:
-            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://gothub.com/fcoagz/pydolarvenezuela")
-        return rates[currency_code]
+            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pydolarvenezuela")
+        return rates[currency_code] if not prettify else f'Bs. {rates[currency_code]}'
```

## pyDolarVenezuela/scraping_monitor.py

```diff
@@ -23,9 +23,9 @@
             'enparalelovzlavip': self._get_results_price(soup)[4],
             'binance': self._get_results_price(soup)[5]
         }
 
         if not monitor_code:
             return results
         if monitor_code not in results:
-            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://gothub.com/fcoagz/pydolarvenezuela")
+            raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pydolarvenezuela")
         return results[monitor_code] if not prettify else f'Bs. {results[monitor_code]}'
```

## Comparing `pyDolarVenezuela-1.0.5.dist-info/LICENSE` & `pyDolarVenezuela-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyDolarVenezuela-1.0.5.dist-info/METADATA` & `pyDolarVenezuela-1.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.0.5
+Version: 1.0.6
 Summary: esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pydolarvenezuela
 Project-URL: Bug Tracker, https://github.com/fcoagz/pydolarvenezuela/issues
@@ -45,23 +45,23 @@
 
 get_value_enparalelovzla = monitor.get_value_monitors(monitor_code='enparalelovzla', prettify=True)
 get_value_binance = monitor.get_value_monitors(monitor_code='binance', prettify=False)
 ```
 
 La clase `pyDolarVenezuela.Bcv` tiene el siguiente metodo:
 
-- `Bcv().get_rate()`: Te muestra los valores de las tasas de cambio del Banco Central de Venezuela. EUR, CNY, TRY, USD.
+- `Bcv().get_rates()`: Te muestra los valores de las tasas de cambio del Banco Central de Venezuela. EUR, CNY, TRY, USD.
 
 Los parametros del metodo ante mencionado son los siguientes:
 
 - `currency_code`: Acepta un código de moneda o fecha como argumento.
 - `prettify`: Acepta un valor booleano si desea que el valor de la moneda salga junto con el simbolo de Bolivares. `Bs. [VALOR]`.
 
 ### Ejemplo
 ``` py
 import pyDolarVenezuela as pdv
 
 bcv = pdv.Bcv()
 
-get_value_usd = bcv.get_rate(currency_code='USD', prettify=True)
-get_value_eur = bcv.get_rate(currency_code='EUR', prettify=False)
+get_value_usd = bcv.get_rates(currency_code='USD', prettify=True)
+get_value_eur = bcv.get_rates(currency_code='EUR', prettify=False)
 ```
```

## Comparing `pyDolarVenezuela-1.0.5.dist-info/RECORD` & `pyDolarVenezuela-1.0.6.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pyDolarVenezuela/__init__.py,sha256=qRuciApRxwvKFedEQdPW5BQYYS_HetzBjuDNDvBgacc,68
 pyDolarVenezuela/request.py,sha256=QSHBpDboWuNz5q4nkqms9AXQLeRnCeslaalx5Q37KlE,216
-pyDolarVenezuela/scraping_bcv.py,sha256=YbJyBhrar6r2V8CiNz_gcieCoTvinWz-8v9_GiMgnCk,1522
-pyDolarVenezuela/scraping_monitor.py,sha256=IHN8Iu8mMIKoasJTzVPT4bbr5wJSfBPY3w_vZ2wnuWo,1351
-pyDolarVenezuela-1.0.5.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
-pyDolarVenezuela-1.0.5.dist-info/METADATA,sha256=4rTDDyNp7cdfo4a15iqTN1ITKOCGgLDOPF7CHh8DGvM,2576
-pyDolarVenezuela-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyDolarVenezuela-1.0.5.dist-info/top_level.txt,sha256=DqT65xfdAAw8yCgxoWQ1UWnzpZ-LGoBUkgMVnY0N8ro,17
-pyDolarVenezuela-1.0.5.dist-info/RECORD,,
+pyDolarVenezuela/scraping_bcv.py,sha256=QX3N46Z-Aj0fCKsHu4zuKwIpFBJZ_z0KleLk0rlP-V4,1597
+pyDolarVenezuela/scraping_monitor.py,sha256=ghfje8qpQnnpbXrY8LdyfkrMW8spL-8XspGGUIJs6BQ,1351
+pyDolarVenezuela-1.0.6.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
+pyDolarVenezuela-1.0.6.dist-info/METADATA,sha256=855KI_KHFoZ-v5O0hO0CU24SxWRfExPe5psFfWEmAR4,2579
+pyDolarVenezuela-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyDolarVenezuela-1.0.6.dist-info/top_level.txt,sha256=DqT65xfdAAw8yCgxoWQ1UWnzpZ-LGoBUkgMVnY0N8ro,17
+pyDolarVenezuela-1.0.6.dist-info/RECORD,,
```

