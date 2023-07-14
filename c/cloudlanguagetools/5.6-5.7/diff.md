# Comparing `tmp/cloudlanguagetools-5.6.tar.gz` & `tmp/cloudlanguagetools-5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlanguagetools-5.6.tar", last modified: Tue Jun  6 08:37:44 2023, max compression
+gzip compressed data, was "cloudlanguagetools-5.7.tar", last modified: Fri Jul 14 14:29:46 2023, max compression
```

## Comparing `cloudlanguagetools-5.6.tar` & `cloudlanguagetools-5.7.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-06 08:37:44.653119 cloudlanguagetools-5.6/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-06-06 08:37:44.652119 cloudlanguagetools-5.6/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-06 08:37:44.652119 cloudlanguagetools-5.6/cloudlanguagetools/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/amazon.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/argostranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)    23230 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/azure.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/cereproc.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2133 2023-06-06 08:37:03.000000 cloudlanguagetools-5.6/cloudlanguagetools/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/deepl.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/dictionarylookup.py
--rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/easypronunciation.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6830 2023-06-06 08:37:03.000000 cloudlanguagetools-5.6/cloudlanguagetools/elevenlabs.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/encryption.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/epitran.py
--rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/forvo.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/fptai.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8418 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/google.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6123 2023-06-06 08:37:03.000000 cloudlanguagetools-5.6/cloudlanguagetools/keys.py
--rw-r--r--   0 luc       (1000) luc       (1000)    12687 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/languages.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/libretranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/mandarincantonese.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/naver.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1705 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/openai.py
--rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/options.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/pythainlp.py
--rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/service.py
--rw-r--r--   0 luc       (1000) luc       (1000)    17858 2023-06-06 08:37:03.000000 cloudlanguagetools-5.6/cloudlanguagetools/servicemanager.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/spacy.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/test_services.py
--rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/tokenization.py
--rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/translationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/transliterationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1115 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/ttsvoice.py
--rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/vocalware.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/voicen.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/watson.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-5.6/cloudlanguagetools/wenlin.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-06-06 08:37:44.652119 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     1400 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-06-06 08:37:44.000000 cloudlanguagetools-5.6/cloudlanguagetools.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-06-06 08:37:44.653119 cloudlanguagetools-5.6/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)      929 2023-06-06 08:37:41.000000 cloudlanguagetools-5.6/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/cloudlanguagetools/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/amazon.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/argostranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/azure.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/cereproc.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    16859 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/chatapi.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8739 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/chatmodel.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/deepl.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/dictionarylookup.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-5.7/cloudlanguagetools/easypronunciation.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6883 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/elevenlabs.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/encryption.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/epitran.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/forvo.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/fptai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/google.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/keys.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/languages.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/libretranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/mandarincantonese.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/naver.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/openai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/options.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/pythainlp.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/service.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/servicemanager.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/spacy.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/test_services.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/tokenization.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/translationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/transliterationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/ttsvoice.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/vocalware.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/voicen.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/watson.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/wenlin.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     1462 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)      929 2023-07-14 14:29:43.000000 cloudlanguagetools-5.7/setup.py
```

### Comparing `cloudlanguagetools-5.6/LICENSE` & `cloudlanguagetools-5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/PKG-INFO` & `cloudlanguagetools-5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.6
+Version: 5.7
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/amazon.py` & `cloudlanguagetools-5.7/cloudlanguagetools/amazon.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/argostranslate.py` & `cloudlanguagetools-5.7/cloudlanguagetools/argostranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/azure.py` & `cloudlanguagetools-5.7/cloudlanguagetools/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 
 import azure.cognitiveservices.speech
 import azure.cognitiveservices.speech.audio
 
 logger = logging.getLogger(__name__)
 
 AUDIO_LOCALE_OVERRIDE_MAP = {
+    'sr-Latn-RS': 'sr_RS'
+}
+
+GENDER_MAP = {
+    'Female': cloudlanguagetools.constants.Gender.Female,
+    'Male': cloudlanguagetools.constants.Gender.Male,
+    'Neutral': cloudlanguagetools.constants.Gender.Any,
 }
 
 class AzureVoice(cloudlanguagetools.ttsvoice.TtsVoice):
     def __init__(self, voice_data):
         # print(voice_data)
         self.service = cloudlanguagetools.constants.Service.Azure
         self.service_fee = cloudlanguagetools.constants.ServiceFee.paid
@@ -35,15 +42,15 @@
         locale = AUDIO_LOCALE_OVERRIDE_MAP.get(locale, locale)
         language_enum_name = locale.replace('-', '_')
         self.audio_language = cloudlanguagetools.languages.AudioLanguage[language_enum_name]
         self.name = voice_data['Name']
         self.display_name = voice_data['DisplayName']
         self.local_name = voice_data['LocalName']
         self.short_name = voice_data['ShortName']
-        self.gender = cloudlanguagetools.constants.Gender[voice_data['Gender']]
+        self.gender = GENDER_MAP[voice_data['Gender']]
 
         self.locale = locale
         self.voice_type = voice_data['VoiceType']
 
 
     def get_voice_key(self):
         return {
@@ -202,15 +209,15 @@
         audio_format = cloudlanguagetools.options.AudioFormat[audio_format_str]
 
         audio_format_map = {
             cloudlanguagetools.options.AudioFormat.mp3: 'Audio24Khz96KBitRateMonoMp3',
             cloudlanguagetools.options.AudioFormat.ogg_opus: 'Ogg48Khz16BitMonoOpus'
         }
 
-        output_temp_file = tempfile.NamedTemporaryFile()
+        output_temp_file = tempfile.NamedTemporaryFile(prefix=f'cloudlanguage_tools_{self.__class__.__name__}_audio', suffix=f'.{audio_format.name}')
         output_temp_filename = output_temp_file.name
         speech_config = azure.cognitiveservices.speech.SpeechConfig(subscription=self.key, region=self.region)
         speech_config.set_speech_synthesis_output_format(azure.cognitiveservices.speech.SpeechSynthesisOutputFormat[audio_format_map[audio_format]])
         synthesizer = azure.cognitiveservices.speech.SpeechSynthesizer(speech_config=speech_config, audio_config=None)
 
         default_pitch = 0
         default_rate = 1.0
@@ -373,28 +380,35 @@
         request = requests.post(constructed_url, headers=self.get_translator_headers(), json=body, timeout=cloudlanguagetools.constants.RequestTimeout)
         response = request.json()
 
         assert(len(response) == 1)
         return response[0]['text']
 
     # supported languages: https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/language-support#speech-to-text
-    def speech_to_text(self, mp3_filepath, language, audio_format):
+    def speech_to_text(self, mp3_filepath, audio_format, language=None):
         speech_config = azure.cognitiveservices.speech.SpeechConfig(subscription=self.key, region=self.region)
 
         if audio_format == cloudlanguagetools.options.AudioFormat.mp3:
             sound = pydub.AudioSegment.from_mp3(mp3_filepath)
         elif audio_format in [cloudlanguagetools.options.AudioFormat.ogg_opus, cloudlanguagetools.options.AudioFormat.ogg_vorbis]:
             sound = pydub.AudioSegment.from_ogg(mp3_filepath)
         wav_filepath = tempfile.NamedTemporaryFile(suffix='.wav').name
         sound.export(wav_filepath, format="wav")
 
         audio_input = azure.cognitiveservices.speech.audio.AudioConfig(filename=wav_filepath)
 
         # Creates a recognizer with the given settings
-        speech_recognizer = azure.cognitiveservices.speech.SpeechRecognizer(speech_config=speech_config, audio_config=audio_input, language=language)
+        if language != None:
+            # we know which language
+            logger.info(f'configuration speech recognition for language {language}')
+            speech_recognizer = azure.cognitiveservices.speech.SpeechRecognizer(speech_config=speech_config, audio_config=audio_input, language=language)
+        else:
+            # language unknown
+            logger.info(f'configuration speech recognition for any language')
+            speech_recognizer = azure.cognitiveservices.speech.SpeechRecognizer(speech_config=speech_config, audio_config=audio_input)
 
         # Starts speech recognition, and returns after a single utterance is recognized. The end of a
         # single utterance is determined by listening for silence at the end or until a maximum of 15
         # seconds of audio is processed.  The task returns the recognition text as result. 
         # Note: Since recognize_once() returns only a single utterance, it is suitable only for single
         # shot recognition like command or query. 
         # For long-running multi-utterance recognition, use start_continuous_recognition() instead.
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/cereproc.py` & `cloudlanguagetools-5.7/cloudlanguagetools/cereproc.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/deepl.py` & `cloudlanguagetools-5.7/cloudlanguagetools/deepl.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/dictionarylookup.py` & `cloudlanguagetools-5.7/cloudlanguagetools/dictionarylookup.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/easypronunciation.py` & `cloudlanguagetools-5.7/cloudlanguagetools/easypronunciation.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/elevenlabs.py` & `cloudlanguagetools-5.7/cloudlanguagetools/elevenlabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         return audio_language_enum
 
     def get_tts_voice_list(self) -> List[ElevenLabsVoice]:
         result = []
 
         # first, get all models to get list of languages
         url = "https://api.elevenlabs.io/v1/models"
-        response = requests.get(url, headers=self.get_headers())
+        response = requests.get(url, headers=self.get_headers(), timeout=cloudlanguagetools.constants.RequestTimeout)
         response.raise_for_status()
         model_data = response.json()
         # model_data: 
         # [{'can_be_finetuned': True,
         # 'can_do_text_to_speech': True,
         # 'can_do_voice_conversion': False,
         # 'description': 'Use our standard English language model to generate speech '
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/encryption.py` & `cloudlanguagetools-5.7/cloudlanguagetools/encryption.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/epitran.py` & `cloudlanguagetools-5.7/cloudlanguagetools/epitran.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/forvo.py` & `cloudlanguagetools-5.7/cloudlanguagetools/forvo.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/fptai.py` & `cloudlanguagetools-5.7/cloudlanguagetools/fptai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/google.py` & `cloudlanguagetools-5.7/cloudlanguagetools/google.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,34 +7,42 @@
 import google.cloud.translate_v2
 import google.api_core.exceptions
 import cloudlanguagetools.service
 import cloudlanguagetools.constants
 import cloudlanguagetools.options
 import cloudlanguagetools.languages
 
+logger = logging.getLogger(__name__)
+
 def language_code_to_enum(language_code):
     override_map = {
         'cmn-TW': cloudlanguagetools.languages.AudioLanguage.zh_TW,
         'cmn-CN': cloudlanguagetools.languages.AudioLanguage.zh_CN,
         'yue-HK': cloudlanguagetools.languages.AudioLanguage.zh_HK
     }
     if language_code in override_map:
         return override_map[language_code]
     language_enum_name = language_code.replace('-', '_')
     return cloudlanguagetools.languages.AudioLanguage[language_enum_name]
 
+GENDER_MAP = {
+    google.cloud.texttospeech.SsmlVoiceGender.SSML_VOICE_GENDER_UNSPECIFIED: cloudlanguagetools.constants.Gender.Any,
+    google.cloud.texttospeech.SsmlVoiceGender.NEUTRAL: cloudlanguagetools.constants.Gender.Any,
+    google.cloud.texttospeech.SsmlVoiceGender.MALE: cloudlanguagetools.constants.Gender.Male,
+    google.cloud.texttospeech.SsmlVoiceGender.FEMALE: cloudlanguagetools.constants.Gender.Female,
+}
+
 class GoogleVoice(cloudlanguagetools.ttsvoice.TtsVoice):
     def __init__(self, voice_data):
+        logger.debug(f'processing voice {voice_data}')
         self.service = cloudlanguagetools.constants.Service.Google
         self.service_fee = cloudlanguagetools.constants.ServiceFee.paid
         self.name = voice_data.name
         self.google_ssml_gender = google.cloud.texttospeech.SsmlVoiceGender(voice_data.ssml_gender)
-        gender_str = self.google_ssml_gender.name.lower().capitalize()
-        self.gender = cloudlanguagetools.constants.Gender[gender_str]
-        assert len(voice_data.language_codes) == 1
+        self.gender = GENDER_MAP[self.google_ssml_gender]
         self.google_language_code = voice_data.language_codes[0]
         self.audio_language = language_code_to_enum(self.google_language_code)
 
     def get_voice_shortname(self):
         return self.name
 
     def get_voice_key(self):
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/languages.py` & `cloudlanguagetools-5.7/cloudlanguagetools/languages.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+from strenum import StrEnum
 
 class Language(enum.Enum):
     af = ("Afrikaans")
     ak = ("Akan")
     ay = ("Aymara")
     bh = ("Bihari")
     sq = ("Albanian")
@@ -16,18 +17,20 @@
     bo = ("Tibetan")
     be = ("Belarusian")
     bm = ("Bambara")
     bho = ("Bhojpuri")
     bn = ("Bangla")
     bs = ("Bosnian")
     bg = ("Bulgarian")
+    brx = ("Bodo")
     ca = ("Catalan")
     ceb = ("Cebuano")
     ckb = ("Kurdish (Sorani)")
     doi = ("Dogri")
+    dsb = ("Lower Sorbian")
     ny = ("Chichewa")
     co = ("Corsican")
     hr = ("Croatian")
     cs = ("Czech")
     da = ("Danish")
     dv = ("Divehi")
     nl = ("Dutch")
@@ -71,14 +74,15 @@
     km = ("Khmer")
     kri = ("Krio")
     lg = ("Luganda")
     ln = ("Lingala")
     lus = ("Mizo")
     rw = ("Kinyarwanda")
     ko = ("Korean")
+    ks = ("Kashmiri")
     ku = ("Kurdish (Central)")
     ky = ("Kyrgyz")
     lo = ("Lao")
     la = ("Latin")
     lv = ("Latvian")
     lt = ("Lithuanian")
     lb = ("Luxembourgish")
@@ -168,14 +172,67 @@
     zh_tw = ("Chinese (Traditional)")
     zh_lit = ("Chinese (Literary)")
 
 
     def __init__(self, lang_name):
         self.lang_name = lang_name        
 
+# maintain a smaller subset of commonly used languages
+# for chatbot purposes, trimming to the common list of languages saves tokens
+class CommonLanguage(enum.Enum):
+    af = ("Afrikaans")
+    ar = ("Arabic")
+    eu = ("Basque")
+    bg = ("Bulgarian")
+    ca = ("Catalan")
+    hr = ("Croatian")
+    cs = ("Czech")
+    da = ("Danish")
+    nl = ("Dutch")
+    en = ("English")
+    eo = ("Esperanto")
+    et = ("Estonian")
+    tl = ("Filipino")
+    fi = ("Finnish")
+    fr = ("French")
+    de = ("German")
+    el = ("Greek")
+    iw = ("Hebrew")
+    hi = ("Hindi")
+    hu = ("Hungarian")
+    is_ = ("Icelandic")
+    id_ = ("Indonesian")
+    ga = ("Irish")
+    it = ("Italian")
+    ja = ("Japanese")
+    ko = ("Korean")
+    lt = ("Lithuanian")
+    ne = ("Nepali")
+    no = ("Norwegian")
+    pl = ("Polish")
+    ro = ("Romanian")
+    ru = ("Russian")
+    sk = ("Slovak")
+    sl = ("Slovenian")
+    es = ("Spanish")
+    sv = ("Swedish")
+    th = ("Thai")
+    tr = ("Turkish")
+    uk = ("Ukrainian")
+    vi = ("Vietnamese")
+    cy = ("Welsh")
+    he = ("Hebrew")
+    fil = ("Filipino")
+    pt_pt = ("Portuguese")
+    yue = ("Cantonese")
+    zh_cn = ("Chinese")
+
+    def __init__(self, lang_name):
+        self.lang_name = lang_name        
+
 class AudioLanguage(enum.Enum):
     af_ZA = (Language.af, "Afrikaans (South Africa)")
     am_ET = (Language.am, "Amharic (Ethiopia)")
     an_ES = (Language.an, "Aragonese (Spain)")
     # arabic
     ar_AE = (Language.ar, "Arabic (United Arab Emirates)")
     ar_BH = (Language.ar, "Arabic (Bahrain)")
@@ -354,15 +411,16 @@
     Language.en: AudioLanguage.en_US,
     Language.es: AudioLanguage.es_ES,
     Language.fr: AudioLanguage.fr_FR,
     Language.nl: AudioLanguage.nl_NL,
     Language.sw: AudioLanguage.sw_TZ,
     Language.ta: AudioLanguage.ta_IN,
     Language.ur: AudioLanguage.ur_PK,
-    Language.zh_cn: AudioLanguage.zh_CN
+    Language.zh_cn: AudioLanguage.zh_CN,
+    Language.yue: AudioLanguage.zh_HK,
 }
 
 # if only one locale is available, make that the default
 language_map_to_audio_language = {}
 for audio_language in AudioLanguage:
     if audio_language.lang not in language_map_to_audio_language:
         language_map_to_audio_language[audio_language.lang] = []
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/libretranslate.py` & `cloudlanguagetools-5.7/cloudlanguagetools/libretranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/mandarincantonese.py` & `cloudlanguagetools-5.7/cloudlanguagetools/mandarincantonese.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/naver.py` & `cloudlanguagetools-5.7/cloudlanguagetools/naver.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/pythainlp.py` & `cloudlanguagetools-5.7/cloudlanguagetools/pythainlp.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/servicemanager.py` & `cloudlanguagetools-5.7/cloudlanguagetools/servicemanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 import os
 import base64
 import tempfile
 import logging
 import timeit
+import cachetools
+from typing import List
 import cloudlanguagetools.constants
 import cloudlanguagetools.languages
 import cloudlanguagetools.errors
 import cloudlanguagetools.azure
 import cloudlanguagetools.google
 import cloudlanguagetools.watson
 import cloudlanguagetools.naver
 import cloudlanguagetools.amazon
 import cloudlanguagetools.forvo
 import cloudlanguagetools.cereproc
 import cloudlanguagetools.vocalware
 import cloudlanguagetools.fptai
 import cloudlanguagetools.voicen
 import cloudlanguagetools.elevenlabs
+import cloudlanguagetools.deepl
+import cloudlanguagetools.epitran
+import cloudlanguagetools.mandarincantonese
+import cloudlanguagetools.easypronunciation
+import cloudlanguagetools.pythainlp
+import cloudlanguagetools.spacy
+import cloudlanguagetools.wenlin
+import cloudlanguagetools.libretranslate
+import cloudlanguagetools.openai
 import cloudlanguagetools.encryption
+import cloudlanguagetools.translationlanguage
 
-LOAD_NLP_MODELS = os.environ.get('CLOUDLANGUAGETOOLS_CORE_LOAD_NLP', 'yes') == 'yes'
 LOAD_TEST_SERVICES_ONLY = os.environ.get('CLOUDLANGUAGETOOLS_CORE_TEST_SERVICES', 'no') == 'yes'
 
 if LOAD_TEST_SERVICES_ONLY:
     import cloudlanguagetools.test_services
 
-if LOAD_NLP_MODELS:
-    import cloudlanguagetools.deepl
-    import cloudlanguagetools.epitran
-    import cloudlanguagetools.mandarincantonese
-    import cloudlanguagetools.easypronunciation
-    import cloudlanguagetools.pythainlp
-    import cloudlanguagetools.spacy
-    import cloudlanguagetools.wenlin
-    import cloudlanguagetools.libretranslate
-    import cloudlanguagetools.openai
 
 class ServiceManager():
     def  __init__(self):
         self.services = {}
 
         if LOAD_TEST_SERVICES_ONLY:
-            self.services[cloudlanguagetools.constants.Service.TestServiceA.name] = cloudlanguagetools.test_services.TestServiceA()
-            self.services[cloudlanguagetools.constants.Service.TestServiceB.name] = cloudlanguagetools.test_services.TestServiceB()
+            self.services[cloudlanguagetools.constants.Service.TestServiceA] = cloudlanguagetools.test_services.TestServiceA()
+            self.services[cloudlanguagetools.constants.Service.TestServiceB] = cloudlanguagetools.test_services.TestServiceB()
         else:
-            self.services[cloudlanguagetools.constants.Service.Azure.name] = cloudlanguagetools.azure.AzureService()
-            self.services[cloudlanguagetools.constants.Service.Google.name] = cloudlanguagetools.google.GoogleService()
-            self.services[cloudlanguagetools.constants.Service.Watson.name] = cloudlanguagetools.watson.WatsonService()
-            self.services[cloudlanguagetools.constants.Service.Naver.name] = cloudlanguagetools.naver.NaverService()
-            self.services[cloudlanguagetools.constants.Service.Amazon.name] = cloudlanguagetools.amazon.AmazonService()
-            self.services[cloudlanguagetools.constants.Service.Forvo.name] = cloudlanguagetools.forvo.ForvoService()
-            self.services[cloudlanguagetools.constants.Service.CereProc.name] = cloudlanguagetools.cereproc.CereProcService()
-            self.services[cloudlanguagetools.constants.Service.VocalWare.name] = cloudlanguagetools.vocalware.VocalWareService()
-            self.services[cloudlanguagetools.constants.Service.FptAi.name] = cloudlanguagetools.fptai.FptAiService()
-            self.services[cloudlanguagetools.constants.Service.Voicen.name] = cloudlanguagetools.voicen.VoicenService()
-            self.services[cloudlanguagetools.constants.Service.ElevenLabs.name] = cloudlanguagetools.elevenlabs.ElevenLabsService()
-
-            if LOAD_NLP_MODELS:
-                self.services[cloudlanguagetools.constants.Service.EasyPronunciation.name] = cloudlanguagetools.easypronunciation.EasyPronunciationService()
-                self.services[cloudlanguagetools.constants.Service.Epitran.name] = cloudlanguagetools.epitran.EpitranService()
-                self.services[cloudlanguagetools.constants.Service.DeepL.name] = cloudlanguagetools.deepl.DeepLService()
-                self.services[cloudlanguagetools.constants.Service.PyThaiNLP.name] = cloudlanguagetools.pythainlp.PyThaiNLPService()
-                self.services[cloudlanguagetools.constants.Service.Spacy.name] = cloudlanguagetools.spacy.SpacyService()
-                self.services[cloudlanguagetools.constants.Service.MandarinCantonese.name] = cloudlanguagetools.mandarincantonese.MandarinCantoneseService()            
-                self.services[cloudlanguagetools.constants.Service.Wenlin.name] = cloudlanguagetools.wenlin.WenlinService()
-                self.services[cloudlanguagetools.constants.Service.LibreTranslate.name] = cloudlanguagetools.libretranslate.LibreTranslateService()
-                self.services[cloudlanguagetools.constants.Service.OpenAI.name] = cloudlanguagetools.openai.OpenAIService()
+            self.services[cloudlanguagetools.constants.Service.Azure] = cloudlanguagetools.azure.AzureService()
+            self.services[cloudlanguagetools.constants.Service.Google] = cloudlanguagetools.google.GoogleService()
+            self.services[cloudlanguagetools.constants.Service.Watson] = cloudlanguagetools.watson.WatsonService()
+            self.services[cloudlanguagetools.constants.Service.Naver] = cloudlanguagetools.naver.NaverService()
+            self.services[cloudlanguagetools.constants.Service.Amazon] = cloudlanguagetools.amazon.AmazonService()
+            self.services[cloudlanguagetools.constants.Service.Forvo] = cloudlanguagetools.forvo.ForvoService()
+            self.services[cloudlanguagetools.constants.Service.CereProc] = cloudlanguagetools.cereproc.CereProcService()
+            self.services[cloudlanguagetools.constants.Service.VocalWare] = cloudlanguagetools.vocalware.VocalWareService()
+            self.services[cloudlanguagetools.constants.Service.FptAi] = cloudlanguagetools.fptai.FptAiService()
+            self.services[cloudlanguagetools.constants.Service.Voicen] = cloudlanguagetools.voicen.VoicenService()
+            self.services[cloudlanguagetools.constants.Service.ElevenLabs] = cloudlanguagetools.elevenlabs.ElevenLabsService()
+            self.services[cloudlanguagetools.constants.Service.EasyPronunciation] = cloudlanguagetools.easypronunciation.EasyPronunciationService()
+            self.services[cloudlanguagetools.constants.Service.Epitran] = cloudlanguagetools.epitran.EpitranService()
+            self.services[cloudlanguagetools.constants.Service.DeepL] = cloudlanguagetools.deepl.DeepLService()
+            self.services[cloudlanguagetools.constants.Service.PyThaiNLP] = cloudlanguagetools.pythainlp.PyThaiNLPService()
+            self.services[cloudlanguagetools.constants.Service.Spacy] = cloudlanguagetools.spacy.SpacyService()
+            self.services[cloudlanguagetools.constants.Service.MandarinCantonese] = cloudlanguagetools.mandarincantonese.MandarinCantoneseService()            
+            self.services[cloudlanguagetools.constants.Service.Wenlin] = cloudlanguagetools.wenlin.WenlinService()
+            self.services[cloudlanguagetools.constants.Service.LibreTranslate] = cloudlanguagetools.libretranslate.LibreTranslateService()
+            self.services[cloudlanguagetools.constants.Service.OpenAI] = cloudlanguagetools.openai.OpenAIService()
 
     def configure_default(self):
         # use the stored keys to configure services
         self.configure_services(cloudlanguagetools.encryption.decrypt())
 
     def configure_services(self, config):
         for service_name, value in config.items():
-            if service_name in self.services:
-                self.services[service_name].configure(value)
+            service_enum = cloudlanguagetools.constants.Service[service_name]
+            if service_enum in self.services:
+                self.services[service_enum].configure(value)
 
     def get_language_data_json(self):
         # retrieve all language data (tts, translation, transliteration, etc)
         logging.info('retrieving language data')
         
         logging.info('retrieving language list')
         language_list = self.get_language_list()
@@ -138,86 +138,94 @@
 
     def get_language_list(self):
         result_dict = {}
         for language in cloudlanguagetools.languages.Language:
             result_dict[language.name] = language.lang_name
         return result_dict
 
+    @cachetools.cached(cache=cachetools.TTLCache(maxsize=1024, ttl=cloudlanguagetools.constants.TTLCacheTimeout))
     def get_tts_voice_list(self):
         result = []
         for key, service in self.services.items():
             logging.info(f'retrieving voice list from {key}')
             result.extend(service.get_tts_voice_list())
         return result
 
     def get_tts_voice_list_json(self):
         tts_voice_list = self.get_tts_voice_list()
         return [voice.json_obj() for voice in tts_voice_list]
 
-    def get_translation_language_list(self):
+    @cachetools.cached(cache=cachetools.TTLCache(maxsize=1024, ttl=cloudlanguagetools.constants.TTLCacheTimeout))
+    def get_translation_language_list(self) -> List[cloudlanguagetools.translationlanguage.TranslationLanguage]:
         result = []
         for key, service in self.services.items():
             result.extend(service.get_translation_language_list())
         return result        
 
     def get_translation_language_list_json(self):
         """return list of languages supported for translation, using plain objects/strings"""
         language_list = self.get_translation_language_list()
         return [language.json_obj() for language in language_list]
 
+    @cachetools.cached(cache=cachetools.TTLCache(maxsize=1024, ttl=cloudlanguagetools.constants.TTLCacheTimeout))
     def get_transliteration_language_list(self):
         result = []
         for key, service in self.services.items():
             result.extend(service.get_transliteration_language_list())
         return result
 
     def get_transliteration_language_list_json(self):
         """return list of languages supported for transliteration, using plain objects/strings"""
         language_list = self.get_transliteration_language_list()
         return [language.json_obj() for language in language_list]
 
+    @cachetools.cached(cache=cachetools.TTLCache(maxsize=1024, ttl=cloudlanguagetools.constants.TTLCacheTimeout))
     def get_tokenization_options(self):
         result = []
         for key, service in self.services.items():
             result.extend(service.get_tokenization_options())
         return result
 
     def get_tokenization_options_json(self):
         """return list of languages supported for tokenization, using plain objects/strings"""
         tokenization_list = self.get_tokenization_options()
         return [tokenization_option.json_obj() for tokenization_option in tokenization_list]
 
     # dictionary lookups
 
+    @cachetools.cached(cache=cachetools.TTLCache(maxsize=1024, ttl=cloudlanguagetools.constants.TTLCacheTimeout))
     def get_dictionary_lookup_options(self):
         result = []
         for key, service in self.services.items():
             result.extend(service.get_dictionary_lookup_list())
         return result
 
     def get_dictionary_lookup_options_json(self):
         dictionary_lookup_list = self.get_dictionary_lookup_options()
         return [dict_lookup_option.json_obj() for dict_lookup_option in dictionary_lookup_list]
 
-    def get_tts_audio(self, text, service, voice_id, options):
-        service = self.services[service]
+    def get_tts_audio(self, text, service_name, voice_id, options):
+        service_enum = cloudlanguagetools.constants.Service[service_name]
+        service = self.services[service_enum]
         return service.get_tts_audio(text, voice_id, options)
 
-    def get_translation(self, text, service, from_language_key, to_language_key):
+    def get_translation(self, text, service_name: str, from_language_key, to_language_key):
         """return text"""
-        service = self.services[service]
+        service_enum = cloudlanguagetools.constants.Service[service_name]
+        service = self.services[service_enum]
         return service.get_translation(text, from_language_key, to_language_key)
 
     def get_all_translations(self, text, from_language, to_language):
         global_starttime = timeit.default_timer()
 
         translation_language_list = self.get_translation_language_list()
 
         result = {}
-        for service_name, service in self.services.items():
+        for service_enum, service in self.services.items():
+            service_name = service_enum.name
             # locate from language key
             from_language_entries = [x for x in translation_language_list if x.service.name == service_name and x.get_language_code() == from_language]
             if len(from_language_entries) == 1:
                 starttime = timeit.default_timer()
                 # this service provides the "from" language in translation list
                 from_language_id = from_language_entries[0].get_language_id()
                 # locate to language key
@@ -233,24 +241,27 @@
                         logging.exception(f'could not retrieve translation for service {service_name}, text: {text}')
                     time_diff = timeit.default_timer() - starttime
                     logging.info(f'get_all_translation processing time for {service_name}: {time_diff:.1f}')
         global_time_diff = timeit.default_timer() - global_starttime
         logging.info(f'get_all_translation total processing time: {global_time_diff:.1f}')
         return result
 
-    def get_transliteration(self, text, service, transliteration_key):
-        service = self.services[service]
+    def get_transliteration(self, text, service_name: str, transliteration_key):
+        service_enum = cloudlanguagetools.constants.Service[service_name]
+        service = self.services[service_enum]
         return service.get_transliteration(text, transliteration_key)
 
-    def get_tokenization(self, text, service, tokenization_key):
-        service = self.services[service]
+    def get_tokenization(self, text, service_name: str, tokenization_key):
+        service_enum = cloudlanguagetools.constants.Service[service_name]
+        service = self.services[service_enum]
         return service.get_tokenization(text, tokenization_key)
 
-    def get_dictionary_lookup(self, text, service, lookup_key):
-        service = self.services[service]
+    def get_dictionary_lookup(self, text, service_name, lookup_key):
+        service_enum = cloudlanguagetools.constants.Service[service_name]
+        service = self.services[service_enum]
         return service.get_dictionary_lookup(text, lookup_key)
 
     def get_breakdown(self, text, tokenization_option, translation_option, transliteration_option):
         
         # first, tokenize
         tokenization_service = tokenization_option['service']
         tokenization_key = tokenization_option['tokenization_key']
@@ -299,31 +310,31 @@
 
     def get_jyutping_supported_languages(self):
         return [
             cloudlanguagetools.languages.Language.yue
         ]        
 
     def get_pinyin(self, text, tone_numbers, spaces, corrections=[]):
-        return self.services[cloudlanguagetools.constants.Service.MandarinCantonese.name].get_pinyin(text, tone_numbers, spaces, corrections)
+        return self.services[cloudlanguagetools.constants.Service.MandarinCantonese].get_pinyin(text, tone_numbers, spaces, corrections)
 
     def get_jyutping(self, text, tone_numbers, spaces, corrections=[]):
-        return self.services[cloudlanguagetools.constants.Service.MandarinCantonese.name].get_jyutping(text, tone_numbers, spaces, corrections)
+        return self.services[cloudlanguagetools.constants.Service.MandarinCantonese].get_jyutping(text, tone_numbers, spaces, corrections)
 
     # LLM APIs
     # ========
 
     def openai_single_prompt(self, text, max_tokens=None):
-        return self.services[cloudlanguagetools.constants.Service.OpenAI.name].single_prompt(text, max_tokens)
+        return self.services[cloudlanguagetools.constants.Service.OpenAI].single_prompt(text, max_tokens)
 
     def openai_full_query(self, messages, max_tokens=None):
-        return self.services[cloudlanguagetools.constants.Service.OpenAI.name].full_query(messages, max_tokens)
+        return self.services[cloudlanguagetools.constants.Service.OpenAI].full_query(messages, max_tokens)
 
     def detect_language(self, text_list):
         """returns an enum from languages.Language"""
-        service = self.services[cloudlanguagetools.constants.Service.Azure.name]
+        service = self.services[cloudlanguagetools.constants.Service.Azure]
         result = service.detect_language(text_list)
         return result
 
     def service_cost(self, text, service_name, request_type: cloudlanguagetools.constants.RequestType):
         """return the cost of using a service, in characters"""
         service = cloudlanguagetools.constants.Service[service_name]
         character_length = len(text)
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/spacy.py` & `cloudlanguagetools-5.7/cloudlanguagetools/spacy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -64,12 +64,12 @@
             cloudlanguagetools.languages.Language.zh_cn,
             cloudlanguagetools.languages.Language.zh_tw,
             cloudlanguagetools.languages.Language.yue
         ]
         for language in chinese_language_list:
             # chinese variants
             result.extend([
-                SpacyTokenization(language, 'zh_char', 'Characters'),
                 SpacyTokenization(language, 'zh_jieba', 'Jieba (words)'),
+                SpacyTokenization(language, 'zh_char', 'Characters'),
                 SpacyTokenization(language, 'zh_pkuseg', 'PKUSeg (words)')
             ])
         return result
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/test_services.py` & `cloudlanguagetools-5.7/cloudlanguagetools/test_services.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/tokenization.py` & `cloudlanguagetools-5.7/cloudlanguagetools/tokenization.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/translationlanguage.py` & `cloudlanguagetools-5.7/cloudlanguagetools/translationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/transliterationlanguage.py` & `cloudlanguagetools-5.7/cloudlanguagetools/transliterationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/ttsvoice.py` & `cloudlanguagetools-5.7/cloudlanguagetools/ttsvoice.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 
 class TtsVoice():
     def __init__(self):
         pass
 
     def get_gender(self):
         return self.gender
@@ -28,7 +29,9 @@
             'voice_key': self.get_voice_key(),
             'voice_description': self.get_voice_description(),
             'voice_name': self.get_voice_shortname(),
             'options': self.get_options(),
             'service_fee': self.service_fee.name
         }
    
+    def __repr__(self):
+        return json.dumps(self.json_obj(), indent=4, sort_keys=True, ensure_ascii=False)
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/vocalware.py` & `cloudlanguagetools-5.7/cloudlanguagetools/vocalware.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/voicen.py` & `cloudlanguagetools-5.7/cloudlanguagetools/voicen.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/watson.py` & `cloudlanguagetools-5.7/cloudlanguagetools/watson.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools/wenlin.py` & `cloudlanguagetools-5.7/cloudlanguagetools/wenlin.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools.egg-info/PKG-INFO` & `cloudlanguagetools-5.7/cloudlanguagetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.6
+Version: 5.7
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.6/cloudlanguagetools.egg-info/SOURCES.txt` & `cloudlanguagetools-5.7/cloudlanguagetools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 README.rst
 setup.py
 cloudlanguagetools/__init__.py
 cloudlanguagetools/amazon.py
 cloudlanguagetools/argostranslate.py
 cloudlanguagetools/azure.py
 cloudlanguagetools/cereproc.py
+cloudlanguagetools/chatapi.py
+cloudlanguagetools/chatmodel.py
 cloudlanguagetools/constants.py
 cloudlanguagetools/deepl.py
 cloudlanguagetools/dictionarylookup.py
 cloudlanguagetools/easypronunciation.py
 cloudlanguagetools/elevenlabs.py
 cloudlanguagetools/encryption.py
 cloudlanguagetools/epitran.py
```

### Comparing `cloudlanguagetools-5.6/setup.py` & `cloudlanguagetools-5.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from setuptools.command.install import install
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='cloudlanguagetools',
-      version='5.6',
+      version='5.7',
       description='Interface with various cloud APIs for language processing such as translation, text to speech',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Topic :: Text Processing :: Linguistic',
       ],      
       license='GPL',
       packages=['cloudlanguagetools'],
       install_requires=[
           'clt_wenlin>=1.0',
-          'clt_requirements>=0.8',
-          'pinyin_jyutping>=0.8',
+          'clt_requirements>=0.9',
+          'pinyin_jyutping>=0.9',
       ],
       )
```

