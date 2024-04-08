# Comparing `tmp/isne_recommendation-0.1.2.tar.gz` & `tmp/isne_recommendation-0.1.3.tar.gz`

## Comparing `isne_recommendation-0.1.2.tar` & `isne_recommendation-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/.dockerignore
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/Dockerfile
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/app.py
--rw-r--r--   0        0        0    30262 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/cleandata.ipynb
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/get_courses.py
--rw-r--r--   0        0        0    19403 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/hybrid.ipynb
--rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/hybrid.py
--rw-r--r--   0        0        0    31234 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/knn.ipynb
--rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/knn.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/requirements.txt
--rw-r--r--   0        0        0    14206 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/test.ipynb
--rw-r--r--   0        0        0    19188 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/tfidf.ipynb
--rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/tfidf.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/pickle/i_dataset.pickle
--rw-r--r--   0        0        0  1847202 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/pickle/tfidf_X.pickle
--rw-r--r--   0        0        0    97646 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/pickle/tfidf_matrix.pickle
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/pickle/tfidf_y.pickle
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/pickle/ui_dataset.pickle
--rw-r--r--   0        0        0    10179 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/src/isne_recommendation/FeatureRatingsKNN.py
--rw-r--r--   0        0        0    11276 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/src/isne_recommendation/Hybrid.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/src/isne_recommendation/TfidfLinearKernel.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/src/isne_recommendation/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/templates/homepage.html
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/templates/predata.html
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/templates/recommendation.html
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/LICENSE
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/README.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 isne_recommendation-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/.dockerignore
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/Dockerfile
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/app.py
+-rw-r--r--   0        0        0    30262 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/cleandata.ipynb
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/get_courses.py
+-rw-r--r--   0        0        0    19403 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/hybrid.ipynb
+-rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/hybrid.py
+-rw-r--r--   0        0        0    31234 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/knn.ipynb
+-rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/knn.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/requirements.txt
+-rw-r--r--   0        0        0    13781 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/test.ipynb
+-rw-r--r--   0        0        0    19188 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/tfidf.ipynb
+-rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/tfidf.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/pickle/i_dataset.pickle
+-rw-r--r--   0        0        0  1847202 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/pickle/tfidf_X.pickle
+-rw-r--r--   0        0        0    97646 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/pickle/tfidf_matrix.pickle
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/pickle/tfidf_y.pickle
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/pickle/ui_dataset.pickle
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/src/isne_recommendation/FeatureRatingsKNN.py
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/src/isne_recommendation/Hybrid.py
+-rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/src/isne_recommendation/TfidfLinearKernel.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/src/isne_recommendation/__init__.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/templates/homepage.html
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/templates/predata.html
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/templates/recommendation.html
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 isne_recommendation-0.1.3/PKG-INFO
```

### Comparing `isne_recommendation-0.1.2/.dockerignore` & `isne_recommendation-0.1.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/Dockerfile` & `isne_recommendation-0.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/app.py` & `isne_recommendation-0.1.3/app.py`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/cleandata.ipynb` & `isne_recommendation-0.1.3/cleandata.ipynb`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/get_courses.py` & `isne_recommendation-0.1.3/get_courses.py`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/hybrid.ipynb` & `isne_recommendation-0.1.3/hybrid.ipynb`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/hybrid.py` & `isne_recommendation-0.1.3/hybrid.py`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/knn.ipynb` & `isne_recommendation-0.1.3/knn.ipynb`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/knn.py` & `isne_recommendation-0.1.3/knn.py`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/test.ipynb` & `isne_recommendation-0.1.3/test.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9709635416666667%*

 * *Differences: {"'cells'": "{1: {'source': ['import pandas as pd\\n', 'from src.isne_recommendation import "*

 * *            "TfidfLinearKernel, FeatureRatingsKNN, Hybrid']}, 5: {'execution_count': 3, 'outputs': "*

 * *            "{0: {'execution_count': 3}}}, 6: {'execution_count': 4, 'source': ['train, test = "*

 * *            "TfidfLinearKernel.train_test_split(ui_data, test_size=0.25)']}, 7: "*

 * *            "{'execution_count': 5, 'outputs': {0: {'execution_count': 5}}}, 8: "*

 * *            "{'execution_count': 6, 'outputs': {0: {'exe […]*

```diff
@@ -9,15 +9,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pandas as pd"
+                "import pandas as pd\n",
+                "from src.isne_recommendation import TfidfLinearKernel, FeatureRatingsKNN, Hybrid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Read datasets"
@@ -40,23 +41,14 @@
                 "# Evaluation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
-            "outputs": [],
-            "source": [
-                "from src.isne_recommendation import TfidfLinearKernel"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
@@ -144,88 +136,79 @@
                             "52  Medical Applications of Particle Accelerators ...  0.185854\n",
                             "31  Foundations of Public Health Practice: Behavio...  0.175814\n",
                             "3                            Biomedical Visualisation  0.170230\n",
                             "8                        COVID-19 - A clinical update  0.168129\n",
                             "40       Health Care IT: Challenges and Opportunities  0.166725"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model = TfidfLinearKernel.fit(i_data)\n",
                 "prediction = TfidfLinearKernel.predict('Martha Long', i_data, ui_data, model, 10)\n",
                 "prediction"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
-                "train, test = TfidfLinearKernel.train_test_split(ui_data, test_size=0.2)"
+                "train, test = TfidfLinearKernel.train_test_split(ui_data, test_size=0.25)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.1469440832249675"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "hit_rate = TfidfLinearKernel.hit_rate(train, test, i_data, model)\n",
                 "hit_rate"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.02578870900788709"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "f1_score = TfidfLinearKernel.f1_score(train, test, i_data, model)\n",
                 "f1_score"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from src.isne_recommendation import FeatureRatingsKNN"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -265,89 +248,80 @@
                             "                                              Course  Cosine Distance  \\\n",
                             "0  Addiction Treatment: Clinical Skills for Healt...         0.670731   \n",
                             "\n",
                             "      Score  \n",
                             "0  0.329269  "
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model = FeatureRatingsKNN.fit(ui_data)\n",
                 "prediction = FeatureRatingsKNN.predict('Martha Long', ui_data, model, 10)\n",
                 "prediction"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
-                "train, test = FeatureRatingsKNN.train_test_split(ui_data, test_size=0.2)\n",
+                "train, test = FeatureRatingsKNN.train_test_split(ui_data, test_size=0.25)\n",
                 "model = FeatureRatingsKNN.fit(train)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.48244473342002603"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "hit_rate = FeatureRatingsKNN.hit_rate(train, test, model)\n",
                 "hit_rate"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.07923412204234122"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "f1_score = FeatureRatingsKNN.f1_score(train, test, model)\n",
                 "f1_score"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from src.isne_recommendation import Hybrid"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -442,68 +416,68 @@
                             "0                         A Crash Course in Data Science  0.054594\n",
                             "79     Write A Feature Length Screenplay For Film Or ...  0.053081\n",
                             "67                  Sharpened Visions: A Poetry Workshop  0.051187\n",
                             "45     Introduction to Supply Chain Finance & Blockch...  0.049684\n",
                             "31     Foundations of Public Health Practice: Behavio...  0.047820"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model = Hybrid.fit(i_data, ui_data)\n",
                 "prediction = Hybrid.predict('Martha Long', i_data, ui_data, model, 10)\n",
                 "prediction"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
-                "train, test = Hybrid.train_test_split(ui_data, test_size=0.2)\n",
+                "train, test = Hybrid.train_test_split(ui_data, test_size=0.25)\n",
                 "model = Hybrid.fit(i_data, train)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.6917808219178082"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "hit_rate = Hybrid.hit_rate(train, test, i_data, model)\n",
                 "hit_rate"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.11624699531071445"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "f1_score = Hybrid.f1_score(train, test, i_data, model)\n",
                 "f1_score"
```

### Comparing `isne_recommendation-0.1.2/tfidf.ipynb` & `isne_recommendation-0.1.3/tfidf.ipynb`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/tfidf.py` & `isne_recommendation-0.1.3/tfidf.py`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/pickle/tfidf_X.pickle` & `isne_recommendation-0.1.3/pickle/tfidf_X.pickle`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/pickle/tfidf_matrix.pickle` & `isne_recommendation-0.1.3/pickle/tfidf_matrix.pickle`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/src/isne_recommendation/FeatureRatingsKNN.py` & `isne_recommendation-0.1.3/src/isne_recommendation/FeatureRatingsKNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,16 @@
 
     # Iterate through each row to determine the split
     for index, row in user_courses.iterrows():
         if row['username'] != current_user:
             # We're at a new user, so reset the counter
             course_counter = 0
             current_user = row['username']
-
-        if course_counter < ( ( 1 - test_size ) * row['course_count'] - 1 ):
+        ceil_value = np.floor( ( 1 - test_size ) * row['course_count'] - 1 )
+        if course_counter <= ceil_value:
             split_list.append(True)  # Training data
         else:
             split_list.append(False)  # Testing data
 
         course_counter += 1
 
     # Add the split information to the DataFrame
```

### Comparing `isne_recommendation-0.1.2/src/isne_recommendation/Hybrid.py` & `isne_recommendation-0.1.3/src/isne_recommendation/Hybrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,16 +194,16 @@
 
     # Iterate through each row to determine the split
     for index, row in user_courses.iterrows():
         if row['username'] != current_user:
             # We're at a new user, so reset the counter
             course_counter = 0
             current_user = row['username']
-
-        if course_counter < ( ( 1 - test_size ) * row['course_count'] - 1 ):
+        ceil_value = np.floor( ( 1 - test_size ) * row['course_count'] - 1 )
+        if course_counter <= ceil_value:
             split_list.append(True)  # Training data
         else:
             split_list.append(False)  # Testing data
 
         course_counter += 1
 
     # Add the split information to the DataFrame
```

### Comparing `isne_recommendation-0.1.2/src/isne_recommendation/TfidfLinearKernel.py` & `isne_recommendation-0.1.3/src/isne_recommendation/TfidfLinearKernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,16 @@
 
     # Iterate through each row to determine the split
     for index, row in user_courses.iterrows():
         if row['username'] != current_user:
             # We're at a new user, so reset the counter
             course_counter = 0
             current_user = row['username']
-
-        if course_counter < ( ( 1 - test_size ) * row['course_count'] - 1 ):
+        ceil_value = np.floor( ( 1 - test_size ) * row['course_count'] - 1 )
+        if course_counter <= ceil_value:
             split_list.append(True)  # Training data
         else:
             split_list.append(False)  # Testing data
 
         course_counter += 1
 
     # Add the split information to the DataFrame
```

### Comparing `isne_recommendation-0.1.2/templates/homepage.html` & `isne_recommendation-0.1.3/templates/homepage.html`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/templates/predata.html` & `isne_recommendation-0.1.3/templates/predata.html`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/.gitignore` & `isne_recommendation-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/LICENSE` & `isne_recommendation-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/README.md` & `isne_recommendation-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `isne_recommendation-0.1.2/pyproject.toml` & `isne_recommendation-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "isne-recommendation"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
   'fuzzywuzzy==0.18.0',
   'joblib==1.3.2',
   'Levenshtein==0.25.0',
   'numpy==1.26.4',
   'pandas==1.5.3',
   'python-dateutil==2.9.0.post0',
```

### Comparing `isne_recommendation-0.1.2/PKG-INFO` & `isne_recommendation-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: isne-recommendation
-Version: 0.1.2
+Version: 0.1.3
 Summary: The recommendation system aims to suggest the best suitable courses for learners who have taken at least one course.
 Project-URL: Homepage, https://github.com/startg2545/recommendation-system
 Project-URL: Issues, https://github.com/startg2545/recommendation-system/issues
 Author-email: Newin Yamaguchi <newin_yamaguchi@cmu.ac.th>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

