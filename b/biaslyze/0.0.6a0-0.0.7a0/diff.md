# Comparing `tmp/biaslyze-0.0.6a0.tar.gz` & `tmp/biaslyze-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biaslyze-0.0.6a0.tar", max compression
+gzip compressed data, was "biaslyze-0.0.7a0.tar", max compression
```

## Comparing `biaslyze-0.0.6a0.tar` & `biaslyze-0.0.7a0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.6a0/LICENSE
--rw-r--r--   0        0        0     3457 2023-06-22 11:24:11.649837 biaslyze-0.0.6a0/README.md
--rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.6a0/biaslyze/__init__.py
--rw-r--r--   0        0        0     6931 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/_plotting.py
--rw-r--r--   0        0        0      220 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/bias_detectors/__init__.py
--rw-r--r--   0        0        0    13446 2023-06-22 11:25:40.993149 biaslyze-0.0.6a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
--rw-r--r--   0        0        0     5547 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/bias_detectors/lime_biasdetector.py
--rw-r--r--   0        0        0     5511 2023-06-22 11:25:40.993149 biaslyze-0.0.6a0/biaslyze/concept_class.py
--rw-r--r--   0        0        0     1831 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/concept_detectors.py
--rw-r--r--   0        0        0    64680 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/concepts.py
--rw-r--r--   0        0        0    12924 2023-06-22 11:25:40.993149 biaslyze-0.0.6a0/biaslyze/results/counterfactual_detection_results.py
--rw-r--r--   0        0        0     4990 2023-06-01 14:53:12.469622 biaslyze-0.0.6a0/biaslyze/results/lime_detection_results.py
--rw-r--r--   0        0        0     2546 2023-06-22 11:25:40.997149 biaslyze-0.0.6a0/biaslyze/text_representation.py
--rw-r--r--   0        0        0     1681 2023-06-22 11:25:13.421364 biaslyze-0.0.6a0/pyproject.toml
--rw-r--r--   0        0        0     5102 1970-01-01 00:00:00.000000 biaslyze-0.0.6a0/setup.py
--rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 biaslyze-0.0.6a0/PKG-INFO
+-rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.7a0/LICENSE
+-rw-r--r--   0        0        0     3887 2023-07-14 16:24:22.552701 biaslyze-0.0.7a0/README.md
+-rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.7a0/biaslyze/__init__.py
+-rw-r--r--   0        0        0    12586 2023-07-14 15:08:56.944651 biaslyze-0.0.7a0/biaslyze/_plotly_dashboard.py
+-rw-r--r--   0        0        0     6931 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/_plotting.py
+-rw-r--r--   0        0        0      281 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/augmentors.py
+-rw-r--r--   0        0        0      220 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/bias_detectors/__init__.py
+-rw-r--r--   0        0        0    14155 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
+-rw-r--r--   0        0        0     5547 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/bias_detectors/lime_biasdetector.py
+-rw-r--r--   0        0        0     6546 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/concept_class.py
+-rw-r--r--   0        0        0     1831 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/concept_detectors.py
+-rw-r--r--   0        0        0    62578 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/concepts.py
+-rw-r--r--   0        0        0    13637 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/results/counterfactual_detection_results.py
+-rw-r--r--   0        0        0     4990 2023-06-01 14:53:12.469622 biaslyze-0.0.7a0/biaslyze/results/lime_detection_results.py
+-rw-r--r--   0        0        0     2992 2023-07-14 15:02:55.749820 biaslyze-0.0.7a0/biaslyze/text_representation.py
+-rw-r--r--   0        0        0     1756 2023-07-14 16:24:22.552701 biaslyze-0.0.7a0/pyproject.toml
+-rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 biaslyze-0.0.7a0/setup.py
+-rw-r--r--   0        0        0     5918 1970-01-01 00:00:00.000000 biaslyze-0.0.7a0/PKG-INFO
```

### Comparing `biaslyze-0.0.6a0/LICENSE` & `biaslyze-0.0.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.6a0/README.md` & `biaslyze-0.0.7a0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 
-<p align="center">
-  <h1>biaslyze - The NLP Bias Identification Toolkit</h1>
-</p>
+<div align="center">
+  <img src="resources/biaslyze-logo-no-bg.png" alt="Biaslyze" height="220px">
+  <h1>The NLP Bias Identification Toolkit</h1>
+</div>
 
-<p align="center">
+<div align="center">
     <a href="https://github.com/biaslyze-dev/biaslyze/blob/main/LICENSE">
         <img alt="licence" src="https://img.shields.io/github/license/biaslyze-dev/biaslyze">
     </a>
     <a href="https://pypi.org/project/biaslyze/">
         <img alt="pypi" src="https://img.shields.io/pypi/v/biaslyze">
     </a>
     <a href="https://pypi.org/project/biaslyze/">
         <img alt="pypi" src="https://img.shields.io/pypi/pyversions/biaslyze">
     </a>
-</p>
+</div>
 
 
 Bias is often subtle and difficult to detect in NLP models, as the protected attributes are less obvious and can take many forms in language (e.g. proxies, double meanings, ambiguities etc.). Therefore, technical bias testing is a key step in avoiding algorithmically mediated discrimination. However, it is currently conducted too rarely due to the effort involved, missing resources or lack of awareness for the problem.
 
-Biaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.
+Biaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for developers, researchers and teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.
+
+## Supported Models
+
+All text classification models with probability output are supported. This includes models from scikit-learn, tensorflow, pytorch, huggingface transformers and others. 
+See the tutorials section for examples.
 
 ## Installation
 
 Installation can be done using pypi:
 ```bash
 pip install biaslyze
 ```
@@ -49,31 +55,32 @@
 # see a summary of the detection
 detection_res.report()
 
 # visualize the counterfactual scores
 detection_res.visualize_counterfactual_scores(concept="religion", top_n=10)
 ```
 
+You will get results as Boxplots, among others, indicating the impact of keywords and concepts on the prediction of your model.
 Example output:
 ![](resources/hatespeech_dl_scores_religion.png)
 
 
-You can see a more detailed example in the [tutorial](tutorials/tutorial-toxic-comments/).
+See more detailed examples in the [tutorial](tutorials/tutorial-toxic-comments/).
 
 
 ## Development setup
 
 - First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation
 - Run `make install` to install the dependencies and get the spacy basemodels.
 - Now you can use `biaslyze` in your jupyter notebooks.
 
 
 ### Adding concepts and keywords
 
-You can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/keyword-based-targeted-lime/biaslyze/concepts.py).
+You can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py).
 
 ## Preview/build the documentation with mkdocs
 
 To preview the documentation run `make doc-preview`. This will launch a preview of the documentation on `http://127.0.0.1:8000/`.
 To build the documentation html run `make doc`.
```

#### html2text {}

```diff
@@ -1,40 +1,46 @@
-****** biaslyze - The NLP Bias Identification Toolkit ******
+                                  [Biaslyze]
+               ****** The NLP Bias Identification Toolkit ******
                             [licence] [pypi] [pypi]
 Bias is often subtle and difficult to detect in NLP models, as the protected
 attributes are less obvious and can take many forms in language (e.g. proxies,
 double meanings, ambiguities etc.). Therefore, technical bias testing is a key
 step in avoiding algorithmically mediated discrimination. However, it is
 currently conducted too rarely due to the effort involved, missing resources or
 lack of awareness for the problem. Biaslyze helps to get started with the
 analysis of bias within NLP models and offers a concrete entry point for
-further impact assessments and mitigation measures. Especially for teams with
-limited resources, our toolbox offers a low-effort approach to bias testing in
-NLP use cases. ## Installation Installation can be done using pypi: ```bash pip
-install biaslyze ``` Then you need to download the required spacy models:
-```bash python -m spacy download en_core_web_sm ``` ## Quickstart ```python
-from biaslyze.bias_detectors import CounterfactualBiasDetector bias_detector =
-CounterfactualBiasDetector() # detect bias in the model based on the given
-texts # here, clf is a scikit-learn text classification pipeline trained for a
-binary classification task detection_res = bias_detector.process( texts=texts,
+further impact assessments and mitigation measures. Especially for developers,
+researchers and teams with limited resources, our toolbox offers a low-effort
+approach to bias testing in NLP use cases. ## Supported Models All text
+classification models with probability output are supported. This includes
+models from scikit-learn, tensorflow, pytorch, huggingface transformers and
+others. See the tutorials section for examples. ## Installation Installation
+can be done using pypi: ```bash pip install biaslyze ``` Then you need to
+download the required spacy models: ```bash python -m spacy download
+en_core_web_sm ``` ## Quickstart ```python from biaslyze.bias_detectors import
+CounterfactualBiasDetector bias_detector = CounterfactualBiasDetector() #
+detect bias in the model based on the given texts # here, clf is a scikit-learn
+text classification pipeline trained for a binary classification task
+detection_res = bias_detector.process( texts=texts,
 predict_func=clf.predict_proba ) # see a summary of the detection
 detection_res.report() # visualize the counterfactual scores
 detection_res.visualize_counterfactual_scores(concept="religion", top_n=10) ```
-Example output: ![](resources/hatespeech_dl_scores_religion.png) You can see a
-more detailed example in the [tutorial](tutorials/tutorial-toxic-comments/). ##
-Development setup - First you need to install poetry to manage your python
-environment: https://python-poetry.org/docs/#installation - Run `make install`
-to install the dependencies and get the spacy basemodels. - Now you can use
-`biaslyze` in your jupyter notebooks. ### Adding concepts and keywords You can
-add concepts and new keywords for existing concepts by editing [concepts.py]
-(https://github.com/biaslyze-dev/biaslyze/blob/keyword-based-targeted-lime/
-biaslyze/concepts.py). ## Preview/build the documentation with mkdocs To
-preview the documentation run `make doc-preview`. This will launch a preview of
-the documentation on `http://127.0.0.1:8000/`. To build the documentation html
-run `make doc`. ## Run the automated tests `make test` ## Style guide We are
-using isort and black: `make style` For linting we are running ruff: `make
-lint` ## Contributing Follow the google style guide for python: https://
-google.github.io/styleguide/pyguide.html This project uses black, isort and
-ruff to enforce style. Apply it by running `make style` and `make lint`. ##
-Acknowledgements * Funded from March 2023 until August 2023 by ![logos of the
-"Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund and OKFN-
-Deutschland](resources/pf_funding_logos.svg)
+You will get results as Boxplots, among others, indicating the impact of
+keywords and concepts on the prediction of your model. Example output: ![]
+(resources/hatespeech_dl_scores_religion.png) See more detailed examples in the
+[tutorial](tutorials/tutorial-toxic-comments/). ## Development setup - First
+you need to install poetry to manage your python environment: https://python-
+poetry.org/docs/#installation - Run `make install` to install the dependencies
+and get the spacy basemodels. - Now you can use `biaslyze` in your jupyter
+notebooks. ### Adding concepts and keywords You can add concepts and new
+keywords for existing concepts by editing [concepts.py](https://github.com/
+biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py). ## Preview/build the
+documentation with mkdocs To preview the documentation run `make doc-preview`.
+This will launch a preview of the documentation on `http://127.0.0.1:8000/`. To
+build the documentation html run `make doc`. ## Run the automated tests `make
+test` ## Style guide We are using isort and black: `make style` For linting we
+are running ruff: `make lint` ## Contributing Follow the google style guide for
+python: https://google.github.io/styleguide/pyguide.html This project uses
+black, isort and ruff to enforce style. Apply it by running `make style` and
+`make lint`. ## Acknowledgements * Funded from March 2023 until August 2023 by
+![logos of the "Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund
+and OKFN-Deutschland](resources/pf_funding_logos.svg)
```

### Comparing `biaslyze-0.0.6a0/biaslyze/_plotting.py` & `biaslyze-0.0.7a0/biaslyze/_plotting.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.6a0/biaslyze/bias_detectors/counterfactual_biasdetector.py` & `biaslyze-0.0.7a0/biaslyze/bias_detectors/counterfactual_biasdetector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Detect hints of bias by calculating counterfactual token scores for protected concepts."""
-import random
 from typing import Callable, List, Optional
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 from tqdm import tqdm
 
 from biaslyze.concept_class import Concept, load_concepts
 from biaslyze.concept_detectors import KeywordConceptDetector
 from biaslyze.results.counterfactual_detection_results import (
     CounterfactualConceptResult,
     CounterfactualDetectionResult,
     CounterfactualSample,
 )
+from biaslyze.augmentors import CounterfactualTextAugmentor
 from biaslyze.text_representation import TextRepresentation, process_texts_with_spacy
 
 
 class CounterfactualBiasDetector:
     """Detect hints of bias by calculating counterfactual token scores for protected concepts.
 
     The counterfactual score is defined as the difference between the predicted
@@ -52,23 +52,26 @@
         # visualize the counterfactual sample scores
         detection_res.visualize_counterfactual_score_by_sample_histogram(concepts=["religion", "gender"])
         ```
 
     Attributes:
         use_tokenizer: If keywords should only be searched in tokenized text. Can be useful for short keywords like 'she'.
         concept_detector: an instance of KeywordConceptDetector
+        text_augmentor: an instance of CounterfactualTextAugmentor
     """
 
     def __init__(
         self,
         use_tokenizer: bool = False,
         concept_detector: KeywordConceptDetector = KeywordConceptDetector(),
+        text_augmentor: CounterfactualTextAugmentor = CounterfactualTextAugmentor(), 
     ):
         self.use_tokenizer = use_tokenizer
         self.concept_detector = concept_detector
+        self.text_augmentor = text_augmentor
 
         # overwrite use_tokenizer
         self.concept_detector.use_tokenizer = self.use_tokenizer
 
         # load the concepts
         self.concepts = load_concepts()
 
@@ -121,15 +124,15 @@
         # find bias relevant texts
         detected_texts = self.concept_detector.detect(texts)
 
         # limit the number of counterfactual samples per text if max_counterfactual_samples is given
         if max_counterfactual_samples:
             max_counterfactual_samples_per_text = max_counterfactual_samples // len(
                 detected_texts
-            )
+            ) + 1
 
         results = []
         for concept in self.concepts:
             if concepts_to_consider and concept.name not in concepts_to_consider:
                 continue
             logger.info(f"Processing concept {concept.name}...")
             score_dict = dict()
@@ -137,25 +140,31 @@
             counterfactual_samples = _extract_counterfactual_concept_samples(
                 texts=detected_texts,
                 concept=concept,
                 labels=labels,
                 n_texts=max_counterfactual_samples_per_text,
             )
             if not counterfactual_samples:
-                logger.warning(f"No samples containing {concept} found. Skipping.")
+                logger.warning(f"No samples containing {concept.name} found. Skipping.")
                 continue
 
             # calculate counterfactual scores for each keyword
             for keyword in tqdm(concept.keywords):
                 # get the counterfactual scores
-                counterfactual_scores = _calculate_counterfactual_scores(
-                    bias_keyword=keyword.text,
-                    predict_func=predict_func,
-                    samples=counterfactual_samples,
-                )
+                try:
+                    counterfactual_scores = _calculate_counterfactual_scores(
+                        bias_keyword=keyword.text,
+                        predict_func=predict_func,
+                        samples=counterfactual_samples,
+                    )
+                except ValueError:
+                    logger.warning(
+                        f"Could not calculate counterfactual scores for keyword {keyword.text}. Skipping."
+                    )
+                    continue
                 # add to score dict
                 score_dict[keyword.text] = counterfactual_scores
                 # add scores to samples
                 original_keyword_samples = [
                     sample
                     for sample in counterfactual_samples
                     if (sample.keyword == keyword.text)
@@ -191,53 +200,55 @@
 
 
 def _extract_counterfactual_concept_samples(
     concept: Concept,
     texts: List[str],
     labels: Optional[List[str]] = None,
     n_texts: Optional[int] = None,
+    respect_function: bool = True,
 ) -> List[CounterfactualSample]:
     """Extract counterfactual samples for a given concept from a list of texts.
 
     A counterfactual sample is defined as a text where a keyword of the
     given concept is replaced by another keyword of the same concept.
 
     Args:
         concept: The concept to extract counterfactual samples for.
         texts: The texts to extract counterfactual samples from.
         tokenizer: The tokenizer to use for tokenization.
         labels: Optional. Used to add labels to the counterfactual results.
         n_texts: Optional. The number of counterfactual texts to return. Defaults to None, which returns all possible counterfactual texts.
+        respect_function: If True, only replace keywords with the same function.
 
     Returns:
         A list of CounterfactualSample objects.
     """
     counterfactual_samples = []
     original_texts = []
     text_representations: List[TextRepresentation] = process_texts_with_spacy(texts)
-    for idx, (text, text_representation) in tqdm(
-        enumerate(zip(texts, text_representations)), total=len(texts)
+    for idx, text_representation in tqdm(
+        enumerate(text_representations), total=len(text_representations)
     ):
         present_keywords = concept.get_present_keywords(text_representation)
         if present_keywords:
-            original_texts.append(text)
+            original_texts.append(text_representation.text)
             for orig_keyword in present_keywords:
                 counterfactual_texts = concept.get_counterfactual_texts(
-                    orig_keyword, text_representation, n_texts=n_texts
+                    orig_keyword, text_representation, n_texts=n_texts, respect_function=respect_function
                 )
                 for counterfactual_text, counterfactual_keyword in counterfactual_texts:
                     counterfactual_samples.append(
                         CounterfactualSample(
                             text=counterfactual_text,
                             orig_keyword=orig_keyword.text,
                             keyword=counterfactual_keyword.text,
                             concept=concept.name,
                             tokenized=text_representation,
                             label=labels[idx] if labels else None,
-                            source_text=text,
+                            source_text=text_representation.text,
                         )
                     )
     logger.info(
         f"Extracted {len(counterfactual_samples)} counterfactual sample texts for concept {concept.name} from {len(original_texts)} original texts."
     )
     return counterfactual_samples
```

### Comparing `biaslyze-0.0.6a0/biaslyze/bias_detectors/lime_biasdetector.py` & `biaslyze-0.0.7a0/biaslyze/bias_detectors/lime_biasdetector.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.6a0/biaslyze/concept_class.py` & `biaslyze-0.0.7a0/biaslyze/concept_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,39 +16,63 @@
 
     Attributes:
         text (str): The word that is the keyword.
         function (List[str]): The possible functions of the keyword.
         category (str): The category of the keyword.
     """
 
-    def __init__(self, text: str, function: List[str], category: str):
+    def __init__(self, text: str, functions: List[str], category: str):
         """The constructor for the Keyword class."""
         self.text = text
-        self.function = function
+        self.functions = functions
         self.category = category
 
     def __str__(self) -> str:
         return f"Keyword({self.text}, {self.function}, {self.category})"
 
     def __repr__(self) -> str:
         return f"Keyword({self.text}, {self.function}, {self.category})"
 
-    def can_replace_token(self, token: Token) -> bool:
-        """Returns True if the keyword can replace the given token."""
+    def can_replace_token(self, token: Token, respect_function: bool = False) -> bool:
+        """Returns True if the keyword can replace the given token.
+
+        Args:
+            token (Token): The token to replace.
+            respect_function (bool): Whether to respect the function of the keyword. Defaults to False.
+        """
+        if respect_function:
+            return True
+            # return token.function in self.functions
         return True
 
     def equal_to_token(self, token: Token) -> bool:
         """Returns True if the given token is equal to the keyword."""
         if self.text.lower() == token.text.lower():
             return True
         return False
 
     def get_keyword_in_style_of_token(self, token: Token) -> str:
-        """Returns the keyword text in the style of the given token."""
-        return self.text
+        """Returns the keyword text in the style of the given token.
+
+        Uses the shape of the token to determine the style.
+
+        Args:
+            token (Token): The token to get the style from.
+
+        Returns:
+            str: The keyword text in the style of the given token.
+        """
+        if "X" not in token.shape:
+            return self.text.lower()
+        elif "x" not in token.shape:
+            return self.text.upper()
+        elif token.shape[0] == "X":
+            return self.text.capitalize()
+        else:
+            return self.text
 
 
 class Concept:
     """
     A class used to represent a concept in the biaslyze package.
 
     Attributes:
@@ -64,17 +88,17 @@
     @classmethod
     def from_dict_keyword_list(cls, name: str, keywords: List[dict]):
         """Constructs a Concept object from a list of dictionaries."""
         keyword_list = []
         for keyword in keywords:
             keyword_list.append(
                 Keyword(
-                    keyword["keyword"],
-                    keyword["function"],
-                    keyword.get("category", None),
+                    text=keyword["keyword"],
+                    functions=keyword["function"],
+                    category=keyword.get("category", None),
                 )
             )
         return cls(name, keyword_list)
 
     def get_present_keywords(
         self, text_representation: TextRepresentation
     ) -> List[Keyword]:
@@ -86,48 +110,52 @@
         return present_keywords
 
     def get_counterfactual_texts(
         self,
         keyword: Keyword,
         text_representation: TextRepresentation,
         n_texts: Optional[int] = None,
+        respect_function: bool = True,
     ) -> List[Tuple[str, Keyword]]:
         """Returns a counterfactual texts based on a specific keyword for the given text representation.
 
         Args:
             keyword (Keyword): The keyword in the text to replace.
             text_representation (TextRepresentation): The text representation to replace the keyword in.
             n_texts (Optional[int]): The number of counterfactual texts to return. Defaults to None, which returns all possible counterfactual texts.
+            respect_function (bool): Whether to respect the function of the keyword. Defaults to True.
 
         Returns:
             List[Tuple[str, Keyword]]: A list of tuples containing the counterfactual text and the keyword that was replaced.
         """
         counterfactual_texts = []
         for token in text_representation.tokens:
             # check if the token is equal to the keyword
             if keyword.equal_to_token(token):
                 # shuffle the keywords
                 random.shuffle(self.keywords)
                 # create a counterfactual text for each keyword until n_texts is reached
                 for counterfactual_keyword in self.keywords:
                     # check if the keyword can be replaced by another keyword
-                    if counterfactual_keyword.can_replace_token(token):
+                    if counterfactual_keyword.can_replace_token(
+                        token, respect_function
+                    ):
                         # create the counterfactual text
                         counterfactual_text = (
                             text_representation.text[: token.start]
                             + counterfactual_keyword.get_keyword_in_style_of_token(
                                 token
                             )
                             + text_representation.text[token.end :]
                         )
                         counterfactual_texts.append(
                             (counterfactual_text, counterfactual_keyword)
                         )
                     # check if n_texts is reached and return the counterfactual texts
-                    if len(counterfactual_texts) == n_texts:
+                    if n_texts and (len(counterfactual_texts) >= n_texts):
                         return counterfactual_texts
         return counterfactual_texts
 
 
 def load_concepts() -> List[Concept]:
     """Loads the concepts from the concepts.py file.
```

### Comparing `biaslyze-0.0.6a0/biaslyze/concept_detectors.py` & `biaslyze-0.0.7a0/biaslyze/concept_detectors.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.6a0/biaslyze/results/counterfactual_detection_results.py` & `biaslyze-0.0.7a0/biaslyze/results/counterfactual_detection_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """This module contains classes to store and process the results of counterfactual bias detection runs."""
+import warnings
 from collections import defaultdict
 from typing import List, Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
+from biaslyze._plotly_dashboard import _plot_dashboard
 from biaslyze._plotting import _plot_box_plot, _plot_histogram_dashboard
 
 
 class CounterfactualSample:
     """A sample for counterfactual bias detection.
 
     Attributes:
@@ -113,15 +115,19 @@
             For each concept, the maximum mean and maximum standard deviation of the counterfactual scores is shown.
         """
         for concept_result in self.concept_results:
             print(
                 f"""Concept: {concept_result.concept}\t\tMax-Mean Counterfactual Score: {np.abs(concept_result.scores.mean()).max():.5f}\t\tMax-Std Counterfactual Score: {concept_result.scores.std().max():.5f}"""
             )
 
-    def visualize_counterfactual_scores(
+    def dashboard(self, num_keywords: int = 10):
+        """Start a dash dashboard with interactive box plots."""
+        _plot_dashboard(self, num_keywords=num_keywords)
+
+    def __visualize_counterfactual_scores(
         self, concept: str, top_n: Optional[int] = None
     ):
         """
         Visualize the counterfactual scores for a given concept.
 
         The score is calculated by comparing the prediction of the original sample with the prediction of the counterfactual sample.
         For every keyword shown all concept keywords are replaced with the keyword shown. The difference in the prediction to the original is then calculated.
@@ -134,36 +140,42 @@
 
         Returns:
             The matplotlib plot.
 
         Raises:
             ValueError: If the concept is not found in the results.
         """
+        warnings.warn(
+            "This method is deprecated. Use dashboard() instead.", DeprecationWarning
+        )
         dataf = self._get_result_by_concept(concept=concept)
         ax = _plot_box_plot(dataf, top_n=top_n)
         ax.set_title(
             f"Distribution of counterfactual scores for concept '{concept}'\nsorted by median score"
         )
         ax.set_xlabel(
             "Counterfactual scores - differences from zero indicate the direction of bias."
         )
         plt.show()
 
-    def visualize_counterfactual_sample_scores(
+    def __visualize_counterfactual_sample_scores(
         self, concept: str, top_n: Optional[int] = None
     ):
         """Visualize the counterfactual scores given concept.
 
         This differs from visualize_counterfactual_score_by_sample in that it shows the counterfactual
         score grouped by the original keyword in the text, not the counterfactual keyword.
 
         Args:
             concept: The concept to visualize.
             top_n: If given, only the top n keywords are shown.
         """
+        warnings.warn(
+            "This method is deprecated. Use dashboard() instead.", DeprecationWarning
+        )
         dataf = self._get_result_by_concept(concept=concept)
         samples = self._get_counterfactual_samples_by_concept(concept=concept)
 
         # get the original samples
         original_samples = [
             sample for sample in samples if (sample.keyword == sample.orig_keyword)
         ]
@@ -176,32 +188,35 @@
         counterfactual_df = pd.DataFrame(
             dict([(k, pd.Series(v)) for k, v in counterfactual_plot_dict.items()])
         )
 
         # plot
         ax = _plot_box_plot(counterfactual_df, top_n=top_n)
         ax.set_title(
-            f"Distribution of counterfactual scores for concept '{concept}' by original keyword\nsorted by median score"
+            f"Distribution of counterfactual scores for concept '{concept}' by original keyword\nsorted by median score\ndifference from zero indicates bias, positive values indicate bias towards the positive class"
         )
         ax.set_xlabel(
-            "Counterfactual scores - differences from zero indicate the direction of bias."
+            "Counterfactual scores - difference in probability of positive class from original sample."
         )
         plt.show()
 
-    def visualize_counterfactual_score_by_sample_histogram(
+    def __visualize_counterfactual_score_by_sample_histogram(
         self, concepts: Optional[List[str]] = None
     ):
         """Visualize the counterfactual scores for each sample as a histogram.
 
         Args:
             concepts: If given, only the concepts in this list are shown. Otherwise, all concepts are shown.
 
         Raises:
             ValueError: If no samples are found for the given concepts.
         """
+        warnings.warn(
+            "This method is deprecated. Use dashboard() instead.", DeprecationWarning
+        )
         all_scores = []
         all_samples = []
         for concept_result in self.concept_results:
             # check if the concept is in the list of concepts to show
             if concepts and (concept_result.concept not in concepts):
                 continue
             dataf = concept_result.scores.copy()
```

### Comparing `biaslyze-0.0.6a0/biaslyze/results/lime_detection_results.py` & `biaslyze-0.0.7a0/biaslyze/results/lime_detection_results.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.6a0/biaslyze/text_representation.py` & `biaslyze-0.0.7a0/biaslyze/text_representation.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,41 +2,45 @@
 
 from typing import List, Optional
 
 import spacy
 from tqdm import tqdm
 
 SPACY_TOKENIZER = spacy.load(
-    "en_core_web_sm", disable=["parser", "tagger", "ner", "lemmatizer"]
+    "en_core_web_sm", disable=["parser", "ner", "lemmatizer"] # "tagger"
 )
 
 
 class Token:
     """A class used to represent a token in the biaslyze package.
 
     Attributes:
         text (str): The text of the token.
         start (int): The start index of the token in the text.
         end (int): The end index of the token in the text.
         whitespace_after (str): The whitespace after the token.
+        shape (str): The shape of the token as defined by spacy (e.g. Xxxx).
+        function (Optional[List[str]]): The possible functions of the token (e.g. ["name", "verb"]).
     """
 
     def __init__(
         self,
         text: str,
         start: int,
         end: int,
         whitespace_after: str,
+        shape: str,
         function: Optional[List[str]] = None,
     ):
         """The constructor for the Token class."""
         self.text = text
         self.start = start
         self.end = end
         self.whitespace_after = whitespace_after
+        self.shape = shape
         self.function = function
 
 
 class TextRepresentation:
     """A class used to represent a text in the biaslyze package.
 
     Attributes:
@@ -57,23 +61,30 @@
 
     def __contains__(self, string: str) -> bool:
         """
         Returns True if the given string is contained in the text representation.
 
         Should be extended to support more complex queries.
         """
-        return string in [token.text.lower() for token in self.tokens]
+        return string.lower() in [token.text.lower() for token in self.tokens]
 
     @classmethod
     def from_spacy_doc(cls, doc: spacy.tokens.Doc):
         """Constructs a TextRepresentation object from a spacy doc."""
         tokens = []
         for token in doc:
             tokens.append(
-                Token(token.text, token.idx, token.idx + len(token), token.whitespace_)
+                Token(
+                    text=token.text,
+                    start=token.idx,
+                    end=token.idx + len(token),
+                    whitespace_after=token.whitespace_,
+                    shape=token.shape_,
+                    function=token.pos_,
+                )
             )
         return cls(doc.text, tokens)
 
 
 def process_texts_with_spacy(texts: List[str]) -> List[TextRepresentation]:
     """Processes the given texts with spacy."""
     # spacy_text_representations = SPACY_TOKENIZER.pipe(texts)
```

### Comparing `biaslyze-0.0.6a0/pyproject.toml` & `biaslyze-0.0.7a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biaslyze"
-version = "0.0.6-alpha"
+version = "0.0.7-alpha"
 description = "The NLP Bias Identification Toolkit"
 authors = [
     "Tobias Sterbak & Stina Lohmüller <hello@biaslyze.org>",
 ]
 maintainers = [
     "Tobias Sterbak <hello@tobiassterbak.com>",
     "Stina Lohmüller <slohmueller@posteo.de>",
@@ -43,19 +43,23 @@
 nvidia-cufft-cu11 = "^10.9.0.58"
 nvidia-curand-cu11 = "^10.3.0.86"
 nvidia-cusolver-cu11 = "^11.4.1.48"
 nvidia-cusparse-cu11 = "^11.7.5.86"
 nvidia-nccl-cu11 = "^2.16.5"
 nvidia-nvtx-cu11 = "^11.8.86"
 triton = "^2.0.0.post1"
+dash = "^2.11.1"
+plotly = "^5.15.0"
 
 [tool.poetry.group.dev.dependencies]
 mkdocs-material = "^9.1.1"
 material-plausible-plugin = "^0.2.0"
 mkgendocs = "^0.9.2"
+Pillow = "^10.0.0"
+CairoSVG = "^2.7.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 ruff = "^0.0.254"
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.isort]
```

### Comparing `biaslyze-0.0.6a0/setup.py` & `biaslyze-0.0.7a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bertopic==0.13.0',
  'bokeh>=3.1.0,<4.0.0',
+ 'dash>=2.11.1,<3.0.0',
  'eli5>=0.13.0,<0.14.0',
  'jupyterlab>=3.5.2,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
  'matplotlib>=3.7.1,<4.0.0',
  'numpy==1.23.2',
  'nvidia-cublas-cu11>=11.11.3.6,<12.0.0.0',
  'nvidia-cuda-cupti-cu11>=11.8.87,<12.0.0',
@@ -23,26 +24,27 @@
  'nvidia-cufft-cu11>=10.9.0.58,<11.0.0.0',
  'nvidia-curand-cu11>=10.3.0.86,<11.0.0.0',
  'nvidia-cusolver-cu11>=11.4.1.48,<12.0.0.0',
  'nvidia-cusparse-cu11>=11.7.5.86,<12.0.0.0',
  'nvidia-nccl-cu11>=2.16.5,<3.0.0',
  'nvidia-nvtx-cu11>=11.8.86,<12.0.0',
  'pandas>=1.5.3,<2.0.0',
+ 'plotly>=5.15.0,<6.0.0',
  'scikit-learn>=1.2.0,<2.0.0',
  'scipy==1.8.0',
  'spacy>=3.5.0,<4.0.0',
  'transformers>=4.26.1,<5.0.0',
  'triton>=2.0.0.post1,<3.0.0',
  'umap-learn>=0.5.3,<0.6.0']
 
 setup_kwargs = {
     'name': 'biaslyze',
-    'version': '0.0.6a0',
+    'version': '0.0.7a0',
     'description': 'The NLP Bias Identification Toolkit',
-    'long_description': '\n<p align="center">\n  <h1>biaslyze - The NLP Bias Identification Toolkit</h1>\n</p>\n\n<p align="center">\n    <a href="https://github.com/biaslyze-dev/biaslyze/blob/main/LICENSE">\n        <img alt="licence" src="https://img.shields.io/github/license/biaslyze-dev/biaslyze">\n    </a>\n    <a href="https://pypi.org/project/biaslyze/">\n        <img alt="pypi" src="https://img.shields.io/pypi/v/biaslyze">\n    </a>\n    <a href="https://pypi.org/project/biaslyze/">\n        <img alt="pypi" src="https://img.shields.io/pypi/pyversions/biaslyze">\n    </a>\n</p>\n\n\nBias is often subtle and difficult to detect in NLP models, as the protected attributes are less obvious and can take many forms in language (e.g. proxies, double meanings, ambiguities etc.). Therefore, technical bias testing is a key step in avoiding algorithmically mediated discrimination. However, it is currently conducted too rarely due to the effort involved, missing resources or lack of awareness for the problem.\n\nBiaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.\n\n## Installation\n\nInstallation can be done using pypi:\n```bash\npip install biaslyze\n```\n\nThen you need to download the required spacy models:\n```bash\npython -m spacy download en_core_web_sm\n```\n\n## Quickstart\n\n```python\nfrom biaslyze.bias_detectors import CounterfactualBiasDetector\n\nbias_detector = CounterfactualBiasDetector()\n\n# detect bias in the model based on the given texts\n# here, clf is a scikit-learn text classification pipeline trained for a binary classification task\ndetection_res = bias_detector.process(\n    texts=texts,\n    predict_func=clf.predict_proba\n)\n\n# see a summary of the detection\ndetection_res.report()\n\n# visualize the counterfactual scores\ndetection_res.visualize_counterfactual_scores(concept="religion", top_n=10)\n```\n\nExample output:\n![](resources/hatespeech_dl_scores_religion.png)\n\n\nYou can see a more detailed example in the [tutorial](tutorials/tutorial-toxic-comments/).\n\n\n## Development setup\n\n- First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation\n- Run `make install` to install the dependencies and get the spacy basemodels.\n- Now you can use `biaslyze` in your jupyter notebooks.\n\n\n### Adding concepts and keywords\n\nYou can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/keyword-based-targeted-lime/biaslyze/concepts.py).\n\n## Preview/build the documentation with mkdocs\n\nTo preview the documentation run `make doc-preview`. This will launch a preview of the documentation on `http://127.0.0.1:8000/`.\nTo build the documentation html run `make doc`.\n\n\n## Run the automated tests\n\n`make test`\n\n\n## Style guide\n\nWe are using isort and black: `make style`\nFor linting we are running ruff: `make lint`\n\n## Contributing\n\nFollow the google style guide for python: https://google.github.io/styleguide/pyguide.html\n\nThis project uses black, isort and ruff to enforce style. Apply it by running `make style` and `make lint`.\n\n## Acknowledgements\n\n* Funded from March 2023 until August 2023 by ![logos of the "Bundesministerium für Bildung und Forschung", Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)\n',
+    'long_description': '\n<div align="center">\n  <img src="resources/biaslyze-logo-no-bg.png" alt="Biaslyze" height="220px">\n  <h1>The NLP Bias Identification Toolkit</h1>\n</div>\n\n<div align="center">\n    <a href="https://github.com/biaslyze-dev/biaslyze/blob/main/LICENSE">\n        <img alt="licence" src="https://img.shields.io/github/license/biaslyze-dev/biaslyze">\n    </a>\n    <a href="https://pypi.org/project/biaslyze/">\n        <img alt="pypi" src="https://img.shields.io/pypi/v/biaslyze">\n    </a>\n    <a href="https://pypi.org/project/biaslyze/">\n        <img alt="pypi" src="https://img.shields.io/pypi/pyversions/biaslyze">\n    </a>\n</div>\n\n\nBias is often subtle and difficult to detect in NLP models, as the protected attributes are less obvious and can take many forms in language (e.g. proxies, double meanings, ambiguities etc.). Therefore, technical bias testing is a key step in avoiding algorithmically mediated discrimination. However, it is currently conducted too rarely due to the effort involved, missing resources or lack of awareness for the problem.\n\nBiaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for developers, researchers and teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.\n\n## Supported Models\n\nAll text classification models with probability output are supported. This includes models from scikit-learn, tensorflow, pytorch, huggingface transformers and others. \nSee the tutorials section for examples.\n\n## Installation\n\nInstallation can be done using pypi:\n```bash\npip install biaslyze\n```\n\nThen you need to download the required spacy models:\n```bash\npython -m spacy download en_core_web_sm\n```\n\n## Quickstart\n\n```python\nfrom biaslyze.bias_detectors import CounterfactualBiasDetector\n\nbias_detector = CounterfactualBiasDetector()\n\n# detect bias in the model based on the given texts\n# here, clf is a scikit-learn text classification pipeline trained for a binary classification task\ndetection_res = bias_detector.process(\n    texts=texts,\n    predict_func=clf.predict_proba\n)\n\n# see a summary of the detection\ndetection_res.report()\n\n# visualize the counterfactual scores\ndetection_res.visualize_counterfactual_scores(concept="religion", top_n=10)\n```\n\nYou will get results as Boxplots, among others, indicating the impact of keywords and concepts on the prediction of your model.\nExample output:\n![](resources/hatespeech_dl_scores_religion.png)\n\n\nSee more detailed examples in the [tutorial](tutorials/tutorial-toxic-comments/).\n\n\n## Development setup\n\n- First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation\n- Run `make install` to install the dependencies and get the spacy basemodels.\n- Now you can use `biaslyze` in your jupyter notebooks.\n\n\n### Adding concepts and keywords\n\nYou can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py).\n\n## Preview/build the documentation with mkdocs\n\nTo preview the documentation run `make doc-preview`. This will launch a preview of the documentation on `http://127.0.0.1:8000/`.\nTo build the documentation html run `make doc`.\n\n\n## Run the automated tests\n\n`make test`\n\n\n## Style guide\n\nWe are using isort and black: `make style`\nFor linting we are running ruff: `make lint`\n\n## Contributing\n\nFollow the google style guide for python: https://google.github.io/styleguide/pyguide.html\n\nThis project uses black, isort and ruff to enforce style. Apply it by running `make style` and `make lint`.\n\n## Acknowledgements\n\n* Funded from March 2023 until August 2023 by ![logos of the "Bundesministerium für Bildung und Forschung", Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)\n',
     'author': 'Tobias Sterbak & Stina Lohmüller',
     'author_email': 'hello@biaslyze.org',
     'maintainer': 'Tobias Sterbak',
     'maintainer_email': 'hello@tobiassterbak.com',
     'url': 'https://biaslyze.org',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,61 +1,67 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['biaslyze',
 'biaslyze.bias_detectors', 'biaslyze.results'] package_data = \ {'': ['*']}
 install_requires = \ ['bertopic==0.13.0', 'bokeh>=3.1.0,<4.0.0',
-'eli5>=0.13.0,<0.14.0', 'jupyterlab>=3.5.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
-'matplotlib>=3.7.1,<4.0.0', 'numpy==1.23.2', 'nvidia-cublas-
-cu11>=11.11.3.6,<12.0.0.0', 'nvidia-cuda-cupti-cu11>=11.8.87,<12.0.0', 'nvidia-
-cuda-nvrtc-cu11>=11.8.89,<12.0.0', 'nvidia-cuda-runtime-cu11>=11.8.89,<12.0.0',
-'nvidia-cudnn-cu11>=8.9.1.23,<9.0.0.0', 'nvidia-cufft-
+'dash>=2.11.1,<3.0.0', 'eli5>=0.13.0,<0.14.0', 'jupyterlab>=3.5.2,<4.0.0',
+'loguru>=0.6.0,<0.7.0', 'matplotlib>=3.7.1,<4.0.0', 'numpy==1.23.2', 'nvidia-
+cublas-cu11>=11.11.3.6,<12.0.0.0', 'nvidia-cuda-cupti-cu11>=11.8.87,<12.0.0',
+'nvidia-cuda-nvrtc-cu11>=11.8.89,<12.0.0', 'nvidia-cuda-runtime-
+cu11>=11.8.89,<12.0.0', 'nvidia-cudnn-cu11>=8.9.1.23,<9.0.0.0', 'nvidia-cufft-
 cu11>=10.9.0.58,<11.0.0.0', 'nvidia-curand-cu11>=10.3.0.86,<11.0.0.0', 'nvidia-
 cusolver-cu11>=11.4.1.48,<12.0.0.0', 'nvidia-cusparse-
 cu11>=11.7.5.86,<12.0.0.0', 'nvidia-nccl-cu11>=2.16.5,<3.0.0', 'nvidia-nvtx-
-cu11>=11.8.86,<12.0.0', 'pandas>=1.5.3,<2.0.0', 'scikit-learn>=1.2.0,<2.0.0',
-'scipy==1.8.0', 'spacy>=3.5.0,<4.0.0', 'transformers>=4.26.1,<5.0.0',
-'triton>=2.0.0.post1,<3.0.0', 'umap-learn>=0.5.3,<0.6.0'] setup_kwargs =
-{ 'name': 'biaslyze', 'version': '0.0.6a0', 'description': 'The NLP Bias
-Identification Toolkit', 'long_description': '\n
+cu11>=11.8.86,<12.0.0', 'pandas>=1.5.3,<2.0.0', 'plotly>=5.15.0,<6.0.0',
+'scikit-learn>=1.2.0,<2.0.0', 'scipy==1.8.0', 'spacy>=3.5.0,<4.0.0',
+'transformers>=4.26.1,<5.0.0', 'triton>=2.0.0.post1,<3.0.0', 'umap-
+learn>=0.5.3,<0.6.0'] setup_kwargs = { 'name': 'biaslyze', 'version':
+'0.0.7a0', 'description': 'The NLP Bias Identification Toolkit',
+'long_description': '\n
+                                \n [Biaslyze]\n
+               ****** The NLP Bias Identification Toolkit ******
                                       \n
-****** biaslyze - The NLP Bias Identification Toolkit ******
-\n
 \n\n
                 \n \n_[licence]\n\n \n_[pypi]\n\n \n_[pypi]\n\n
 \n\n\nBias is often subtle and difficult to detect in NLP models, as the
 protected attributes are less obvious and can take many forms in language (e.g.
 proxies, double meanings, ambiguities etc.). Therefore, technical bias testing
 is a key step in avoiding algorithmically mediated discrimination. However, it
 is currently conducted too rarely due to the effort involved, missing resources
 or lack of awareness for the problem.\n\nBiaslyze helps to get started with the
 analysis of bias within NLP models and offers a concrete entry point for
-further impact assessments and mitigation measures. Especially for teams with
-limited resources, our toolbox offers a low-effort approach to bias testing in
-NLP use cases.\n\n## Installation\n\nInstallation can be done using pypi:
-\n```bash\npip install biaslyze\n```\n\nThen you need to download the required
-spacy models:\n```bash\npython -m spacy download en_core_web_sm\n```\n\n##
+further impact assessments and mitigation measures. Especially for developers,
+researchers and teams with limited resources, our toolbox offers a low-effort
+approach to bias testing in NLP use cases.\n\n## Supported Models\n\nAll text
+classification models with probability output are supported. This includes
+models from scikit-learn, tensorflow, pytorch, huggingface transformers and
+others. \nSee the tutorials section for examples.\n\n##
+Installation\n\nInstallation can be done using pypi:\n```bash\npip install
+biaslyze\n```\n\nThen you need to download the required spacy models:
+\n```bash\npython -m spacy download en_core_web_sm\n```\n\n##
 Quickstart\n\n```python\nfrom biaslyze.bias_detectors import
 CounterfactualBiasDetector\n\nbias_detector = CounterfactualBiasDetector()\n\n#
 detect bias in the model based on the given texts\n# here, clf is a scikit-
 learn text classification pipeline trained for a binary classification
 task\ndetection_res = bias_detector.process(\n texts=texts,\n
 predict_func=clf.predict_proba\n)\n\n# see a summary of the
 detection\ndetection_res.report()\n\n# visualize the counterfactual
 scores\ndetection_res.visualize_counterfactual_scores(concept="religion",
-top_n=10)\n```\n\nExample output:\n![](resources/
-hatespeech_dl_scores_religion.png)\n\n\nYou can see a more detailed example in
-the [tutorial](tutorials/tutorial-toxic-comments/).\n\n\n## Development
-setup\n\n- First you need to install poetry to manage your python environment:
-https://python-poetry.org/docs/#installation\n- Run `make install` to install
-the dependencies and get the spacy basemodels.\n- Now you can use `biaslyze` in
-your jupyter notebooks.\n\n\n### Adding concepts and keywords\n\nYou can add
-concepts and new keywords for existing concepts by editing [concepts.py](https:
-//github.com/biaslyze-dev/biaslyze/blob/keyword-based-targeted-lime/biaslyze/
-concepts.py).\n\n## Preview/build the documentation with mkdocs\n\nTo preview
-the documentation run `make doc-preview`. This will launch a preview of the
-documentation on `http://127.0.0.1:8000/`.\nTo build the documentation html run
-`make doc`.\n\n\n## Run the automated tests\n\n`make test`\n\n\n## Style
+top_n=10)\n```\n\nYou will get results as Boxplots, among others, indicating
+the impact of keywords and concepts on the prediction of your model.\nExample
+output:\n![](resources/hatespeech_dl_scores_religion.png)\n\n\nSee more
+detailed examples in the [tutorial](tutorials/tutorial-toxic-comments/
+).\n\n\n## Development setup\n\n- First you need to install poetry to manage
+your python environment: https://python-poetry.org/docs/#installation\n- Run
+`make install` to install the dependencies and get the spacy basemodels.\n- Now
+you can use `biaslyze` in your jupyter notebooks.\n\n\n### Adding concepts and
+keywords\n\nYou can add concepts and new keywords for existing concepts by
+editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/main/
+biaslyze/concepts.py).\n\n## Preview/build the documentation with mkdocs\n\nTo
+preview the documentation run `make doc-preview`. This will launch a preview of
+the documentation on `http://127.0.0.1:8000/`.\nTo build the documentation html
+run `make doc`.\n\n\n## Run the automated tests\n\n`make test`\n\n\n## Style
 guide\n\nWe are using isort and black: `make style`\nFor linting we are running
 ruff: `make lint`\n\n## Contributing\n\nFollow the google style guide for
 python: https://google.github.io/styleguide/pyguide.html\n\nThis project uses
 black, isort and ruff to enforce style. Apply it by running `make style` and
 `make lint`.\n\n## Acknowledgements\n\n* Funded from March 2023 until August
 2023 by ![logos of the "Bundesministerium fÃ¼r Bildung und Forschung",
 Prodotype Fund and OKFN-Deutschland](resources/pf_funding_logos.svg)\n',
```

### Comparing `biaslyze-0.0.6a0/PKG-INFO` & `biaslyze-0.0.7a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biaslyze
-Version: 0.0.6a0
+Version: 0.0.7a0
 Summary: The NLP Bias Identification Toolkit
 Home-page: https://biaslyze.org
 License: BSD-3-Clause
 Keywords: NLP,bias,ethics,fairness
 Author: Tobias Sterbak & Stina Lohmüller
 Author-email: hello@biaslyze.org
 Maintainer: Tobias Sterbak
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: bertopic (==0.13.0)
 Requires-Dist: bokeh (>=3.1.0,<4.0.0)
+Requires-Dist: dash (>=2.11.1,<3.0.0)
 Requires-Dist: eli5 (>=0.13.0,<0.14.0)
 Requires-Dist: jupyterlab (>=3.5.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (==1.23.2)
 Requires-Dist: nvidia-cublas-cu11 (>=11.11.3.6,<12.0.0.0)
 Requires-Dist: nvidia-cuda-cupti-cu11 (>=11.8.87,<12.0.0)
@@ -30,44 +31,51 @@
 Requires-Dist: nvidia-cufft-cu11 (>=10.9.0.58,<11.0.0.0)
 Requires-Dist: nvidia-curand-cu11 (>=10.3.0.86,<11.0.0.0)
 Requires-Dist: nvidia-cusolver-cu11 (>=11.4.1.48,<12.0.0.0)
 Requires-Dist: nvidia-cusparse-cu11 (>=11.7.5.86,<12.0.0.0)
 Requires-Dist: nvidia-nccl-cu11 (>=2.16.5,<3.0.0)
 Requires-Dist: nvidia-nvtx-cu11 (>=11.8.86,<12.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: scipy (==1.8.0)
 Requires-Dist: spacy (>=3.5.0,<4.0.0)
 Requires-Dist: transformers (>=4.26.1,<5.0.0)
 Requires-Dist: triton (>=2.0.0.post1,<3.0.0)
 Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
 Project-URL: Repository, https://github.com/biaslyze-dev/biaslyze/issues
 Description-Content-Type: text/markdown
 
 
-<p align="center">
-  <h1>biaslyze - The NLP Bias Identification Toolkit</h1>
-</p>
+<div align="center">
+  <img src="resources/biaslyze-logo-no-bg.png" alt="Biaslyze" height="220px">
+  <h1>The NLP Bias Identification Toolkit</h1>
+</div>
 
-<p align="center">
+<div align="center">
     <a href="https://github.com/biaslyze-dev/biaslyze/blob/main/LICENSE">
         <img alt="licence" src="https://img.shields.io/github/license/biaslyze-dev/biaslyze">
     </a>
     <a href="https://pypi.org/project/biaslyze/">
         <img alt="pypi" src="https://img.shields.io/pypi/v/biaslyze">
     </a>
     <a href="https://pypi.org/project/biaslyze/">
         <img alt="pypi" src="https://img.shields.io/pypi/pyversions/biaslyze">
     </a>
-</p>
+</div>
 
 
 Bias is often subtle and difficult to detect in NLP models, as the protected attributes are less obvious and can take many forms in language (e.g. proxies, double meanings, ambiguities etc.). Therefore, technical bias testing is a key step in avoiding algorithmically mediated discrimination. However, it is currently conducted too rarely due to the effort involved, missing resources or lack of awareness for the problem.
 
-Biaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.
+Biaslyze helps to get started with the analysis of bias within NLP models and offers a concrete entry point for further impact assessments and mitigation measures. Especially for developers, researchers and teams with limited resources, our toolbox offers a low-effort approach to bias testing in NLP use cases.
+
+## Supported Models
+
+All text classification models with probability output are supported. This includes models from scikit-learn, tensorflow, pytorch, huggingface transformers and others. 
+See the tutorials section for examples.
 
 ## Installation
 
 Installation can be done using pypi:
 ```bash
 pip install biaslyze
 ```
@@ -94,31 +102,32 @@
 # see a summary of the detection
 detection_res.report()
 
 # visualize the counterfactual scores
 detection_res.visualize_counterfactual_scores(concept="religion", top_n=10)
 ```
 
+You will get results as Boxplots, among others, indicating the impact of keywords and concepts on the prediction of your model.
 Example output:
 ![](resources/hatespeech_dl_scores_religion.png)
 
 
-You can see a more detailed example in the [tutorial](tutorials/tutorial-toxic-comments/).
+See more detailed examples in the [tutorial](tutorials/tutorial-toxic-comments/).
 
 
 ## Development setup
 
 - First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation
 - Run `make install` to install the dependencies and get the spacy basemodels.
 - Now you can use `biaslyze` in your jupyter notebooks.
 
 
 ### Adding concepts and keywords
 
-You can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/keyword-based-targeted-lime/biaslyze/concepts.py).
+You can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py).
 
 ## Preview/build the documentation with mkdocs
 
 To preview the documentation run `make doc-preview`. This will launch a preview of the documentation on `http://127.0.0.1:8000/`.
 To build the documentation html run `make doc`.
```

#### html2text {}

```diff
@@ -1,66 +1,74 @@
-Metadata-Version: 2.1 Name: biaslyze Version: 0.0.6a0 Summary: The NLP Bias
+Metadata-Version: 2.1 Name: biaslyze Version: 0.0.7a0 Summary: The NLP Bias
 Identification Toolkit Home-page: https://biaslyze.org License: BSD-3-Clause
 Keywords: NLP,bias,ethics,fairness Author: Tobias Sterbak & Stina LohmÃ¼ller
 Author-email: hello@biaslyze.org Maintainer: Tobias Sterbak Maintainer-email:
 hello@tobiassterbak.com Requires-Python: >=3.10,<3.11 Classifier: License ::
 OSI Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Dist: bertopic (==0.13.0)
-Requires-Dist: bokeh (>=3.1.0,<4.0.0) Requires-Dist: eli5 (>=0.13.0,<0.14.0)
-Requires-Dist: jupyterlab (>=3.5.2,<4.0.0) Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist:
-numpy (==1.23.2) Requires-Dist: nvidia-cublas-cu11 (>=11.11.3.6,<12.0.0.0)
-Requires-Dist: nvidia-cuda-cupti-cu11 (>=11.8.87,<12.0.0) Requires-Dist:
-nvidia-cuda-nvrtc-cu11 (>=11.8.89,<12.0.0) Requires-Dist: nvidia-cuda-runtime-
-cu11 (>=11.8.89,<12.0.0) Requires-Dist: nvidia-cudnn-cu11 (>=8.9.1.23,<9.0.0.0)
-Requires-Dist: nvidia-cufft-cu11 (>=10.9.0.58,<11.0.0.0) Requires-Dist: nvidia-
-curand-cu11 (>=10.3.0.86,<11.0.0.0) Requires-Dist: nvidia-cusolver-cu11
+Requires-Dist: bokeh (>=3.1.0,<4.0.0) Requires-Dist: dash (>=2.11.1,<3.0.0)
+Requires-Dist: eli5 (>=0.13.0,<0.14.0) Requires-Dist: jupyterlab
+(>=3.5.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
+matplotlib (>=3.7.1,<4.0.0) Requires-Dist: numpy (==1.23.2) Requires-Dist:
+nvidia-cublas-cu11 (>=11.11.3.6,<12.0.0.0) Requires-Dist: nvidia-cuda-cupti-
+cu11 (>=11.8.87,<12.0.0) Requires-Dist: nvidia-cuda-nvrtc-cu11
+(>=11.8.89,<12.0.0) Requires-Dist: nvidia-cuda-runtime-cu11 (>=11.8.89,<12.0.0)
+Requires-Dist: nvidia-cudnn-cu11 (>=8.9.1.23,<9.0.0.0) Requires-Dist: nvidia-
+cufft-cu11 (>=10.9.0.58,<11.0.0.0) Requires-Dist: nvidia-curand-cu11
+(>=10.3.0.86,<11.0.0.0) Requires-Dist: nvidia-cusolver-cu11
 (>=11.4.1.48,<12.0.0.0) Requires-Dist: nvidia-cusparse-cu11
 (>=11.7.5.86,<12.0.0.0) Requires-Dist: nvidia-nccl-cu11 (>=2.16.5,<3.0.0)
 Requires-Dist: nvidia-nvtx-cu11 (>=11.8.86,<12.0.0) Requires-Dist: pandas
-(>=1.5.3,<2.0.0) Requires-Dist: scikit-learn (>=1.2.0,<2.0.0) Requires-Dist:
-scipy (==1.8.0) Requires-Dist: spacy (>=3.5.0,<4.0.0) Requires-Dist:
-transformers (>=4.26.1,<5.0.0) Requires-Dist: triton (>=2.0.0.post1,<3.0.0)
-Requires-Dist: umap-learn (>=0.5.3,<0.6.0) Project-URL: Repository, https://
-github.com/biaslyze-dev/biaslyze/issues Description-Content-Type: text/markdown
-****** biaslyze - The NLP Bias Identification Toolkit ******
+(>=1.5.3,<2.0.0) Requires-Dist: plotly (>=5.15.0,<6.0.0) Requires-Dist: scikit-
+learn (>=1.2.0,<2.0.0) Requires-Dist: scipy (==1.8.0) Requires-Dist: spacy
+(>=3.5.0,<4.0.0) Requires-Dist: transformers (>=4.26.1,<5.0.0) Requires-Dist:
+triton (>=2.0.0.post1,<3.0.0) Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
+Project-URL: Repository, https://github.com/biaslyze-dev/biaslyze/issues
+Description-Content-Type: text/markdown
+                                  [Biaslyze]
+               ****** The NLP Bias Identification Toolkit ******
                             [licence] [pypi] [pypi]
 Bias is often subtle and difficult to detect in NLP models, as the protected
 attributes are less obvious and can take many forms in language (e.g. proxies,
 double meanings, ambiguities etc.). Therefore, technical bias testing is a key
 step in avoiding algorithmically mediated discrimination. However, it is
 currently conducted too rarely due to the effort involved, missing resources or
 lack of awareness for the problem. Biaslyze helps to get started with the
 analysis of bias within NLP models and offers a concrete entry point for
-further impact assessments and mitigation measures. Especially for teams with
-limited resources, our toolbox offers a low-effort approach to bias testing in
-NLP use cases. ## Installation Installation can be done using pypi: ```bash pip
-install biaslyze ``` Then you need to download the required spacy models:
-```bash python -m spacy download en_core_web_sm ``` ## Quickstart ```python
-from biaslyze.bias_detectors import CounterfactualBiasDetector bias_detector =
-CounterfactualBiasDetector() # detect bias in the model based on the given
-texts # here, clf is a scikit-learn text classification pipeline trained for a
-binary classification task detection_res = bias_detector.process( texts=texts,
+further impact assessments and mitigation measures. Especially for developers,
+researchers and teams with limited resources, our toolbox offers a low-effort
+approach to bias testing in NLP use cases. ## Supported Models All text
+classification models with probability output are supported. This includes
+models from scikit-learn, tensorflow, pytorch, huggingface transformers and
+others. See the tutorials section for examples. ## Installation Installation
+can be done using pypi: ```bash pip install biaslyze ``` Then you need to
+download the required spacy models: ```bash python -m spacy download
+en_core_web_sm ``` ## Quickstart ```python from biaslyze.bias_detectors import
+CounterfactualBiasDetector bias_detector = CounterfactualBiasDetector() #
+detect bias in the model based on the given texts # here, clf is a scikit-learn
+text classification pipeline trained for a binary classification task
+detection_res = bias_detector.process( texts=texts,
 predict_func=clf.predict_proba ) # see a summary of the detection
 detection_res.report() # visualize the counterfactual scores
 detection_res.visualize_counterfactual_scores(concept="religion", top_n=10) ```
-Example output: ![](resources/hatespeech_dl_scores_religion.png) You can see a
-more detailed example in the [tutorial](tutorials/tutorial-toxic-comments/). ##
-Development setup - First you need to install poetry to manage your python
-environment: https://python-poetry.org/docs/#installation - Run `make install`
-to install the dependencies and get the spacy basemodels. - Now you can use
-`biaslyze` in your jupyter notebooks. ### Adding concepts and keywords You can
-add concepts and new keywords for existing concepts by editing [concepts.py]
-(https://github.com/biaslyze-dev/biaslyze/blob/keyword-based-targeted-lime/
-biaslyze/concepts.py). ## Preview/build the documentation with mkdocs To
-preview the documentation run `make doc-preview`. This will launch a preview of
-the documentation on `http://127.0.0.1:8000/`. To build the documentation html
-run `make doc`. ## Run the automated tests `make test` ## Style guide We are
-using isort and black: `make style` For linting we are running ruff: `make
-lint` ## Contributing Follow the google style guide for python: https://
-google.github.io/styleguide/pyguide.html This project uses black, isort and
-ruff to enforce style. Apply it by running `make style` and `make lint`. ##
-Acknowledgements * Funded from March 2023 until August 2023 by ![logos of the
-"Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund and OKFN-
-Deutschland](resources/pf_funding_logos.svg)
+You will get results as Boxplots, among others, indicating the impact of
+keywords and concepts on the prediction of your model. Example output: ![]
+(resources/hatespeech_dl_scores_religion.png) See more detailed examples in the
+[tutorial](tutorials/tutorial-toxic-comments/). ## Development setup - First
+you need to install poetry to manage your python environment: https://python-
+poetry.org/docs/#installation - Run `make install` to install the dependencies
+and get the spacy basemodels. - Now you can use `biaslyze` in your jupyter
+notebooks. ### Adding concepts and keywords You can add concepts and new
+keywords for existing concepts by editing [concepts.py](https://github.com/
+biaslyze-dev/biaslyze/blob/main/biaslyze/concepts.py). ## Preview/build the
+documentation with mkdocs To preview the documentation run `make doc-preview`.
+This will launch a preview of the documentation on `http://127.0.0.1:8000/`. To
+build the documentation html run `make doc`. ## Run the automated tests `make
+test` ## Style guide We are using isort and black: `make style` For linting we
+are running ruff: `make lint` ## Contributing Follow the google style guide for
+python: https://google.github.io/styleguide/pyguide.html This project uses
+black, isort and ruff to enforce style. Apply it by running `make style` and
+`make lint`. ## Acknowledgements * Funded from March 2023 until August 2023 by
+![logos of the "Bundesministerium fÃ¼r Bildung und Forschung", Prodotype Fund
+and OKFN-Deutschland](resources/pf_funding_logos.svg)
```

