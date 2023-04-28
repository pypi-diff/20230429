# Comparing `tmp/PrimeBotFramework-0.0.8.tar.gz` & `tmp/PrimeBotFramework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrimeBotFramework-0.0.8.tar", last modified: Tue Dec 20 13:07:08 2022, max compression
+gzip compressed data, was "PrimeBotFramework-0.0.9.tar", last modified: Tue Dec 20 17:49:26 2022, max compression
```

## Comparing `PrimeBotFramework-0.0.8.tar` & `PrimeBotFramework-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.624910 PrimeBotFramework-0.0.8/
--rw-rw-rw-   0        0        0      779 2022-12-20 13:00:03.000000 PrimeBotFramework-0.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0       30 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3693 2022-12-20 13:07:08.624429 PrimeBotFramework-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.599463 PrimeBotFramework-0.0.8/PrimeBot/
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.611426 PrimeBotFramework-0.0.8/PrimeBot/CpfCnpj/
--rw-rw-rw-   0        0        0     1897 2022-12-20 12:30:05.000000 PrimeBotFramework-0.0.8/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0        0        0      693 2022-12-19 19:04:36.000000 PrimeBotFramework-0.0.8/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0        0        0      336 2022-12-20 12:54:48.000000 PrimeBotFramework-0.0.8/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.613419 PrimeBotFramework-0.0.8/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0        0        0     2912 2022-12-20 11:57:30.000000 PrimeBotFramework-0.0.8/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.614419 PrimeBotFramework-0.0.8/PrimeBot/Documents/
--rw-rw-rw-   0        0        0     1115 2022-12-20 11:58:03.000000 PrimeBotFramework-0.0.8/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.616412 PrimeBotFramework-0.0.8/PrimeBot/Elastic/
--rw-rw-rw-   0        0        0     1292 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.8/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.617409 PrimeBotFramework-0.0.8/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0        0        0     9261 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.8/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.620683 PrimeBotFramework-0.0.8/PrimeBot/Mongo/
--rw-rw-rw-   0        0        0      431 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.8/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.622398 PrimeBotFramework-0.0.8/PrimeBot/Vault/
--rw-rw-rw-   0        0        0     2828 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.8/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.8/PrimeBot/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 13:07:08.607436 PrimeBotFramework-0.0.8/PrimeBotFramework.egg-info/
--rw-rw-rw-   0        0        0     3693 2022-12-20 13:07:08.000000 PrimeBotFramework-0.0.8/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2022-12-20 13:07:08.000000 PrimeBotFramework-0.0.8/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 13:07:08.000000 PrimeBotFramework-0.0.8/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2022-12-20 13:07:08.000000 PrimeBotFramework-0.0.8/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-20 13:07:08.000000 PrimeBotFramework-0.0.8/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2307 2022-12-20 13:06:05.000000 PrimeBotFramework-0.0.8/README.md
--rw-rw-rw-   0        0        0      213 2022-12-20 12:32:35.000000 PrimeBotFramework-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-12-20 13:07:08.625451 PrimeBotFramework-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      971 2022-12-20 13:00:17.000000 PrimeBotFramework-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.560529 PrimeBotFramework-0.0.9/
+-rw-rw-rw-   0        0        0      868 2022-12-20 17:47:57.000000 PrimeBotFramework-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       30 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3786 2022-12-20 17:49:26.559531 PrimeBotFramework-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.535594 PrimeBotFramework-0.0.9/PrimeBot/
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.548559 PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0        0        0     1932 2022-12-20 17:44:24.000000 PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0        0        0      693 2022-12-20 17:45:49.000000 PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0        0        0      336 2022-12-20 17:44:43.000000 PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.549556 PrimeBotFramework-0.0.9/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0        0        0     2912 2022-12-20 11:57:30.000000 PrimeBotFramework-0.0.9/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.550554 PrimeBotFramework-0.0.9/PrimeBot/Documents/
+-rw-rw-rw-   0        0        0     1115 2022-12-20 11:58:03.000000 PrimeBotFramework-0.0.9/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.553548 PrimeBotFramework-0.0.9/PrimeBot/Elastic/
+-rw-rw-rw-   0        0        0     1292 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.554544 PrimeBotFramework-0.0.9/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0        0        0     9261 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.556540 PrimeBotFramework-0.0.9/PrimeBot/Mongo/
+-rw-rw-rw-   0        0        0      431 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.557538 PrimeBotFramework-0.0.9/PrimeBot/Vault/
+-rw-rw-rw-   0        0        0     2828 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-12-20 11:50:56.000000 PrimeBotFramework-0.0.9/PrimeBot/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 17:49:26.544569 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/
+-rw-rw-rw-   0        0        0     3786 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-12-20 17:49:26.000000 PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2307 2022-12-20 13:06:05.000000 PrimeBotFramework-0.0.9/README.md
+-rw-rw-rw-   0        0        0      213 2022-12-20 12:32:35.000000 PrimeBotFramework-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-12-20 17:49:26.560529 PrimeBotFramework-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      971 2022-12-20 17:46:18.000000 PrimeBotFramework-0.0.9/setup.py
```

### Comparing `PrimeBotFramework-0.0.8/CHANGELOG.txt` & `PrimeBotFramework-0.0.9/CHANGELOG.txt`

 * *Files 7% similar despite different names*

```diff
@@ -27,8 +27,12 @@
 
 ------------------
 0.0.7 (2022-12-13)
 - DeathByCaptcha: Alteracoes nos retornos das exceptions
 
 ------------------
 0.0.8 (2022-12-20)
-- CpfCnpj: Inclusão da biblioteca
+- CpfCnpj: Inclusão da biblioteca
+
+------------------
+0.0.9 (2022-12-20)
+- CpfCnpj: Ajustes para importação do model
```

### Comparing `PrimeBotFramework-0.0.8/PKG-INFO` & `PrimeBotFramework-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 0.0.8
+Version: 0.0.9
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Melque Lima
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
@@ -170,7 +170,11 @@
 ------------------
 0.0.7 (2022-12-13)
 - DeathByCaptcha: Alteracoes nos retornos das exceptions
 
 ------------------
 0.0.8 (2022-12-20)
 - CpfCnpj: InclusÃ£o da biblioteca
+
+------------------
+0.0.9 (2022-12-20)
+- CpfCnpj: Ajustes para importaÃ§Ã£o do model
```

### Comparing `PrimeBotFramework-0.0.8/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
-from api_codes import Package, Error
-import model
-
+from PrimeBot.CpfCnpj.model import Endereco, DadosEmpresa, Erro
+from PrimeBot.CpfCnpj.api_codes import Package, Error
 
 def set_token(token: str) -> None:
     global TOKEN
     TOKEN = token
 
 
 def consulta_cnpj(cnpj: str) -> dict:
@@ -25,35 +24,35 @@
         Error.CONTA_BLOQUEADA.value,
         Error.CREDITOS_INSUFICIENTES.value,
         Error.PACOTE_INVALIDO.value,
     ]
 
     if response_json["status"]:
         endereco = response_json["matrizEndereco"]
-        resultado = model.DadosEmpresa(
+        resultado = DadosEmpresa(
             razao_social=response_json["razao"],
             situacao=response_json["situacao"]["nome"],
-            endereco=model.Endereco(
+            endereco= Endereco(
                 logradouro=endereco["logradouro"],
                 bairro=endereco["bairro"],
                 cep=endereco["cep"],
                 cidade=endereco["cidade"],
                 uf=endereco["uf"],
             ),
         )
     elif response_json["erroCodigo"] == Error.BLACKLIST.value:
-        resultado = model.Erro(
+        resultado = Erro(
             erro=response_json["blacklist"]["motivo"],
             codigo=response_json["erroCodigo"],
         )
     elif response_json["erroCodigo"] in error_list:
-        resultado = model.Erro(
+        resultado = Erro(
             erro=response_json["erro"],
             codigo=response_json["erroCodigo"],
         )
     else:
-        resultado = model.Erro(
+        resultado = Erro(
             erro="Erro desconhecido",
             codigo=999,
         )
 
-    return resultado.dict()
+    return resultado.dict()
```

### Comparing `PrimeBotFramework-0.0.8/PrimeBot/CpfCnpj/api_codes.py` & `PrimeBotFramework-0.0.9/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-0.0.8/PrimeBot/DeathByCaptcha/__init__.py` & `PrimeBotFramework-0.0.9/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-0.0.8/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-0.0.9/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-0.0.8/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-0.0.9/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-0.0.8/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-0.0.9/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-0.0.8/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-0.0.9/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-0.0.8/PrimeBotFramework.egg-info/PKG-INFO` & `PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 0.0.8
+Version: 0.0.9
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Melque Lima
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
@@ -170,7 +170,11 @@
 ------------------
 0.0.7 (2022-12-13)
 - DeathByCaptcha: Alteracoes nos retornos das exceptions
 
 ------------------
 0.0.8 (2022-12-20)
 - CpfCnpj: InclusÃ£o da biblioteca
+
+------------------
+0.0.9 (2022-12-20)
+- CpfCnpj: Ajustes para importaÃ§Ã£o do model
```

### Comparing `PrimeBotFramework-0.0.8/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-0.0.9/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-0.0.8/README.md` & `PrimeBotFramework-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-0.0.8/setup.py` & `PrimeBotFramework-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='PrimeBotFramework',
-  version='0.0.8',
+  version='0.0.9',
   description='Um pacote de padronizacao de pacotes a serem utilizados pela Prime',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='',
   license='MIT',
```

