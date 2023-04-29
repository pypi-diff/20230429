# Comparing `tmp/hugging_py_face-0.1.1.tar.gz` & `tmp/hugging_py_face-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hugging_py_face-0.1.1.tar", last modified: Tue Apr 18 17:55:57 2023, max compression
+gzip compressed data, was "dist\hugging_py_face-0.2.0.tar", last modified: Sat Apr 29 16:07:13 2023, max compression
```

## Comparing `hugging_py_face-0.1.1.tar` & `hugging_py_face-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/
--rw-rw-rw-   0        0        0     6177 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4692 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face/
--rw-rw-rw-   0        0        0      466 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/__about__.py
--rw-rw-rw-   0        0        0      112 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/__init__.py
--rw-rw-rw-   0        0        0     3877 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/audio_processing.py
--rw-rw-rw-   0        0        0     2844 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/computer_vision.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face/config/
--rw-rw-rw-   0        0        0      719 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/config/config.yaml
--rw-rw-rw-   0        0        0      320 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/config_parser.py
--rw-rw-rw-   0        0        0     1479 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/multimedia_processing.py
--rw-rw-rw-   0        0        0    17264 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/hugging_py_face/nlp.py
-drwxrwxrwx   0        0        0        0 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/
--rw-rw-rw-   0        0        0     6177 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/hugging_py_face.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 17:55:57.000000 hugging_py_face-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-04-18 17:55:35.000000 hugging_py_face-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/
+-rw-rw-rw-   0        0        0     6177 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4692 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/hugging_py_face/
+-rw-rw-rw-   0        0        0      466 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/__about__.py
+-rw-rw-rw-   0        0        0      112 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/__init__.py
+-rw-rw-rw-   0        0        0     3877 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/audio_processing.py
+-rw-rw-rw-   0        0        0     2852 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/computer_vision.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/hugging_py_face/config/
+-rw-rw-rw-   0        0        0      827 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/config/config.yaml
+-rw-rw-rw-   0        0        0      265 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/config/logging.yaml
+-rw-rw-rw-   0        0        0      320 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/config_parser.py
+-rw-rw-rw-   0        0        0       63 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/exceptions.py
+-rw-rw-rw-   0        0        0     2471 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/multimedia_processing.py
+-rw-rw-rw-   0        0        0    24493 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/hugging_py_face/nlp.py
+drwxrwxrwx   0        0        0        0 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/hugging_py_face.egg-info/
+-rw-rw-rw-   0        0        0     6177 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/hugging_py_face.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/hugging_py_face.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/hugging_py_face.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/hugging_py_face.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/hugging_py_face.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 16:07:13.000000 hugging_py_face-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-04-29 16:06:49.000000 hugging_py_face-0.2.0/setup.py
```

### Comparing `hugging_py_face-0.1.1/PKG-INFO` & `hugging_py_face-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugging_py_face
-Version: 0.1.1
+Version: 0.2.0
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.1.1/README.md` & `hugging_py_face-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.1.1/hugging_py_face/audio_processing.py` & `hugging_py_face-0.2.0/hugging_py_face/audio_processing.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.1.1/hugging_py_face/computer_vision.py` & `hugging_py_face-0.2.0/hugging_py_face/computer_vision.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,10 +39,10 @@
         Perform object detection on an image from a file path or an url.
 
         :param inputs: a string or a list of strings of the file paths or urls of the images to perform object detection on.
         :param model: the model to use for the object detection task. If not provided, the recommended model from Hugging Face will be used.
         :return: a list of dictionaries each containing the label, the confidence score for that label, and the bounding box coordinates.
         """
         if type(inputs) == list:
-            return self._query(inputs, model=model, task="object-detection")
+            return self._query_in_list(inputs, model=model, task="object-detection")
         elif type(inputs) == str:
             return self._query(inputs, model=model, task="object-detection")
```

### Comparing `hugging_py_face-0.1.1/hugging_py_face/config/config.yaml` & `hugging_py_face-0.2.0/hugging_py_face/config/config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 BASE_URL: https://api-inference.huggingface.co/models
 TASK_MODEL_MAP:
   fill-mask: bert-base-uncased
   summarization: facebook/bart-large-cnn
   question-answering: deepset/roberta-base-squad2
+  table-question-answering: google/tapas-base-finetuned-wtq
   sentence-similarity: sentence-transformers/all-MiniLM-L6-v2
   text-classification: distilbert-base-uncased-finetuned-sst-2-english
   text-generation: gpt2
   zero-shot-classification: facebook/bart-large-mnli
   conversational: microsoft/DialoGPT-large
   feature-extraction: julien-c/distilbert-feature-extraction
   image-classification: google/vit-base-patch16-224
   object-detection: facebook/detr-resnet-50
   speech-recognition: facebook/wav2vec2-base-960h
-  audio-classification: superb/hubert-large-superb-er
+  audio-classification: superb/hubert-large-superb-er
+MAX_RETRIES: 5
+HTTP_SERVICE_UNAVAILABLE: 503
```

### Comparing `hugging_py_face-0.1.1/hugging_py_face/multimedia_processing.py` & `hugging_py_face-0.2.0/hugging_py_face/multimedia_processing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 import json
+import time
+import logging
 import requests
+import logging.config
 from typing import Text, Dict, List, Optional, Union
+
 from .config_parser import ConfigParser
+from .exceptions import HTTPServiceUnavailableException
+
+logging_config_parser = ConfigParser('config/logging.yaml')
+logging.config.dictConfig(logging_config_parser.get_config_dict())
+logger = logging.getLogger()
 
 
 class MultimediaProcessing:
     def __init__(self, api_token):
         self.api_token = api_token
 
         config_parser = ConfigParser()
         self.config = config_parser.get_config_dict()
 
+        self.logger = logger
+
     def _query(self, input: Text, model: Optional[Text] = None, task: Optional[Text] = None) -> Union[Dict, List]:
         api_url = f"{self.config['BASE_URL']}/{model if model is not None else self.config['TASK_MODEL_MAP'][task]}"
 
         headers = {
             "Authorization": f"Bearer {self.api_token}"
         }
 
@@ -24,15 +35,30 @@
 
             data = response.content
 
         else:
             with open(input, "rb") as f:
                 data = f.read()
 
+        retries = 0
+
+        while retries < self.config['MAX_RETRIES']:
+            retries += 1
+
         response = requests.request("POST", api_url, headers=headers, data=data)
-        return json.loads(response.content.decode("utf-8"))
+        if response.status_code == int(self.config['HTTP_SERVICE_UNAVAILABLE']):
+            self.logger.info(f"Status code: {response.status_code}.")
+            self.logger.info("Retrying..")
+            time.sleep(1)
+        else:
+            return json.loads(response.content.decode("utf-8"))
+
+        self.logger.info(f"Status code: {response.status_code}.")
+        self.logger.info("Connection to the server failed after reaching maximum retry attempts.")
+        self.logger.debug(f"Response: {json.loads(response.content.decode('utf-8'))}.")
+        raise HTTPServiceUnavailableException("The HTTP service is unavailable.")
 
     def _query_in_list(self, inputs: List[Text], model: Optional[Text] = None, task: Optional[Text] = None) -> List[Union[Dict, List]]:
         return [self._query(input, model, task) for input in inputs]
 
     def _query_in_df(self, df, input_column: Text, model: Optional[Text] = None, task: Optional[Text] = None) -> List[Union[Dict, List]]:
         return self._query_in_list(df[input_column].tolist(), model, task)
```

### Comparing `hugging_py_face-0.1.1/hugging_py_face/nlp.py` & `hugging_py_face-0.2.0/hugging_py_face/nlp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import json
+import time
+import logging
 import requests
+import pandas as pd
+import logging.config
 from pandas import DataFrame
 from typing import Text, List, Dict, Optional, Union
 
 from .config_parser import ConfigParser
+from .exceptions import HTTPServiceUnavailableException
+
+logging_config_parser = ConfigParser('config/logging.yaml')
+logging.config.dictConfig(logging_config_parser.get_config_dict())
+logger = logging.getLogger()
 
 
 class NLP:
     def __init__(self, api_token):
         self.api_token = api_token
 
         config_parser = ConfigParser()
         self.config = config_parser.get_config_dict()
 
+        self.logger = logger
+
     def _query(self, inputs: Union[Text, List, Dict], parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None, task: Optional[Text] = None) -> Union[Dict, List]:
         api_url = f"{self.config['BASE_URL']}/{model if model is not None else self.config['TASK_MODEL_MAP'][task]}"
 
         headers = {
             "Authorization": f"Bearer {self.api_token}"
         }
 
@@ -26,16 +37,31 @@
 
         if parameters is not None:
             data['parameters'] = parameters
 
         if options is not None:
             data['options'] = options
 
-        response = requests.request("POST", api_url, headers=headers, data=json.dumps(data))
-        return json.loads(response.content.decode("utf-8"))
+        retries = 0
+
+        while retries < self.config['MAX_RETRIES']:
+            retries += 1
+
+            response = requests.request("POST", api_url, headers=headers, data=json.dumps(data))
+            if response.status_code == int(self.config['HTTP_SERVICE_UNAVAILABLE']):
+                self.logger.info(f"Status code: {response.status_code}.")
+                self.logger.info("Retrying..")
+                time.sleep(1)
+            else:
+                return json.loads(response.content.decode("utf-8"))
+
+        self.logger.info(f"Status code: {response.status_code}.")
+        self.logger.info("Connection to the server failed after reaching maximum retry attempts.")
+        self.logger.debug(f"Response: {json.loads(response.content.decode('utf-8'))}.")
+        raise HTTPServiceUnavailableException("The HTTP service is unavailable.")
 
     def _query_in_df(self, df: DataFrame, column: Text, parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None, task: Optional[Text] = None) -> Union[Dict, List]:
         return self._query(df[column].tolist(), parameters, options, model, task)
 
     def fill_mask(self, text: Union[Text, List], options: Optional[Dict] = None, model: Optional[Text] = None) -> List:
         """
         Fill in a masked portion(token) of a string or a list of strings.
@@ -107,14 +133,74 @@
                 "question": question,
                 "context": context
             },
             model=model,
             task='question-answering'
         )
 
+    def question_answering_in_df(self, df: DataFrame, question_column: Text, context_column: Text, model: Optional[Text] = None) -> DataFrame:
+        """
+        Generate answers for a column of questions based on a provided column of context.
+
+        :param df: a pandas DataFrame containing the questions to be answered along with the relevant context.
+        :param question_column: the column containing the questions to be answered.
+        :param context_column: the column containing the relevant context for each question.
+        :param model: the model to use for the question answering task. If not provided, the recommended model from Hugging Face will be used.
+        :return: a pandas DataFrame with the answers for the questions. The answers will be added as a new column called 'predictions' to the original DataFrame.
+        """
+        answers = []
+        for index, row in df.iterrows():
+            answer = self._query(
+                {
+                    "question": row[question_column],
+                    "context": row[context_column]
+                },
+                model=model,
+                task='question-answering'
+            )
+            answers.append(answer['answer'])
+
+        df['predictions'] = answers
+        return df
+
+    def table_question_answering(self, question: Union[Text, List], table: Dict[Text, List], options: Optional[Dict] = None, model: Optional[Text] = None) -> List:
+        """
+
+        :param question: a string or a list of strings of the question(s) to be answered.
+        :param table: a dict of lists representing a table of data.
+        :param options: a dict of options. For more information, see the `detailed parameters for the table question answering task <https://huggingface.co/docs/api-inference/detailed_parameters#table-question-answering-task>`_.
+        :param model: the model to use for the table question answering task. If not provided, the recommended model from Hugging Face will be used.
+        :return: a dict or a list of dicts of the answers.
+        """
+        return self._query(
+            {
+                "query": question,
+                "table": table
+            },
+            options=options,
+            model=model,
+            task='table-question-answering'
+        )
+
+    def table_question_answering_task_in_df(self, df: DataFrame, question: Union[Text, List], options: Optional[Dict] = None, model: Optional[Text] = None) -> DataFrame:
+        answers = self._query(
+            {
+                "query": question,
+                "table": df.to_dict('list')
+            },
+            options=options,
+            model=model,
+            task='table-question-answering'
+        )
+
+        return pd.DataFrame({
+            "question": question,
+            "predictions": [answer['answer'] for answer in answers]
+        })
+
     def sentence_similarity(self, source_sentence: Text, sentences: List, options: Optional[Dict] = None, model: Optional[Text] = None) -> List:
         """
         Calculate the semantic similarity between one text and a list of other sentences by comparing their embeddings.
 
         :param source_sentence: the string that you wish to compare the other strings with.
         :param sentences: a list of strings which will be compared against the source_sentence.
         :param options: a dict of options. For more information, see the `detailed parameters for the sentence similarity task <https://huggingface.co/docs/api-inference/detailed_parameters#sentence-similarity-task>`_.
@@ -127,14 +213,40 @@
                 "sentences": sentences
             },
             options=options,
             model=model,
             task='sentence-similarity'
         )
 
+    def sentence_similarity_in_df(self, df: DataFrame, source_sentence_column: Text, sentence_column: Text, options: Optional[Dict] = None, model: Optional[Text] = None) -> DataFrame:
+        """
+        Calculate the semantic similarity between sentences in two columns by comparing their embeddings.
+
+        :param df: a pandas DataFrame containing the source sentences and the sentences to be compared against.
+        :param source_sentence_column: the column containing the strings that you wish to compare the other strings with.
+        :param sentence_column: the column containing the strings which will be compared against the source_sentence.
+        :param options: a dict of options. For more information, see the `detailed parameters for the sentence similarity task <https://huggingface.co/docs/api-inference/detailed_parameters#sentence-similarity-task>`_.
+        :param model: the model to use for the sentence similarity task. If not provided, the recommended model from Hugging Face will be used.
+        :return: a pandas DataFrame with the similarity scores for the sentences. The scores will be added as a new column called 'predictions' to the original DataFrame.
+        """
+        scores = []
+        for index, row in df.iterrows():
+            score = self._query(
+                {
+                    "source_sentence": row[source_sentence_column],
+                    "sentences": [row[sentence_column]]
+                },
+                model=model,
+                task='sentence-similarity'
+            )
+            scores.append(score[0])
+
+        df['predictions'] = scores
+        return df
+
     def text_classification(self, text: Union[Text, List], options: Optional[Dict] = None, model: Optional[Text] = None) -> Union[Dict, List]:
         """
         Analyze the sentiment of a string or a list of strings.
 
         :param text: a string or list of strings to be analyzed.
         :param options: a dict of options. For more information, see the `detailed parameters for the summarization task <https://huggingface.co/docs/api-inference/detailed_parameters#text-classification-task>`_.
         :param model: the model to use for the text classification task. If not provided, the recommended model from Hugging Face will be used.
@@ -200,14 +312,30 @@
             text,
             parameters=parameters,
             options=options,
             model=model,
             task='zero-shot-classification'
         )
 
+    def zero_shot_classification_in_df(self, df: DataFrame, column: Text, candidate_labels: List, parameters: Optional[Dict] = {}, options: Optional[Dict] = None, model: Optional[Text] = None):
+        """
+
+        :param df: a pandas DataFrame containing the strings to be classified.
+        :param column: the column containing the strings to be classified.
+        :param candidate_labels: a list of strings that are potential classes for inputs.
+        :param parameters: a dict of parameters excluding candidate_labels which is passed in as a separate argument. For more information, see the `detailed parameters for the zero shot classification task <https://huggingface.co/docs/api-inference/detailed_parameters#zeroshot-classification-task>`_.
+        :param options: a dict of options. For more information, see the `detailed parameters for the zero shot classification task <https://huggingface.co/docs/api-inference/detailed_parameters#zeroshot-classification-task>`_.
+        :param model: the model to use for the zero shot classification task. If not provided, the recommended model from Hugging Face will be used.
+        :return: a pandas DataFrame with the classifications. The classifications will be added as a new column called 'predictions' to the original DataFrame.
+        """
+        parameters['candidate_labels'] = candidate_labels
+        predictions = self._query_in_df(df, column, parameters=parameters, options=options, model=model, task='zero-shot-classification')
+        df['predictions'] = [prediction['labels'][0] for prediction in predictions]
+        return df
+
     def conversational(self, text: Union[Text, List], past_user_inputs: Optional[List] = None, generated_responses: Optional[List] = None, parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None) -> Union[Dict, List]:
         """
         Corresponds to any chatbot like structure: pass in some text along with the past_user_inputs and generated_responses to receive a response.
 
         :param text: a string or list of strings representing the last input(s) from the user in the conversation.
         :param past_user_inputs: a list of strings corresponding to the earlier replies from the user. Should be of the same length of generated_responses. Each response from the bot will contain past_user_inputs previously passed into the model.
         :param generated_responses: a list of strings corresponding to the earlier replies from the model. Each response from the bot will contain generated_responses from earlier replies from the model.
```

### Comparing `hugging_py_face-0.1.1/hugging_py_face.egg-info/PKG-INFO` & `hugging_py_face-0.2.0/hugging_py_face.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugging-py-face
-Version: 0.1.1
+Version: 0.2.0
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.1.1/setup.py` & `hugging_py_face-0.2.0/setup.py`

 * *Files identical despite different names*

