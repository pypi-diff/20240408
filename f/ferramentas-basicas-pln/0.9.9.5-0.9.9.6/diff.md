# Comparing `tmp/ferramentas-basicas-pln-0.9.9.5.tar.gz` & `tmp/ferramentas-basicas-pln-0.9.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferramentas-basicas-pln-0.9.9.5.tar", last modified: Sun Apr  7 02:06:19 2024, max compression
+gzip compressed data, was "ferramentas-basicas-pln-0.9.9.6.tar", last modified: Sun Apr  7 02:07:08 2024, max compression
```

## Comparing `ferramentas-basicas-pln-0.9.9.5.tar` & `ferramentas-basicas-pln-0.9.9.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 02:06:19.418626 ferramentas-basicas-pln-0.9.9.5/
--rw-rw-rw-   0        0        0    13948 2024-04-07 02:06:19.417625 ferramentas-basicas-pln-0.9.9.5/PKG-INFO
--rw-rw-rw-   0        0        0    13600 2024-04-04 00:37:59.000000 ferramentas-basicas-pln-0.9.9.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 02:06:19.412620 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln/
--rw-rw-rw-   0        0        0     1039 2024-04-04 00:37:19.000000 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln/__init__.py
--rw-rw-rw-   0        0        0    43914 2024-04-07 02:05:22.000000 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln/main.py
-drwxrwxrwx   0        0        0        0 2024-04-07 02:06:19.417625 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln.egg-info/
--rw-rw-rw-   0        0        0    13948 2024-04-07 02:06:19.000000 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-07 02:06:19.000000 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 02:06:19.000000 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-07 02:06:19.000000 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-07 02:06:19.000000 ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 02:06:19.419628 ferramentas-basicas-pln-0.9.9.5/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-04-07 02:04:34.000000 ferramentas-basicas-pln-0.9.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:07:08.171494 ferramentas-basicas-pln-0.9.9.6/
+-rw-rw-rw-   0        0        0    13948 2024-04-07 02:07:08.170493 ferramentas-basicas-pln-0.9.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0    13600 2024-04-04 00:37:59.000000 ferramentas-basicas-pln-0.9.9.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 02:07:08.163910 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln/
+-rw-rw-rw-   0        0        0     1032 2024-04-07 02:06:59.000000 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln/__init__.py
+-rw-rw-rw-   0        0        0    43914 2024-04-07 02:05:22.000000 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln/main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:07:08.169491 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln.egg-info/
+-rw-rw-rw-   0        0        0    13948 2024-04-07 02:07:08.000000 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-07 02:07:08.000000 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 02:07:08.000000 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-07 02:07:08.000000 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-07 02:07:08.000000 ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 02:07:08.171494 ferramentas-basicas-pln-0.9.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-04-07 02:06:43.000000 ferramentas-basicas-pln-0.9.9.6/setup.py
```

### Comparing `ferramentas-basicas-pln-0.9.9.5/PKG-INFO` & `ferramentas-basicas-pln-0.9.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferramentas-basicas-pln
-Version: 0.9.9.5
+Version: 0.9.9.6
 Summary: Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.
 Author: Igor Caetano de Souza
 Project-URL: GitHub Repository, https://github.com/IgorCaetano/ferramentas_basicas_pln
 Description-Content-Type: text/markdown
 Requires-Dist: regex
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.5 Summary:
+Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.6 Summary:
 Kit de ferramentas para processos bÃ¡sicos de Processamento de Linguagem
 Natural. Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
 github.com/IgorCaetano/ferramentas_basicas_pln Description-Content-Type: text/
 markdown Requires-Dist: regex # Ferramentas bÃ¡sicas para Processamento de
 Linguagem Natural Este pacote Ã© um kit de ferramentas (variadas funÃ§Ãµes)
 para execuÃ§Ã£o de processos bÃ¡sicos relacionados as etapas iniciais de
 processamento de linguagem natural. VVeerrss?Ã?£oo eemm iinnggll?Ã?ªss ((cclliiqquuee ppaarraa eexxppaannddiirr))
```

### Comparing `ferramentas-basicas-pln-0.9.9.5/README.md` & `ferramentas-basicas-pln-0.9.9.6/README.md`

 * *Files identical despite different names*

### Comparing `ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln/__init__.py` & `ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 from .main import STRING_CARACTERES_ESPECIAIS_PADRAO,CARACTERES_NORMAIS
 from .main import LISTA_STOPWORDS_PADRAO_FREQUENCIA,LISTA_STOPWORDS_PADRAO_TOKENIZACAO,LISTA_PONTOS_FINAIS_PADRAO_FRASES,DICIONARIO_CONFIG_PADRAO_TOKENIZACAO
 from .main import DIGITO_DIA,DIGITO_MES,DIGITO_ANO,PADRAO_REGEX_DATA
 from .main import DDD_PAIS, DDD_ESTADO, DDD_CELULAR, PADRAO_REGEX_TELEFONE_CELULAR
 from .main import PADRAO_REGEX_EMAIL,PADRAO_REGEX_LINKS, PADRAO_REGEX_NUMEROS,PADRAO_REGEX_DINHEIRO,PADRAO_REGEX_CPF,PADRAO_REGEX_CEP,PADRAO_REGEX_RG
 from .main import padronizarRG,padronizarCPF,padronizarCEP,padronizarDatas,padronizarDinheiros,padronizarEmails,padronizarLinks,padronizarNumeros,normalizarTexto,padronizarTelefoneCelular,padronizarTextoParaMinuscula
-from .main import coletarTextoDeArquivoTxt,removerCaracteresEspeciais,removerCaracteresMaisQueEspeciais,removerEspacosEmBrancoExtras,transformarTextoSubstituindoCaracteres,verificarExistenciaDeElemento,contarFrequenciaDePalavras,formatarTexto,tokenizarTexto,organizaTextoPelasLinhas
+from .main import coletarTextoDeArquivoTxt,removerCaracteresEspeciais,removerCaracteresEstranhos,removerEspacosEmBrancoExtras,transformarTextoSubstituindoCaracteres,verificarExistenciaDeElemento,contarFrequenciaDePalavras,formatarTexto,tokenizarTexto,organizaTextoPelasLinhas
```

### Comparing `ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln/main.py` & `ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln/main.py`

 * *Files identical despite different names*

### Comparing `ferramentas-basicas-pln-0.9.9.5/ferramentas_basicas_pln.egg-info/PKG-INFO` & `ferramentas-basicas-pln-0.9.9.6/ferramentas_basicas_pln.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferramentas-basicas-pln
-Version: 0.9.9.5
+Version: 0.9.9.6
 Summary: Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.
 Author: Igor Caetano de Souza
 Project-URL: GitHub Repository, https://github.com/IgorCaetano/ferramentas_basicas_pln
 Description-Content-Type: text/markdown
 Requires-Dist: regex
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.5 Summary:
+Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.6 Summary:
 Kit de ferramentas para processos bÃ¡sicos de Processamento de Linguagem
 Natural. Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
 github.com/IgorCaetano/ferramentas_basicas_pln Description-Content-Type: text/
 markdown Requires-Dist: regex # Ferramentas bÃ¡sicas para Processamento de
 Linguagem Natural Este pacote Ã© um kit de ferramentas (variadas funÃ§Ãµes)
 para execuÃ§Ã£o de processos bÃ¡sicos relacionados as etapas iniciais de
 processamento de linguagem natural. VVeerrss?Ã?£oo eemm iinnggll?Ã?ªss ((cclliiqquuee ppaarraa eexxppaannddiirr))
```

### Comparing `ferramentas-basicas-pln-0.9.9.5/setup.py` & `ferramentas-basicas-pln-0.9.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open(r'README.md','r',encoding='utf-8') as f:
     descricao_longa = f.read()
 
 setup(
     name='ferramentas-basicas-pln',
-    version='0.9.9.5',
+    version='0.9.9.6',
     packages=find_packages(),
     install_requires = ['regex'],
     description='Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.',
     long_description=descricao_longa,
     long_description_content_type="text/markdown",
     author='Igor Caetano de Souza',
     project_urls={
```

