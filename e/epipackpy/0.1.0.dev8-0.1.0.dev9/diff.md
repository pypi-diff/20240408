# Comparing `tmp/epipackpy-0.1.0.dev8.tar.gz` & `tmp/epipackpy-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epipackpy-0.1.0.dev8.tar", last modified: Tue Mar 12 14:45:36 2024, max compression
+gzip compressed data, was "epipackpy-0.1.0.dev9.tar", last modified: Mon Apr  8 21:25:43 2024, max compression
```

## Comparing `epipackpy-0.1.0.dev8.tar` & `epipackpy-0.1.0.dev9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-03-12 14:45:36.256701 epipackpy-0.1.0.dev8/
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1081 2023-11-08 15:14:12.000000 epipackpy-0.1.0.dev8/LICENSE.txt
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1692 2024-03-12 14:45:36.252701 epipackpy-0.1.0.dev8/PKG-INFO
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      945 2023-11-16 15:12:22.000000 epipackpy-0.1.0.dev8/README.md
-drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-03-12 14:45:36.185701 epipackpy-0.1.0.dev8/epipackpy/
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      119 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev8/epipackpy/__init__.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)       26 2024-03-12 14:38:33.000000 epipackpy-0.1.0.dev8/epipackpy/_version.py
-drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-03-12 14:45:36.214701 epipackpy-0.1.0.dev8/epipackpy/data/
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)       85 2023-11-14 23:26:50.000000 epipackpy-0.1.0.dev8/epipackpy/data/__init__.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     6048 2023-11-16 21:03:13.000000 epipackpy-0.1.0.dev8/epipackpy/data/dataload.py
-drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-03-12 14:45:36.246701 epipackpy-0.1.0.dev8/epipackpy/model/
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      269 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev8/epipackpy/model/__init__.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)    17394 2024-03-12 14:22:47.000000 epipackpy-0.1.0.dev8/epipackpy/model/bridge_model.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     8118 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev8/epipackpy/model/classifier.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     4510 2023-11-10 20:07:34.000000 epipackpy-0.1.0.dev8/epipackpy/model/classifier_oor.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)    10964 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev8/epipackpy/model/loss.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)    26486 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev8/epipackpy/model/net.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     6592 2023-11-10 20:05:16.000000 epipackpy-0.1.0.dev8/epipackpy/model/peak_model.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1779 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev8/epipackpy/model/utils.py
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)    19055 2023-11-10 20:07:06.000000 epipackpy-0.1.0.dev8/epipackpy/model/vae_online.py
-drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-03-12 14:45:36.208701 epipackpy-0.1.0.dev8/epipackpy.egg-info/
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1692 2024-03-12 14:45:36.000000 epipackpy-0.1.0.dev8/epipackpy.egg-info/PKG-INFO
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      580 2024-03-12 14:45:36.000000 epipackpy-0.1.0.dev8/epipackpy.egg-info/SOURCES.txt
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)        1 2024-03-12 14:45:36.000000 epipackpy-0.1.0.dev8/epipackpy.egg-info/dependency_links.txt
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)        1 2024-03-12 14:45:36.000000 epipackpy-0.1.0.dev8/epipackpy.egg-info/not-zip-safe
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      196 2024-03-12 14:45:36.000000 epipackpy-0.1.0.dev8/epipackpy.egg-info/requires.txt
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)       10 2024-03-12 14:45:36.000000 epipackpy-0.1.0.dev8/epipackpy.egg-info/top_level.txt
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)       38 2024-03-12 14:45:36.256701 epipackpy-0.1.0.dev8/setup.cfg
--rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1243 2023-11-14 23:32:13.000000 epipackpy-0.1.0.dev8/setup.py
+drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-04-08 21:25:43.293934 epipackpy-0.1.0.dev9/
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1081 2023-11-08 15:14:12.000000 epipackpy-0.1.0.dev9/LICENSE.txt
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1692 2024-04-08 21:25:43.292934 epipackpy-0.1.0.dev9/PKG-INFO
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      945 2023-11-16 15:12:22.000000 epipackpy-0.1.0.dev9/README.md
+drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-04-08 21:25:43.266934 epipackpy-0.1.0.dev9/epipackpy/
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      119 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev9/epipackpy/__init__.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)       26 2024-04-08 21:24:40.000000 epipackpy-0.1.0.dev9/epipackpy/_version.py
+drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-04-08 21:25:43.279934 epipackpy-0.1.0.dev9/epipackpy/data/
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)       85 2023-11-14 23:26:50.000000 epipackpy-0.1.0.dev9/epipackpy/data/__init__.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     6048 2023-11-16 21:03:13.000000 epipackpy-0.1.0.dev9/epipackpy/data/dataload.py
+drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-04-08 21:25:43.290934 epipackpy-0.1.0.dev9/epipackpy/model/
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      269 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev9/epipackpy/model/__init__.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)    17394 2024-03-12 14:22:47.000000 epipackpy-0.1.0.dev9/epipackpy/model/bridge_model.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     8975 2024-04-08 21:19:34.000000 epipackpy-0.1.0.dev9/epipackpy/model/classifier.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     4510 2023-11-10 20:07:34.000000 epipackpy-0.1.0.dev9/epipackpy/model/classifier_oor.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)    10964 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev9/epipackpy/model/loss.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)    27702 2024-04-08 21:19:35.000000 epipackpy-0.1.0.dev9/epipackpy/model/net.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     6667 2024-03-12 20:50:28.000000 epipackpy-0.1.0.dev9/epipackpy/model/peak_model.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1779 2023-11-08 15:51:45.000000 epipackpy-0.1.0.dev9/epipackpy/model/utils.py
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)    19055 2023-11-10 20:07:06.000000 epipackpy-0.1.0.dev9/epipackpy/model/vae_online.py
+drwxr-xr-x   0 ycheng430 (3173705) gtperson  (2626)        0 2024-04-08 21:25:43.276934 epipackpy-0.1.0.dev9/epipackpy.egg-info/
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1692 2024-04-08 21:25:43.000000 epipackpy-0.1.0.dev9/epipackpy.egg-info/PKG-INFO
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      580 2024-04-08 21:25:43.000000 epipackpy-0.1.0.dev9/epipackpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)        1 2024-04-08 21:25:43.000000 epipackpy-0.1.0.dev9/epipackpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)        1 2024-04-08 21:25:43.000000 epipackpy-0.1.0.dev9/epipackpy.egg-info/not-zip-safe
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)      196 2024-04-08 21:25:43.000000 epipackpy-0.1.0.dev9/epipackpy.egg-info/requires.txt
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)       10 2024-04-08 21:25:43.000000 epipackpy-0.1.0.dev9/epipackpy.egg-info/top_level.txt
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)       38 2024-04-08 21:25:43.294934 epipackpy-0.1.0.dev9/setup.cfg
+-rw-r--r--   0 ycheng430 (3173705) gtperson  (2626)     1243 2023-11-14 23:32:13.000000 epipackpy-0.1.0.dev9/setup.py
```

### Comparing `epipackpy-0.1.0.dev8/LICENSE.txt` & `epipackpy-0.1.0.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/PKG-INFO` & `epipackpy-0.1.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epipackpy
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: EpiPack: scATAC-seq integration, reference mapping and cell type annotation
 Home-page: https://github.com/ZhangLabGT/EpiPack
 Author: Yuqi Cheng
 Author-email: ycheng430@gatech.edu
 License: MIT
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `epipackpy-0.1.0.dev8/README.md` & `epipackpy-0.1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/epipackpy/data/dataload.py` & `epipackpy-0.1.0.dev9/epipackpy/data/dataload.py`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/epipackpy/model/bridge_model.py` & `epipackpy-0.1.0.dev9/epipackpy/model/bridge_model.py`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/epipackpy/model/classifier.py` & `epipackpy-0.1.0.dev9/epipackpy/model/classifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import pandas as pd
 import numpy as np
 import torch
 from torch.utils.data import Dataset, DataLoader
 import torch.nn as nn
 from typing import Literal
 from tqdm import tqdm
-from .net import classifier_layer, CosCell, InnerCos, InnerCosLoss, CenterLoss
+from .net import classifier_layer, CosCell, ArcCell, CenterLoss
 from sklearn.model_selection import train_test_split
 import torch.nn.functional as F
-from .loss import contrastive_loss
-from .utils import cosine_dist
+import torch.utils.data as Data
 
 
 class classifier_dataset(Dataset):
     def __init__(self, ref_emb, ref_label = None, train=None):
         
         #check promoter/enhancer matrix
         assert not len(ref_emb) == 0, "Lack of the enhancer matrix"
@@ -35,36 +34,36 @@
 
 
 
 class Classifier(nn.Module):
     def __init__(self, 
                  ref_latent_emb,  
                  ref_label,
-                 class_num,
                  hidden_num,
                  z_dim: int = 30,  
                  dropout_rate: float = 0.1,
                  layer_num: int = 1, 
                  batch_size: int = 128, 
                  batchnorm: bool = True,
                  device: Literal['auto','gpu','cpu'] = 'auto'):
 
         super(Classifier, self).__init__()
  
         self.ref_latent_emb = ref_latent_emb
         self.ref_label = ref_label
-        self.class_num = class_num
         self.hidden_num = hidden_num
         self.batch_size = batch_size
         self.layer_num = layer_num
         self.dropout_rate = dropout_rate
         self.z_dim = z_dim
         self.device = device
         self.batchnorm = batchnorm
 
+        self.class_num = len(np.unique(self.ref_label))
+
         print("- Classifier initializing...")
 
         assert self.ref_latent_emb.shape[0] == len(self.ref_label), "Reference label set has different cell numbers with reference embedding."
 
         #model initialization
         if self.device == 'auto':
             self.device_use = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
@@ -86,115 +85,132 @@
             n_output = self.z_dim, 
             n_hidden = self.hidden_num,
             dropout_rate= self.dropout_rate,
             use_layer_norm = False,
             use_batch_norm = self.batchnorm
             ).to(self.device_use)
 
-        #self.Coscell = CosCell(self.z_dim, self.class_num).to(self.device_use)
+        self.Coscell = CosCell(self.z_dim, self.class_num).to(self.device_use)
+        #self.Coscell = ArcCell(self.z_dim, self.class_num).to(self.device_use)
         #self.Coscell = nn.Linear(self.z_dim, self.class_num).to(self.device_use)
 
         self.class_mu = []
         for i in np.unique(self.ref_label):
             mu_class = self.ref_latent_emb[np.where(self.ref_label==i)]
             self.class_mu.append(np.mean(mu_class, axis=0).tolist())
 
         self.class_mu = np.array(self.class_mu)
     
         ## split train test
         #X_train, X_test, y_train, y_test = train_test_split(self.ref_latent_emb, self.ref_label, test_size = 0.2, stratify=self.ref_label)
         self.train_dataset = classifier_dataset(self.ref_latent_emb, self.ref_label, train=True)
         #self.test_dataset = classifier_dataset(X_test, y_test, train=False)
-        self.train_loader = DataLoader(dataset = self.train_dataset, batch_size = self.batch_size, shuffle = True)
+
+        ## balancing
+        class_sample_count = torch.tensor([(self.ref_label == t).sum() for t in np.unique(self.ref_label)])
+
+        weight = 1. / class_sample_count.float()
+        samples_weight = torch.tensor([weight[t] for t in self.ref_label])
+        samplr = Data.WeightedRandomSampler(samples_weight, len(samples_weight))
+
+        self.train_loader = DataLoader(dataset = self.train_dataset, batch_size = self.batch_size, sampler = samplr)
         #self.test_loader = DataLoader(dataset=self.test_dataset, batch_size=len(self.test_dataset), shuffle=False)
 
         print("- Classifier intialization completed.")
     
     def inference(self, x):
 
         out = self.Encoder(x)
-        #z = self.Coscell(out)
+        z = self.Coscell(out)
         
-        return{"cls_latent": out}
+        return{"cls_latent": out, "class_z": z}
             
     
     def train_model(self, 
                     nepochs:int = 50, 
                     weight_decay:float = 5e-4, 
                     learning_rate:float = 1e-4,
-                    #inner_reg:float = 1,
-                    optim: Literal = ['Adam', 'SGD']):
+                    inner_reg:float = 1):
+                    #optim: Literal = ['Adam', 'SGD']):
         
         self.train()
         
-        #criterion = torch.nn.CrossEntropyLoss().to(self.device_use)
-        #self.criterion_inner = CenterLoss(self.class_num, self.z_dim).to(self.device_use)
+        criterion = torch.nn.CrossEntropyLoss().to(self.device_use)
+        self.criterion_inner = CenterLoss(self.class_num, self.z_dim, center_init=self.class_mu, device=self.device_use).to(self.device_use)
 
         #optimizer_main = torch.optim.Adam(self.Encoder.parameters(), lr=learning_rate, weight_decay=weight_decay)
         #optimizer_inter = torch.optim.Adam(self.Coscell.parameters(), lr=learning_rate, weight_decay=weight_decay)
-        if optim == 'Adam':
-            self.optimizer = torch.optim.Adam(self.Encoder.parameters(),
+        
+        #if optim == 'Adam':
+        self.optimizer = torch.optim.Adam([{'params': self.Encoder.parameters()}, {'params': self.Coscell.parameters()}],
                                 lr=learning_rate,
                                 weight_decay=weight_decay)
-            #self.optimizer_inner  = torch.optim.Adam(self.criterion_inner.parameters(),
-            #                    lr=learning_rate,
-            #                    weight_decay=weight_decay)
-        elif optim == 'SGD':
-            self.optimizer = torch.optim.SGD([{'params': self.Encoder.parameters()}, {'params': self.Coscell.parameters()}],
+        self.optimizer_inner  = torch.optim.Adam(self.criterion_inner.parameters(),
                                 lr=learning_rate,
-                                momentum=0.9,
                                 weight_decay=weight_decay)
-            #self.optimizer_inner  = torch.optim.SGD(self.criterion_inner.parameters(),
-            #                    lr=learning_rate,
-            #                    momentum=0.9,
-            #                    weight_decay=weight_decay)
+        #elif optim == 'SGD':
+        #    self.optimizer = torch.optim.SGD([{'params': self.Encoder.parameters()}, {'params': self.Coscell.parameters()}],
+        #                        lr=learning_rate,
+        #                        momentum=0.9,
+        #                        weight_decay=weight_decay)
+        #    self.optimizer_inner  = torch.optim.SGD(self.criterion_inner.parameters(),
+        #                        lr=learning_rate,
+        #                        momentum=0.9,
+        #                        weight_decay=weight_decay)
 
         loop = tqdm(range(nepochs), total=nepochs, desc="Epochs")
+        
         for epoch in loop:
             for id, x in enumerate(self.train_loader):
                 
                 dict_inf = self.inference(x['ref_emb'].to(self.device_use))
 
-                loss = contrastive_loss(dict_inf['cls_latent'], x["ref_label"].long().to(self.device_use))
-                #loss_inner = self.criterion_inner(dict_inf['cls_latent'], x["ref_label"].long().to(self.device_use))
-                #loss_inner = inner_reg
+                #loss = contrastive_loss(dict_inf['cls_latent'], x["ref_label"].long().to(self.device_use))
+                loss_inner = self.criterion_inner(dict_inf['cls_latent'], x["ref_label"].long().to(self.device_use))
+                loss_inter = criterion(dict_inf['class_z'], x["ref_label"].long().to(self.device_use))
 
-                #loss = loss_inter + inner_reg*loss_inner
+                loss = loss_inter + inner_reg*loss_inner
 
                 # Backward and optimize
                 self.optimizer.zero_grad()
-                #self.optimizer_inner.zero_grad()
+                self.optimizer_inner.zero_grad()
                 loss.backward()
                 nn.utils.clip_grad_norm_(self.parameters(), 10)
                 self.optimizer.step()
 
                 #for param in self.criterion_inner.parameters():
                 #    param.grad.data *= (1. / inner_reg)
 
-                #self.optimizer_inner.step()
+                self.optimizer_inner.step()
 
                 #if id == (interval_num-1):
                 #    print("epoch:{}/{}, train_bce:{}".format(epoch, nepochs, loss))
 
             #test
             #with torch.no_grad():
             #    for id, x in enumerate(self.test_loader):
 
             #        dict_inf = self.inference(x['ref_emb'].to(self.device_use))
-            #        loss_test= criterion(dict_inf['logit'], x["ref_label"].long().to(self.device_use))
+            #        loss_inner_test = self.criterion_inner(dict_inf['cls_latent'], x["ref_label"].long().to(self.device_use))
+            #        loss_inter_test = criterion(dict_inf['class_z'], x["ref_label"].long().to(self.device_use))
 
-            #loop.set_postfix(loss_inter = loss_inter.item(), loss_inner = loss_inner.item())
-            loop.set_postfix(loss_inter = loss.item())
+            loop.set_postfix(loss_inter_val = loss_inter.item(), loss_inner_val = loss_inner.item())
+            #loop.set_postfix(loss_inter = loss.item())
 
         
     def get_z(self, input):
         self.eval()
         z_latent = self.inference(torch.FloatTensor(input).to(self.device_use))
 
-        return z_latent
+        temp = F.softmax(z_latent['class_z'], dim=1)
+        pred = torch.argmax(temp, dim=1).cpu()
+
+        result = list(pred.numpy()) 
+
+        return result, z_latent['cls_latent']
     
     #def get_dis(self, input):
     #    query_emb = torch.FloatTensor(input).to(self.device_use)
     #    ctrs = self.criterion_inner.get_centers()
     #
     #    cos_diff = cosine_dist(query_emb, ctrs)
     #
```

### Comparing `epipackpy-0.1.0.dev8/epipackpy/model/classifier_oor.py` & `epipackpy-0.1.0.dev9/epipackpy/model/classifier_oor.py`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/epipackpy/model/loss.py` & `epipackpy-0.1.0.dev9/epipackpy/model/loss.py`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/epipackpy/model/net.py` & `epipackpy-0.1.0.dev9/epipackpy/model/net.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable
 import torch
 from torch import nn as nn
 import collections
 import torch.nn.functional as F
 from .utils import cosine_dist
+import math
 
 def identity(x):
     return x
 
 def one_hot(index: torch.Tensor, n_cat: int) -> torch.Tensor:
     """One hot a tensor of categories."""
     onehot = torch.zeros(index.size(0), n_cat, device=index.device)
@@ -408,15 +409,15 @@
 
     def __init__(
         self,
         n_input: int,
         n_output: int,
         n_cat_list: Iterable[int] = None,
         n_layers: int = 1,
-        n_hidden: int = 50,
+        n_hidden: int = 64,
         dropout_rate: float = 0.1,
         inject_covariates: bool = False,
         use_batch_norm: bool = False,
         use_layer_norm: bool = False
     ):
         super().__init__()
 
@@ -428,15 +429,15 @@
             n_hidden=n_hidden,
             dropout_rate=dropout_rate,
             inject_covariates=inject_covariates,
             use_batch_norm=use_batch_norm,
             use_layer_norm=use_layer_norm,
             use_activation=True,
             bias=True,
-            activation_fn=nn.LeakyReLU,
+            activation_fn=nn.ReLU,
         )
 
         self.mean_layer = nn.Linear(n_hidden, n_output)
 
 
     def forward(self, x: torch.Tensor, *cat_list: int):
         """
@@ -487,14 +488,55 @@
 
 
     def forward(self, input):
         cosine = F.linear(F.normalize(input), F.normalize(self.weight))
         output = self.s * cosine
 
         return output
+
+class ArcCell(nn.Module):
+    r"""Implement of large margin arc distance: :
+        Args:
+            in_features: size of each input sample
+            out_features: size of each output sample
+            s: norm of input feature
+            m: margin
+
+            cos(theta + m)
+        """
+    def __init__(self, in_features, out_features, s=30.0, m=0.50):
+        super(ArcCell, self).__init__()
+        self.in_features = in_features
+        self.out_features = out_features
+        self.s = s
+        self.m = m
+        self.weight = nn.Parameter(torch.FloatTensor(out_features, in_features))
+        nn.init.xavier_uniform_(self.weight)
+
+        self.cos_m = math.cos(m)
+        self.sin_m = math.sin(m)
+        self.th = math.cos(math.pi - m)
+        self.mm = math.sin(math.pi - m) * m
+
+    def forward(self, input, label, device):
+        # --------------------------- cos(theta) & phi(theta) ---------------------------
+        cosine = F.linear(F.normalize(input), F.normalize(self.weight))
+        sine = torch.sqrt((1.0 - torch.pow(cosine, 2)).clamp(0, 1))
+        phi = cosine * self.cos_m - sine * self.sin_m
+
+        phi = torch.where(cosine > self.th, phi, cosine - self.mm)
+        # --------------------------- convert label to one-hot ---------------------------
+        # one_hot = torch.zeros(cosine.size(), requires_grad=True, device='cuda')
+        one_hot = torch.zeros(cosine.size(), device=device)
+        one_hot.scatter_(1, label.view(-1, 1).long(), 1)
+        # -------------torch.where(out_i = {x_i if condition_i else y_i) -------------
+        output = (one_hot * phi) + ((1.0 - one_hot) * cosine)  # you can use torch.where if your torch.__version__ is 0.4
+        output *= self.s
+
+        return output
     
 class InnerCos(nn.Module):
 
     def __init__(self, in_feature, n_class):
         super(InnerCos, self).__init__()
         self.in_feature = in_feature
         self.n_class = n_class
@@ -546,52 +588,43 @@
     Reference:
     Wen et al. A Discriminative Feature Learning Approach for Deep Face Recognition. ECCV 2016.
     
     Args:
         num_classes (int): number of classes.
         feat_dim (int): feature dimension.
     """
-    def __init__(self, num_classes=10, feat_dim=2, center_init=None):
+    def __init__(self, num_classes=10, feat_dim=2, center_init=None, device=None):
         super(CenterLoss, self).__init__()
         self.num_classes = num_classes
         self.feat_dim = feat_dim
+        self.device = device
 
         self.centers = nn.Parameter(torch.zeros(self.num_classes, self.feat_dim), requires_grad=True)
-        self.centers.data = torch.from_numpy(center_init).float()
+        #self.centers.data = torch.from_numpy(center_init).float()
 
     def forward(self, x, labels):
         """
         Args:
             x: feature matrix with shape (batch_size, feat_dim).
             labels: ground truth labels with shape (batch_size).
         """
-        batch_size = x.size(0)
 
-        ##inner
+        batch_size = x.size(0)
         distmat = torch.pow(x, 2).sum(dim=1, keepdim=True).expand(batch_size, self.num_classes) + \
                   torch.pow(self.centers, 2).sum(dim=1, keepdim=True).expand(self.num_classes, batch_size).t()
-        distmat.addmm_(self.centers, self.centers.t(), beta=1, alpha=-2)
-        
-        ##center
-        distmat = torch.pow(self.centers, 2).sum(dim=1, keepdim=True).expand(batch_size, self.num_classes) + \
-                  torch.pow(self.centers, 2).sum(dim=1, keepdim=True).expand(self.num_classes, batch_size).t()
-        distmat.addmm_(self.centers, self.centers.t(), beta=1, alpha=-2)
+        distmat.addmm_(x, self.centers.t(), beta=1, alpha=-2)
 
-        classes = torch.arange(self.num_classes).long()
+        classes = torch.arange(self.num_classes).long().to(self.device)
         labels = labels.unsqueeze(1).expand(batch_size, self.num_classes)
-        mask_in = labels.eq(classes.expand(batch_size, self.num_classes))
-        mask_out = labels.ne(classes.expand(batch_size, self.num_classes))
+        mask = labels.eq(classes.expand(batch_size, self.num_classes))
 
-        dist_in = distmat * mask_in.float()
-        loss_inner = dist_in.clamp(min=1e-12, max=1e+12).sum() / batch_size
-        
-        dist_out = distmat * mask_out.float()
-        loss_inter = dist_out.clamp(min=1e-12, max=1e+12).sum() / batch_size
+        dist = distmat * mask.float()
+        loss = dist.clamp(min=1e-12, max=1e+12).sum() / batch_size
 
-        return loss_inner, loss_inter
+        return loss
     
 ######################################
 #         Decoder materials          #
 ###################################### 
 
 # Decoder poisson test
 class DecoderPoissonVAE(nn.Module):
```

### Comparing `epipackpy-0.1.0.dev8/epipackpy/model/peak_model.py` & `epipackpy-0.1.0.dev9/epipackpy/model/peak_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,29 @@
                  layer_num: int = 2, 
                  batch_size: int = 512, 
                  hidden_dim: int = 256, 
                  dropout_rate: float = 0.1, 
                  z_dim: int = 50, 
                  device: Literal['auto','gpu','cpu'] = 'auto',
                  lib_size: bool = True,
-                 region_factor: bool = False):
+                 region_factor: bool = False,
+                 denosing: bool = False):
 
         super(Peak_Model, self).__init__()
  
         self.enhancer_count = count_enhancer
         self.batch_size = batch_size
         self.hidden_dim = hidden_dim
         self.layer_num = layer_num
         self.dropout_rate = dropout_rate
         self.z_dim = z_dim
         self.device = device
         self.lib_size = lib_size
         self.region_factor = region_factor
+        self.denoising = denosing
 
         print("- Model initializing...")
 
         #model initialization
         if self.device == 'auto':
             self.device_use = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
             if torch.cuda.is_available():
```

### Comparing `epipackpy-0.1.0.dev8/epipackpy/model/utils.py` & `epipackpy-0.1.0.dev9/epipackpy/model/utils.py`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/epipackpy/model/vae_online.py` & `epipackpy-0.1.0.dev9/epipackpy/model/vae_online.py`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/epipackpy.egg-info/PKG-INFO` & `epipackpy-0.1.0.dev9/epipackpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epipackpy
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: EpiPack: scATAC-seq integration, reference mapping and cell type annotation
 Home-page: https://github.com/ZhangLabGT/EpiPack
 Author: Yuqi Cheng
 Author-email: ycheng430@gatech.edu
 License: MIT
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `epipackpy-0.1.0.dev8/epipackpy.egg-info/SOURCES.txt` & `epipackpy-0.1.0.dev9/epipackpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epipackpy-0.1.0.dev8/setup.py` & `epipackpy-0.1.0.dev9/setup.py`

 * *Files identical despite different names*

